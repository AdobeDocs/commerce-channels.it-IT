---
title: Aggiorna informazioni richieste di Amazon
description: Il canale di vendita Amazon fornisce la scheda Incompleta per monitorare i prodotti del catalogo Commerce per i quali mancano le informazioni richieste da Amazon.
feature: Sales Channels, Merchandising, Catalog Management, Products
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Aggiorna informazioni richieste (elenco incompleto)

Le inserzioni visualizzate nella scheda _[!UICONTROL Incomplete]_includono i prodotti del catalogo [!DNL Commerce] che soddisfano i requisiti di idoneità di Amazon definiti nelle regole di inserzione, ma che non contengono le informazioni richieste da Amazon prima dell&#39;inserzione.

## Aggiorna le informazioni richieste (impossibile assegnarle all’elenco di Amazon) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Visualizza le inserzioni nella scheda _[!UICONTROL Incomplete]_in [Gestisci le inserzioni](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fare clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l&#39;elenco che si desidera aggiornare.

1. Esamina le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per le quali stai tentando di ottenere una corrispondenza con un’inserzione di Amazon.

1. Per **[!UICONTROL Assign ASIN]**, immettere il codice ASIN assegnato da Amazon per l&#39;elenco che si desidera associare al prodotto del catalogo.

1. Per salvare la corrispondenza del prodotto, fare clic su **[!UICONTROL Save Listing Update]**.

L’inserzione ora corrisponde al tuo catalogo e viene aggiornata e pubblicata in Amazon in base alle impostazioni della tua cron e dell’inserzione. È stato rimosso anche dalla scheda _[!UICONTROL Incomplete]_.

![Assegna manualmente ASIN per nessuna corrispondenza di elenco](assets/amazon-listing-update-assign-asin.png){width="600" zoomable="yes"}

## Aggiorna informazioni richieste (trovate più corrispondenze) {#update-required-info-multiple-matches-found}

1. Visualizza le inserzioni nella scheda _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Nella colonna _Azione_, fare clic su **Seleziona** > **Aggiorna informazioni richieste** per l&#39;elenco che si desidera aggiornare.

1. Esamina le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per le quali stai tentando di ottenere una corrispondenza con un’inserzione di Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli il codice ASIN corretto per l&#39;inserzione che desideri associare a questo prodotto.

   Le opzioni elencate includono i prodotti del catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, è possibile scegliere `Manually Enter Correct ASIN` e immettere manualmente il codice ASIN per il prodotto.

1. Se si immette manualmente il codice ASIN, immettere il codice ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fare clic su **[!UICONTROL Save Listing Update]**.

![Seleziona manualmente il codice ASIN da più corrispondenze possibili](assets/amazon-listing-update-multiple-matches.png){width="600" zoomable="yes"}

## Aggiorna informazioni richieste (con varianti) {#update-required-info-has-variants}

1. Visualizza le inserzioni nella scheda _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fare clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l&#39;elenco che si desidera aggiornare.

1. Esamina le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per le quali stai tentando di ottenere una corrispondenza con un’inserzione di Amazon.

1. Per **[!UICONTROL Select Correct Amazon Listing]**, scegli il codice ASIN corretto per l&#39;inserzione che desideri associare a questo prodotto.

   Le opzioni elencate includono i prodotti del catalogo identificati come possibili corrispondenze. Se nessuna delle opzioni è corretta, è possibile selezionare `Manually Enter Correct ASIN` e immettere manualmente il codice ASIN per il prodotto.

1. Se si immette manualmente il codice ASIN, immettere il codice ASIN corretto per **[!UICONTROL Manually Assign ASIN]**.

1. Per salvare la corrispondenza del prodotto, fare clic su **[!UICONTROL Save Listing Update]**.

## Aggiorna informazioni richieste (condizione mancante) {#update-required-info-missing-condition}

1. Visualizza le inserzioni nella scheda _[!UICONTROL Incomplete]_in [Gestisci le inserzioni](./managing-product-listings.md).

1. Nella colonna _[!UICONTROL Action]_, fare clic su **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**per l&#39;elenco che si desidera aggiornare.

1. Esamina le informazioni sul prodotto del catalogo (SKU e Nome prodotto) per le quali stai tentando di ottenere una corrispondenza con un’inserzione di Amazon.

1. Per **[!UICONTROL Condition]**, scegliere la condizione appropriata.

   L&#39;elenco delle opzioni disponibili dipende dalle impostazioni della [condizione dell&#39;elenco prodotti](./product-listing-condition.md).

1. Per salvare la corrispondenza del prodotto, fare clic su **[!UICONTROL Save Listing Update]**.

![Aggiorna manualmente la condizione mancante](assets/amazon-update-listing-missing-condition.png){width="600" zoomable="yes"}
