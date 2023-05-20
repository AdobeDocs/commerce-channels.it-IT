---
title: Prezzo di vendita
description: Utilizza le impostazioni Prezzo inserzione per determinare l'origine del prezzo e il valore del prezzo di base (predefinito) per le tue inserzioni Amazon.
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

# Prezzo di vendita

[!UICONTROL Listing Price] Le impostazioni fanno parte delle impostazioni dell&#39;inserzione del Negozio. Le impostazioni dell&#39;inserzione sono accessibili da [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni definiscono quali [!DNL Commerce] attributo di determinazione prezzi da utilizzare come origine del prezzo, che è il valore di prezzo di base (predefinito) per le inserzioni Amazon. Queste impostazioni vengono utilizzate dal [regole di determinazione prezzi](./pricing-rule-general-settings.md) per regolare automaticamente il prezzo dell’inserzione Amazon in base al valore impostato per _[!UICONTROL Magento Price Source]_.

Puoi configurare il [ambito di determinazione prezzi](./price-scope.md) come sito globale o sito Web. Se l&#39;ambito di determinazione prezzi è impostato su `Global`, esiste un’unica fonte di prezzo per tutti i tuoi negozi/siti web. Se l&#39;ambito di determinazione prezzi è impostato su `Website`, l’origine del prezzo utilizza la logica di fallback del prezzo del sito web (se disponibile) seguita dal prezzo predefinito (globale).

Se una regola di inserzione è impostata per essere applicata a più siti Web, l&#39;ordine in cui viene utilizzato il prezzo del sito Web è determinato dall&#39;impostazione di priorità del sito Web definita nella [regola di elenco](./listing-rules.md). Queste regole ti consentono di definire i prezzi dei prodotti all’interno del catalogo. Per verificare se si utilizza l&#39;ambito di prezzo del sito Web, vedere [Ambito prezzo catalogo](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target="_blank"}.

Le opzioni elencate in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_, e _[!UICONTROL Strike Through Price (MSRP)]_includere gli attributi di determinazione prezzi configurati. Gli attributi di determinazione prezzi sono [!DNL Commerce] attributi del prodotto con il valore Tipo di input catalogo per Proprietario negozio impostato su `Price`. Consulta [Tipi di input degli attributi](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target="_blank"}.

## Configura le impostazioni del prezzo dell&#39;inserzione {#configure-listing-price-settings}

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi _[!UICONTROL Listing Price]_sezione.

1. Per **[!UICONTROL Magento Price Source]** (obbligatorio), scegli un’opzione.

   Il valore predefinito è `Price`. Questa impostazione determina l&#39;origine del prezzo utilizzata per le inserzioni Amazon. Se si crea [regole di determinazione prezzi](./pricing-products.md), le regole vengono applicate al valore definito per l’attributo selezionato qui. È possibile selezionare qualsiasi attributo di determinazione prezzi configurato. Tuttavia, se l&#39;attributo selezionato non viene compilato per un prodotto, l&#39;origine del prezzo del prodotto viene impostata automaticamente su `Price` quando vengono applicate le regole di determinazione prezzi per determinare il prezzo di listino di Amazon pubblicato.

1. Per **[!UICONTROL Minimum Advertised Price (MAP)**], scegli un’opzione.

   L&#39;impostazione predefinita è nessuna selezione. Questa impostazione consente di impostare un prezzo minimo annunciato (MAP) per un prodotto. Quando si definisce un attributo di determinazione prezzi e il prezzo di un prodotto scende al di sotto del prezzo minimo determinato (in base all&#39;origine e alle regole di determinazione prezzi), questo valore diventa il MAP dell&#39;inserzione. Questa impostazione consente di implementare [regole di determinazione prezzi](./pricing-products.md), pur continuando a controllare il prezzo minimo di un prodotto. Per evitare che il prezzo di un&#39;inserzione sia troppo basso, scegliere un attributo di determinazione prezzi da utilizzare come MAP. Tuttavia, se il campo di determinazione prezzi selezionato non è definito per un prodotto, il MAP non viene utilizzato.

