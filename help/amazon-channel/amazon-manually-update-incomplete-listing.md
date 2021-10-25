---
title: Aggiorna informazioni richieste (elenco non completo)
description: Il canale di vendita di Amazon fornisce la scheda Incomplete per monitorare i prodotti del catalogo Commerce in cui mancano le informazioni richieste da Amazon.
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Aggiorna informazioni richieste (elenco incompleto)

Elenco visualizzato sul _[!UICONTROL Incomplete]_includi le [!DNL Commerce] cataloghi di prodotti che soddisfano i requisiti di idoneità di Amazon definiti nelle regole di elenco, ma per i quali mancano le informazioni richieste da Amazon prima dell’inserimento nell’elenco.

## Aggiorna le informazioni richieste (impossibile assegnarle all&#39;elenco Amazon) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Visualizza gli elenchi nella _[!UICONTROL Incomplete]_scheda in [Gestisci elenchi](./managing-product-listings.md).

1. In _[!UICONTROL Action]_colonna, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Assign ASIN]**, immetti l’ASIN assegnato da Amazon per l’elenco che desideri associare al prodotto catalogo.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

L’elenco viene ora associato al catalogo e l’elenco viene quindi aggiornato e pubblicato in Amazon in base alle impostazioni del cron e dell’elenco. Viene inoltre rimosso dalla _[!UICONTROL Incomplete]_scheda .

![Assegnazione manuale di ASIN per nessuna corrispondenza dell&#39;elenco](assets/amazon-listing-update-assign-asin.png)

## Aggiorna le informazioni richieste (Trovate più corrispondenze) {#update-required-info-multiple-matches-found}

1. Visualizza gli elenchi nella _[!UICONTROL Incomplete]_scheda in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. In _Azione_ colonna, fai clic su **Seleziona** > **Aggiorna informazioni richieste** per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli l&#39;ASIN corretto per l&#39;elenco che desideri associare a questo prodotto.

   Le opzioni elencate qui includono prodotti di catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, puoi scegliere `Manually Enter Correct ASIN` e immettere manualmente l&#39;ASIN per il prodotto.

1. Se si immette l&#39;ASIN manualmente, immettere l&#39;ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

![Selezionare manualmente ASIN da più corrispondenze possibili](assets/amazon-listing-update-multiple-matches.png)

## Aggiorna le informazioni richieste (ha varianti) {#update-required-info-has-variants}

1. Visualizza gli elenchi nella _[!UICONTROL Incomplete]_scheda in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. In _[!UICONTROL Action]_colonna, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli l&#39;ASIN corretto per l&#39;elenco che desideri associare a questo prodotto.

   Le opzioni elencate qui includono prodotti di catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, puoi selezionare `Manually Enter Correct ASIN` e immettere manualmente l&#39;ASIN per il prodotto.

1. Se si immette l&#39;ASIN manualmente, immettere l&#39;ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

![Selezionare manualmente ASIN da possibili corrispondenze a varianti](assets/amazon-listing-update-multiple-matches.png)

## Aggiorna le informazioni richieste (condizione mancante) {#update-required-info-missing-condition}

1. Visualizza gli elenchi nella _[!UICONTROL Incomplete]_scheda in [Gestisci elenchi](./managing-product-listings.md).

1. In _[!UICONTROL Action]_colonna, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Condition]**, scegli la condizione appropriata.

   L’elenco delle opzioni disponibili dipende dal [Condizione dell’elenco dei prodotti](./product-listing-condition.md) impostazioni.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]** .

![Aggiorna manualmente la condizione mancante](assets/amazon-update-listing-missing-condition.png)
