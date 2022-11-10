---
title: 'Installazione [!DNL Channel Manager]'
description: '''Installa il[!DNL Channel Manager] estensione."'
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 31af7107c0b27a236b94f7725b7a107d1027789c
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---


# Installa [!DNL Channel Manager]

Consulta la sezione [requisiti](onboard.md#requirements) e raccogliere le informazioni necessarie prima di installare Channel Manager.

## Installare l’estensione

Le istruzioni di installazione di Channel Manager dipendono dall’implementazione di Adobe Commerce o Magenti Open Source in locale o su un’infrastruttura cloud.

- Installa su un [Istanza locale](#install-on-an-on-premises-instance).

- Installa su un [[!DNL Adobe Commerce] sull&#39;istanza dell&#39;infrastruttura cloud](#install-adobe-commerce-on-cloud-infrastructure)

Entrambi i metodi richiedono l’utilizzo dell’interfaccia CLI (Command Line Interface).

>[!NOTE]
>
>Per informazioni sull’installazione [!DNL Commerce] software che utilizza CLI, vedi [Installazione generale CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}.

### Installazione su un&#39;istanza on-premise

Utilizzare queste istruzioni per l&#39;installazione [!DNL Channel Manager] su Adobe Commerce e Magento Open Source a un’istanza locale.

1. Accedi a [!DNL Commerce] come server [utente con autorizzazioni](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;} per scrivere in [!DNL Commerce] file system.

1. Inserisci il tuo sito web in [modalità di manutenzione](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}.

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Da [!DNL Commerce] directory principale del progetto, aggiungi Channel Manager a `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Se richiesto, immetti le chiavi di accesso dal [!DNL Commerce] conto.

   La tua chiave pubblica è il tuo nome utente; la tua chiave privata è la tua password.

1. Aggiorna le dipendenze e installa l&#39;estensione.

   ```bash
   composer update magento/channel-manager
   ```

   La `composer update` il comando aggiorna solo le dipendenze necessarie per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizza invece questo comando: `composer update`.

1. Attendi che Compositore completi l’aggiornamento delle dipendenze del progetto e risolva eventuali errori.

1. Verifica l’installazione del modulo:

   - Controlla lo stato del modulo.

      ```bash
      bin/magento module:status Magento_SalesChannels
      ```
      Risposta di esempio:

      ```terminal
      Module is enabled
      ```

   - Se il modulo non è abilitato, abilitalo.

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. Registra l&#39;estensione.

   ```bash
   bin/magento setup:upgrade
   ```

1. Se richiesto, ricompilare il [!DNL Commerce] progetto.

   ```bash
   bin/magento setup:di:compile
   ```

1. Pulisci la cache.

   ```bash
   bin/magento cache:clean
   ```

1. Disattiva la modalità di manutenzione.

   ```bash
   bin/magento maintenance:disable
   ```

### Installare su un’istanza di Adobe Commerce su Cloud Infrastructure

Lavora in un ramo di sviluppo quando aggiungi un&#39;estensione all&#39;istanza cloud.

Per informazioni sull’utilizzo dei rami, consulta [Introduzione alla creazione di rami](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori di Adobe Commerce.

Durante l&#39;installazione, il nome dell&#39;estensione (`magento\channel-manager`) viene inserito automaticamente nel [app/etc/config.php](https://devdocs.magento.com/cloud/live/sens-data-over.html#configuration-data)File {target=&quot;_blank&quot;}. Non è necessario modificare direttamente il file.

1. Nella workstation locale, passa alla directory principale del progetto Cloud.

1. Creare o estrarre uno sviluppo [filiale](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}.

1. Utilizzando il nome del Compositore , aggiungi l’estensione al `require` della sezione `composer.json` file.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. Aggiorna le dipendenze e installa l&#39;estensione.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   La `composer update` il comando aggiorna solo le dipendenze necessarie per [!DNL Channel Manager]. Per aggiornare tutte le dipendenze, utilizza invece questo comando: `composer update`.

1. Aggiungi, conferma e invia modifiche al codice: includi le modifiche a entrambi i tipi di `composer.lock` e `composer.json` file.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. Al termine del processo di compilazione e distribuzione, utilizza SSH per accedere all’ambiente remoto e verifica che l’estensione sia installata correttamente.

```bash
   bin/magento module:status Magento_SalesChannels
```

Risposta di esempio:

```terminal
Module is enabled
```

Se il modulo è disabilitato, [attivarla nell’ambiente locale](https://devdocs.magento.com/cloud/howtos/install-components.html#manage-extensions) e distribuire le modifiche.


1. Dopo aver installato correttamente l&#39;estensione, accedi al [!UICONTROL Admin] a [configurare Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Per istruzioni su come aggiornare Channel Manager a una nuova versione, vedi [Aggiornamento di moduli ed estensioni](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}.


## Risoluzione dei problemi

Utilizza le seguenti informazioni per risolvere gli errori che si verificano durante il processo di installazione di Channel Manager.

### Tasti compositore errati

Se la [chiavi di accesso](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} utilizzato per l&#39;autenticazione nell&#39;archivio Composer non è valido o non è collegato al [!DNL MAGE ID] utilizzato per la [!DNL Channel Manager] viene visualizzato il seguente errore.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Controlla la configurazione della chiave:

1. Trova la posizione del `auth.json` file:

   ```bash
   $ composer config –global home
   ```

1. Visualizza la `auth.json` file.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Verifica che le credenziali in auth.json corrispondano [le chiavi associate all’ID MAGE](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} utilizzato per la registrazione al servizio Channel Manager.

### Memoria insufficiente per PHP

Viene visualizzato il seguente errore se al sistema non è stata assegnata una quantità di memoria sufficiente per PHP.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Utilizza uno dei metodi seguenti per risolvere il problema di memoria:

- [Aumenta il limite di memoria per PHP](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit){target=&quot;_blank&quot;} nell&#39;ambiente `php.ini` file. Inoltre, verifica che l’istanza Commerce disponga della [valori consigliati](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target=&quot;_blank&quot;} per altre impostazioni PHP.

- Specificare il limite di memoria dalla riga di comando.

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   Ad esempio:

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### Visualizzazione mancante

Se ricevi un errore su un elemento mancante `process_catalog_exporter_view` durante l&#39;installazione di Channel Manager, prova [aggiornamento degli indici](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}.

```bash
php bin/magento indexer:refresh
```

### Errori di distribuzione cloud

Per problemi durante la distribuzione dell&#39;estensione nel cloud, vedi [errore di distribuzione dell&#39;estensione](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}.
