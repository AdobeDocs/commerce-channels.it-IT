---
title: Canale di vendita Amazon - [!UICONTROL Listing Price]
description: Utilizza le impostazioni Prezzo inserzione per determinare l'origine del prezzo e il valore del prezzo di base (predefinito) per le tue inserzioni Amazon.
feature: Sales Channels, Products, Price Rules
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 0%

---

# [!UICONTROL Listing Price]

Le impostazioni di [!UICONTROL Listing Price] fanno parte delle impostazioni dell&#39;inserzione dello store. Le impostazioni dell&#39;inserzione sono accessibili dal [dashboard dell&#39;archivio](./amazon-store-dashboard.md).

Queste impostazioni definiscono quale attributo di determinazione prezzi [!DNL Commerce] utilizzare come origine del prezzo, che è il valore di prezzo di base (predefinito) per le inserzioni Amazon. Queste impostazioni vengono utilizzate dalle [regole di determinazione prezzi](./pricing-rule-general-settings.md) per adeguare automaticamente il prezzo dell&#39;inserzione di Amazon relativo al valore impostato per _[!UICONTROL Magento Price Source]_.

Puoi configurare l&#39;[ambito di determinazione prezzi](./price-scope.md) come globale o sito Web. Se l&#39;ambito di determinazione prezzi è impostato su `Global`, esiste un&#39;unica origine di prezzo per tutti i negozi/siti Web. Se l&#39;ambito di determinazione prezzi è impostato su `Website`, l&#39;origine prezzo utilizza la logica di fallback del prezzo del sito Web (se disponibile) seguita dal prezzo predefinito (globale).

Se una regola di elenco è impostata per essere applicata a più siti Web, l&#39;ordine in cui viene utilizzato il prezzo del sito Web è determinato dall&#39;impostazione di priorità del sito Web definita nella [regola di elenco](./listing-rules.md). Queste regole ti consentono di definire i prezzi dei prodotti all’interno del catalogo. Per verificare se si utilizza l&#39;ambito prezzi del sito Web, vedere [Ambito prezzi catalogo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html).

Le opzioni elencate in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ e _[!UICONTROL Strike Through Price (MSRP)]_includono gli attributi di determinazione prezzi configurati. Gli attributi di determinazione prezzi sono [!DNL Commerce] attributi di prodotto con il valore Tipo di input catalogo per Proprietario negozio impostato su `Price`. Vedi [Tipi di input attributo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/attributes-input-types.html).

## Configura le impostazioni del prezzo dell&#39;inserzione {#configure-listing-price-settings}

1. Fare clic su **[!UICONTROL Listing Settings]** nel dashboard dell&#39;archivio.

1. Espandere la sezione _[!UICONTROL Listing Price]_.

1. Per **[!UICONTROL Magento Price Source]** (obbligatorio), scegliere un&#39;opzione.

   Il valore predefinito è `Price`. Questa impostazione determina l&#39;origine del prezzo utilizzata per le inserzioni Amazon. Se crei [regole di determinazione prezzi](./pricing-products.md), queste vengono applicate al valore definito per l&#39;attributo selezionato qui. È possibile selezionare qualsiasi attributo di determinazione prezzi configurato. Tuttavia, se l&#39;attributo selezionato non viene compilato per un prodotto, l&#39;origine prezzo per il prodotto torna automaticamente a `Price` quando vengono applicate le regole di determinazione prezzi per determinare il prezzo di listino Amazon pubblicato.

1. Per **[!UICONTROL Minimum Advertised Price (MAP)**], scegliere un&#39;opzione.

   L&#39;impostazione predefinita è nessuna selezione. Questa impostazione consente di impostare un prezzo minimo annunciato (MAP) per un prodotto. Quando si definisce un attributo di determinazione prezzi e il prezzo di un prodotto scende al di sotto del prezzo minimo determinato (in base all&#39;origine e alle regole di determinazione prezzi), questo valore diventa il MAP dell&#39;inserzione. Questa impostazione ti consente di implementare [regole di prezzo](./pricing-products.md), controllando al contempo il prezzo minimo per un prodotto. Per evitare che il prezzo di un&#39;inserzione sia troppo basso, scegliere un attributo di determinazione prezzi da utilizzare come MAP. Tuttavia, se il campo di determinazione prezzi selezionato non è definito per un prodotto, il MAP non viene utilizzato.

