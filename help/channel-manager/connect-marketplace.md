---
title: 'Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]'
description: "Collegare una visualizzazione di Commerce Store a  [!DNL Walmart Marketplace]  per creare il canale di vendita per gestire gli elenchi di prodotti, le scorte, i prezzi e gli ordini di Commerce per le vendite di Walmart Marketplace."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channels, Install, Integration
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]

Dopo aver installato Channel Manager nell&#39;istanza [!DNL Commerce], creare un canale di vendita in Channel Manager e configurare le credenziali per connettere [!DNL Channel Manager] a [!DNL Walmart Marketplace].

1. [Crea il canale di vendita](#create-the-sales-channel) selezionando lo store [!DNL Commerce] per gli elenchi di prodotti.

1. [Connetti il canale a [!DNL Walmart Marketplace] aggiungendo [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Completare la configurazione del canale di vendita](#complete-sales-channel-store-setup) per gestire le inserzioni, le scorte, i prezzi e gli ordini per l&#39;assortimento di prodotti [!DNL Walmart Marketplace].

>[!NOTE]
>
>Channel Manager richiede una connessione uno a uno tra un account Walmart e una visualizzazione store [!DNL Commerce]. Non è possibile collegare la stessa visualizzazione Store a più account Walmart.

## Creare il canale di vendita

1. Dall&#39;amministratore, aprire [!DNL Channel Manager] selezionando **[!UICONTROL Marketing** > _Canali _> **Channel Manager]**.

1. Nella sezione **[!UICONTROL Marketplaces available to connect]**, selezionare **[!UICONTROL Get Started]**.

   ![Connetti nuovo archivio [!DNL Walmart] a [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. Se necessario, configurare l&#39;account [!DNL Walmart Marketplace Seller].

1. Configura l&#39;archivio e la connessione:

   - Selezionare **[!UICONTROL Add Credentials]**.

   - Selezionare la visualizzazione dello store [!DNL Commerce] che offre i prodotti che si desidera vendere sul marketplace.

     ![Configura connessione tra [!DNL Commerce] e [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}

   - Immettere un **[!UICONTROL store name]** univoco.

   - Selezionare **[!UICONTROL Adobe [!DNL Commerce] site]** per l&#39;elenco dei prodotti e l&#39;elaborazione degli ordini.

   - Per ricevere le notifiche relative a [!DNL Channel Manager], aggiungere un **[!UICONTROL email address]**.

1. Connetti il canale a [!DNL Walmart Marketplace].

   - Aggiungi le credenziali per [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) dal tuo account [!DNL Walmart Marketplace Seller].

   - Se non si dispone delle credenziali, recuperarle da [!DNL Walmart Marketplace Developer Portal] selezionando **[!UICONTROL Get API credentials]**.

     Sul portale per sviluppatori, seleziona la tua regione (Stati Uniti e Canada) e quindi accedi.

     Account di accesso ![[!DNL Walmart Marketplace]](assets/walmart-marketplace-login-page.png){width="600"}

   - Nel modulo della chiave API, copiare e salvare i valori **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]** per [!UICONTROL Adobe Inc Production API key] in un percorso sicuro.

     ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >Se la chiave [!DNL Adobe Inc] non è elencata nel Portale per sviluppatori, selezionare **[!UICONTROL Add New Key for a Solution Provider]** per configurare le autorizzazioni e generare la chiave. Per informazioni dettagliate sulla configurazione, vedere [Generare a [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Tornare a [!DNL Channel Manager] per aggiungere le credenziali alle informazioni di **[!UICONTROL Walmart Connection]**.

     Quando aggiungi le credenziali, Adobe nasconde il segreto client e memorizza il valore in un archivio protetto.

1. Selezionare **[!UICONTROL Save Store]** per applicare la configurazione e connettersi a [!DNL Walmart marketplace].

1. Dopo la connessione, [completare l&#39;installazione dell&#39;archivio](complete-sales-channel-store-setup.md) dalla pagina dell&#39;archivio **[!UICONTROL Channel Manager]**.

![Imposta primo archivio](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### Risoluzione dei problemi di connessione

Se la connessione a [!DNL Walmart] non riesce, vedere le [Domande frequenti su Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"} per suggerimenti per la risoluzione dei problemi.

- Da [!DNL Walmart Developer Portal], verificare di aver copiato le credenziali corrette per la chiave API di produzione per [!UICONTROL Adobe Inc.]

- Verificare che la configurazione di accesso per [!UICONTROL Walmart Adobe API key] disponga delle autorizzazioni corrette. Vedere [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Verificare che il servizio [!DNL Walmart API] sia disponibile dalla [pagina di stato API Walmart](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}.
