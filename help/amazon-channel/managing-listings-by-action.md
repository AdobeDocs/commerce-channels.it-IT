---
title: Gestire gli elenchi di prodotti per azione
description: Quando gestisci gli elenchi di Amazon, puoi applicare un’azione a singoli o più elenchi.
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Gestire gli elenchi di prodotti per azione

La pagina _[!UICONTROL Product Listings]_contiene diverse schede dalle quali puoi visualizzare gli stati di tutti gli elenchi e far corrispondere i prodotti agli elenchi di Amazon.

Le attività di elenco disponibili sono leggermente diverse in ogni scheda, ma i [controlli area di lavoro](./workspace-controls.md) sono gli stessi e consentono di personalizzare i dati visualizzati per le inserzioni.

Le opzioni sotto **[!UICONTROL Actions]** possono applicare l’azione a più elenchi, mentre le opzioni sotto **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_applicano l’azione solo all’elenco individuale.

Vedere anche [Gestire gli elenchi per stato / Tab](./managing-listings-by-tab.md).

| Azione | Descrizione | Schede |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | Utilizzato per spostare di nuovo i prodotti incompleti attraverso il processo di corrispondenza. Per tentare la riconversione, devi modificare le impostazioni [Listing](./listing-settings.md) e [Ricerca nel catalogo](./catalog-search.md) per aumentare il potenziale di corrispondenza automatica. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | Corrispondenza manuale dei prodotti del catalogo agli elenchi di Amazon selezionando un elenco a cui associare i dati, immettendo un ASIN per la corrispondenza o assegnando una condizione mancante. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | Visualizza informazioni aggiuntive sui prodotti attivi, incluso il registro delle attività di elenco, che mostra le modifiche su un singolo SKU/Prodotto. | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | Crea un prodotto di catalogo [!DNL Commerce] utilizzando le informazioni importate con l’elenco Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| Cerca corrispondenza automatica | Cerca una corrispondenza automatica tra il catalogo [!DNL Commerce] e gli elenchi Amazon in base alle impostazioni dei criteri di ricerca. Per tentare la riconversione, devi modificare le impostazioni [Listing](./listing-settings.md) e [Ricerca nel catalogo](./catalog-search.md) per aumentare il potenziale di corrispondenza automatica. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | Seleziona manualmente un prodotto esistente nel catalogo [!DNL Commerce] e assegnalo all’elenco Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | Crea un prodotto di catalogo [!DNL Commerce] utilizzando le informazioni importate con l’elenco Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | (Azione di massa) Utilizzato per rimettere in vendita un elenco che è stato terminato o per elencare manualmente un prodotto che soddisfa i requisiti di idoneità per le regole di elenco, ma il _[!UICONTROL Product Listing Actions]_non è impostato su `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | (Azione di elenco singolo) Utilizzato per rimettere in vendita un elenco che è stato terminato. Questa azione viene utilizzata anche per elencare manualmente un prodotto che soddisfa l’idoneità delle regole di elenco quando _[!UICONTROL Product Listing Actions]_non è impostato su `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | (Azione di massa) Utilizzato per terminare e rimuovere manualmente gli elenchi dei prodotti esistenti in Amazon. Le inserzioni terminate possono essere rielencate purché soddisfino l’idoneità alle regole per le inserzioni. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | (Azione di massa) Modificare manualmente un &quot;override&quot; esistente che imposta il testo del prezzo, del tempo di gestione, della condizione e delle note di vendita per una singola inserzione, ignorando altri valori predefiniti della inserzione, impostazioni e regole. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | Creare manualmente un &quot;override&quot; per impostare il testo relativo a prezzo, tempo di gestione, condizione e note di vendita per un singolo elenco, ignorando altri valori predefiniti, impostazioni e regole dell&#39;inserzione. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | Utilizzato se è necessario modificare l’ASIN corrispondente al prodotto del catalogo (ad esempio: se il prodotto è stato confrontato con l’elenco ASIN errato). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | Può essere utilizzato per due funzioni:<br><br>Può essere utilizzato per creare una relazione 1-a-2 tra il prodotto di catalogo e due elenchi Amazon. Esempio: Amazon presenta il prodotto elencato con valori ASIN diversi. È possibile associare un prodotto catalogo a entrambi gli elenchi ASIN per il prodotto.<br><br>Può essere utilizzato per controllare un elenco in diverse aree geografiche di Amazon. Esempio: Hai un prodotto di catalogo con diversi metodi di spedizione definiti in base all’area Amazon (l’area geografica degli Stati Uniti è FBA e l’area del Canada è FBM). Per controllare il magazzino/la quantità, è possibile creare un SKU alias venditore e inserire lo stesso prodotto in quella regione con un SKU venditore diverso. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | Utilizzato per modificare il metodo di evasione associato al prodotto (Eseguito da Amazon: FBA o realizzata da Merchant: FBM). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | (Azione di elenco singolo) Utilizzato per terminare e rimuovere manualmente gli elenchi dei prodotti esistenti in Amazon. Le inserzioni terminate possono essere rielencate purché soddisfino l’idoneità alle regole per le inserzioni. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | (Azione di inserzione singola) Modificare manualmente un &quot;override&quot; esistente che imposta il testo del prezzo, del tempo di gestione, della condizione e delle note di vendita per una singola inserzione, ignorando altri valori predefiniti, impostazioni e regole dell&#39;inserzione. | [[!UICONTROL Overrides]](./overrides.md) |

## Accedere agli elenchi dei prodotti

1. Nella barra laterale _Amministratore_, vai a **Marketing** > _Canali_ > **Sales Channel Amazon**.

1. Fai clic su **Visualizza archivio** sulla scheda del negozio.

1. Nel dashboard dello store, fai clic su **Gestisci elenchi** nella sezione _Memorizza elenchi_.
