---
title: Pronto per l'elenco
description: Il canale di vendita Amazon fornisce la scheda Pronto per l’elenco per aiutarti a esaminare i prodotti Commerce che soddisfano i requisiti di idoneità ma che non sono elencati automaticamente.
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

La _[!UICONTROL Ready to List]_la scheda mostra le [!DNL Commerce] catalogo di prodotti che soddisfano le impostazioni dell’elenco e sono pronti per la pubblicazione in Amazon as a **nuovo**elenco. A differenza di altre schede dell’elenco, questa scheda non viene sempre visualizzata nella scheda [_[!UICONTROL Product Listings]_](./managing-product-listings.md) pagina.

La _[!UICONTROL Ready to List]_viene visualizzata solo quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`. Questa impostazione comunica al canale di vendita Amazon che tutti i nuovi elenchi di Amazon devono essere pubblicati manualmente.

Quando [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) è impostato su `Automatically List Eligible Products`, il canale di vendita Amazon pubblica automaticamente nuovi annunci per i prodotti di catalogo idonei. Poiché i nuovi elenchi vengono pubblicati automaticamente, la variabile _[!UICONTROL Ready to List]_la scheda non viene visualizzata.

Sotto _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: Scegliere di ripubblicare l&#39;elenco nel [!DNL Amazon Marketplace]. Vedi [Pubblicare un elenco Amazon](./publish-listings-manually.md)

Sotto **[!UICONTROL Select]** in _[!UICONTROL Action]_colonna:

- **[!UICONTROL Publish On Amazon]**: Scegliere di ripubblicare l&#39;elenco nel [!DNL Amazon Marketplace]. Vedi [Pubblicare un elenco Amazon](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’elenco, tra cui [Elenco del registro delle attività](./product-listing-details.md#listing-activity-log), [Prezzi concorrenza Buy Box](./product-listing-details.md#buy-box-competitor-pricing)e [Prezzi più bassi per i concorrenti](./product-listing-details.md#lowest-competitor-pricing). Questa azione è disponibile solo per la visualizzazione. Non è possibile apportare modifiche nei dettagli dell’elenco. Vedi [Visualizza dettagli](./product-listing-details.md).

Hai alcune opzioni da usare manualmente [pubblicare un nuovo elenco in Amazon](./publish-listings-manually.md).

>[!NOTE]
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Pronto per l&#39;elenco](assets/amazon-ready-to-list.png)

## Colonne predefinite

| Colonna | Descrizione |
|---|---|
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Prezzo di listino del prodotto più il suo prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto viene inserito nell’elenco attivo in Amazon. |
| [!UICONTROL Status] | Lo stato dell’elenco, definito da Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_e scegli un’opzione:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Cause comuni di elenchi pronti per l’elenco

- **[!UICONTROL Ready to List]** - Il prodotto viene associato a un ASIN di Amazon ed è pianificato per l’inserimento nell’elenco. Se [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) nelle impostazioni dell&#39;inserzione è impostato su `Do Not Automatically List Eligible Products`, questo stato rappresenta i prodotti pronti per essere elencati manualmente.

- **[!UICONTROL List in Progress]** - L’elenco dei prodotti è stato inviato ad Amazon ed è in attesa di conferma da parte di Amazon.