1. Per **[!UICONTROL Strike Through Price (MSRP)]**, scegli un’opzione.

   L&#39;impostazione predefinita è nessuna selezione. Questa impostazione determina quale attributo di prezzo viene utilizzato come prezzo di vendita consigliato dal produttore per un prodotto. Se il prezzo dell&#39;inserzione è inferiore al prezzo MSRP definito, l&#39;inserzione Amazon viene visualizzata con una barratura del prezzo MSRP con il prezzo dell&#39;inserzione più basso, insieme all&#39;importo e alla percentuale di &quot;salvataggio&quot; calcolati. Tuttavia, se il campo di determinazione prezzi selezionato non è definito per un prodotto, il piano MSRP non viene calcolato.

   >[!NOTE]
   >
   >Questa impostazione è valida solo per le inserzioni che hanno vinto [Buy Box](./buy-box-competitor-pricing.md) posizione. Il Buy Box viene assegnato da Amazon al venditore che ha il prodotto elencato di solito al prezzo migliore, insieme ad altri fattori come la spedizione FBA/Prime offerta, la disponibilità e le prestazioni del venditore.

1. Per **Applica IVA**, scegli un’opzione:

   - `Disabled` - (Impostazione predefinita) Scegli quando non desideri applicare l&#39;IVA al prezzo dell&#39;inserzione.

   - `Enabled` - Scegli quando applicare l&#39;IVA al prezzo dell&#39;inserzione. L’IVA viene generalmente utilizzata come imposta sulle vendite nei paesi europei e viene aggiunta al prezzo finale indicato in Amazon. L&#39;IVA non si applica al prezzo finale per le inserzioni utilizzate in una regola di determinazione prezzi intelligente, a meno che [prezzo base](./floor-price.md) è un hit.
   >[!NOTE]
   >
   >Le imprese dell&#39;Unione europea (UE) sono tenute a inviare fatture agli acquirenti, in modo che il cliente possa trasferire l&#39;imposta. È possibile generare queste fatture e calcolare le imposte personalmente oppure utilizzare un servizio di calcolo delle imposte come Amazon VAT Calculation Service. Amazon consiglia di registrarsi al [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target="_blank"}. Se scegli un metodo diverso, sei responsabile della conformità IVA.>
   >
   >Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

1. Per **[!UICONTROL VAT Percentage]**, immettere il valore per l&#39;aliquota IVA.

   Il valore predefinito è `0.00`. Questo valore viene utilizzato per calcolare l&#39;importo IVA da aggiungere al prezzo di listino. Se `10.2` L&#39;inserzione comporta l&#39;applicazione di un&#39;IVA del 10,20%. Questo campo è disattivato quando il campo Applica imposta sul valore aggiunto (IVA) è impostato su `Disabled`.

1. **(solo per i negozi del Regno Unito)** Per **[!UICONTROL Amazon Product Tax Code (PTC)]**, scegli un’opzione:

   - `Do Not Manage PTC` - (Impostazione predefinita) Scegli se utilizzi un servizio di calcolo delle imposte di terze parti o se tutti i calcoli delle imposte sono già stati impostati nel [!DNL Amazon Seller Central] account. Quando viene scelto, il canale di vendita Amazon non invia informazioni sul codice fiscale del prodotto al tuo [!DNL Amazon Seller Central] account.

   - `Set Default PTC` - Scegliere se si dispone di un codice IVA prodotto universale (PTC) che si desidera utilizzare per tutti i prodotti. Una volta scelto, devi completare _[!UICONTROL Default PTC]_.

      - Per **[!UICONTROL Default PTC]**, inserisci il PTC predefinito da utilizzare per tutte le inserzioni Amazon idonee. Se il PTC predefinito è impostato nel [!DNL Amazon Seller Central] account, lascia vuoto questo campo. Le modifiche apportate a questo campo non influiscono sulle inserzioni esistenti di Amazon. Per modificare il PTC predefinito per un&#39;inserzione esistente, l&#39;inserzione deve essere [terminato](./end-listings-manually.md) e viene creata una nuova inserzione.
   >[!NOTE]
   >
   >Se utilizzi il Servizio di calcolo IVA di Amazon, devi conoscere la categoria fiscale dei tuoi prodotti. Un PTC è il codice ID della categoria fiscale di Amazon per gli acquisti B2B nell’UE. Consulta [Codici imposta prodotto di Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}.

1. Per **[!UICONTROL Currency Conversion]**, scegli un’opzione.

   Il valore predefinito è `Disabled`. Queste opzioni dipendono dal [!DNL Commerce] [valuta](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target="_blank"} impostazioni. Se non sono disponibili opzioni, impostare le impostazioni di valuta.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Prezzo di vendita](assets/amazon-listing-price.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Magento Price Source] | Determina l&#39;origine del prezzo utilizzata durante la creazione delle inserzioni Amazon. Il valore predefinito è `Price`. Se scegli un attributo diverso, ad esempio `Amazon Price` o `Special Price`, il valore definito per l’attributo viene utilizzato per l’inserzione in Amazon. Tuttavia, se l’attributo selezionato non è definito, `Price` viene utilizzato. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Il [!DNL Commerce] Attributo per la determinazione dei prezzi MAP. Scegliendo l&#39;opzione MAP, l&#39;inserzione Amazon viene automaticamente impostata sul prezzo MAP se quest&#39;ultimo è inferiore al prezzo MAP. |
