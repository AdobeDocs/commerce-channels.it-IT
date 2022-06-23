---
title: '''Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]'''
description: '"Collegare una visualizzazione Negozio Commerce a [!DNL Walmart Marketplace] creare il canale di vendita per gestire gli elenchi dei prodotti Commerce, le scorte, i prezzi e gli ordini per le vendite di Walmart Marketplace."'
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8146be1c94ffb1c8abd0d28e53d3476fd78f2c62
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Connetti [!DNL Channel Manager] a [!DNL Walmart Marketplace]

Dopo aver installato Channel Manager sul tuo [!DNL Commerce] istanza, crea un canale di vendita in Channel Manager e configura le credenziali per la connessione [!DNL Channel Manager] a [!DNL Walmart Marketplace].

1. [Creare il canale di vendita](#create-the-sales-channel) selezionando la [!DNL Commerce] conservare gli elenchi dei prodotti.

1. [Collegare il canale a [!DNL Walmart Marketplace] aggiungendo [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Impostazione completa del canale di vendita](#complete-store-setup) per gestire elenchi, scorte, prezzi e ordini per le [!DNL Walmart Marketplace] assortimento di prodotti.

>[!NOTE]
>
>Channel Manager richiede una connessione one-to-one tra un account Walmart e un [!DNL Commerce] visualizzazione archivio. Non è possibile collegare la stessa visualizzazione store a più account Walmart.

## Creare il canale di vendita

1. Dall’amministratore, apri [!DNL Channel Manager] selezionando **[!UICONTROL Marketing** > _Canali _> **Channel Manager]**.

1. In **[!UICONTROL Marketplaces available to connect]** sezione , seleziona **[!UICONTROL Get Started]**.

   ![Collega nuovo [!DNL Walmart] archiviare [!DNL Channel Manager]](assets/channel-manager-home.png)

1. Se necessario, configura il [!DNL Walmart Marketplace Seller] conto.

1. Configura l&#39;archivio e la connessione:

   - Seleziona **[!UICONTROL Add Credentials]**.

   - Seleziona la [!DNL Commerce] vista negozio che offre i prodotti che desideri vendere sul mercato.

      ![Configura la connessione tra [!DNL Commerce] e [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - Immettere un valore univoco **[!UICONTROL store name]**.

   - Seleziona la **[!UICONTROL Adobe [!DNL Commerce] site]** per gli elenchi dei prodotti e l&#39;elaborazione degli ordini.

   - Per ricevere notifiche relative a [!DNL Channel Manager], aggiungi un **[!UICONTROL email address]**.

1. Collegare il canale a [!DNL Walmart Marketplace].

   - Aggiungi le credenziali per [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) dal [!DNL Walmart Marketplace Seller] conto.

   - Se non disponi delle credenziali, recuperale dal [!DNL Walmart Marketplace Developer Portal] selezionando **[!UICONTROL Get API credentials]**.

      Sul Developer Portal, seleziona la tua area geografica (Stati Uniti e Canada), quindi effettua l’accesso.

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
