---
title: Gestire gli elenchi di prodotti Amazon per azione
description: Quando gestisci le inserzioni di Amazon, puoi applicare un’azione a una o più inserzioni.
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Gestire gli elenchi di prodotti Amazon per azione

Il _[!UICONTROL Product Listings]_La pagina contiene diverse schede da cui puoi visualizzare gli stati di tutte le inserzioni e abbinare i tuoi prodotti alle inserzioni di Amazon.

Le attività di inserzione disponibili sono leggermente diverse in ogni scheda, ma il [controlli workspace](./workspace-controls.md) sono le stesse e ti consentono di personalizzare i dati visualizzati per le inserzioni.

Opzioni in **[!UICONTROL Actions]** può applicare l’azione a più inserzioni, mentre le opzioni in **[!UICONTROL Select]** nel _[!UICONTROL Action]_applica l’azione solo alla singola inserzione.

Vedi anche [Gestisci le inserzioni per Stato / Scheda](./managing-listings-by-tab.md).

| Azione | Descrizione | Schede |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | Utilizzato per spostare di nuovo i prodotti incompleti attraverso il processo di corrispondenza. Per tentare una nuova corrispondenza, è necessario modificare il [Elenco](./listing-settings.md) e [Ricerca nel catalogo](./catalog-search.md) per aumentare il potenziale di abbinamento automatico. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | Abbina manualmente i prodotti del catalogo alle inserzioni di Amazon selezionando un&#39;inserzione da abbinare, inserendo un codice ASIN da abbinare o assegnando una condizione mancante. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | Visualizza ulteriori informazioni sui prodotti attivi, tra cui il registro attività elenco, che mostra le modifiche su un singolo SKU/prodotto. | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | Creare un [!DNL Commerce] catalogo prodotti utilizzando le informazioni importate con l’elenco di Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| Tenta corrispondenza automatica | Tenta una corrispondenza automatica tra [!DNL Commerce] catalogo e le inserzioni Amazon in base alle impostazioni dei criteri di ricerca. Per tentare una nuova corrispondenza, è necessario modificare il [Elenco](./listing-settings.md) e [Ricerca nel catalogo](./catalog-search.md) per aumentare il potenziale di abbinamento automatico. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | Seleziona manualmente un prodotto esistente nel tuo [!DNL Commerce] e assegnarlo all’elenco di Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | Creare un [!DNL Commerce] catalogo prodotti utilizzando le informazioni importate con l’elenco di Amazon. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | (Azione di massa) Utilizzato per rimettere in vendita un&#39;inserzione scaduta o per mettere in vendita manualmente un prodotto che soddisfa le regole di idoneità dell&#39;inserzione, ma _[!UICONTROL Product Listing Actions]_non è impostato su `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | (Azione di inserzione singola) Utilizzato per rimettere in vendita un’inserzione scaduta. Questa azione viene utilizzata anche per elencare manualmente un prodotto che soddisfa l’idoneità alle regole dell’inserzione quando _[!UICONTROL Product Listing Actions]_non è impostato su `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | (Azione di massa) Utilizzata per terminare e rimuovere manualmente le inserzioni per i tuoi prodotti che esistono su Amazon. Le inserzioni scadute possono essere rimesse in vendita purché soddisfino i requisiti per le regole di inserzione. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | (Azione di massa) Modifica manualmente una &quot;sostituzione&quot; esistente che imposta il testo del prezzo, del tempo di gestione, della condizione e delle note del venditore per una singola inserzione, ignorando altri valori predefiniti, impostazioni e regole dell&#39;inserzione. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | Crea manualmente una &quot;sostituzione&quot; che imposta il testo del prezzo, del tempo di gestione, della condizione e delle note del venditore per una singola inserzione, ignorando altri valori predefiniti, impostazioni e regole dell&#39;inserzione. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | Utilizzato se l’ASIN corrisponde al prodotto del catalogo deve essere modificato (ad esempio: se il prodotto corrisponde all’elenco ASIN errato). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | Può servire due funzioni:<br><br>Può essere utilizzato per creare una relazione da 1 a 2 tra il prodotto del catalogo e due inserzioni Amazon. Esempio: in Amazon il prodotto è elencato con valori ASIN diversi. Puoi abbinare il prodotto del catalogo a entrambi gli elenchi ASIN per il prodotto.<br><br>Può essere utilizzato per controllare un elenco in diverse aree geografiche di Amazon. Esempio: hai un prodotto catalogo con diversi metodi di spedizione definiti in base all’area Amazon (l’area Stati Uniti è FBA e l’area Canada è FBM). Per controllare le scorte/quantità, puoi creare uno SKU di un venditore di alias e rimettere in vendita lo stesso prodotto in quell’area geografica con uno SKU di venditore diverso. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | Utilizzato per modificare il metodo di evasione associato al prodotto (evaso da Amazon: FBA o evaso da commerciante: FBM). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | (Azione di inserzione singola) Utilizzata per terminare e rimuovere manualmente le inserzioni per i prodotti esistenti su Amazon. Le inserzioni scadute possono essere rimesse in vendita purché soddisfino i requisiti per le regole di inserzione. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | (Azione di messa in vendita singola) Modifica manualmente una &quot;sostituzione&quot; esistente che imposta il testo del prezzo, del tempo di gestione, della condizione e delle note del venditore per una singola messa in vendita, ignorando altri valori predefiniti, impostazioni e regole di messa in vendita. | [[!UICONTROL Overrides]](./overrides.md) |

## Accedere agli elenchi di prodotti

1. Il giorno _Amministratore_ barra laterale, vai a **Marketing** > _Canali_ > **Sales Channel Amazon**.

1. Clic **Visualizza store** sulla scheda del negozio.

1. Nel dashboard del negozio, fai clic su **Gestisci le inserzioni** nel _Inserzioni in Negozio_ sezione.
