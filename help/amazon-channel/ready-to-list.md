---
title: Canale di vendita Amazon - [!UICONTROL Ready to List]
description: Il canale di vendita Amazon fornisce la scheda Pronto per l’elenco per aiutarti a esaminare i prodotti Commerce che soddisfano i criteri di idoneità ma non vengono elencati automaticamente.
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

Il _[!UICONTROL Ready to List]_mostra il tuo [!DNL Commerce] catalogo prodotti che soddisfano le impostazioni dell’inserzione e sono pronti per essere pubblicati in Amazon as a **nuovo**elenco. A differenza di altre schede di inserzione, questa scheda non viene sempre visualizzata nella [_[!UICONTROL Product Listings]_](./managing-product-listings.md) pagina.

Il _[!UICONTROL Ready to List]_viene visualizzata solo quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`. Questa impostazione comunica al canale di vendita Amazon che qualsiasi nuova inserzione Amazon deve essere pubblicata manualmente.

Quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) è impostato su `Automatically List Eligible Products`, il canale di vendita Amazon pubblica automaticamente nuove inserzioni per i prodotti catalogo idonei. Poiché le nuove inserzioni vengono pubblicate automaticamente, _[!UICONTROL Ready to List]_non viene visualizzata.

Sotto _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: scegli di ripubblicare l’inserzione in [!DNL Amazon Marketplace]. Consulta [Pubblicare un’inserzione Amazon](./publish-listings-manually.md)

Sotto **[!UICONTROL Select]** nel _[!UICONTROL Action]_colonna:

- **[!UICONTROL Publish On Amazon]**: scegli di ripubblicare l’inserzione in [!DNL Amazon Marketplace]. Consulta [Pubblicare un’inserzione Amazon](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’inserzione, tra cui [Elenco registro attività](./product-listing-details.md#listing-activity-log), [Prezzi dei concorrenti Buy Box](./product-listing-details.md#buy-box-competitor-pricing), e [Prezzi più bassi per i concorrenti](./product-listing-details.md#lowest-competitor-pricing). Questa azione è solo per la visualizzazione. Non è possibile apportare modifiche ai dettagli dell&#39;inserzione. Consulta [Visualizza dettagli](./product-listing-details.md).

Sono disponibili alcune opzioni per l&#39;esecuzione manuale [pubblicare una nuova inserzione in Amazon](./publish-listings-manually.md).

>[!NOTE]
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Pronto per l&#39;elenco](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## Colonne predefinite

| Colonna | Descrizione |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN è l&#39;acronimo di [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Condition] | Il [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Il prezzo di listino del prodotto più il prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto è inserito nell’elenco attivo di Amazon. |
| [!UICONTROL Status] | Lo stato dell’inserzione, definito da Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** nel _[!UICONTROL Action]_e scegli un’opzione:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Cause comuni delle inserzioni pronte per l&#39;elenco

- **[!UICONTROL Ready to List]** - Il prodotto viene confrontato con un codice ASIN di Amazon ed è pianificato per l’inserimento nell’elenco. Se [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`, questo stato rappresenta i prodotti pronti per l’inserimento nell’elenco manuale.

- **[!UICONTROL List in Progress]** : l’elenco dei prodotti è stato inviato ad Amazon ed è in attesa della conferma di accettazione da parte di Amazon.
