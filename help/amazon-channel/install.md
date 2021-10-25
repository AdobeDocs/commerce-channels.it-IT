---
title: Installare l’estensione
description: Per integrare [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] e vendere tramite [!DNL Amazon Marketplace], scarica e installa l’estensione Amazon Sales Channel.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installare l’estensione

>[!IMPORTANT]
>
>Solo [!DNL Amazon Sales Channel] le versioni di estensione 4.0+ sono supportate per Adobe Commerce e le versioni di Magenti Open Source 2.4.x. Se esegui una versione 2.3.x, consulta la documentazione per [versione del canale di vendita Amazon compatibile](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}. Per ulteriori informazioni sulla compatibilità delle versioni, consulta la sezione [Disponibilità](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.

La [!UICONTROL Amazon Sales Channel] l’estensione installa e aggiunge funzionalità per integrare il catalogo Commerce con [!DNL Amazon Seller Accounts] per vendere tramite [!DNL Amazon Marketplace]. Per esaminare ulteriori informazioni, consulta la sezione [Sales Channel Amazon](https://marketplace.magento.com/magento-module-amazon.html) in [!DNL Commerce Marketplace] e [note sulla versione](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) nella documentazione per gli sviluppatori.

## Requisiti

- **Istanza Commerce**: La [!DNL Amazon Sales Channel] L&#39;estensione può essere installata su istanze con Magenti Open Source, Adobe Commerce e Adobe Commerce sulle versioni 2.3.x o successive dell&#39;infrastruttura cloud. Non è più supportato nelle versioni 2.1, 2.2 o 1.x.
- **Account web Commerce**: Devi disporre di un account web Commerce, utilizzato per creare e monitorare una chiave API.
- **Chiave API**: Crea una chiave API del canale di vendita Amazon tramite il tuo account web Commerce. Le istruzioni seguenti includono questi passaggi.

## Installa

Per informazioni più dettagliate sull&#39;utilizzo del Compositore per questo processo, vedi [installazione di estensioni](https://devdocs.magento.com/extensions/install/)Istruzioni per {target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Fai clic sul pulsante **[!UICONTROL Marketplace]** , quindi fai clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione , seleziona la versione .

1. Per il nome e la versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Utilizza il nome e le informazioni sulla versione per aggiornare la voce del connettore servizi nel `composer.json` file.

   - Aggiungi il nome e la versione dell&#39;estensione al tuo `composer.json` file.

   - Passa alla [!DNL Commerce] directory di progetto e aggiorna il tuo `composer.json` file.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Inserisci il tuo [chiavi di autenticazione](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}. La tua chiave pubblica è il tuo nome utente; la tua chiave privata è la tua password.

   - Attendi che Compositore completi l’aggiornamento delle dipendenze del progetto e assicurati che non ci siano errori.


1. [Verifica dell&#39;estensione](https://devdocs.magento.com/extensions/install/#verify-the-extension){target=&quot;_blank&quot;}.

## Aggiungi la chiave API del canale di vendita Amazon

Dopo l’installazione, immetti un [Chiave API](./amazon-verify-api-key.md) per completare la configurazione.

## Impostare le opzioni di configurazione del canale Amazon

Hai le seguenti opzioni per configurare il canale di vendita Amazon. Non è necessario modificare queste impostazioni per iniziare l’onboarding e la vendita su Amazon. È consigliabile che gli amministratori avanzati considerino queste opzioni.

1. Accedi all’amministratore.

1. Sulla _Amministratore_ barra laterale, vai a **Negozi** > _Impostazioni_ > **Configurazione**.

1. Fai clic su **Sales Channel**, quindi **Impostazioni globali**.

1. Per **Cancella cronologia log**, definisce l’intervallo per la cancellazione dei registri raccolti.

   Le opzioni includono `Once Daily`, `Once Weekly`e `Once Monthly` (predefinito).

1. (Facoltativo) Per **Origine attività in background (CRON)**, modifica l’impostazione in `Command Line (CLI) CRON`.

   Questa impostazione è consigliata per **_utenti/amministratori avanzati_**.

1. Fai clic su **[!UICONTROL Save Config]**.

## Aggiorna l&#39;estensione

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Fai clic sul pulsante **[!UICONTROL Marketplace]** , quindi fai clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione , seleziona la versione .

1. Per il nome e la versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Completa il [istruzioni per l&#39;aggiornamento dell&#39;estensione](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.