1. Per **[!UICONTROL Strike Through Price (MSRP)]**, scegliere un&#39;opzione.

   L&#39;impostazione predefinita è nessuna selezione. Questa impostazione determina quale attributo di prezzo viene utilizzato come prezzo di vendita consigliato dal produttore per un prodotto. Se il prezzo dell&#39;inserzione è inferiore al prezzo MSRP definito, l&#39;inserzione Amazon viene visualizzata con una barratura del prezzo MSRP con il prezzo dell&#39;inserzione più basso, insieme all&#39;importo e alla percentuale di &quot;salvataggio&quot; calcolati. Tuttavia, se il campo di determinazione prezzi selezionato non è definito per un prodotto, il piano MSRP non viene calcolato.

   >[!NOTE]
   >
   >Questa impostazione è valida solo per le inserzioni che hanno vinto la posizione [Buy Box](./buy-box-competitor-pricing.md). Il Buy Box viene assegnato da Amazon al venditore che ha il prodotto elencato di solito al prezzo migliore, insieme ad altri fattori come la spedizione FBA/Prime offerta, la disponibilità e le prestazioni del venditore.

1. Per **Applica imposta sul valore aggiunto (IVA)**, scegliere un&#39;opzione:

   - `Disabled` - (Predefinito) Scegli quando non vuoi applicare l&#39;IVA al prezzo dell&#39;inserzione.

   - `Enabled` - Scegli quando applicare l&#39;IVA al prezzo dell&#39;inserzione. L’IVA viene generalmente utilizzata come imposta sulle vendite nei paesi europei e viene aggiunta al prezzo finale indicato in Amazon. L&#39;IVA non viene applicata al prezzo finale per le inserzioni utilizzate in una regola di determinazione prezzi intelligente, a meno che non venga raggiunto il [prezzo minimo](./floor-price.md).

   >[!NOTE]
   >
   >Le imprese dell&#39;Unione europea (UE) sono tenute a inviare fatture agli acquirenti, in modo che il cliente possa trasferire l&#39;imposta. È possibile generare queste fatture e calcolare le imposte personalmente oppure utilizzare un servizio di calcolo delle imposte come Amazon VAT Calculation Service. Amazon consiglia di iscriversi al [Servizio di calcolo IVA di Amazon](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;). Se scegli un metodo diverso, sei responsabile della conformità IVA.>
   >
   >Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

1. Per **[!UICONTROL VAT Percentage]**, immetti il valore per l&#39;aliquota IVA.

   Il valore predefinito è `0.00`. Questo valore viene utilizzato per calcolare l&#39;importo IVA da aggiungere al prezzo di listino. Se si immette `10.2`, al prezzo dell&#39;inserzione verrà applicata un&#39;IVA del 10,20%. Questo campo è disabilitato quando il campo Applica imposta sul valore aggiunto (IVA) è impostato su `Disabled`.

1. **(Solo per i negozi del Regno Unito)** Per **[!UICONTROL Amazon Product Tax Code (PTC)]**, scegli un&#39;opzione:

   - `Do Not Manage PTC` - (impostazione predefinita) Scegliere se si sta utilizzando un servizio di calcolo delle imposte di terze parti o se tutti i calcoli delle imposte sono già stati impostati nel proprio account [!DNL Amazon Seller Central]. Quando viene scelto, il canale di vendita Amazon non invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central].

   - `Set Default PTC` - Scegliere se si desidera utilizzare un codice IVA universale per tutti i prodotti. Una volta scelto, devi completare _[!UICONTROL Default PTC]_.

      - Per **[!UICONTROL Default PTC]**, immetti il PTC predefinito da utilizzare per tutte le inserzioni Amazon idonee. Se il PTC predefinito è impostato nel tuo account [!DNL Amazon Seller Central], lascia vuoto questo campo. Le modifiche apportate a questo campo non influiscono sulle inserzioni esistenti di Amazon. Per modificare il PTC predefinito per un&#39;inserzione esistente, l&#39;inserzione deve essere [scaduta](./end-listings-manually.md) e deve essere creata una nuova inserzione.

   >[!NOTE]
   >
   >Se utilizzi il Servizio di calcolo IVA di Amazon, devi conoscere la categoria fiscale dei tuoi prodotti. Un PTC è il codice ID della categoria fiscale di Amazon per gli acquisti B2B nell’UE. Consulta [Codici imposta prodotto di Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}.

1. Per **[!UICONTROL Currency Conversion]**, scegliere un&#39;opzione.

   Il valore predefinito è `Disabled`. Queste opzioni dipendono dalle impostazioni di [!DNL Commerce] [valuta](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html). Se non sono disponibili opzioni, impostare le impostazioni di valuta.

1. Al termine, fare clic su **[!UICONTROL Save listing settings]**.

![Prezzo di vendita](assets/amazon-listing-price.png){width="500" zoomable="yes"}

