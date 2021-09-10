---
title: Gestire gli elenchi dei prodotti in base a stato/scheda
description: Quando gestisci gli elenchi di Amazon, puoi applicare le azioni agli elenchi in base allo stato.
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Gestire gli elenchi dei prodotti in base allo stato / scheda

La pagina _[!UICONTROL Product Listings]_contiene diverse schede dalle quali puoi visualizzare gli stati di tutti gli elenchi e far corrispondere i prodotti agli elenchi di Amazon.

Le attività di elenco disponibili sono leggermente diverse in ogni scheda, ma i [controlli area di lavoro](./workspace-controls.md) sono gli stessi e consentono di personalizzare i dati visualizzati per le inserzioni.

Le opzioni sotto **[!UICONTROL Actions]** possono applicare l’azione a più elenchi, mentre le opzioni sotto **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_applicano l’azione solo all’elenco individuale.

Vedere anche [Gestire gli elenchi per azione](./managing-listings-by-action.md).

![Schede Elenco prodotti](assets/amazon-product-listings-tabs.png)

| Scheda | Descrizione | Azioni |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Mostra i prodotti del catalogo [!DNL Commerce] che soddisfano le impostazioni di elenco definite ma che non contengono le informazioni richieste da Amazon per un elenco.<br><br>Se  _[!UICONTROL Automatic List Action]_è impostato su  `Automatically List Eligible Products` nelle  [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni, questi elementi sono **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Mostra gli elenchi Amazon esistenti (in base alle informazioni ricevute da Amazon) che non corrispondono a un prodotto nel catalogo [!DNL Commerce]. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Cerca corrispondenza automatica<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Mostra i prodotti catalogo pronti per la creazione di elenchi Amazon, ma lo store è impostato per non pubblicare automaticamente nuovi elenchi. Questa scheda viene utilizzata per pubblicare manualmente i nuovi elenchi.<br><br>Se  _[!UICONTROL Automatic List Action]_è impostato su  `Do Not Automatically List Eligible Products` nelle  [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) impostazioni, questi elementi sono **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Mostra i prodotti catalogo pubblicati in Amazon, ma Amazon non ha approvato l’elenco per lo stato Attivo. | [ EndListing(s) su ](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>AmazonSwitch su Fulfill by Amazon/Merchant<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Mostra gli elenchi di Amazon che sono stati confrontati con un prodotto nel catalogo [!DNL Commerce], sono stati pubblicati in Amazon e sono stati da Amazon per lo stato Attivo. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Eseguito da Amazon/Merchant<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Mostra gli elenchi di Amazon che soddisfano i criteri per una sostituzione definita e a cui è stata applicata la sostituzione. Le sostituzioni hanno la priorità rispetto a qualsiasi altra impostazione dell’account. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Mostra gli elenchi Amazon esistenti che non sono più idonei, in base alle [impostazioni di elenco ](./listing-settings.md) definite. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Passa a Eseguito da Amazon/Merchant<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Mostra gli elenchi di Amazon che sono stati terminati manualmente (rimossi) da Amazon. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Accedere agli elenchi dei prodotti

1. Nella barra laterale _Amministratore_, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL View Store]** nella scheda del negozio.

1. Nel dashboard dello store, fai clic su **[!UICONTROL Manage Listings]** nella sezione _[!UICONTROL Store Listings]_.
