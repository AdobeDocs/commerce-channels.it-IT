---
title: Prezzo di listino
description: Utilizza le impostazioni del prezzo di listino per determinare l'origine del prezzo e il valore del prezzo di base (predefinito) per gli annunci Amazon.
redirect_from: /sales-channels/asc/ob-listing-price.html: 
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 1509
ht-degree: 0%

---

# Prezzo di listino

[!UICONTROL Listing Price] Le impostazioni fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell&#39;elenco sono accessibili dal [dashboard del negozio](./amazon-store-dashboard.md).

Queste impostazioni definiscono quale [!DNL Commerce] attributo di prezzo utilizzare come origine del prezzo, che è il valore di prezzo base (predefinito) per le inserzioni in Amazon. Queste impostazioni vengono utilizzate dalle [regole di determinazione dei prezzi](./pricing-rule-general-settings.md) per regolare automaticamente il prezzo di listino di Amazon in relazione al valore impostato per _[!UICONTROL Magento Price Source]_.

Puoi configurare il tuo [ambito tariffario](./price-scope.md) come globale o come sito web. Se l&#39;ambito dei prezzi è impostato su `Global`, esiste un&#39;unica fonte di prezzo per tutti i tuoi negozi/siti web. Se l’ambito del prezzo è impostato su `Website`, l’origine del prezzo utilizza la logica di fallback del prezzo del sito web (se disponibile) seguita dal prezzo predefinito (globale).

Se una regola di elenco è impostata per essere applicata a più siti web, l&#39;ordine in cui viene utilizzato il prezzo del sito web è determinato dall&#39;impostazione di priorità del sito web definita nella [regola di elenco](./listing-rules.md). Queste regole ti consentono di definire i prezzi dei prodotti in tutto il catalogo. Per vedere se utilizzi un ambito prezzi sito web, consulta [Area prezzi catalogo](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target=&quot;_blank&quot;}.

Le opzioni elencate in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ e _[!UICONTROL Strike Through Price (MSRP)]_includono gli attributi di determinazione prezzi configurati. Gli attributi di determinazione prezzi sono attributi di prodotto [!DNL Commerce] con il valore Tipo di input catalogo per Proprietario archivio impostato su `Price`. Vedere [Tipi di input attributo](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target=&quot;_blank&quot;}.

## Configurare le impostazioni del prezzo di listino {#configure-listing-price-settings}

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione _[!UICONTROL Listing Price]_.

1. Per **[!UICONTROL Magento Price Source]** (obbligatorio), scegli un’opzione.

   Il valore predefinito è `Price`. Questa impostazione determina l&#39;origine del prezzo utilizzato per le inserzioni Amazon. Se crei [regole di determinazione prezzi](./pricing-products.md), queste vengono applicate al valore definito per l&#39;attributo selezionato qui. È possibile selezionare qualsiasi attributo di prezzo configurato. Tuttavia, se l&#39;attributo selezionato non viene compilato per un prodotto, l&#39;origine del prezzo del prodotto viene ripristinata in modo predefinito a `Price` quando vengono applicate le regole di prezzo per determinare il prezzo di listino pubblicato di Amazon.

