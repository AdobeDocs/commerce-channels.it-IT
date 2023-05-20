---
title: Ricerca nel catalogo
description: Per impostare la corrispondenza degli attributi che consente di mappare i prodotti idonei del catalogo Commerce con le inserzioni di Amazon, aggiorna le impostazioni di Ricerca nel catalogo.
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Ricerca nel catalogo

_Ricerca nel catalogo_ Le impostazioni fanno parte delle impostazioni dell&#39;inserzione del Negozio. Le impostazioni dell&#39;inserzione sono accessibili da [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni consentono di impostare la corrispondenza degli attributi che facilita la mappatura degli idonei [!DNL Commerce] prodotti con inserzioni Amazon. Una volta eseguito il mapping, Amazon attiva le azioni relative alla determinazione dei prezzi, alla quantità, alle sostituzioni e alla sincronizzazione di ordini e prodotti.

La definizione di questi valori di mappatura aumenta la possibilità di corrispondenze esatte, riducendo al minimo la necessità di abbinare manualmente gli elenchi di prodotti. Aggiunta di attributi come parte del [Attività di pre-configurazione](./amazon-pre-setup-tasks.md), il canale di vendita Amazon ha un potenziale più elevato per abbinare automaticamente i prodotti durante l’onboarding e sincronizzare i dati dei prodotti tra Amazon e [!DNL Commerce].

Se crei solo l’attributo ASIN di Amazon (senza aggiungere valori ASIN per prodotto), il tuo [!DNL Commerce] I prodotti potrebbero non corrispondere automaticamente alle inserzioni Amazon. È possibile [assegna manualmente](./creating-assigning-catalog-products.md) i tuoi prodotti. Tuttavia, la corrispondenza manuale non crea gli elementi di dati necessari per condividere e sincronizzare i dati di prodotto.

>[!IMPORTANT]
>
>Se hai creato manualmente una corrispondenza con un prodotto e desideri aggiornare un ASIN, UPC o un altro elemento dati per il prodotto, devi aggiornare i dati in due posizioni. Aggiornalo nel tuo [!DNL Commerce] e nell’inserzione Amazon nel tuo [!DNL Amazon Seller Central] account.

È consigliabile mappare questi attributi e valori, se disponibili. Il completamento di questa mappatura non è richiesto, ma è utile per la corrispondenza dei prodotti e richiesto per la corretta sincronizzazione dei cataloghi tra Amazon e [!DNL Commerce].

Se desideri aggiungere attributi, consulta [Creare attributi di prodotto per corrispondenza Amazon](./ob-creating-magento-attributes.md).

## Configura [!UICONTROL Catalog Search] impostazioni

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi _[!UICONTROL Catalog Search]_sezione.

1. Per **[!UICONTROL ASIN]**, scegli l’attributo del prodotto creato per il valore Amazon ASIN.

   Un ASIN ([!DNL Amazon Standard Identification Number]) è un blocco univoco di dieci lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento.

1. Per **[!UICONTROL EAN]**, scegli l’attributo del prodotto creato per il valore EAN di Amazon.

   Il numero di articolo europeo (EAN) è uno standard di codice a barre, un codice di identificazione del prodotto a 12 o 13 cifre. Ogni EAN identifica in modo univoco il prodotto, il produttore e i relativi attributi; in genere, l&#39;EAN viene stampato su un&#39;etichetta o un imballaggio di prodotto come codice a barre. Amazon richiede codici EAN per migliorare la qualità dei risultati della ricerca e la qualità del catalogo. È possibile ottenere gli EAN dal produttore.

1. Per **[!UICONTROL GCID]**, scegli l’attributo del prodotto creato per il valore GCIN di Amazon.

   Il Global Catalog Identifier (GCID) è un ID per prodotti che non hanno un codice UPC o ISBN. Il registro dei marchi di Amazon consente di registrarsi come proprietario del marchio e di creare un ID univoco per i prodotti.

