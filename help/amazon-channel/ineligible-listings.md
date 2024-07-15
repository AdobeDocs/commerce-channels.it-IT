---
title: Inserzioni Amazon non ammissibili
description: Il canale di vendita Amazon fornisce la scheda [!UICONTROL Ineligible] per aiutarti a gestire gli articoli che non sono idonei come inserzione in base alle tue regole di inserzione correnti.
feature: Sales Channels, Products
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Inserzioni Amazon non ammissibili

La scheda _[!UICONTROL Ineligible]_mostra un elenco di tutti i prodotti attualmente pubblicati su Amazon ma che non sono idonei come inserzioni in base alle regole di inserzione correnti. Se un prodotto precedente era idoneo e le regole di inserzione vengono modificate in modo da renderlo non idoneo, la quantità associata a un prodotto scende a 0 e il prodotto viene contrassegnato come_ non idoneo _. Tuttavia, è ancora presente in [!DNL Amazon Seller Account].

Per spostare un prodotto fuori dalla scheda _[!UICONTROL Ineligible]_, puoi [modificare le regole di inserzione](./listing-rules.md) per rendere i prodotti idonei.

Le azioni disponibili nella scheda _[!UICONTROL Ineligible]_includono:

In _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: scegliere di rimuovere tutte le inserzioni selezionate da [!DNL Amazon Marketplace]. Vedi [Terminare un&#39;inserzione Amazon](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: scegliere di modificare le impostazioni di sostituzione per l&#39;elenco. Vedi [Sostituzioni](./overrides.md) o [Modificare o rimuovere una sostituzione](./creating-editing-overrides.md#edit-override-single-listing).

In **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_:

- **[!UICONTROL View Details]**: scegliere di visualizzare i dettagli dell&#39;inserzione, tra cui il [Registro attività inserzione](./product-listing-details.md#listing-activity-log), il [Prezzo Buy Box concorrente](./product-listing-details.md#buy-box-competitor-pricing) e il [Prezzo concorrente più basso](./product-listing-details.md#lowest-competitor-pricing). Questa azione è solo per la visualizzazione. Non è possibile apportare modifiche ai dettagli dell&#39;inserzione. Vedi [Visualizza dettagli](./product-listing-details.md).

- **[!UICONTROL Create Override]**: scegliere di creare una sostituzione e applicarla a questa voce. Vedere [Creare un&#39;override](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: scegliere di modificare il codice ASIN assegnato al prodotto catalogo. Questa azione viene utilizzata se un prodotto nel catalogo ha restituito un codice ASIN errato. Vedi [Modifica un ASIN assegnato](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: scegliere di creare uno SKU alias da utilizzare per creare un&#39;inserzione Amazon dallo stesso prodotto catalogo. Consulta [Creare uno SKU del venditore di alias](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: scegliere di modificare il metodo di evasione associato all&#39;ordine. Vedere [Configurare le impostazioni di Evasione completata da](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: scegliere di rimuovere l&#39;inserzione da [!DNL Amazon Marketplace]. Vedi [Terminare un&#39;inserzione Amazon](./end-listings-manually.md).

>[!NOTE]
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Inserzioni Amazon non ammissibili](assets/amazon-ineligible-listings.png){width="600" zoomable="yes"}

Le home page del canale di vendita Amazon condividono alcuni [controlli dell&#39;area di lavoro](./workspace-controls.md) comuni che consentono di personalizzare i dati visualizzati.

## Colonne predefinite

| Colonna | Descrizione |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Il prezzo di listino del prodotto più il prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto è inserito nell’elenco attivo di Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un&#39;azione, fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e selezionare un&#39;opzione:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Crea sostituzione](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
