---
title: Gestisci gli elenchi di prodotti Amazon per stato/scheda
description: Quando gestisci le inserzioni di Amazon, puoi applicare azioni alle inserzioni in base allo stato.
feature: Sales Channels, Products
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Gestisci gli elenchi di prodotti Amazon per stato/scheda

La pagina _[!UICONTROL Product Listings]_contiene diverse schede dalle quali è possibile visualizzare gli stati di tutte le inserzioni e abbinare i prodotti alle inserzioni di Amazon.

Le attività disponibili per le inserzioni sono leggermente diverse in ogni scheda, ma i [controlli dell&#39;area di lavoro](./workspace-controls.md) sono gli stessi e consentono di personalizzare i dati visualizzati per le inserzioni.

Le opzioni in **[!UICONTROL Actions]** possono applicare l&#39;azione a più inserzioni, mentre le opzioni in **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_applicano l&#39;azione solo alla singola inserzione.

Vedi anche [Gestione inserzioni per azione](./managing-listings-by-action.md).

![Schede Elenco prodotti](assets/amazon-product-listings-tabs.png){width="600" zoomable="yes"}

| Linguetta | Descrizione | Azioni |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Mostra i prodotti del catalogo [!DNL Commerce] che soddisfano le impostazioni definite per l&#39;inserzione ma non contengono le informazioni richieste da Amazon per un&#39;inserzione.<br><br>Se _[!UICONTROL Automatic List Action]_è impostato su `Automatically List Eligible Products` nelle impostazioni di [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md), questi elementi sono **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Mostra gli elenchi Amazon esistenti (in base alle informazioni ricevute da Amazon) che non corrispondono a un prodotto nel catalogo [!DNL Commerce]. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Tenta corrispondenza automatica<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Mostra i prodotti del catalogo pronti per la creazione di inserzioni Amazon, ma lo store non è impostato per la pubblicazione automatica di nuove inserzioni. Questa scheda viene utilizzata per pubblicare manualmente le nuove inserzioni.<br><br>Se _[!UICONTROL Automatic List Action]_è impostato su `Do Not Automatically List Eligible Products` nelle impostazioni di [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md), questi elementi sono **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Mostra i prodotti del catalogo pubblicati in Amazon, ma Amazon non ha approvato l’inserzione per lo stato Attivo. | [Fine inserzioni in Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Evaso da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Mostra le tue inserzioni Amazon che sono state confrontate con un prodotto nel catalogo [!DNL Commerce], che sono state pubblicate in Amazon e che sono state pubblicate da Amazon per lo stato Attivo. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Soddisfatto da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Mostra le inserzioni di Amazon che soddisfano i criteri per una sostituzione definita e a cui è stata applicata la sostituzione. Le sostituzioni hanno priorità rispetto a qualsiasi altra impostazione dell’account. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Mostra le tue inserzioni esistenti di Amazon che non sono più idonee, in base alle [impostazioni di inserzione](./listing-settings.md) definite. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Soddisfatto da Amazon/Commerciante<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Mostra le inserzioni Amazon scadute (rimosse) manualmente da Amazon. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Accedere agli elenchi di prodotti

1. Nella barra laterale _Admin_, passa a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fare clic su **[!UICONTROL View Store]** sulla scheda dello store.

1. Nel dashboard dell&#39;archivio fare clic su **[!UICONTROL Manage Listings]** nella sezione _[!UICONTROL Store Listings]_.
