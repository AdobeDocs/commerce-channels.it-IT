---
title: Ricerca nel catalogo
description: Per impostare la corrispondenza degli attributi che consente di mappare i prodotti del catalogo Commerce idonei con gli elenchi di Amazon, aggiorna le impostazioni di Ricerca nel catalogo.
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Ricerca nel catalogo

_Ricerca nel catalogo_ Le impostazioni fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell’elenco sono accessibili dal [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni consentono di impostare la corrispondenza degli attributi per facilitare la mappatura degli attributi idonei [!DNL Commerce] prodotti con elenchi Amazon. Quando viene mappata, Amazon attiva azioni relative a prezzi, quantità, sostituzioni e sincronizzazione di ordini e prodotti.

La definizione di questi valori di mappatura aumenta il potenziale di corrispondenze esatte, riducendo al minimo la necessità di abbinare manualmente gli elenchi di prodotti. Aggiunta di attributi come parte del [Attività pre-installazione](./amazon-pre-setup-tasks.md), il canale di vendita Amazon ha un potenziale più elevato per abbinare automaticamente i prodotti durante l&#39;onboarding e la sincronizzazione dei dati dei prodotti tra Amazon e [!DNL Commerce].

Se crei solo l’attributo Amazon ASIN (senza aggiungere valori ASIN per prodotto), il tuo [!DNL Commerce] i prodotti potrebbero non corrispondere automaticamente agli elenchi di Amazon. È possibile [assegnazione manuale](./creating-assigning-catalog-products.md) i prodotti. Tuttavia, la corrispondenza manuale non crea gli elementi dati necessari per condividere e sincronizzare i dati del prodotto.

>[!IMPORTANT]
>
>Se si corrisponde manualmente un prodotto e si desidera aggiornare un ASIN, un UPC o un altro elemento dati per il prodotto, è necessario aggiornare i dati in due posizioni. Aggiorna nel tuo [!DNL Commerce] catalogo e nell’elenco Amazon nel tuo [!DNL Amazon Seller Central] conto.

È consigliabile mappare questi attributi e valori, se disponibili. Il completamento di questa mappatura non è necessario, ma è vantaggioso per la corrispondenza dei prodotti e richiesto per la corretta sincronizzazione del catalogo tra Amazon e [!DNL Commerce].

Per aggiungere attributi, consulta [Creare attributi di prodotto per Amazon Matching](./ob-creating-magento-attributes.md).

## Configura [!UICONTROL Catalog Search] impostazioni

1. Fai clic su **[!UICONTROL Listing Settings]** sul dashboard dello store.

1. Espandi la _[!UICONTROL Catalog Search]_sezione .

1. Per **[!UICONTROL ASIN]**, scegli l’attributo di prodotto creato per il valore ASIN di Amazon.

   Un ASO ([!DNL Amazon Standard Identification Number]) è un blocco univoco di dieci lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo.

1. Per **[!UICONTROL EAN]**, scegli l’attributo di prodotto creato per il valore EAN di Amazon.

   Il numero di articolo europeo (EAN) è uno standard di codice a barre, un codice di identificazione del prodotto a 12 o 13 cifre. Ogni EAN identifica in modo univoco il prodotto, il fabbricante e i suoi attributi; in genere, l’EAN viene stampato su un’etichetta di prodotto o su un imballaggio come codice a barre. Amazon richiede codici EAN per migliorare la qualità dei risultati di ricerca e la qualità del catalogo. È possibile ottenere le EAN dal produttore.

1. Per **[!UICONTROL GCID]**, scegli l’attributo di prodotto creato per il valore GCIN di Amazon.

   L’identificatore del catalogo globale (GCID) è un ID per i prodotti privi di codice UPC o ISBN. Il registro dei marchi di Amazon consente di registrarsi come proprietario del marchio e creare un ID univoco per i prodotti.

1. Per **[!UICONTROL ISBN]**, scegli l’attributo di prodotto creato per il valore ISBN di Amazon.

   Il codice a barre ISBN (International Standard Book Number) è un codice a barre unico per l&#39;identificazione dei libri commerciali. Ogni codice ISBN identifica in modo univoco un libro. Un ISBN ha dieci o 13 cifre. Tutte le ISBN assegnate dopo il 1° gennaio 2007 hanno 13 cifre.

1. Per **[!UICONTROL UPC]**, scegli l’attributo di prodotto creato per il valore UPC di Amazon.

   Il codice UPC (Universal Product Code) è un codice a barre a 12 cifre utilizzato ampiamente per gli imballaggi al dettaglio negli Stati Uniti.

1. Per **[!UICONTROL General Search]**, scegli l’attributo di prodotto da utilizzare per una corrispondenza di ricerca generale.

   Questo attributo è selezionabile per la corrispondenza [!DNL Commerce] prodotti per l’elenco Amazon appropriato. La ricerca generale utilizza ricerche di parole chiave dal catalogo. Di conseguenza, si consiglia di utilizzare un [!DNL Commerce] attributo che contiene parole chiave rilevanti, ad esempio SKU del prodotto o nome del prodotto. La ricerca generale può restituire molte possibili corrispondenze e in tali casi puoi selezionare l’elenco Amazon appropriato tra le possibili corrispondenze. Una selezione comune per questo campo è `Product Name`.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Ricerca nel catalogo](assets/amazon-catalog-search.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per [!DNL Amazon Standard Identification Number]. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL EAN (European Article Number)] | Codice di identificazione del prodotto a 12 o 13 cifre. Il numero di articolo europeo (EAN) è uno standard di codice a barre, un codice di identificazione del prodotto a 12 o 13 cifre. Ogni EAN identifica in modo univoco il prodotto, il fabbricante e i suoi attributi; in genere, l’EAN viene stampato su un’etichetta di prodotto o su un imballaggio come codice a barre. Amazon richiede codici EAN per migliorare la qualità dei risultati di ricerca e la qualità del catalogo. È possibile ottenere le EAN dal produttore. |
| [!UICONTROL GCID (Global Catalog Identifier)] | L’identificatore del catalogo globale (GCID) è un ID per i prodotti privi di codice UPC o ISBN. Il registro dei marchi di Amazon consente di registrarsi come proprietario del marchio e creare un ID univoco per i prodotti che potrebbero non avere un UPC o ISBN. |
| [!UICONTROL ISBN (International Standard Book Number)] | Codice a barre di identificazione del libro commerciale univoco a 10 o 13 cifre. Il codice a barre ISBN (International Standard Book Number) è un codice a barre unico per l&#39;identificazione dei libri commerciali. Ogni codice ISBN identifica in modo univoco un libro. Un ISBN ha dieci o 13 cifre. Tutte le ISBN assegnate dopo il 1° gennaio 2007 hanno 13 cifre. |
| UPC (Codice prodotto universale) | Codice a barre a 12 cifre. Il codice UPC (Universal Product Code) è un codice a barre a 12 cifre utilizzato ampiamente per gli imballaggi al dettaglio negli Stati Uniti. |
| [!UICONTROL General Search] | Seleziona un attributo. Questo attributo è selezionabile per la corrispondenza [!DNL Commerce] prodotti per l’elenco Amazon appropriato. La ricerca generale utilizza ricerche di parole chiave dal catalogo. Di conseguenza, si consiglia di utilizzare un [!DNL Commerce] attributo che contiene parole chiave rilevanti, ad esempio SKU del prodotto o nome del prodotto. La ricerca generale può restituire molte possibili corrispondenze e in tali casi puoi selezionare l’elenco Amazon appropriato tra le possibili corrispondenze. Una selezione comune per questo campo è `Product Name`. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