| [!UICONTROL Strike Through Price (MSRP)] | Il [!DNL Commerce] attributo che rappresenta la determinazione prezzi MSRP. Se il prezzo dell&#39;inserzione Amazon è inferiore al prezzo MSRP, viene visualizzato uno strike-through del prezzo MSRP e del prezzo dell&#39;inserzione. Questa impostazione viene utilizzata anche per calcolare l&#39;importo e la percentuale del &quot;salvataggio&quot;, ma questa funzione si applica solo alle inserzioni che hanno vinto il [Buy Box](./buy-box-competitor-pricing.md) posizione. |
| [!UICONTROL Apply Value Added Tax (VAT)] | L&#39;IVA è utilizzata dai venditori nell&#39;Unione europea.<br><br>Scegli `Disabled` se non desideri aggiungere l’IVA ai prezzi di inserzione.<br><br>Scegli `Enabled` e quindi inserire la Percentuale IVA per applicare l&#39;IVA ai prezzi dell&#39;inserzione. |
| [!UICONTROL VAT Percentage] | Definisci la percentuale da utilizzare per calcolare l&#39;importo IVA da aggiungere al prezzo di inserzione per le inserzioni Amazon. <br><br>Se si immette `5`, al prezzo di vendita finale verrà applicata un&#39;IVA del 5% dopo l&#39;applicazione di tutte le regole di determinazione dei prezzi. L&#39;IVA non si applica al prezzo finale per le inserzioni utilizzate in una regola di determinazione prezzi intelligente, a meno che il [piano](./floor-price.md) o [soffitto](./optional-ceiling-price.md) è un hit. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Solo per i Negozi del Regno Unito) Determina se il canale di vendita Amazon invia le informazioni sul codice fiscale del prodotto al tuo [!DNL Amazon Seller Central] account. <br><br>Seleziona **Non gestire PTC** se si utilizza un servizio di calcolo delle imposte di terze parti o si dispone già di tutti i calcoli delle imposte impostati nel [!DNL Amazon Seller Central] account. Quando è impostato su questa opzione, il canale di vendita Amazon non invia informazioni sul codice IVA del prodotto al tuo [!DNL Amazon Seller Central] account.<br><br>Seleziona **Imposta PTC predefinito** se si dispone di un codice imposta prodotto universale da utilizzare per tutti i prodotti.<br><br>Consulta [Codici imposta prodotto di Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}. |
| [!UICONTROL Default PTC] | Viene visualizzato solo quando **Codice imposta prodotto Amazon (PTC)** è impostato su `Set Default PTC`. Immettere il PTC predefinito da utilizzare per tutte le inserzioni Amazon idonee. Se il PTC predefinito è impostato nel [!DNL Amazon Seller Central] account, lascia vuoto questo campo. <br><br>Le modifiche apportate a questo campo non influiscono sulle inserzioni esistenti. L’inserzione deve essere [terminato](./end-listings-manually.md) e viene creata una nuova inserzione per rendere effettiva la modifica. |
| [!UICONTROL Currency Conversion] | Consente il [!DNL Commerce] storefront valuta predefinita per convertire accuratamente nella tua valuta Amazon predefinita per pubblicare i prezzi delle inserzioni nella valuta corretta. La conversione della valuta si basa sempre sul [!DNL Commerce] valuta predefinita.<br><br>Puoi comunque visualizzare le impostazioni predefinite [!DNL Commerce] e le valute di Amazon quando sono disponibili altre valute. Se il valore predefinito [!DNL Commerce] La valuta corrisponde alla valuta Amazon predefinita; lascia disabilitata la funzione Conversione valuta.<br><br>Ad esempio, se [!DNL Commerce] La valuta predefinita è CAD (Dollaro canadese) e la valuta predefinita di Amazon è USD. È necessario abilitare la funzione Conversione valuta e scegliere il tasso di conversione da CAD a USD. Le opzioni visualizzate si basano sul [!DNL Commerce] conversioni di valuta. Se l&#39;opzione desiderata non è visualizzata, [imposta la valuta in [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target="_blank"}. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
