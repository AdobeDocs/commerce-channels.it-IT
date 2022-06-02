---
title: Collegare il canale di vendita a [!DNL Walmart Marketplace]
description: Configura il canale di vendita e collegati a Walmart Marketplace.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: aaab7aa7feb05264c24386e62193564dc5ae8fe3
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Collegare il canale di vendita a [!DNL Walmart Marketplace]

Dopo aver installato Channel Manager sul tuo [!DNL Commerce] istanza, collegare un [!DNL Commerce] archiviare [!DNL Walmart Marketplace].

1. [Creare il canale di vendita](#create-the-sales-channel) selezionando Commerce store per gli elenchi di prodotti.

1. [Collegare il canale a [!DNL Walmart Marketplace] aggiungendo [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Impostazione completa del canale di vendita](#complete-store-setup) per gestire elenchi, scorte, prezzi e ordini per le [!DNL Walmart Marketplace] assortimento di prodotti.

## Creare il canale di vendita

1. Dall’amministratore, apri [!DNL Channel Manager] selezionando **[!UICONTROL Marketing** > _Canali _> **Channel Manager]**.

1. In **[!UICONTROL Marketplaces available to connect]** sezione , seleziona **[!UICONTROL Get Started]**.

   ![Collega nuovo [!DNL Walmart] archiviare [!DNL Channel Manager]](assets/channel-manager-home.png)

1. Se necessario, configura il [!DNL Walmart Marketplace Seller] conto.

1. Configura l&#39;archivio e la connessione:

   - Seleziona **[!UICONTROL Add Credentials]**.

   - Seleziona la [!DNL Commerce] visualizzazione archivio per connettersi al marketplace.

      ![Configurare la connessione tra Commerce e [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - Immettere un valore univoco **[!UICONTROL store name]**.

   - Seleziona la **[!UICONTROL Adobe Commerce site]** per gli elenchi dei prodotti.

   - Aggiungi un **[!UICONTROL email address]** per ricevere notifiche relative al servizio [!DNL Channel Manager].

1. Collegare il canale a [!DNL Walmart Marketplace].

   - Aggiungi le credenziali per [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) dal [!DNL Walmart Marketplace Seller] conto.

   - Se non disponi delle credenziali, recuperale dal [!DNL Walmart Marketplace Developer Portal] selezionando **[!UICONTROL Get API credentials]**.

      Sul Developer Portal seleziona la tua area geografica (Stati Uniti e Canada), quindi effettua l’accesso.

      ![[!DNL Walmart Marketplace] accesso account](assets/walmart-marketplace-login-page.png)

   - Nel modulo della chiave API, copia e salva il **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]** per [!UICONTROL Adobe Inc Production API key] in una posizione sicura.

      ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Se la [!DNL Adobe Inc] la chiave non è elencata in Developer Portal, seleziona **[!UICONTROL Add New Key for a Solution Provider]** per configurare le autorizzazioni e generare la chiave. Per informazioni dettagliate sulla configurazione, consulta [Genera un [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Torna a [!DNL Channel Manager] per aggiungere le credenziali al **[!UICONTROL Walmart Connection]** informazioni.

      Quando si aggiungono le credenziali, Adobe nasconde il segreto client e memorizza il valore in un insieme di credenziali protetto.

1. Seleziona **[!UICONTROL Save Store]** per applicare la configurazione e connettersi al [!DNL Walmart marketplace].

1. Dopo la connessione, [configurazione completa dello store](complete-store-setup.md) dal **[!UICONTROL Channel Manager]** pagina store.

![Imposta primo store](assets/channel-manager-setup-first-store.png)

### Risoluzione dei problemi di connessione

Se la connessione a [!DNL Walmart] fallisce, vedi [Domande frequenti su Marketplace Walmart](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} per suggerimenti sulla risoluzione dei problemi.

- Da [!DNL Walmart Developer Portal], verifica di aver copiato le credenziali corrette per la chiave API di produzione per [!UICONTROL Adobe Inc.]

- Verifica che la configurazione di accesso per [!UICONTROL Walmart Adobe API key] dispone delle autorizzazioni corrette. Vedi [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Conferma che [!DNL Walmart API] il servizio è disponibile dal [Pagina di stato API di Walmart](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
