---
title: Installare l’estensione
description: Per integrare [!DNL Commerce] catalogo con [!DNL Amazon Seller Accounts] e vendere tramite [!DNL Amazon Marketplace], scarica e installa l’estensione di Sales Channel Amazon.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Installare l’estensione

>[!IMPORTANT]
>
>Solo [!DNL Amazon Sales Channel] le versioni di estensione 4.0+ sono supportate per le versioni di Adobe Commerce e Magenti Open Source 2.4.x. Se esegui una versione 2.3.x, consulta la documentazione di [versione del canale di vendita Amazon compatibile](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target="_blank"}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target="_blank"} nella documentazione per gli sviluppatori.

Il [!UICONTROL Amazon Sales Channel] L’estensione installa e aggiunge funzioni per integrare il catalogo Commerce con [!DNL Amazon Seller Accounts] per vendere tramite [!DNL Amazon Marketplace]. Per ulteriori informazioni, vedere [Sales Channel Amazon](https://marketplace.magento.com/magento-module-amazon.html) pagina in [!DNL Commerce Marketplace] e [note sulla versione](release-notes.md).

## Requisiti

- **Istanza Commerce**: Il [!DNL Amazon Sales Channel] l’estensione può essere installata sulle istanze con Magenti Open Source, Adobe Commerce e Adobe Commerce nelle versioni 2.3.x o successive dell’infrastruttura cloud. Non è più supportato nelle versioni 2.1, 2.2 o 1.x.
- **Account Web Commerce**: è necessario disporre di un account web Commerce, utilizzato per creare e tenere traccia di una chiave API.
- **Chiave API**: crea una chiave API del canale di vendita di Amazon tramite il tuo account web Commerce. Le istruzioni seguenti includono questi passaggi.

## Installa

Per informazioni più dettagliate sull&#39;utilizzo di Composer per questo processo, vedere [installazione dell’estensione](https://devdocs.magento.com/extensions/install/){target="_blank"} istruzioni nella documentazione per gli sviluppatori.

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Fai clic su **[!UICONTROL Marketplace]** e quindi fare clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione, seleziona la versione.

1. Per nome e versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Utilizza il nome e le informazioni sulla versione per aggiornare la voce del connettore servizi nel tuo `composer.json` file.

   - Aggiungi il nome e la versione dell&#39;estensione al tuo `composer.json` file.

   - Accedi al tuo [!DNL Commerce] directory del progetto e aggiornare `composer.json` file.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Immetti il [chiavi di autenticazione](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"}. La chiave pubblica è il nome utente; la chiave privata è la password.

   - Attendi che Composer finisca di aggiornare le dipendenze del progetto e assicurati che non vi siano errori.


1. [Verificare l’estensione](https://devdocs.magento.com/extensions/install/#verify-the-extension){target="_blank"}.

## Aggiungi la chiave API del canale di vendita Amazon

Dopo l&#39;installazione, immettere un [Chiave API](./amazon-verify-api-key.md) per completare la configurazione.

## Impostare le opzioni di configurazione del canale Amazon

Sono disponibili le seguenti opzioni per la configurazione del canale di vendita Amazon. Non è necessario modificare queste impostazioni per iniziare l’onboarding e la vendita su Amazon. Si consiglia agli amministratori avanzati di prendere in considerazione queste opzioni.

1. Accedi ad Admin.

1. Il giorno _Amministratore_ barra laterale, vai a **Negozi** > _Impostazioni_ > **Configurazione**.

1. Clic **Sales Channel**, quindi **Impostazioni globali**.

1. Per **Cancella cronologia registro**, definisci l’intervallo per cancellare i registri raccolti.

   Le opzioni includono `Once Daily`, `Once Weekly`, e `Once Monthly` (impostazione predefinita).

1. (Facoltativo) Per **Origine attività in background (CRON)**, modifica l’impostazione in `Command Line (CLI) CRON`.

   Questa impostazione è consigliata per **_utenti/amministratori avanzati_**.

1. Clic **[!UICONTROL Save Config]**.

## Aggiornare l’estensione

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Fai clic su **[!UICONTROL Marketplace]** e quindi fare clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione, seleziona la versione.

1. Per nome e versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Completa il [istruzioni per l’aggiornamento dell’estensione](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target="_blank"} nella documentazione per gli sviluppatori.
