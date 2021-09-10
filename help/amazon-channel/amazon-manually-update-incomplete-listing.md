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

Gli elenchi visualizzati nella scheda _[!UICONTROL Incomplete]_includono i prodotti di catalogo [!DNL Commerce] che soddisfano i requisiti di idoneità di Amazon definiti nelle regole di elenco, ma che non contengono le informazioni richieste da Amazon prima dell’inserimento nell’elenco.

## Aggiorna le informazioni richieste (impossibile assegnarle all&#39;elenco Amazon) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Visualizza gli elenchi nella scheda _[!UICONTROL Incomplete]_in [Gestisci elenchi](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Assign ASIN]**, immetti l’ASIN assegnato da Amazon per l’elenco da abbinare al prodotto del catalogo.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

L’elenco viene ora associato al catalogo e l’elenco viene quindi aggiornato e pubblicato in Amazon in base alle impostazioni del cron e dell’elenco. Viene inoltre rimosso dalla scheda _[!UICONTROL Incomplete]_.

![Assegnazione manuale di ASIN per nessuna corrispondenza dell&#39;elenco](assets/amazon-listing-update-assign-asin.png)

## Aggiorna le informazioni richieste (Trovate più corrispondenze) {#update-required-info-multiple-matches-found}

1. Visualizza gli elenchi nella scheda _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Nella colonna _Azione_, fai clic su **Seleziona** > **Aggiorna informazioni richieste** per l&#39;elenco che desideri aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli l’ASIN corretto per l’elenco a cui desideri associare il prodotto.

   Le opzioni elencate qui includono prodotti di catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, è possibile scegliere `Manually Enter Correct ASIN` e immettere manualmente l&#39;ASIN per il prodotto.

1. Se si immette l&#39;ASIN manualmente, immettere l&#39;ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

![Selezionare manualmente ASIN da più corrispondenze possibili](assets/amazon-listing-update-multiple-matches.png)

## Aggiorna le informazioni richieste (ha varianti) {#update-required-info-has-variants}

1. Visualizza gli elenchi nella scheda _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli l’ASIN corretto per l’elenco a cui desideri associare il prodotto.

   Le opzioni elencate qui includono prodotti di catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, è possibile selezionare `Manually Enter Correct ASIN` e immettere manualmente l&#39;ASIN per il prodotto.

1. Se si immette l&#39;ASIN manualmente, immettere l&#39;ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]**.

![Selezionare manualmente ASIN da possibili corrispondenze a varianti](assets/amazon-listing-update-multiple-matches.png)

## Aggiorna le informazioni richieste (condizione mancante) {#update-required-info-missing-condition}

1. Visualizza gli elenchi nella scheda _[!UICONTROL Incomplete]_in [Gestisci elenchi](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l’elenco da aggiornare.

1. Controlla le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per cui stai cercando di trovare una corrispondenza con un elenco Amazon.

1. Per **[!UICONTROL Condition]**, scegli la condizione appropriata.

   L&#39;elenco delle opzioni disponibili dipende dalle impostazioni [Product Listing Condition](./product-listing-condition.md).

1. Per salvare la corrispondenza del prodotto, fai clic su **[!UICONTROL Save Listing Update]** .

![Aggiorna manualmente la condizione mancante](assets/amazon-update-listing-missing-condition.png)
