---
title: 'Installa [!DNL Channel Manager]'
description: '''Installa l''estensione [!DNL Channel Manager].'''
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# Installa [!DNL Channel Manager]

Rivedi i [requisiti](onboard.md#requirements) e raccogli le informazioni richieste prima di installare Channel Manager.

## Installare l’estensione

Le istruzioni di installazione di Channel Manager dipendono dall’implementazione di Adobe Commerce o del Magento Open Source on-premise o dall’infrastruttura cloud.

- Installa in un&#39;istanza [locale](#install-on-an-on-premises-instance).

- Installa in un&#39;istanza [[!DNL Adobe Commerce] dell&#39;infrastruttura cloud](#install-adobe-commerce-on-cloud-infrastructure)

Entrambi i metodi richiedono l&#39;utilizzo dell&#39;interfaccia CLI (Command Line Interface).

>[!NOTE]
>
>Per informazioni sull&#39;installazione del software [!DNL Commerce] tramite CLI, vedere [Installare un&#39;estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### Eseguire l’installazione in un’istanza locale

Utilizzare queste istruzioni per installare [!DNL Channel Manager] in Adobe Commerce e per eseguire il Magento Open Source a un&#39;istanza locale.

1. Accedere al server [!DNL Commerce] come [utente con autorizzazioni](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) per scrivere nel file system [!DNL Commerce].

1. Imposta il tuo sito Web in [modalità di manutenzione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Dalla directory principale del progetto [!DNL Commerce], aggiungere Channel Manager a `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Se richiesto, immettere le chiavi di accesso dall&#39;account [!DNL Commerce].

   La chiave pubblica è il nome utente; la chiave privata è la password.

1. Aggiorna le dipendenze e installa l’estensione.

   ```bash
   composer update magento/channel-manager
   ```

   Il comando `composer update` aggiorna solo le dipendenze richieste per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizzare questo comando: `composer update`.

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

1. Se richiesto, ricompilare il progetto [!DNL Commerce].

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

Per informazioni sull&#39;utilizzo dei rami, vedere [Introduzione alla creazione di rami](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) nella _Guida di Commerce sull&#39;infrastruttura cloud_.

Durante l&#39;installazione, il nome dell&#39;estensione (`magento\channel-manager`) viene inserito automaticamente nel file [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html). Non è necessario modificare direttamente il file.

1. Nella workstation locale, passa alla directory principale del progetto Cloud.

1. Crea o estrai un [ramo](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) di sviluppo.

1. Utilizzando il nome del Compositore, aggiungere l&#39;estensione alla sezione `require` del file `composer.json`.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. Aggiorna le dipendenze e installa l’estensione.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   Il comando `composer update` aggiorna solo le dipendenze richieste per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizzare questo comando: `composer update`.

1. Aggiungere, eseguire il commit e inviare le modifiche al codice; includere le modifiche al file `composer.lock` e al file `composer.json`.

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

Se il modulo è disabilitato, [abilitarlo nell&#39;ambiente locale](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) e distribuire le modifiche.


1. Dopo aver installato l&#39;estensione, accedere a [!UICONTROL Admin] per [configurare Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Per istruzioni su come aggiornare Channel Manager a una nuova versione, consulta [Aggiornare moduli ed estensioni](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## Risoluzione dei problemi

Utilizzare le informazioni seguenti per risolvere gli errori che si verificano durante il processo di installazione di Channel Manager.

### Tasti composizione errati

Se le [chiavi di accesso](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) utilizzate per l&#39;autenticazione nell&#39;archivio del Compositore non sono valide o non sono collegate alle [!DNL MAGE ID] utilizzate per la registrazione al servizio [!DNL Channel Manager], viene visualizzato il seguente errore.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controlla la configurazione della chiave:

1. Trovare il percorso del file `auth.json`:

   ```bash
   $ composer config –global home
   ```

1. Visualizza il file `auth.json`.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Verificare che le credenziali nel file auth.json corrispondano alle [chiavi associate all&#39;ID MAGE](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) utilizzato per la registrazione al servizio Channel Manager.

### Memoria insufficiente per PHP

Se il sistema non dispone di memoria sufficiente per PHP, viene visualizzato il seguente errore.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Per risolvere il problema di memoria, utilizzare uno dei metodi seguenti:

- [Aumentare il limite di memoria per PHP](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) nel file dell&#39;ambiente `php.ini`. Verificare inoltre che l&#39;istanza di Commerce disponga dei [valori consigliati](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) per altre impostazioni PHP.

- Specificare il limite di memoria dalla riga di comando.

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  Ad esempio:

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### Vista mancante

Se durante l&#39;installazione di Channel Manager viene visualizzato un errore relativo a `process_catalog_exporter_view` mancante, provare ad [aggiornare gli indicizzatori](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### Errori di distribuzione cloud

Per i problemi relativi alla distribuzione dell&#39;estensione nel cloud, vedere [errore di distribuzione dell&#39;estensione](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
