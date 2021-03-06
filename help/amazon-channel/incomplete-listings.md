---
title: Inserzioni incomplete
description: Il canale di vendita Amazon fornisce [!UICONTROL Incomplete] per identificare e soddisfare i requisiti di idoneità per gli elenchi di Amazon incompleti.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Elenchi incompleti

La _[!UICONTROL Incomplete]_elenca i [!DNL Commerce] catalogo di prodotti che soddisfano i requisiti di idoneità di Amazon (definiti nel [regole di elenco](./listing-rules.md)), ma mancano le informazioni richieste da Amazon (ad esempio Amazon ASIN o una condizione di prodotto definita).

Vi sono quattro possibili cause di un elenco incompleto, ciascuna identificata dal suo stato.

| Stato | Motivo | Azione |
|--- |--- |--- |
| Condizione mancante | Amazon accetta gli elenchi in varie condizioni (ad esempio _Nuovo_, _Ristrutturato_, _Utilizzato: Simile a nuovo_) richiede una condizione definita. | Aggiorna le informazioni richieste e manualmente [assegnare una condizione](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) a un elenco. |
| Impossibile assegnare all&#39;elenco Amazon | Corrispondenza automatica dell&#39;elenco al catalogo non riuscita. Se non viene trovata alcuna corrispondenza, l’elenco non può essere gestito da Amazon Sales Channel | Aggiorna le informazioni richieste e manualmente [assegnare un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) al prodotto del catalogo per la corrispondenza con l’elenco. |
| Trovate più corrispondenze | Corrispondenza automatica dell&#39;elenco al catalogo non riuscita. Se vengono trovate più corrispondenze possibili, è necessario selezionare la corrispondenza corretta per il prodotto. | Aggiorna le informazioni richieste e manualmente [scegli una partita di prodotto](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) per il prodotto e l’elenco. |
| Presenta varianti | Se il prodotto presenta varianti, ad esempio una t-shirt disponibile in diverse dimensioni o colori, è necessario scegliere la variante nel catalogo da assegnare correttamente e abbinare all’elenco | Aggiorna le informazioni richieste e manualmente [scegli la variante corretta](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) per assegnare e abbinare l&#39;elenco. |

>[!NOTE]
>Quando gli elenchi incompleti vengono correttamente associati ai prodotti del catalogo, l’elenco viene spostato da _[!UICONTROL Incomplete]_e vengono pubblicati in Amazon in base al [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni.

Le azioni disponibili sul _[!UICONTROL Incomplete]_include:

Sotto _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Scegli di avviare il processo automatico per far corrispondere i dati degli elenchi Amazon ai tuoi [!DNL Commerce] catalogo. Se i prodotti non corrispondono automaticamente, rivedi il tuo [_[!UICONTROL Catalog Search]_](./catalog-search.md) opzioni nella lettera dell&#39;inserzione. Se le inserzioni non corrispondono automaticamente dopo l&#39;aggiornamento della _[!UICONTROL Catalog Search]_è possibile associare manualmente i prodotti nella [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) azione.

Sotto **[!UICONTROL Select]** in _[!UICONTROL Action]_colonna:

- **[!UICONTROL Update Required Info]**: Scegli quando gli elenchi non corrispondono automaticamente al catalogo. Puoi manualmente [abbinare i prodotti del catalogo alle inserzioni](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), manualmente [assegnare un ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) a una corrispondenza di catalogo, oppure [assegnare una condizione mancante](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) per l’inserimento nell’elenco.

- **[!UICONTROL View Details]**: scegli di visualizzare i dettagli dell’elenco, tra cui [Elenco del registro delle attività](./product-listing-details.md#listing-activity-log), [Prezzi concorrenza Buy Box](./product-listing-details.md#buy-box-competitor-pricing)e [Prezzi più bassi per i concorrenti](./product-listing-details.md#lowest-competitor-pricing). Questa azione è disponibile solo per la visualizzazione. Non è possibile apportare modifiche nei dettagli dell’elenco. Vedi [Visualizza dettagli](./product-listing-details.md).

>[!NOTE]
>
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Elenchi Amazon incompleti](assets/amazon-incomplete-listings.png)

Le home page del canale di vendita Amazon condividono alcune [controlli dell&#39;area di lavoro](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

| Colonna | Descrizione |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Condition] | La [condizione](./product-listing-condition.md) del prodotto. |
| [!UICONTROL Landed Price] | Prezzo di listino del prodotto più il suo prezzo di spedizione. |
| [!UICONTROL Amazon Quantity] | Quantità disponibile quando il prodotto viene inserito nell’elenco attivo in Amazon. |
| [!UICONTROL Status] | Lo stato dell’elenco, definito da Amazon. Vedi la tabella di stato riportata sopra. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_e seleziona un’opzione:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
