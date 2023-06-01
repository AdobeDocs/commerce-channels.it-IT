---
title: Canale di vendita Amazon - Condizione di elenco prodotti
description: Utilizza le impostazioni di condizione dell’elenco dei prodotti per mappare i prodotti Commerce in base a una condizione di prodotto Amazon, ad esempio "Nuovo" o "Rinnovato".
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Condizione di elenco prodotti

Le impostazioni di condizione per l’inserzione del prodotto fanno parte delle impostazioni per l’inserzione nello store. Puoi accedere alle impostazioni dell’inserzione su [dashboard store](./amazon-store-dashboard.md).

Amazon richiede che un elenco di prodotti presenti una condizione definita. Se tutti i prodotti hanno la stessa condizione, puoi selezionare una delle opzioni di condizione di Amazon per rappresentare tutti i prodotti come valore della condizione globale. Le condizioni standard di Amazon includono:

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
>Se vendi prodotti rinnovati, devi iscriverti al [!DNL Amazon Renewed Program]. Consulta [Prodotti rinnovati](./renewed-products.md).

Tuttavia, se il catalogo contiene prodotti in condizioni diverse (ad esempio nuovi, usati e ricondizionati), è necessario scegliere **[!UICONTROL Assign Condition Using Product Attribute]**. Questa impostazione consente di mappare [!DNL Commerce] attributi e valori della condizione alle condizioni dell’inserzione Amazon.

Durante [Attività di pre-configurazione](./amazon-pre-setup-tasks.md), si consiglia di creare un [!DNL Commerce] attributo di prodotto per la condizione di un prodotto. Se offri prodotti in varie condizioni e non hai creato un attributo di condizione, consulta [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md). Dopo la creazione dell’attributo condizione, puoi assegnare un valore di condizione a ciascuno dei prodotti nel tuo [!DNL Commerce] catalogo.

## Configurare le impostazioni

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi **[!UICONTROL Product Listing Condition]** sezione.

1. Per **[!UICONTROL Listing Product Condition]**, scegli un’opzione.

   Scegli una delle condizioni standard di Amazon per il valore della condizione globale per tutte le inserzioni. L&#39;impostazione predefinita è `New`.

   Se hai prodotti/inserzioni con condizioni diverse, scegli `Assign Condition Using Product Attribute` per definire le impostazioni delle condizioni del prodotto nei campi aggiuntivi visualizzati.

1. Per **Attributo condizione**, scegli il [!DNL Commerce] attributo per mappare i valori per ciascuno degli attributi di condizione standard di Amazon.

   Se sono presenti prodotti in `Used` o `Collectible` ma non si distinguono ulteriormente, è possibile eseguire il mapping a un singolo `Used` o `Collectible` Condizione Amazon e lascia vuote le altre. Questo metodo mappa tutti i `Used` o `Collectible` condizioni per la singola condizione Amazon Used o Collectible.

   Ad esempio, hai un singolo `Used` per i prodotti. Quando esegui la mappatura, scegli se desideri eseguirla per la condizione Amazon `Used; Like New`, `Used; Very Good`, `Used; Good`, o `Used; Acceptable`. Completa solo il campo per la condizione Amazon desiderata, lasciando l’altra `Used` opzioni impostate su `--Select Option--`. Nell’immagine di esempio, tutte [!DNL Commerce] prodotti in `Used` La condizione è mappata su Amazon `Used; Very Good` condizione.

   È inoltre possibile immettere un testo descrittivo per le condizioni, ad eccezione di `New`.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Condizione di elenco prodotti](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|---|---|
| [!UICONTROL Listing Product Condition] | La condizione degli elenchi di prodotti. Opzioni: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Se vendi una singola condizione di prodotto, scegli una delle condizioni standard di Amazon. Se il [!DNL Commerce] catalogo contiene prodotti in varie condizioni, scegliere `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | Il [!DNL Commerce] che definisce la condizione per i prodotti. Seleziona l’attributo Magneto creato per il mapping all’attributo condizione di Amazon. In [Esempio di attività di preconfigurazione](./ob-creating-magento-attributes.md) consiglia di denominarlo come `Amazon Condition`. Quando viene scelto, vengono visualizzati campi aggiuntivi per la mappatura delle condizioni standard di Amazon. |
| [!UICONTROL Additional Condition fields] | Per ciascuna delle condizioni standard di Amazon, scegli la condizione corrispondente. Le opzioni sono le etichette di condizione aggiunte quando [ha creato il tuo attributo condizione di Amazon](./ob-creating-magento-attributes.md).<br><br>Se sono presenti prodotti in `Used` o `Collectible` ma non si distinguono ulteriormente, è possibile eseguire il mapping a un singolo `Used` o `Collectible` Condizione Amazon e lascia vuote le altre. Questo metodo mappa tutto `Used` o `Collectible` condizioni per la singola condizione Amazon Used o Collectible. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