1. Per **[!UICONTROL Minimum Advertised Price (MAP)**], scegli un’opzione.

   Il valore predefinito non è selezionato. Questa impostazione consente un prezzo minimo pubblicizzato (MAP) per un prodotto. Quando definisci un attributo di prezzo e il prezzo di listino di un prodotto scende al di sotto del prezzo minimo determinato (in base all&#39;origine e alle regole del prezzo), questo valore diventa la MAPPA per l&#39;elenco. Questa impostazione ti consente di implementare [regole di determinazione dei prezzi](./pricing-products.md), pur continuando a controllare il prezzo minimo per un prodotto. Per evitare che un prezzo di listino sia troppo basso, scegli un attributo di prezzo da utilizzare come MAPPA. Tuttavia, se il campo di determinazione dei prezzi selezionato non è definito per un prodotto, la MAPPA non viene utilizzata.

1. Per **[!UICONTROL Strike Through Price (MSRP)]**, scegli un’opzione.

   Il valore predefinito non è selezionato. Questa impostazione determina quale attributo di prezzo viene utilizzato come prezzo al dettaglio suggerito dal produttore (MSRP) per un prodotto. Se il prezzo di listino è inferiore al valore MSRP definito, l&#39;elenco Amazon viene visualizzato con uno sconto del prezzo MSRP con il prezzo di listino più basso, insieme all&#39;importo e alla percentuale calcolati di &quot;Risparmia&quot;. Tuttavia, se il campo di determinazione dei prezzi selezionato non è definito per un prodotto, il valore MSRP non viene calcolato.

   >[!NOTE]
   >
   >Questa impostazione si applica solo alle inserzioni che hanno vinto la posizione [Buy Box](./buy-box-competitor-pricing.md). Il Buy Box viene assegnato da Amazon al venditore che ha il prodotto elencato di solito al miglior prezzo, insieme ad altri fattori come la spedizione FBA/Prime offerta, la disponibilità e le prestazioni del venditore.

1. Per **Applica imposta sul valore aggiunto (IVA)**, scegli un&#39;opzione:

   - `Disabled` - (Predefinito) Scegli se non applicare l&#39;IVA al prezzo di listino.

   - `Enabled` - Scegliere quando applicare l&#39;IVA al prezzo di listino. L&#39;IVA viene generalmente utilizzata come imposta sulle vendite nei paesi europei e viene aggiunta al prezzo finale elencato all&#39;interno di Amazon. L&#39;IVA non si applica al prezzo finale per gli inserimenti utilizzati nell&#39;ambito di una regola di determinazione intelligente dei prezzi, a meno che non venga colpito il [prezzo minimo](./floor-price.md).
   >[!NOTE]
   >
   >Le imprese dell&#39;Unione europea (UE) sono tenute a inviare fatture agli acquirenti commerciali, in modo che il cliente possa sgravare le imposte. È possibile generare queste fatture e calcolare autonomamente le imposte oppure utilizzare un servizio di calcolo delle imposte come Amazon VAT Calculation Service. Amazon consiglia di registrarsi per il [servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target=&quot;_blank&quot;}. Se scegli un metodo diverso, sei responsabile della conformità IVA.>
   >
   >Potrebbero essere necessari 10-14 giorni perché Amazon verifichi e attivi il tuo account Servizio di calcolo dell&#39;IVA.

1. Per **[!UICONTROL VAT Percentage]**, immettere il valore dell&#39;aliquota IVA.

   Il valore predefinito è `0.00`. Questo valore viene utilizzato per calcolare l&#39;importo dell&#39;IVA da aggiungere al prezzo di quotazione. Se viene inserito `10.2`, al prezzo di listino viene applicata un’IVA del 10,20%. Questo campo è disabilitato quando il campo Applica imposta sul valore aggiunto (IVA) è impostato su `Disabled`.

1. **(Solo store nel Regno Unito)** Per  **[!UICONTROL Amazon Product Tax Code (PTC)]**, scegli un’opzione:

   - `Do Not Manage PTC` - (Impostazione predefinita) Scegliere se si utilizza un servizio di calcolo dell&#39;imposta di terze parti o se tutti i calcoli dell&#39;imposta sono già stati impostati nel  [!DNL Amazon Seller Central] conto. Quando scelto, il canale di vendita Amazon non invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central].

   - `Set Default PTC` - Scegliere se si dispone di un codice di imposta sul prodotto universale (PTC) che si desidera utilizzare per tutti i prodotti. Una volta scelto, devi completare _[!UICONTROL Default PTC]_.

      - Per **[!UICONTROL Default PTC]**, immettere il PTC predefinito da utilizzare per tutti gli elenchi Amazon idonei. Se il PTC predefinito è impostato nell&#39;account [!DNL Amazon Seller Central], lasciare vuoto questo campo. Le modifiche apportate a questo campo non influiscono sugli elenchi Amazon esistenti. Per modificare il PTC predefinito per un elenco esistente, l&#39;elenco deve essere [ended](./end-listings-manually.md) e deve essere creato un nuovo elenco.
   >[!NOTE]
   >
   >Se si utilizza il servizio di calcolo IVA di Amazon, è necessario conoscere la categoria di imposta per i prodotti. A PTC è il codice ID della categoria fiscale Amazon per gli acquisti B2B nell&#39;UE. Consulta [Codici imposta sui prodotti Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}.

1. Per **[!UICONTROL Currency Conversion]**, scegli un’opzione.

   Il valore predefinito è `Disabled`. Queste opzioni dipendono dalle impostazioni [!DNL Commerce] [currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;}. Se non sono disponibili opzioni, impostare le impostazioni della valuta.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Prezzo di listino](assets/amazon-listing-price.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Magento Price Source] | Determina l&#39;origine dei prezzi utilizzata per la creazione degli elenchi Amazon. Il valore predefinito è `Price`. Se scegli un attributo diverso, ad esempio `Amazon Price` o `Special Price`, il valore definito per l’attributo viene utilizzato per l’elenco di Amazon. Tuttavia, se l’attributo selezionato non è definito, viene utilizzato `Price`. |
