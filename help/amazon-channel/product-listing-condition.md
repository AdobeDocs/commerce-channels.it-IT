---
title: Condizione dell’elenco dei prodotti
description: 'Utilizza le impostazioni della condizione di inserimento nell’elenco dei prodotti per mappare i tuoi prodotti Commerce a una condizione di prodotto Amazon, ad esempio "Nuovo" o "Rinnovato".'
redirect_from: /sales-channels/asc/ob-product-listing-condition.html: 
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 526
ht-degree: 0%

---

# Condizione dell’elenco dei prodotti

Le impostazioni delle condizioni per l’elenco dei prodotti fanno parte delle impostazioni dell’elenco degli store. Puoi accedere alle impostazioni dell&#39;elenco sul [dashboard store](./amazon-store-dashboard.md).

Amazon richiede una condizione definita per un elenco di prodotti. Se tutti i prodotti presentano la stessa condizione, puoi selezionare una delle opzioni di condizione di Amazon per rappresentare tutti i prodotti come valore della condizione globale. Le condizioni standard di Amazon includono:

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>Se vendi prodotti rinnovati (rinnovati), devi iscriverti al [!DNL Amazon Renewed Program]. Consulta [Prodotti rinnovati](./renewed-products.md).

Tuttavia, se il catalogo contiene prodotti in condizioni diverse (ad esempio Nuovo, Utilizzato e Rinnovato), è necessario scegliere **[!UICONTROL Assign Condition Using Product Attribute]**. Questa impostazione ti consente di mappare l’attributo e i valori della condizione [!DNL Commerce] alle condizioni dell’elenco di Amazon.

Durante le [attività di preinstallazione](./amazon-pre-setup-tasks.md), ti consigliamo di creare un attributo di prodotto [!DNL Commerce] per le condizioni di un prodotto. Se offri prodotti in diverse condizioni e non hai creato un attributo di condizione, consulta [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md). Una volta creato l’attributo di condizione, puoi assegnare un valore di condizione a ciascuno dei tuoi prodotti nel catalogo [!DNL Commerce].

## Configurare le impostazioni

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione **[!UICONTROL Product Listing Condition]**.

1. Per **[!UICONTROL Listing Product Condition]**, scegli un’opzione.

   Scegli una delle condizioni standard di Amazon per il valore della condizione globale per tutti gli elenchi. L&#39;impostazione predefinita è `New`.

   Se disponi di prodotti/elenchi con condizioni diverse, scegli `Assign Condition Using Product Attribute` per definire le impostazioni di condizione del prodotto nei campi aggiuntivi visualizzati.

1. Per **Attributo condizione**, scegli l&#39;attributo [!DNL Commerce] per mappare i valori per ciascuno degli attributi di condizione standard di Amazon.

   Se disponi di prodotti nella condizione `Used` o `Collectible` ma non effettui ulteriori distinzioni, puoi mappare una singola condizione `Used` o `Collectible` Amazon e lasciare vuote le altre. Questo metodo mappa tutte le condizioni `Used` o `Collectible` alla singola condizione Amazon Usato o Raccoglibile.

   Ad esempio, si dispone di una singola condizione `Used` per i prodotti. Durante la mappatura, scegli se desideri eseguire la mappatura sulla condizione Amazon `Used; Like New`, `Used; Very Good`, `Used; Good` o `Used; Acceptable`. Completa solo il campo per la condizione Amazon desiderata, lasciando le altre opzioni `Used` impostate su `--Select Option--`. Nell’immagine di esempio, tutti i prodotti [!DNL Commerce] nella condizione `Used` sono mappati alla condizione Amazon `Used; Very Good`.

   È inoltre possibile immettere un testo descrittivo per le condizioni, ad eccezione di `New`.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Condizione dell’elenco dei prodotti](assets/amazon-product-listing-condition.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Listing Product Condition] | Le condizioni degli elenchi dei prodotti. Opzioni: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Se vendi una singola condizione di prodotto, scegli una delle condizioni Amazon standard. Se il catalogo [!DNL Commerce] contiene prodotti in diverse condizioni, scegli `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | L’attributo [!DNL Commerce] che definisce la condizione per i prodotti. Seleziona l’attributo Magneto creato per eseguire il mapping all’attributo della condizione Amazon. Nell’ [Esempio di attività di pre-installazione](./ob-creating-magento-attributes.md) consiglia di denominarla come `Amazon Condition`. Quando scelto, vengono visualizzati campi aggiuntivi per la mappatura delle condizioni Amazon standard. |
| [!UICONTROL Additional Condition fields] | Per ciascuna delle condizioni standard di Amazon, scegli la condizione corrispondente. Le opzioni sono le etichette di condizione aggiunte quando [hai creato l&#39;attributo di condizione Amazon](./ob-creating-magento-attributes.md).<br><br>Se disponi di prodotti nella  `Used` condizione  `Collectible` o ma non fai ulteriori distinzioni, puoi mappare una singola condizione  `Used` o  `Collectible` Amazon e lasciare vuote le altre. Questo metodo mappa tutte le condizioni `Used` o `Collectible` alla singola condizione Amazon Usato o Raccoglibile. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
