---
title: Aggiungi prodotti all'archivio canali di vendita
description: Crea assortimento di prodotti per [!DNL Walmart Marketplace] vendite aggiungendo prodotti dal catalogo al canale di vendita
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: ee103895e1035e04a4601857032caa172d493a31
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Aggiungi prodotti all&#39;archivio canali di vendita

Per sincronizzare i prodotti con il canale di vendita Walmart Marketplace, seleziona i prodotti dalla [!DNL Commerce] catalogo dei prodotti e importarli in Channel Manager. I prodotti selezionati devono avere la seguente configurazione di attributi:

- **[!UICONTROL Publish to Channel Manager]** attributo abilitato

- Almeno un attributo di prodotto deve corrispondere a uno degli [attributi richiesti di Walmart Marketplace](map-catalog-attributes.md)-GTIN, ISBN, ISSN, UPC, EAN

Il processo da cui importare i prodotti [!DNL Commerce] al Channel Manager può richiedere fino a 30 minuti o più a seconda del numero di prodotti selezionati.

## Aggiungi prodotti

1. Da un negozio di canali di vendita collegati, seleziona **Aggiungi prodotti** per aprire il catalogo dei prodotti.

   ![Aggiungi prodotti all&#39;archivio canali di vendita](assets/add-initial-products-to-connected-channel.png)

   Il catalogo si apre in una nuova scheda.

1. Dalla griglia del prodotto di catalogo, selezionare i prodotti su cui vendere [!DNL Walmart Marketplace].

   ![Invia prodotti al negozio di canali di vendita](assets/select-products-from-catalog.png)

1. Abilita la **[!UICONTROL Publish to Channel Manager]** per gli elementi selezionati.

   - Da **[!UICONTROL Actions]**, seleziona **[!UICONTROL Update attributes]**.

   - Scorri fino a **[!UICONTROL Publish to Channel Manager]** e attivarlo.

   - Verifica che gli attributi del prodotto includano almeno uno degli ID di prodotto Walmart richiesti.

   - Seleziona **[!UICONTROL Save]**.

      Viene visualizzato un messaggio di conferma.

      ![Importazione di prodotti dal catalogo al messaggio di conferma del canale di vendita](assets/product-import-from-catalog-confirmation.png)

      Se il messaggio indica che l’aggiornamento è pianificato, utilizza la [coda:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] per elaborare immediatamente l&#39;aggiornamento.

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. Al termine dell’operazione di importazione, verifica i prodotti aggiunti tornando a [!DNL Channel Manager] e selezionando **[!UICONTROL Listings]**.

   ![Prodotti importati in un canale di vendita collegato](assets/products-in-marketplace-sales-channel.png)

   Inizialmente, i prodotti sono in *Bozza* stato. Seleziona **[!UICONTROL Refresh products]** per aggiornare la tabella.