| Campo | Descrizione |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Magento Price Source] | Determina l&#39;origine del prezzo utilizzata durante la creazione delle inserzioni Amazon. Il valore predefinito è `Price`. Se si sceglie un attributo diverso, ad esempio `Amazon Price` o `Special Price`, il valore definito per l&#39;attributo viene utilizzato per l&#39;inserzione Amazon. Tuttavia, se l&#39;attributo selezionato non è definito, viene utilizzato `Price`. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Attributo [!DNL Commerce] per la determinazione prezzi MAP. Scegliendo l&#39;opzione MAP, l&#39;inserzione Amazon viene automaticamente impostata sul prezzo MAP se quest&#39;ultimo è inferiore al prezzo MAP. |
| [!UICONTROL Strike Through Price (MSRP)] | Attributo [!DNL Commerce] che rappresenta il prezzo MSRP. Se il prezzo dell&#39;inserzione Amazon è inferiore al prezzo MSRP, viene visualizzato uno strike-through del prezzo MSRP e del prezzo dell&#39;inserzione. Questa impostazione viene utilizzata anche per calcolare l&#39;importo e la percentuale di &quot;Salvataggio&quot;, ma questa funzione si applica solo alle inserzioni che hanno vinto la posizione [Buy Box](./buy-box-competitor-pricing.md). |
| [!UICONTROL Apply Value Added Tax (VAT)] | L&#39;IVA è utilizzata dai venditori nell&#39;Unione europea.<br><br>Scegliere `Disabled` se non si desidera aggiungere l&#39;IVA ai prezzi di vendita.<br><br>Scegliere `Enabled`, quindi immettere la percentuale IVA per applicare l&#39;IVA ai prezzi di vendita. |
| [!UICONTROL VAT Percentage] | Definisci la percentuale da utilizzare per calcolare l&#39;importo IVA da aggiungere al prezzo di inserzione per le inserzioni Amazon. <br><br>Se si immette `5`, verrà applicata un&#39;IVA del 5% al prezzo di messa finale dopo l&#39;applicazione di tutte le regole di determinazione dei prezzi. L&#39;IVA non viene applicata al prezzo finale per le inserzioni utilizzate in una regola di determinazione prezzi intelligente, a meno che non venga raggiunto il [limite](./floor-price.md) o il [massimale](./optional-ceiling-price.md). |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Solo per i Negozi del Regno Unito) Determina se il canale di vendita Amazon invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central]. <br><br>Selezionare **Non gestire PTC** se si utilizza un servizio di calcolo delle imposte di terze parti o se tutti i calcoli delle imposte sono già stati impostati nell&#39;account [!DNL Amazon Seller Central]. Quando è impostato su questa opzione, il canale di vendita Amazon non invia informazioni sul codice fiscale del prodotto al tuo account [!DNL Amazon Seller Central].<br><br>Selezionare **Imposta PTC predefinito** se si dispone di un codice IVA prodotto universale che si desidera utilizzare per tutti i prodotti.<br><br>Consulta [Codici imposta prodotto di Amazon](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}. |
| [!UICONTROL Default PTC] | Viene visualizzato solo quando **Amazon Product Tax Code (PTC)** è impostato su `Set Default PTC`. Immettere il PTC predefinito da utilizzare per tutte le inserzioni Amazon idonee. Se il PTC predefinito è impostato nel tuo account [!DNL Amazon Seller Central], lascia vuoto questo campo. <br><br>Le modifiche apportate a questo campo non influiscono sulle inserzioni esistenti. L&#39;inserzione deve essere [scaduta](./end-listings-manually.md) e per rendere effettiva la modifica è stata creata una nuova inserzione. |
| [!UICONTROL Currency Conversion] | Consente alla tua valuta predefinita di [!DNL Commerce] vetrina di convertirla con precisione nella tua valuta predefinita di Amazon per pubblicare i prezzi delle inserzioni nella valuta corretta. La conversione della valuta è sempre basata sulla valuta predefinita [!DNL Commerce].<br><br>Puoi comunque visualizzare le tue [!DNL Commerce] e le valute Amazon predefinite quando sono disponibili altre valute. Se la valuta predefinita di [!DNL Commerce] corrisponde alla valuta predefinita di Amazon, lascia disabilitata la funzione Conversione valuta.<br><br>Ad esempio, se la valuta predefinita di [!DNL Commerce] è CAD (Dollaro canadese) e la valuta predefinita di Amazon è USD, è necessario abilitare la conversione valuta e scegliere il tasso di conversione da CAD a USD. Le opzioni visualizzate si basano sulle conversioni di valuta [!DNL Commerce] incorporate. Se non trovi l&#39;opzione che stai cercando, [imposta la valuta in [!DNL Commerce]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html). |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
