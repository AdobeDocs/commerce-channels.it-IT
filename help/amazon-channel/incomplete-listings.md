---
title: Inserzioni incomplete
description: Il canale di vendita di Amazon fornisce la scheda [!UICONTROL Incomplete] per aiutarti a identificare e soddisfare i requisiti di idoneità per gli elenchi di Amazon incompleti.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Elenchi incompleti

La scheda _[!UICONTROL Incomplete]_elenca i prodotti del catalogo [!DNL Commerce] che soddisfano i requisiti di idoneità di Amazon (definiti nelle [regole di elenco](./listing-rules.md)), ma mancano le informazioni richieste da Amazon (ad esempio Amazon ASIN o una condizione di prodotto definita).

Vi sono quattro possibili cause di un elenco incompleto, ciascuna identificata dal suo stato.

| Stato | Motivo | Azione |
|--- |--- |--- |
| Condizione mancante | Amazon accetta elenchi in diverse condizioni (ad esempio _Nuovo_, _Rinnovato_, _Utilizzato: Come New_), l&#39;elenco richiede una condizione definita. | Aggiorna le informazioni richieste e assegna manualmente [una condizione](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) a un elenco. |
| Impossibile assegnare all&#39;elenco Amazon | Corrispondenza automatica dell&#39;elenco al catalogo non riuscita. Se non viene trovata alcuna corrispondenza, l’elenco non può essere gestito da Amazon Sales Channel | Aggiorna le informazioni richieste e assegna manualmente [un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) al prodotto del catalogo per la corrispondenza con l&#39;elenco. |
| Trovate più corrispondenze | Corrispondenza automatica dell&#39;elenco al catalogo non riuscita. Se vengono trovate più corrispondenze possibili, è necessario selezionare la corrispondenza corretta per il prodotto. | Aggiorna le informazioni richieste e scegli manualmente [una corrispondenza prodotto](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) per il prodotto e l&#39;elenco. |
| Presenta varianti | Se il prodotto presenta varianti, ad esempio una t-shirt disponibile in diverse dimensioni o colori, è necessario scegliere la variante nel catalogo da assegnare correttamente e abbinare all’elenco | Aggiorna le informazioni richieste e scegli manualmente la variante corretta](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) da assegnare e abbinare a questa inserzione.[ |

>[!NOTE]
>Quando gli elenchi incompleti corrispondono correttamente ai prodotti del catalogo, l’elenco si sposta dalla scheda _[!UICONTROL Incomplete]_e viene pubblicato in Amazon in base alle impostazioni [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md).

Le azioni disponibili nella scheda _[!UICONTROL Incomplete]_includono:

Alla voce _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Scegli di avviare il processo automatico per far corrispondere i dati degli elenchi Amazon al  [!DNL Commerce] catalogo. Se i prodotti non corrispondono automaticamente, rivedi le opzioni [_[!UICONTROL Catalog Search]_](./catalog-search.md) nelle inserzioni. Se le voci non corrispondono automaticamente dopo l&#39;aggiornamento delle opzioni _[!UICONTROL Catalog Search]_, puoi far corrispondere manualmente i prodotti nell&#39;azione [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found).

Sotto **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_:

- **[!UICONTROL Update Required Info]**: Scegli quando gli elenchi non corrispondono automaticamente al catalogo. Puoi [associare manualmente i prodotti del catalogo agli elenchi](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), assegnare manualmente [un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) a una corrispondenza di catalogo oppure [assegnare una condizione mancante](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) all&#39;elenco.

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’elenco, tra cui il  [Registro attività dell’elenco](./product-listing-details.md#listing-activity-log), i prezzi dei concorrenti di  [Buy Box](./product-listing-details.md#buy-box-competitor-pricing) e i prezzi dei concorrenti  [più bassi](./product-listing-details.md#lowest-competitor-pricing). Questa azione è disponibile solo per la visualizzazione. Non è possibile apportare modifiche nei dettagli dell’elenco. Vedere [Visualizza dettagli](./product-listing-details.md).

>[!NOTE]
>
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Elenchi Amazon incompleti](assets/amazon-incomplete-listings.png)

Le home page del canale di vendita Amazon condividono alcuni controlli comuni [workspace](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

| Colonna | Descrizione |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per  [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Prezzo di listino del prodotto più il suo prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto viene inserito nell’elenco attivo in Amazon. |
| [!UICONTROL Status] | Lo stato dell’elenco, definito da Amazon. Vedi la tabella di stato riportata sopra. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e seleziona un’opzione:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
