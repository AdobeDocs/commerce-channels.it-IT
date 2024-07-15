---
title: Canale di vendita Amazon - Condizione di elenco prodotti
description: Utilizza le impostazioni di condizione dell’elenco dei prodotti per mappare i prodotti Commerce a una condizione di prodotto Amazon, ad esempio "Nuovo" o "Rinnovato".
feature: Sales Channels, Products, Merchandising
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Condizione di elenco prodotti

Le impostazioni di condizione per l’inserzione del prodotto fanno parte delle impostazioni per l’inserzione nello store. Puoi accedere alle impostazioni dell&#39;inserzione nel [dashboard dello store](./amazon-store-dashboard.md).

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
>Se vendi prodotti rinnovati, devi iscriverti a [!DNL Amazon Renewed Program]. Vedi [Prodotti rinnovati](./renewed-products.md).

Tuttavia, se il catalogo contiene prodotti in condizioni diverse, ad esempio nuovi, usati e ricondizionati, è necessario scegliere **[!UICONTROL Assign Condition Using Product Attribute]**. Questa impostazione consente di mappare l&#39;attributo e i valori della condizione [!DNL Commerce] alle condizioni dell&#39;inserzione Amazon.

Durante le [attività preliminari](./amazon-pre-setup-tasks.md), si consiglia di creare un attributo di prodotto [!DNL Commerce] per la condizione di un prodotto. Se offri prodotti in varie condizioni e non hai creato un attributo di condizione, consulta [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md). Dopo aver creato l&#39;attributo di condizione, è possibile assegnare un valore di condizione a ciascuno dei prodotti nel catalogo [!DNL Commerce].

## Configurare le impostazioni

1. Fare clic su **[!UICONTROL Listing Settings]** nel dashboard dell&#39;archivio.

1. Espandere la sezione **[!UICONTROL Product Listing Condition]**.

1. Per **[!UICONTROL Listing Product Condition]**, scegliere un&#39;opzione.

   Scegli una delle condizioni standard di Amazon per il valore della condizione globale per tutte le inserzioni. Impostazione predefinita: `New`.

   Se sono presenti prodotti/elenchi con condizioni diverse, scegliere `Assign Condition Using Product Attribute` per definire le impostazioni delle condizioni del prodotto nei campi aggiuntivi visualizzati.

1. Per **Attributo condizione**, scegliere l&#39;attributo [!DNL Commerce] per mappare i valori per ciascuno degli attributi di condizione standard di Amazon.

   Se si dispone di prodotti nella condizione `Used` o `Collectible` ma non si distinguono ulteriormente, è possibile eseguire il mapping a una singola condizione di Amazon `Used` o `Collectible` e lasciare vuoti gli altri. Questo metodo mappa tutte le condizioni di `Used` o `Collectible` alla singola condizione Amazon Used o Collectible.

   Ad esempio, si dispone di una singola condizione `Used` per i prodotti. Durante la mappatura, puoi scegliere se eseguire la mappatura alla condizione Amazon `Used; Like New`, `Used; Very Good`, `Used; Good` o `Used; Acceptable`. Completa solo il campo per la condizione Amazon desiderata, lasciando le altre opzioni `Used` impostate su `--Select Option--`. Nell&#39;immagine di esempio, tutti i prodotti [!DNL Commerce] nella condizione `Used` sono mappati alla condizione Amazon `Used; Very Good`.

   È inoltre possibile immettere un testo descrittivo per le condizioni, ad eccezione di `New`.

1. Al termine, fare clic su **[!UICONTROL Save listing settings]**.

![Condizione dell&#39;elenco prodotti](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Listing Product Condition] | La condizione degli elenchi di prodotti. Opzioni: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Se vendi un singolo prodotto, scegli una delle condizioni standard di Amazon. Se il catalogo [!DNL Commerce] contiene prodotti in varie condizioni, scegliere `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | Attributo [!DNL Commerce] che definisce la condizione per i prodotti. Seleziona l’attributo Magneto creato per il mapping all’attributo condizione di Amazon. Nell&#39;esempio di [Attività precedenti all&#39;installazione](./ob-creating-magento-attributes.md) consiglia di denominarle `Amazon Condition`. Quando viene scelto, vengono visualizzati campi aggiuntivi per la mappatura delle condizioni standard di Amazon. |
| [!UICONTROL Additional Condition fields] | Per ciascuna delle condizioni standard di Amazon, scegli la condizione corrispondente. Le opzioni sono le etichette di condizione aggiunte al momento della [creazione dell&#39;attributo di condizione di Amazon](./ob-creating-magento-attributes.md).<br><br>Se sono presenti prodotti nella condizione `Used` o `Collectible` ma non si distinguono ulteriormente, è possibile eseguire il mapping a una singola condizione di Amazon `Used` o `Collectible` e lasciare vuoti gli altri. Questo metodo mappa tutte le condizioni `Used` o `Collectible` alla singola condizione Amazon Used o Collectible. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
