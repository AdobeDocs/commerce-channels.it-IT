---
title: Aggiungere prodotti a Channel Manager
description: "Crea assortimento di prodotti per [!DNL Walmart Marketplace] vendite aggiungendo prodotti dal catalogo al canale di vendita configurato in Channel Manager."
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Aggiungi prodotti a [!DNL Channel Manager]

Per aggiungere prodotti al [!DNL Walmart Marketplace] canale di vendita, selezionali dall&#39; [!DNL Commerce] catalogo dei prodotti e importali in [!DNL Channel Manager].
Il processo di importazione può richiedere fino a 30 minuti o più, a seconda del numero di prodotti selezionati.

## Prerequisito

**[Mappa attributi catalogo](map-catalog-attributes.md)**- Nella [!DNL Channel Settings] , mappa almeno un attributo da [!DNL Commerce] uno degli identificatori di prodotto Walmart richiesti:-GTIN, ISBN, ISSN, UPC, EAN.

## Requisiti dell’inserzione

[!DNL Commerce] gli elenchi di prodotti devono avere la seguente configurazione di attributi richiesta:

- **[!UICONTROL Connect to Channel Manager]** l&#39;attributo è abilitato

- Fornire valori validi per gli attributi Walmart richiesti.

   - Almeno un attributo di prodotto che corrisponde a uno degli attributi richiesti [!DNL Walmart Marketplace] identificatori di prodotto-GTIN, ISBN, ISSN, UPC, EAN.

   - Prezzo del prodotto specificato con un massimo di due cifre decimali, ad esempio `9.99`

   - Peso del prodotto specificato fino a un massimo di due cifre decimali, ad esempio `1.25`

>[!TIP]
>
>Per ulteriori informazioni sull&#39;ottimizzazione delle inserzioni per il tuo canale di vendita, vedi [Guida all&#39;ottimizzazione della qualità dell&#39;elenco di Walmart Marketplace](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Aggiungi prodotti

1. Da un negozio di canali di vendita collegato, seleziona **Aggiungi prodotti** per aprire il catalogo prodotti.

   ![Aggiungi prodotti al negozio del canale di vendita](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   Il catalogo viene aperto in una nuova scheda.

1. Dalla griglia prodotti del catalogo, seleziona i prodotti su cui vendere [!DNL Walmart Marketplace].

   ![Invia prodotti al negozio del canale di vendita](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. Abilita **[!UICONTROL Connect to Channel Manager]** per gli elementi selezionati.

   - Da **[!UICONTROL Actions]**, seleziona **[!UICONTROL Update attributes]**.

   - Scorri fino a **[!UICONTROL Connect to Channel Manager]** e abilitarlo.

   - Verifica che gli attributi del prodotto includano almeno uno degli attributi richiesti [!DNL Walmart Product IDs].

   - Seleziona **[!UICONTROL Save]**.

     Viene visualizzato un messaggio di conferma.

     ![Messaggio di conferma dell’importazione del prodotto dal catalogo al canale di vendita](assets/product-import-from-catalog-confirmation.png){width="400"}

     Se il messaggio indica che l’aggiornamento è pianificato, utilizza [`queue:consumers:start`](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] per elaborare immediatamente l&#39;aggiornamento.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. Al termine dell’operazione di importazione, verifica i prodotti aggiunti tornando a [!DNL Channel Manager] e selezione **[!UICONTROL Listings]**.

   Inizialmente, i prodotti sono in *Bozza* stato. Seleziona **[!UICONTROL Refresh products]** per aggiornare la tabella.

1. Aggiornare la visualizzazione per mostrare i nuovi prodotti aggiunti a Channel Manager selezionando la **[!UICONTROL Draft]** scheda di stato.

   ![Prodotti importati nel canale di vendita connesso](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


