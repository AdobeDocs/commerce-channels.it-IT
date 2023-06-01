---
title: 'Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]'
description: "Collegare una visualizzazione di Commerce Store a [!DNL Walmart Marketplace] creare il canale di vendita per gestire gli elenchi di prodotti, le scorte, i prezzi e gli ordini di vendita di Walmart Marketplace."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]

Dopo aver installato Channel Manager sul [!DNL Commerce] , crea un canale di vendita in Channel Manager e configura le credenziali per la connessione [!DNL Channel Manager] a [!DNL Walmart Marketplace].

1. [Creare il canale di vendita](#create-the-sales-channel) selezionando la [!DNL Commerce] memorizza per gli elenchi di prodotti.

1. [Connetti il canale a [!DNL Walmart Marketplace] aggiungendo [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Impostazione completa del canale di vendita](#complete-sales-channel-store-setup) per gestire inserzioni, scorte, prezzi e ordini per [!DNL Walmart Marketplace] assortimento di prodotti.

>[!NOTE]
>
>Channel Manager richiede una connessione uno-a-uno tra un account Walmart e un [!DNL Commerce] visualizzazione store. Non è possibile collegare la stessa visualizzazione Store a più account Walmart.

## Creare il canale di vendita

1. Dall’amministratore, apri [!DNL Channel Manager] selezionando **[!UICONTROL Marketing** > _Canali _> **Channel Manager]**.

1. In **[!UICONTROL Marketplaces available to connect]** sezione, seleziona **[!UICONTROL Get Started]**.

   ![Connetti nuovo [!DNL Walmart] memorizza in [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. Se necessario, configura [!DNL Walmart Marketplace Seller] account.

1. Configura l&#39;archivio e la connessione:

   - Seleziona **[!UICONTROL Add Credentials]**.

   - Seleziona la [!DNL Commerce] store view che offre i prodotti che desideri vendere sul marketplace.

      ![Configurare la connessione tra [!DNL Commerce] e [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}

   - Inserisci un valore univoco **[!UICONTROL store name]**.

   - Seleziona la **[!UICONTROL Adobe [!DNL Commerce] site]** per gli elenchi di prodotti e l’elaborazione degli ordini.

   - Per ricevere notifiche relative a [!DNL Channel Manager], aggiungi un **[!UICONTROL email address]**.

1. Connetti il canale a [!DNL Walmart Marketplace].

   - Aggiungi le credenziali per [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) dal tuo [!DNL Walmart Marketplace Seller] account.

   - Se non disponi delle credenziali, recuperale dal [!DNL Walmart Marketplace Developer Portal] selezionando **[!UICONTROL Get API credentials]**.

      Sul portale per sviluppatori, seleziona la tua regione (Stati Uniti e Canada) e quindi accedi.

      ![[!DNL Walmart Marketplace] accesso account](assets/walmart-marketplace-login-page.png){width="600"}

   - Nel modulo della chiave API, copia e salva **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]** valori per [!UICONTROL Adobe Inc Production API key] in un luogo sicuro.

      ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

      >[!NOTE]
      >
      >Se il [!DNL Adobe Inc] non è elencato nel Portale per sviluppatori, seleziona **[!UICONTROL Add New Key for a Solution Provider]** per configurare le autorizzazioni e generare la chiave. Per informazioni dettagliate sulla configurazione, consulta [Genera un [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Torna a [!DNL Channel Manager] per aggiungere le credenziali al **[!UICONTROL Walmart Connection]** informazioni.

      Quando aggiungi le credenziali, Adobe nasconde il segreto client e memorizza il valore in un archivio protetto.

1. Seleziona **[!UICONTROL Save Store]** per applicare la configurazione e connettersi al [!DNL Walmart marketplace].

1. Dopo la connessione, [completa la configurazione del negozio](complete-sales-channel-store-setup.md) dal **[!UICONTROL Channel Manager]** pagina del negozio.

![Imposta primo archivio](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### Risoluzione dei problemi di connessione

Se la connessione a [!DNL Walmart] non riesce, vedi [Domande frequenti su Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"} per suggerimenti sulla risoluzione dei problemi.

- Dalla sezione [!DNL Walmart Developer Portal], verifica di aver copiato le credenziali corrette per la chiave API di produzione per [!UICONTROL Adobe Inc.]

- Verificare che la configurazione di accesso per [!UICONTROL Walmart Adobe API key] dispone delle autorizzazioni corrette. Consulta [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Confermare che [!DNL Walmart API] il servizio è disponibile da [Pagina di stato API di Walmart](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}.
