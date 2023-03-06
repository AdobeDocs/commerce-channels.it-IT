---
title: Inserzioni incomplete
description: Il canale di vendita Amazon offre [!UICONTROL Incomplete] per identificare e soddisfare i requisiti di idoneità per le inserzioni incomplete in Amazon.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Inserzioni incomplete

Il _[!UICONTROL Incomplete]_elenca le opzioni [!DNL Commerce] catalogare prodotti che soddisfano i requisiti di idoneità di Amazon (definiti nel [regole di inserzione](./listing-rules.md)), ma mancano le informazioni richieste da Amazon (ad esempio Amazon ASIN o una condizione di prodotto definita).

Ci sono quattro possibili cause per un&#39;inserzione incompleta, ciascuna identificata dal suo stato.

| Stato | Motivo | Azione |
|--- |--- |--- |
| Condizione mancante | Amazon accetta le inserzioni in varie condizioni (ad esempio _Nuovo_, _Rinnovato_, _Usato: Come nuovo_) richiede una condizione definita. | Aggiorna le informazioni richieste e manualmente [assegna una condizione](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) in un&#39;inserzione. |
| Impossibile assegnare all’elenco di Amazon | Corrispondenza automatica dell&#39;inserzione al catalogo non riuscita. Se non viene trovata alcuna corrispondenza, l’inserzione non può essere gestita dal Sales Channel Amazon | Aggiorna le informazioni richieste e manualmente [assegna un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) al prodotto di catalogo per la corrispondenza con l’inserzione. |
| Più corrispondenze trovate | Corrispondenza automatica dell&#39;inserzione al catalogo non riuscita. Se vengono trovate più corrispondenze possibili, devi selezionare la corrispondenza corretta per il prodotto. | Aggiorna le informazioni richieste e manualmente [scegli una corrispondenza prodotto](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) per il prodotto e l’inserzione. |
| Ha Varianti | Se il prodotto dispone di varianti, ad esempio una t-shirt disponibile in diverse dimensioni o colori, devi scegliere la variante nel catalogo per assegnarla correttamente e farla corrispondere all’inserzione | Aggiorna le informazioni richieste e manualmente [scegli la variante corretta](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) per assegnare e corrispondere a questa inserzione. |

>[!NOTE]
>Quando le inserzioni incomplete vengono associate correttamente ai prodotti del catalogo, l&#39;inserzione si sposta dal _[!UICONTROL Incomplete]_e vengono pubblicati in Amazon in base al [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni.

Le azioni disponibili sul _[!UICONTROL Incomplete]_La scheda include:

Sotto _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: scegli di avviare il processo automatico per la corrispondenza dei dati delle inserzioni Amazon con i tuoi [!DNL Commerce] catalogo. Se i prodotti non corrispondono automaticamente, rivedi il [_[!UICONTROL Catalog Search]_](./catalog-search.md) opzioni nelle lettere dell&#39;inserzione. Se le inserzioni non corrispondono automaticamente dopo l&#39;aggiornamento _[!UICONTROL Catalog Search]_, è possibile far corrispondere i prodotti manualmente in [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) azione.

Sotto **[!UICONTROL Select]** nel _[!UICONTROL Action]_colonna:

- **[!UICONTROL Update Required Info]**: scegli quando le inserzioni non corrispondono automaticamente al catalogo. Puoi eseguire manualmente [abbina prodotti catalogo a inserzioni](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), manualmente [assegna un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) a una corrispondenza del catalogo, oppure [assegna una condizione mancante](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) per l’inserimento nell’elenco.

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’inserzione, tra cui [Elenco registro attività](./product-listing-details.md#listing-activity-log), [Prezzi dei concorrenti Buy Box](./product-listing-details.md#buy-box-competitor-pricing), e [Prezzi più bassi per i concorrenti](./product-listing-details.md#lowest-competitor-pricing). Questa azione è solo per la visualizzazione. Non è possibile apportare modifiche ai dettagli dell&#39;inserzione. Consulta [Visualizza dettagli](./product-listing-details.md).

>[!NOTE]
>
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Inserzioni Amazon incomplete](assets/amazon-incomplete-listings.png)

Le home page del canale di vendita Amazon hanno alcuni punti in comune [controlli workspace](./workspace-controls.md) che ti consentono di personalizzare i dati visualizzati.

| Colonna | Descrizione |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN è l&#39;acronimo di [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Condition] | Il [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Il prezzo di listino del prodotto più il prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto è inserito nell’elenco attivo di Amazon. |
| [!UICONTROL Status] | Lo stato dell’inserzione, definito da Amazon. Vedi la tabella Stato sopra. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** nel _[!UICONTROL Action]_e selezionare un&#39;opzione:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
