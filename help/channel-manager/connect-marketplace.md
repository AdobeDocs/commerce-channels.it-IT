---
title: Collega Sales Channel a [!DNL Walmart Marketplace]
description: Configura il canale di vendita e collegati a Walmart Marketplace.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: a10ab3f7fa7049e48d83a942f6c5441d8147b12c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Connetti a [!DNL Walmart Marketplace]

Dopo aver installato Channel Manager sul tuo [!DNL Commerce] ad esempio, collega un negozio Commerce a Walmart Marketplace.

1. Crea il canale di vendita per [selezione dell’archivio Commerce per gli elenchi di prodotti](#select-the-commerce-store-for-the-sales-channel).

1. [Collegare il canale a [!DNL Walmart Marketplace] aggiungendo le credenziali API di Walmart](#connect-the-channel-to-walmart-marketplace).

1. [Impostazione completa del canale di vendita](#complete-store-setup) puoi gestire elenchi, scorte, prezzi e vendite da Channel Manager.

## Creare il canale di vendita

1. Apri Channel Manager.

   - In Admin, seleziona **[!UICONTROL Marketing** > _Canali _> **Channel Manager]**.

   - Seleziona **[!UICONTROL Connect New Store]**.

      ![Collega Commerce Store a [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/connect-commerce-store-to-marketplace.png)


1. Configura l&#39;archivio e la connessione:

   - Immettere un valore univoco **[!UICONTROL store name]**.

   - Seleziona la **[!UICONTROL Adobe Commerce site]** per gli elenchi dei prodotti.

   - Aggiungi un **[!UICONTROL email address]** per ricevere notifiche relative al servizio [!DNL Channel Manager].

      ![Configurare la connessione tra Commerce e [!DNL Walmart Marketplace] da [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

## Collegare il canale a Walmart Marketplace

1. Aggiungi le credenziali per [!DNL Walmart Marketplace Adobe Production API key] dal [!DNL Walmart Marketplace Seller] conto.

   - Se non disponi delle credenziali, seleziona **[!UICONTROL Get API credentials]** per ottenerli dal [!DNL Walmart Marketplace Developer Portal].

      Se richiesto, seleziona la tua area geografica (Stati Uniti e Canada), quindi effettua l’accesso.

      ![[!DNL Walmart Marketplace] accesso account](assets/walmart-marketplace-login-page.png)

   - Nel modulo della chiave API, copia e salva il **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]** per [!UICONTROL Adobe Inc Production API key] in una posizione sicura.

      ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Se la [!DNL Adobe Inc] la chiave non è elencata in Developer Portal, seleziona **[!UICONTROL Add New Key for a Solution Provider]** per configurare le autorizzazioni e generare la chiave. Per informazioni dettagliate sulla configurazione, consulta [Genera un [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key).

   - Torna a [!DNL Channel Manager] per aggiungere le credenziali al **[!UICONTROL Walmart Connection]** informazioni.

      Quando si aggiungono credenziali a [!DNL Channel Manager], Adobe nasconde il segreto client e memorizza il valore in un archivio protetto.

1. [!UICONTROL Save] la configurazione per stabilire la connessione.

   Dopo la connessione, gestisci il canale da **[!UICONTROL Channel Manager > Marketplace Stores]**.

   ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/manage-connected-stores.png)


### Risoluzione dei problemi di connessione

Se la connessione a Walmart non riesce, vedi la [Domande frequenti su Marketplace Walmart](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} per suggerimenti sulla risoluzione dei problemi.

- Da [!DNL Walmart Developer Portal], verifica di aver copiato le credenziali corrette per la chiave API di produzione per [!UICONTROL Adobe Inc.]

- Verifica che la configurazione di accesso per la chiave API di Adobe Walmart disponga delle autorizzazioni corrette. Vedi [Prerequisiti per Walmart](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key).

- Conferma che il servizio API Walmart sia disponibile dalla pagina [Pagina di stato API di Walmart](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.

## Configurazione completa dello store

Dopo aver collegato un negozio Commerce a [!DNL Walmart Marketplace], puoi completare la configurazione dello store dalla [!DNL Channel Manager Stores] visualizza.

Per completare la configurazione dello store:

1. Dall’amministratore, seleziona **[!UICONTROL Marketing** > **Channel Manager**].

   ![[!DNL Walmart Marketplace API key] pagina di configurazione](assets/connect-commerce-store-config.png)

1. Apri un canale di vendita connesso selezionando l&#39;icona a forma di matita in una riga di voce del negozio.

1. Inizia le operazioni dei canali di vendita.

   - [Aggiungere prodotti dal catalogo Commerce a Channel Manager](add-products-to-connected-channel.md)

   - [Pubblicare prodotti su Walmart utilizzando la corrispondenza dei prodotti](publish-listings-to-marketplace.md)

   - [Visualizza e gestisci inventario e prezzi](inventory-and-price-updates.md)

   - Visualizza e gestisci gli ordini Walmart dall’amministratore di Commerce
