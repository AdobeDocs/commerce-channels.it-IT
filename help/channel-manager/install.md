---
title: 'Installa [!DNL Channel Manager]'
description: 'Installare[!DNL Channel Manager] estensione.'
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---


# Installa [!DNL Channel Manager]

Rivedi [requisiti](onboard.md#requirements) e raccogliere le informazioni richieste prima di installare Channel Manager.

## Installare l’estensione

Le istruzioni di installazione di Channel Manager dipendono dall’implementazione di Adobe Commerce o del Magento Open Source on-premise o dall’infrastruttura cloud.

- Installa su un [Istanza locale](#install-on-an-on-premises-instance).

- Installa su un [[!DNL Adobe Commerce] sull’istanza dell’infrastruttura cloud](#install-adobe-commerce-on-cloud-infrastructure)

Entrambi i metodi richiedono l&#39;utilizzo dell&#39;interfaccia CLI (Command Line Interface).

>[!NOTE]
>
>Per assistenza sull&#39;installazione di [!DNL Commerce] software che utilizza CLI, vedere [Installare un’estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### Eseguire l’installazione in un’istanza locale

Utilizzare queste istruzioni per installare [!DNL Channel Manager] su Adobe Commerce e il Magento Open Source a un’istanza on-premise.

1. Accedi a [!DNL Commerce] server as a [utente con autorizzazioni](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) per scrivere su [!DNL Commerce] file system.

1. Inserisci il tuo sito web in [modalità di manutenzione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Dalla sezione [!DNL Commerce] directory principale del progetto, aggiungi Channel Manager a `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Se richiesto, immettere i tasti di scelta dal [!DNL Commerce] account.

   La chiave pubblica è il nome utente; la chiave privata è la password.

1. Aggiorna le dipendenze e installa l’estensione.

   ```bash
   composer update magento/channel-manager
   ```

   Il `composer update` il comando aggiorna solo le dipendenze richieste per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizzare questo comando: `composer update`.

1. Attendi che Composer completi l&#39;aggiornamento delle dipendenze del progetto e risolva eventuali errori.

1. Verificare l&#39;installazione del modulo:

   - Controlla lo stato del modulo.

     ```bash
     bin/magento module:status Magento_SalesChannels
     ```

     Risposta di esempio:

     ```terminal
     Module is enabled
     ```

   - Se il modulo non è abilitato, attivalo.

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. Registra l&#39;estensione.

   ```bash
   bin/magento setup:upgrade
   ```

1. Se richiesto, ricompila il [!DNL Commerce] progetto.

   ```bash
   bin/magento setup:di:compile
   ```

1. Pulire la cache.

   ```bash
   bin/magento cache:clean
   ```

1. Disattiva la modalità di manutenzione.

   ```bash
   bin/magento maintenance:disable
   ```

### Eseguire l’installazione in un’istanza di Adobe Commerce on Cloud Infrastructure

Lavora in un ramo di sviluppo quando aggiungi un’estensione all’istanza cloud.

Per assistenza sull’utilizzo dei rami, consulta [Introduzione alla creazione di rami](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) nel _Guida di Commerce su infrastruttura cloud_.

Durante l’installazione, il nome dell’estensione (`magento\channel-manager`) viene inserito automaticamente nel [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) file. Non è necessario modificare direttamente il file.

1. Nella workstation locale, passa alla directory principale del progetto Cloud.

1. Creare o estrarre uno sviluppo [filiale](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. Utilizzando il nome del Compositore, aggiungi l’estensione al `require` sezione del `composer.json` file.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. Aggiorna le dipendenze e installa l’estensione.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   Il `composer update` il comando aggiorna solo le dipendenze richieste per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizzare questo comando: `composer update`.

1. Aggiungere, eseguire il commit e inviare le modifiche al codice; queste includono modifiche a entrambi `composer.lock` e `composer.json` file.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m "Install channel manager extension" 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. Al termine del processo di build e distribuzione, utilizza SSH per accedere all’ambiente remoto e verificare che l’estensione sia installata correttamente.

```bash
   bin/magento module:status Magento_SalesChannels
```

Risposta di esempio:

```terminal
Module is enabled
```

Se il modulo è disattivato, [abilitarlo nell’ambiente locale](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) e distribuire le modifiche.


1. Dopo aver installato correttamente l&#39;estensione, accedi a [!UICONTROL Admin] a [configurare Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Per istruzioni su come aggiornare Channel Manager a una nuova versione, consulta [Aggiornare moduli ed estensioni](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## Risoluzione dei problemi

Utilizzare le informazioni seguenti per risolvere gli errori che si verificano durante il processo di installazione di Channel Manager.

### Tasti composizione errati

Se il [tasti di scelta](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) utilizzati per l’autenticazione nell’archivio del Compositore non sono validi o non sono collegati al [!DNL MAGE ID] utilizzato per iscriversi a [!DNL Channel Manager] servizio, viene visualizzato il seguente errore.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controlla la configurazione della chiave:

1. Trova la posizione del `auth.json` file:

   ```bash
   $ composer config –global home
   ```

1. Visualizza `auth.json` file.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Verifica che le credenziali nel file auth.json corrispondano [le chiavi associate all&#39;ID immagine](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) utilizzato per registrarsi al servizio Channel Manager.

### Memoria insufficiente per PHP

Se il sistema non dispone di memoria sufficiente per PHP, viene visualizzato il seguente errore.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Per risolvere il problema di memoria, utilizzare uno dei metodi seguenti:

- [Aumentare il limite di memoria per PHP](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) nell’ambiente `php.ini` file. Inoltre, verifica che l’istanza Commerce disponga del [valori consigliati](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) per altre impostazioni PHP.

- Specificare il limite di memoria dalla riga di comando.

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  Ad esempio:

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### Vista mancante

Se ricevi un errore relativo a un elemento mancante `process_catalog_exporter_view` durante l&#39;installazione di Channel Manager, provare [aggiornamento degli indicizzatori](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### Errori di distribuzione cloud

Per problemi durante la distribuzione dell&#39;estensione nel cloud, vedi [distribuzione dell&#39;estensione non riuscita](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
