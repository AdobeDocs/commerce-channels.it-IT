---
title: Inserzioni non ammissibili
description: Il canale di vendita Amazon fornisce la scheda [!UICONTROL Ineligible] per aiutarti a gestire gli articoli non idonei come inserzione in base alle regole di inserzione correnti.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Elencazioni non ammissibili

La scheda _[!UICONTROL Ineligible]_mostra un elenco di tutti i prodotti attualmente pubblicati su Amazon ma non idonei come elenco in base alle regole di elenco correnti. Se un prodotto precedente era idoneo e le regole di elenco vengono modificate per renderlo non idoneo, la quantità associata a un prodotto scende a 0 e il prodotto viene contrassegnato come_ non idoneo _. Tuttavia, è ancora presente sul [!DNL Amazon Seller Account].

Per spostare un prodotto dalla scheda _[!UICONTROL Ineligible]_, puoi [modificare le regole di inserzione](./listing-rules.md) per consentire l&#39;idoneità dei prodotti.

Le azioni disponibili nella scheda _[!UICONTROL Ineligible]_includono:

Alla voce _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Scegli di rimuovere tutti gli elenchi selezionati dal  [!DNL Amazon Marketplace]. Consulta [Terminare un elenco Amazon](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Scegliere di modificare le impostazioni di sostituzione per l&#39;elenco. Consulta [Ignorazioni](./overrides.md) o [Modificare o rimuovere un override](./creating-editing-overrides.md#edit-override-single-listing).

Sotto **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_:

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’elenco, tra cui il  [Registro attività dell’elenco](./product-listing-details.md#listing-activity-log), i prezzi dei concorrenti di  [Buy Box](./product-listing-details.md#buy-box-competitor-pricing) e i prezzi dei concorrenti  [più bassi](./product-listing-details.md#lowest-competitor-pricing). Questa azione è disponibile solo per la visualizzazione. Non è possibile apportare modifiche nei dettagli dell’elenco. Vedere [Visualizza dettagli](./product-listing-details.md).

- **[!UICONTROL Create Override]**: scegli di creare una sostituzione e di applicarla a questa inserzione. Consulta [Creare un override](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: scegli di modificare l’ASIN assegnato al prodotto del catalogo. Questa azione viene utilizzata se un prodotto del catalogo è stato confrontato con un ASIN errato. Vedere [Modifica di un&#39;ASIN assegnata](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: scegli di creare uno SKU alias che possa essere utilizzato per creare un elenco Amazon dallo stesso prodotto catalogo. Consulta [Creare uno SKU per i venditori alias](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: scegli di modificare il metodo di evasione associato all’ordine. Consultare [Configurare le impostazioni soddisfatte da](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: scegli di rimuovere l’elenco da  [!DNL Amazon Marketplace]. Consulta [Terminare un elenco Amazon](./end-listings-manually.md).

>[!NOTE]
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Elenchi Amazon non consentiti](assets/amazon-ineligible-listings.png)

Le home page del canale di vendita Amazon condividono alcuni controlli comuni [workspace](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

## Colonne predefinite

| Colonna | Descrizione |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per  [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Prezzo di listino del prodotto più il suo prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto viene inserito nell’elenco attivo in Amazon. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e seleziona un’opzione:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Crea sostituzione](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
