---
title: Canale di vendita Amazon - [!UICONTROL Ready to List]
description: Il canale di vendita Amazon fornisce la scheda Pronto per l’elenco per aiutarti a esaminare i prodotti Commerce che soddisfano i requisiti di idoneità ma che non vengono elencati automaticamente.
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

La scheda _[!UICONTROL Ready to List]_mostra i prodotti del catalogo [!DNL Commerce] che soddisfano le impostazioni dell&#39;inserzione e sono pronti per essere pubblicati in Amazon come **nuova**inserzione. A differenza di altre schede dell&#39;elenco, questa scheda non viene sempre visualizzata nella pagina [_[!UICONTROL Product Listings]_](./managing-product-listings.md).

La scheda _[!UICONTROL Ready to List]_viene visualizzata solo quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`. Questa impostazione comunica al canale di vendita Amazon che qualsiasi nuova inserzione Amazon deve essere pubblicata manualmente.

Quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) è impostato su `Automatically List Eligible Products`, il canale di vendita Amazon pubblica automaticamente nuove inserzioni per i prodotti catalogo idonei. Poiché le nuove inserzioni vengono pubblicate automaticamente, la scheda _[!UICONTROL Ready to List]_non viene visualizzata.

In _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: scegliere di ripubblicare l&#39;inserzione in [!DNL Amazon Marketplace]. Vedi [Elenco di Publish e Amazon](./publish-listings-manually.md)

In **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_:

- **[!UICONTROL Publish On Amazon]**: scegliere di ripubblicare l&#39;inserzione in [!DNL Amazon Marketplace]. Vedi [Elenco di Publish e Amazon](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: scegliere di visualizzare i dettagli dell&#39;inserzione, tra cui il [Registro attività inserzione](./product-listing-details.md#listing-activity-log), il [Prezzo Buy Box concorrente](./product-listing-details.md#buy-box-competitor-pricing) e il [Prezzo concorrente più basso](./product-listing-details.md#lowest-competitor-pricing). Questa azione è solo per la visualizzazione. Non è possibile apportare modifiche ai dettagli dell&#39;inserzione. Vedi [Visualizza dettagli](./product-listing-details.md).

Sono disponibili alcune opzioni per [pubblicare manualmente una nuova inserzione in Amazon](./publish-listings-manually.md).

>[!NOTE]
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Pronto per l&#39;elenco](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## Colonne predefinite

| Colonna | Descrizione |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Il prezzo di listino del prodotto più il prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto è inserito nell’elenco attivo di Amazon. |
| [!UICONTROL Status] | Lo stato dell’inserzione, definito da Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un&#39;azione, fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e scegliere un&#39;opzione:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Cause comuni delle inserzioni pronte per l&#39;elenco

- **[!UICONTROL Ready to List]** - Il prodotto corrisponde a un ASIN di Amazon ed è pianificato per l&#39;inserimento nell&#39;elenco. Se [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`, questo stato rappresenta i prodotti pronti per essere inseriti manualmente nell&#39;elenco.

- **[!UICONTROL List in Progress]** - L&#39;elenco dei prodotti è stato inviato ad Amazon ed è in attesa di conferma da parte di Amazon.
