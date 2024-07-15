---
title: Installa l'estensione  [!DNL Amazon Sales Channel]
description: Per integrare il catalogo  [!DNL Commerce]  con  [!DNL Amazon Seller Accounts]  e vendere tramite  [!DNL Amazon Marketplace], scarica e installa l'estensione del Sales Channel Amazon.
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 010a95d7be29354515cf4dcbf5d557eebaa40ed6
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Installa l&#39;estensione [!DNL Amazon Sales Channel]

>[!IMPORTANT]
>
>Per le versioni Adobe Commerce e Magento Open Source 2.4.x sono supportate solo le versioni dell&#39;estensione [!DNL Amazon Sales Channel] 4.0+. Se esegui una versione 2.3.x, consulta la documentazione della [versione compatibile del canale di vendita di Amazon](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). Per ulteriori informazioni sulla compatibilità delle versioni, vedere la pagina [Disponibilità](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) nella documentazione per gli sviluppatori.

L&#39;estensione [!UICONTROL Amazon Sales Channel] installa e aggiunge funzionalità per integrare il catalogo Commerce con [!DNL Amazon Seller Accounts] per la vendita tramite [!DNL Amazon Marketplace]. Per ulteriori informazioni, vedere la pagina [Sales Channel Amazon](https://marketplace.magento.com/magento-module-amazon.html) in [!DNL Commerce Marketplace] e le [note sulla versione](release-notes.md).

## Requisiti

- **Istanza di Commerce**: l&#39;estensione [!DNL Amazon Sales Channel] può essere installata in istanze con Magento Open Source, Adobe Commerce e Adobe Commerce nelle versioni 2.3.x o successive dell&#39;infrastruttura cloud. Non è più supportato nelle versioni 2.1, 2.2 o 1.x.
- **Account Web Commerce**: è necessario disporre di un account Web Commerce utilizzato per creare e tenere traccia di una chiave API.
- **Chiave API**: crea una chiave API del canale di vendita Amazon tramite il tuo account Web Commerce. Le istruzioni seguenti includono questi passaggi.

## Installa

Per informazioni più dettagliate sull&#39;utilizzo di Composer per questo processo, vedere le istruzioni per l&#39;installazione dell&#39;[estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) nella documentazione per gli sviluppatori.

1. Accedi alla [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. Fare clic sulla scheda **[!UICONTROL Marketplace]** e quindi su **[!UICONTROL My Purchases]**.

1. Individuare e selezionare **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione, seleziona la versione.

1. Per il nome e la versione del componente, fare clic su **[!UICONTROL Technical Details]**.

1. Utilizzare le informazioni sul nome e sulla versione per aggiornare la voce del connettore dei servizi nel file `composer.json`.

   - Aggiungere il nome e la versione dell&#39;estensione al file `composer.json`.

   - Passa alla directory del progetto [!DNL Commerce] e aggiorna il file `composer.json`.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Immetti le [chiavi di autenticazione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html). La chiave pubblica è il nome utente; la chiave privata è la password.

   - Attendi che Composer finisca di aggiornare le dipendenze del progetto e assicurati che non vi siano errori.

1. [Verificare l&#39;estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## Aggiungi la chiave API del canale di vendita Amazon

Dopo l&#39;installazione, immettere una [chiave API](./amazon-verify-api-key.md) per completare la configurazione.

## Impostare le opzioni di configurazione del canale Amazon

Sono disponibili le seguenti opzioni per la configurazione del canale di vendita Amazon. Non è necessario modificare queste impostazioni per iniziare l’onboarding e la vendita su Amazon. Si consiglia agli amministratori avanzati di prendere in considerazione queste opzioni.

1. Accedi ad Admin.

1. Nella barra laterale _Admin_, vai a **Archivi** > _Impostazioni_ > **Configurazione**.

1. Fai clic su **Sales Channel**, quindi su **Impostazioni globali**.

1. Per **Cancella cronologia log**, definire l&#39;intervallo per la cancellazione dei log raccolti.

   Le opzioni includono `Once Daily`, `Once Weekly` e `Once Monthly` (impostazione predefinita).

1. (Facoltativo) Per **Attività in background (CRON) Source**, modificare l&#39;impostazione in `Command Line (CLI) CRON`.

   Impostazione consigliata per **_utenti/amministratori avanzati_**.

1. Fare clic su **[!UICONTROL Save Config]**.

## Aggiornare l’estensione

1. Accedi alla [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. Fare clic sulla scheda **[!UICONTROL Marketplace]** e quindi su **[!UICONTROL My Purchases]**.

1. Individuare e selezionare **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione, seleziona la versione.

1. Per il nome e la versione del componente, fare clic su **[!UICONTROL Technical Details]**.

1. Completare le [istruzioni per l&#39;aggiornamento dell&#39;estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) nella _Guida all&#39;installazione_.