1. Per **[!UICONTROL ISBN]**, scegli l’attributo del prodotto creato per il valore ISBN di Amazon.

   L&#39;International Standard Book Number (ISBN) è un codice a barre identificativo unico del libro commerciale. Ogni codice ISBN identifica in modo univoco un libro. Un ISBN ha dieci o tredici cifre. Tutti gli ISBN assegnati dopo il 1° gennaio 2007 hanno 13 cifre.

1. Per **[!UICONTROL UPC]**, scegli l’attributo del prodotto creato per il valore UPC di Amazon.

   L&#39;Universal Product Code (UPC) è un codice a barre a 12 cifre ampiamente utilizzato per gli imballaggi al dettaglio negli Stati Uniti.

1. Per **[!UICONTROL General Search]**, scegli l’attributo del prodotto che desideri utilizzare per una corrispondenza di ricerca generale.

   Questo attributo può essere selezionato per la corrispondenza [!DNL Commerce] nell’elenco Amazon appropriato. La ricerca generale utilizza le ricerche per parola chiave dal catalogo. Pertanto, si consiglia di utilizzare un [!DNL Commerce] attributo contenente parole chiave rilevanti, ad esempio SKU del prodotto o nome del prodotto. La ricerca generale può restituire molte corrispondenze possibili e in questi casi puoi selezionare l’elenco Amazon appropriato tra le possibili corrispondenze. Una selezione comune per questo campo è `Product Name`.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Ricerca nel catalogo](assets/amazon-catalog-search.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN è l&#39;acronimo di [!DNL Amazon Standard Identification Number]. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL EAN (European Article Number)] | Un codice di identificazione del prodotto a 12 o 13 cifre. Il numero di articolo europeo (EAN) è uno standard di codice a barre, un codice di identificazione del prodotto a 12 o 13 cifre. Ogni EAN identifica in modo univoco il prodotto, il produttore e i relativi attributi; in genere, l&#39;EAN viene stampato su un&#39;etichetta o un imballaggio di prodotto come codice a barre. Amazon richiede codici EAN per migliorare la qualità dei risultati della ricerca e la qualità del catalogo. È possibile ottenere gli EAN dal produttore. |
| [!UICONTROL GCID (Global Catalog Identifier)] | Il Global Catalog Identifier (GCID) è un ID per prodotti che non hanno un codice UPC o ISBN. Il registro dei marchi di Amazon consente di registrarsi come proprietario del marchio e di creare un ID univoco per i prodotti che potrebbero non disporre di un UPC o ISBN. |
| [!UICONTROL ISBN (International Standard Book Number)] | Codice a barre identificativo unico del libro commerciale a 10 o 13 cifre. L&#39;International Standard Book Number (ISBN) è un codice a barre identificativo unico del libro commerciale. Ogni codice ISBN identifica in modo univoco un libro. Un ISBN ha dieci o tredici cifre. Tutti gli ISBN assegnati dopo il 1° gennaio 2007 hanno 13 cifre. |
| UPC (Universal Product Code) | Codice a barre a 12 cifre. L&#39;Universal Product Code (UPC) è un codice a barre a 12 cifre ampiamente utilizzato per gli imballaggi al dettaglio negli Stati Uniti. |
| [!UICONTROL General Search] | Seleziona un attributo. Questo attributo può essere selezionato per la corrispondenza [!DNL Commerce] nell’elenco Amazon appropriato. La ricerca generale utilizza le ricerche per parola chiave dal catalogo. Pertanto, si consiglia di utilizzare un [!DNL Commerce] attributo contenente parole chiave rilevanti, ad esempio SKU del prodotto o nome del prodotto. La ricerca generale può restituire molte corrispondenze possibili e in questi casi puoi selezionare l’elenco Amazon appropriato tra le possibili corrispondenze. Una selezione comune per questo campo è `Product Name`. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
