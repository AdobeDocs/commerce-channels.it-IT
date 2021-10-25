---
title: Inserzioni non ammissibili
description: Il canale di vendita Amazon fornisce [!UICONTROL Ineligible] per facilitare la gestione degli elementi, non è idoneo come elenco in base alle regole di elenco correnti.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Elencazioni non ammissibili

La _[!UICONTROL Ineligible]_Visualizza un elenco di tutti i prodotti attualmente pubblicati su Amazon ma non idonei come elenco in base alle regole di elenco correnti. Se un prodotto precedente era idoneo e le regole di elenco vengono modificate per renderlo non idoneo, la quantità associata a un prodotto scende a 0 e il prodotto viene contrassegnato come_ non idoneo _. Tuttavia, è ancora presente sul tuo [!DNL Amazon Seller Account].

Per spostare un prodotto fuori da _[!UICONTROL Ineligible]_è possibile [modificare le regole di inserzione](./listing-rules.md) per consentire l’idoneità dei prodotti.

Le azioni disponibili sul _[!UICONTROL Ineligible]_include:

Sotto _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Scegli di rimuovere tutte le inserzioni selezionate dalla [!DNL Amazon Marketplace]. Vedi [Termina un elenco Amazon](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Scegliere di modificare le impostazioni di sostituzione per l&#39;elenco. Vedi [Sostituzioni](./overrides.md) o [Modificare o rimuovere un override](./creating-editing-overrides.md#edit-override-single-listing).

Sotto **[!UICONTROL Select]** in _[!UICONTROL Action]_colonna:

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’elenco, tra cui [Elenco del registro delle attività](./product-listing-details.md#listing-activity-log), [Prezzi concorrenza Buy Box](./product-listing-details.md#buy-box-competitor-pricing)e [Prezzi più bassi per i concorrenti](./product-listing-details.md#lowest-competitor-pricing). Questa azione è disponibile solo per la visualizzazione. Non è possibile apportare modifiche nei dettagli dell’elenco. Vedi [Visualizza dettagli](./product-listing-details.md).

- **[!UICONTROL Create Override]**: scegli di creare una sostituzione e di applicarla a questa inserzione. Vedi [Creare un override](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: scegli di modificare l’ASIN assegnato al prodotto del catalogo. Questa azione viene utilizzata se un prodotto del catalogo è stato confrontato con un ASIN errato. Vedi [Modificare un ASIN assegnato](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: scegli di creare uno SKU alias che possa essere utilizzato per creare un elenco Amazon dallo stesso prodotto catalogo. Vedi [Creare una SKU del venditore di alias](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: scegli di modificare il metodo di evasione associato all’ordine. Vedi [Configura le impostazioni di Fulmine By](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: scegli di rimuovere l’elenco dalla [!DNL Amazon Marketplace]. Vedi [Termina un elenco Amazon](./end-listings-manually.md).

>[!NOTE]
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Elenchi Amazon non consentiti](assets/amazon-ineligible-listings.png)

Le home page del canale di vendita Amazon condividono alcune [controlli dell&#39;area di lavoro](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

## Colonne predefinite

| Colonna | Descrizione |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Prezzo di listino del prodotto più il suo prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto viene inserito nell’elenco attivo in Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_e seleziona un’opzione:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Crea sostituzione](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
