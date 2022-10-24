---
title: Aggiungi prodotti a Channel Manager
description: '''Crea assortimento di prodotti per [!DNL Walmart Marketplace] vendite aggiungendo prodotti dal catalogo al canale di vendita configurato in Channel Manager." '
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: bc9badeed0f8b5dd6a4fad2633c06c917f7d9d90
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Aggiungi prodotti a [!DNL Channel Manager]

Per aggiungere prodotti al [!DNL Walmart Marketplace] canale di vendita, selezionali dal [!DNL Commerce] catalogo dei prodotti e importarli in [!DNL Channel Manager].
Il processo di importazione può richiedere fino a 30 minuti o più a seconda del numero di prodotti selezionati.

## Prerequisito

**[Mappare gli attributi del catalogo](map-catalog-attributes.md)**—Nel [!DNL Channel Settings] configurazione, mappare almeno un attributo [!DNL Commerce] catalogo di prodotto per uno degli identificatori di prodotto Walmart richiesti:-GTIN, ISBN, ISSN, UPC, EAN.

## Requisiti dell&#39;elenco

[!DNL Commerce] gli elenchi di prodotti devono avere la seguente configurazione di attributi obbligatoria:

- **[!UICONTROL Connect to Channel Manager]** attributo abilitato

- Fornire valori validi per gli attributi Walmart richiesti.

   - Almeno un attributo di prodotto che corrisponde a uno dei requisiti richiesti [!DNL Walmart Marketplace] identificatori del prodotto-GTIN, ISBN, ISSN, UPC, EAN.

   - Prezzo del prodotto specificato a un massimo di due cifre decimali, ad esempio `9.99`

   - Peso del prodotto specificato a un massimo di due cifre decimali, ad esempio `1.25`

>[!TIP]
>
>Per ulteriori informazioni sull&#39;ottimizzazione delle inserzioni per il canale di vendita, consulta [Guida all’ottimizzazione della qualità dell’elenco di marketplace Walmart](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Aggiungi prodotti

1. Da un negozio di canali di vendita collegati, seleziona **Aggiungi prodotti** per aprire il catalogo dei prodotti.

   ![Aggiungi prodotti all&#39;archivio canali di vendita](assets/add-initial-products-to-connected-channel.png)

   Il catalogo si apre in una nuova scheda.

1. Dalla griglia del prodotto di catalogo, selezionare i prodotti su cui vendere [!DNL Walmart Marketplace].

   ![Invia prodotti al negozio di canali di vendita](assets/select-products-from-catalog.png)

1. Abilita la **[!UICONTROL Connect to Channel Manager]** per gli elementi selezionati.

   - Da **[!UICONTROL Actions]**, seleziona **[!UICONTROL Update attributes]**.

   - Scorri fino a **[!UICONTROL Connect to Channel Manager]** e attivarlo.

   - Verifica che gli attributi del prodotto includano almeno uno dei requisiti [!DNL Walmart Product IDs].

   - Seleziona **[!UICONTROL Save]**.

      Viene visualizzato un messaggio di conferma.

      ![Importazione di prodotti dal catalogo al messaggio di conferma del canale di vendita](assets/product-import-from-catalog-confirmation.png)

      Se il messaggio indica che l’aggiornamento è pianificato, utilizza la [coda:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] per elaborare immediatamente l&#39;aggiornamento.

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. Al termine dell’operazione di importazione, verifica i prodotti aggiunti tornando a [!DNL Channel Manager] e selezionando **[!UICONTROL Listings]**.

   Inizialmente, i prodotti sono in *Bozza* stato. Seleziona **[!UICONTROL Refresh products]** per aggiornare la tabella.

1. Aggiorna la visualizzazione per mostrare i nuovi prodotti aggiunti a Channel Manager selezionando la **[!UICONTROL Draft]** scheda di stato.

   ![Prodotti importati in un canale di vendita collegato](assets/products-in-marketplace-sales-channel.png)


