---
title: Condizione dell’elenco dei prodotti
description: Utilizza le impostazioni della condizione di inserimento nell’elenco dei prodotti per mappare i tuoi prodotti Commerce a una condizione di prodotto Amazon, ad esempio "Nuovo" o "Rinnovato".
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Condizione dell’elenco dei prodotti

Le impostazioni delle condizioni per l’elenco dei prodotti fanno parte delle impostazioni dell’elenco degli store. Puoi accedere alle impostazioni dell’elenco nella [dashboard store](./amazon-store-dashboard.md).

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
>Se vendi prodotti rinnovati (rinnovati), devi iscriverti al [!DNL Amazon Renewed Program]. Vedi [Prodotti rinnovati](./renewed-products.md).

Tuttavia, se il catalogo contiene prodotti in condizioni diverse (ad esempio Nuovo, Utilizzato e Rinnovato), è necessario scegliere **[!UICONTROL Assign Condition Using Product Attribute]**. Questa impostazione consente di mappare il [!DNL Commerce] attributo e valori della condizione per le condizioni dell’elenco di Amazon.

Periodo [Attività pre-installazione](./amazon-pre-setup-tasks.md), ti consigliamo di creare un [!DNL Commerce] attributo di prodotto per la condizione di un prodotto. Se offri prodotti in varie condizioni e non hai creato un attributo di condizione, consulta [Crea un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md). Una volta creato l’attributo della condizione, puoi assegnare un valore della condizione a ciascuno dei tuoi prodotti nel tuo [!DNL Commerce] catalogo.

## Configurare le impostazioni

1. Fai clic su **[!UICONTROL Listing Settings]** sul dashboard dello store.

1. Espandi la **[!UICONTROL Product Listing Condition]** sezione .

1. Per **[!UICONTROL Listing Product Condition]**, scegli un’opzione.

   Scegli una delle condizioni standard di Amazon per il valore della condizione globale per tutti gli elenchi. L&#39;impostazione predefinita è `New`.

   Se hai prodotti/inserzioni con condizioni diverse, scegli `Assign Condition Using Product Attribute` per definire le impostazioni di condizione del prodotto nei campi aggiuntivi visualizzati.

1. Per **Attributo condizione**, scegli [!DNL Commerce] per mappare valori per ciascuno degli attributi di condizione standard di Amazon.

   Se hai prodotti nel `Used` o `Collectible` condizione ma non si distingue ulteriormente, è possibile eseguire la mappatura su un singolo `Used` o `Collectible` Condizione Amazon e lasciare gli altri vuoti. Questo metodo mappa tutti i `Used` o `Collectible` condizioni per la singola condizione Amazon Usato o Raccoglibile.

   Ad esempio, hai una sola `Used` condizioni per i prodotti. Durante la mappatura, scegli se desideri eseguire la mappatura sulla condizione Amazon. `Used; Like New`, `Used; Very Good`, `Used; Good`oppure `Used; Acceptable`. Completa solo il campo per la condizione di Amazon desiderata, lasciando l’altro `Used` opzioni impostate su `--Select Option--`. Nell’immagine di esempio, tutti [!DNL Commerce] prodotti `Used` sono mappate su Amazon `Used; Very Good` condizione.

   È inoltre possibile immettere un testo descrittivo per le condizioni, tranne `New`.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Condizione dell’elenco dei prodotti](assets/amazon-product-listing-condition.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Listing Product Condition] | Le condizioni degli elenchi dei prodotti. Opzioni: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Se vendi una singola condizione di prodotto, scegli una delle condizioni Amazon standard. Se [!DNL Commerce] catalogo contiene prodotti in varie condizioni, scegli `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | La [!DNL Commerce] attributo che definisce la condizione per i prodotti. Seleziona l’attributo Magneto creato per eseguire il mapping all’attributo della condizione Amazon. In [Esempio di attività pre-installazione](./ob-creating-magento-attributes.md) consiglia di denominarlo come `Amazon Condition`. Quando scelto, vengono visualizzati campi aggiuntivi per la mappatura delle condizioni Amazon standard. |
| [!UICONTROL Additional Condition fields] | Per ciascuna delle condizioni standard di Amazon, scegli la condizione corrispondente. Le opzioni sono le etichette di condizione aggiunte al momento dell’aggiunta [creazione dell&#39;attributo condizione Amazon](./ob-creating-magento-attributes.md).<br><br>Se hai prodotti nel `Used` o `Collectible` condizione ma non si distingue ulteriormente, è possibile eseguire la mappatura su un singolo `Used` o `Collectible` Condizione Amazon e lasciare gli altri vuoti. Questo metodo mappa tutti `Used` o `Collectible` condizioni per la singola condizione Amazon Usato o Raccoglibile. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
