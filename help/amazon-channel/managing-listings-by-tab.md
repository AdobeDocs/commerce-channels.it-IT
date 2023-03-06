---
title: Gestisci elenchi prodotti per stato/scheda
description: Quando gestisci le inserzioni di Amazon, puoi applicare azioni alle inserzioni in base allo stato.
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Gestisci elenchi prodotti per stato/scheda

Il _[!UICONTROL Product Listings]_La pagina contiene diverse schede da cui puoi visualizzare gli stati di tutte le inserzioni e abbinare i tuoi prodotti alle inserzioni di Amazon.

Le attività di inserzione disponibili sono leggermente diverse in ogni scheda, ma il [controlli workspace](./workspace-controls.md) sono le stesse e ti consentono di personalizzare i dati visualizzati per le inserzioni.

Opzioni in **[!UICONTROL Actions]** può applicare l’azione a più inserzioni, mentre le opzioni in **[!UICONTROL Select]** nel _[!UICONTROL Action]_applica l’azione solo alla singola inserzione.

Vedi anche [Gestisci le inserzioni per Azione](./managing-listings-by-action.md).

![Schede Elenco prodotti](assets/amazon-product-listings-tabs.png)

| Linguetta | Descrizione | Azioni |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Mostra il tuo [!DNL Commerce] cataloga i prodotti che soddisfano le impostazioni definite per l’inserzione ma non contengono le informazioni richieste da Amazon per un’inserzione.<br><br>Se _[!UICONTROL Automatic List Action]_è impostato su `Automatically List Eligible Products` nel tuo [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni, questi elementi sono **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Mostra gli elenchi Amazon esistenti (in base alle informazioni ricevute da Amazon) che non corrispondono a un prodotto nel tuo [!DNL Commerce] catalogo. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Tenta corrispondenza automatica<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Mostra i prodotti del catalogo pronti per la creazione di inserzioni Amazon, ma lo store non è impostato per la pubblicazione automatica di nuove inserzioni. Questa scheda viene utilizzata per pubblicare manualmente le nuove inserzioni.<br><br>Se _[!UICONTROL Automatic List Action]_è impostato su `Do Not Automatically List Eligible Products` nel tuo [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni, questi elementi sono **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Mostra i prodotti del catalogo pubblicati in Amazon, ma Amazon non ha approvato l’inserzione per lo stato Attivo. | [Fine Inserzioni su Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Soddisfatto da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Mostra le tue inserzioni Amazon che sono state abbinate a un prodotto nel tuo [!DNL Commerce] , sono stati pubblicati in Amazon e sono stati impostati da Amazon per lo stato Attivo. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Soddisfatto da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Mostra le inserzioni di Amazon che soddisfano i criteri per una sostituzione definita e a cui è stata applicata la sostituzione. Le sostituzioni hanno priorità rispetto a qualsiasi altra impostazione dell’account. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Mostra le inserzioni esistenti di Amazon che non sono più idonee, in base al [impostazioni elenco](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Soddisfatto da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Mostra le inserzioni Amazon scadute (rimosse) manualmente da Amazon. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Accedere agli elenchi di prodotti

1. Il giorno _Amministratore_ barra laterale, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Clic **[!UICONTROL View Store]** sulla scheda del negozio.

1. Nel dashboard del negozio, fai clic su **[!UICONTROL Manage Listings]** nel _[!UICONTROL Store Listings]_sezione.
