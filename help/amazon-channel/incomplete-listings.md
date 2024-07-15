---
title: Inserzioni Amazon incomplete
description: Il canale di vendita Amazon fornisce la scheda [!UICONTROL Incomplete] per aiutarti a identificare e soddisfare i requisiti di idoneità per le inserzioni Amazon incomplete.
feature: Sales Channels, Products
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Inserzioni Amazon incomplete

Nella scheda _[!UICONTROL Incomplete]_sono elencati i prodotti del catalogo [!DNL Commerce] che soddisfano i requisiti di idoneità di Amazon (definiti nelle [regole per l&#39;elenco](./listing-rules.md)), ma mancano le informazioni richieste da Amazon (ad esempio Amazon ASIN o una condizione di prodotto definita).

Ci sono quattro possibili cause per un&#39;inserzione incompleta, ciascuna identificata dal suo stato.

| Stato | Motivo | Azione |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Condizione mancante | Amazon accetta le inserzioni in varie condizioni (ad esempio _New_, _Refurbished_, _Used: Like New_). L&#39;inserzione richiede una condizione definita. | Aggiorna le informazioni richieste e [assegna manualmente una condizione](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) a un&#39;inserzione. |
| Impossibile assegnare all’elenco di Amazon | Corrispondenza automatica dell&#39;inserzione al catalogo non riuscita. Se non viene trovata alcuna corrispondenza, l’inserzione non può essere gestita dal Sales Channel Amazon | Aggiorna le informazioni richieste e [assegna manualmente un codice ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) al prodotto del catalogo per la corrispondenza all&#39;elenco. |
| Più corrispondenze trovate | Corrispondenza automatica dell&#39;inserzione al catalogo non riuscita. Se vengono trovate più corrispondenze possibili, devi selezionare la corrispondenza corretta per il prodotto. | Aggiorna le informazioni richieste e [scegli manualmente una corrispondenza di prodotto](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) per il prodotto e l&#39;inserzione. |
| Ha Varianti | Se il prodotto dispone di varianti, ad esempio una t-shirt disponibile in diverse dimensioni o colori, devi scegliere la variante nel catalogo per assegnarla correttamente e farla corrispondere all’inserzione | Aggiorna le informazioni richieste e [scegli manualmente la variante corretta](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) da assegnare e abbinare a questa inserzione. |

>[!NOTE]
>Quando le inserzioni incomplete vengono associate correttamente ai prodotti del catalogo, vengono spostate dalla scheda _[!UICONTROL Incomplete]_e pubblicate in Amazon in base alle impostazioni di [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md).

Le azioni disponibili nella scheda _[!UICONTROL Incomplete]_includono:

In _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: scegliere di avviare il processo automatico per la corrispondenza dei dati delle inserzioni Amazon con il catalogo [!DNL Commerce]. Se i prodotti non corrispondono automaticamente, rivedi le opzioni [_[!UICONTROL Catalog Search]_](./catalog-search.md) nelle tue lettere di inserzione. Se le inserzioni non corrispondono automaticamente dopo l&#39;aggiornamento delle opzioni di _[!UICONTROL Catalog Search]_, è possibile abbinare i prodotti manualmente nell&#39;azione [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found).

In **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_:

- **[!UICONTROL Update Required Info]**: scegli quando le inserzioni non corrispondono automaticamente al tuo catalogo. Puoi [abbinare manualmente i prodotti del catalogo alle inserzioni](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), [assegnare manualmente un codice ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) a una corrispondenza del catalogo o [assegnare una condizione mancante](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) per l&#39;inserzione.

- **[!UICONTROL View Details]**: scegliere di visualizzare i dettagli dell&#39;inserzione, tra cui il [Registro attività inserzione](./product-listing-details.md#listing-activity-log), il [Prezzo Buy Box concorrente](./product-listing-details.md#buy-box-competitor-pricing) e il [Prezzo concorrente più basso](./product-listing-details.md#lowest-competitor-pricing). Questa azione è solo per la visualizzazione. Non è possibile apportare modifiche ai dettagli dell&#39;inserzione. Vedi [Visualizza dettagli](./product-listing-details.md).

>[!NOTE]
>
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Inserzioni Amazon incomplete](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Le home page del canale di vendita Amazon condividono alcuni [controlli dell&#39;area di lavoro](./workspace-controls.md) comuni che consentono di personalizzare i dati visualizzati.

| Colonna | Descrizione |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Il prezzo di listino del prodotto più il prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto è inserito nell’elenco attivo di Amazon. |
| [!UICONTROL Status] | Lo stato dell’inserzione, definito da Amazon. Vedi la tabella Stato sopra. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un&#39;azione, fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e selezionare un&#39;opzione:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