| [!UICONTROL Minimum Advertised Price (MAP)] | L&#39;attributo [!DNL Commerce] per i prezzi MAP. Se scegli l’opzione MAP, l’inserzione Amazon viene impostata automaticamente sul prezzo MAP se il prezzo di listino è inferiore al prezzo MAP. |
| [!UICONTROL Strike Through Price (MSRP)] | L&#39;attributo [!DNL Commerce] che rappresenta il prezzo MSRP. Se il prezzo di listino di Amazon è inferiore a quello di MSRP, viene visualizzato uno stralcio del prezzo MSRP e del prezzo di listino. Questa impostazione viene utilizzata anche per calcolare la quantità e la percentuale di salvataggio, ma questa funzione si applica solo agli elenchi che hanno vinto la posizione [Buy Box](./buy-box-competitor-pricing.md). |
| [!UICONTROL Apply Value Added Tax (VAT)] | L&#39;IVA è utilizzata dai venditori dell&#39;Unione europea.<br><br>Scegliere  `Disabled` se non si desidera aggiungere l&#39;IVA ai prezzi di listino.<br><br>Scegliere  `Enabled` e quindi inserire la percentuale IVA per applicare l&#39;IVA ai prezzi di listino. |
| [!UICONTROL VAT Percentage] | Definisci la percentuale da utilizzare per calcolare l&#39;importo dell&#39;IVA da aggiungere al prezzo di listino per le inserzioni Amazon. <br><br>Se si inserisce  `5`, al prezzo finale di listino verrà applicata un&#39;IVA del 5% dopo l&#39;applicazione di tutte le regole di determinazione dei prezzi. L&#39;imposta IVA non si applica al prezzo finale per gli elenchi utilizzati nell&#39;ambito di una regola di determinazione intelligente dei prezzi, a meno che non venga premuto il tasto [floor](./floor-price.md) o [soffitto](./optional-ceiling-price.md). |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Appare solo per i negozi del Regno Unito) Determina se il canale di vendita Amazon invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central]. <br><br>Selezionare  **Non gestire** PTCse si utilizza un servizio di calcolo delle imposte di terze parti o se tutti i calcoli fiscali sono già stati impostati nel proprio  [!DNL Amazon Seller Central] account. Quando è impostata su questa opzione, il canale vendite Amazon non invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central].<br><br>Selezionare  **Imposta** PTC predefinitose si dispone di un codice di imposta sul prodotto universale che si desidera utilizzare per tutti i prodotti.<br><br>Consulta  [Codici imposta prodotto Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}. |
| [!UICONTROL Default PTC] | Viene visualizzato solo quando **Codice fiscale prodotto Amazon (PTC)** è impostato su `Set Default PTC`. Immettere il PTC predefinito da utilizzare per tutti gli elenchi Amazon idonei. Se il PTC predefinito è impostato nell&#39;account [!DNL Amazon Seller Central], lasciare vuoto questo campo. <br><br>Le modifiche apportate a questo campo non influiscono sugli elenchi esistenti. L&#39;elenco deve essere [terminato](./end-listings-manually.md) e deve essere creato un nuovo elenco per rendere effettiva la modifica. |
| [!UICONTROL Currency Conversion] | Consente la conversione accurata della valuta predefinita della vetrina [!DNL Commerce] nella valuta predefinita di Amazon per pubblicare i prezzi delle inserzioni nella valuta corretta. La conversione della valuta è sempre basata sulla [!DNL Commerce] valuta predefinita.<br><br>È comunque possibile visualizzare le valute predefinite  [!DNL Commerce] e Amazon quando sono disponibili altre valute. Se la valuta [!DNL Commerce] predefinita corrisponde alla valuta Amazon predefinita, lasciare disabilitata la conversione della valuta.<br><br>Ad esempio, se la valuta  [!DNL Commerce] predefinita è CAD (Dollaro canadese) e la valuta predefinita di Amazon è USD, è necessario abilitare Conversione valuta e scegliere il CAD del tasso di conversione in USD. Le opzioni presentate si basano sulle conversioni di valuta [!DNL Commerce] integrate. Se l&#39;opzione desiderata non è visibile, [impostare la valuta in [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;}. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
