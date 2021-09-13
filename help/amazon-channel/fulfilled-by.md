---
title: Completato da
description: Utilizza le impostazioni Fulfill By per determinare il modo in cui gli ordini degli elenchi Amazon vengono soddisfatti (spediti).
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Completato da

_[!UICONTROL Fulfilled By]_Le impostazioni fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell&#39;elenco sono accessibili dal [dashboard del negozio](./amazon-store-dashboard.md).

Queste impostazioni definiscono la parte che soddisfa (o spedisce) gli ordini. Se tutti i tuoi ordini vengono eseguiti utilizzando un metodo, scegli tra esercente (tu) o Amazon. Se prevedi di eseguire ordini dalle posizioni e di utilizzare Amazon, è consigliabile utilizzare la terza opzione e configurare un attributo di prodotto [!DNL Commerce].

- **[!UICONTROL Fulfilled by Merchant]** - Scegli se tu, il commerciante, esegui tutti gli ordini. Quando un ordine viene effettuato, l&#39;inventario viene detratto dal catalogo [!DNL Commerce].

- **[!UICONTROL Fulfilled by Amazon]** - Scegli se Amazon soddisfa tutti gli ordini. Con questa opzione, l’inventario dei prodotti non viene detratto dal catalogo [!DNL Commerce] quando viene effettuato un ordine. Le scorte di magazzino per gli ordini evasi di Amazon vengono archiviate e detratte dai rispettivi magazzini. Prima di assegnare questa opzione, devi verificare nel tuo account [!DNL Amazon Seller Central] che i tuoi prodotti siano idonei per la conformità a _Eseguito da Amazon_ (FBA). L’inventario FBA viene gestito direttamente tramite il tuo account [!DNL Amazon Seller Central] . Con questo metodo di evasione, il canale di vendita Amazon non condivide gli aggiornamenti di quantità tra [!DNL Commerce] e Amazon. Pertanto, non tutti gli strumenti di marketing descritti in Impostazioni quantità sono disponibili nel canale di vendita Amazon.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Se i tuoi prodotti possono essere soddisfatti da te e da Amazon, puoi creare un attributo di  [!DNL Commerce] prodotto con valori per Fulfill By Merchant e Fulfill by Amazon. L&#39;impostazione di questo valore per prodotto indica chi soddisfa gli ordini.

Il metodo di evasione è un attributo regionale e si basa sull&#39;impostazione **[!UICONTROL Amazon Marketplace Country]** definita durante l&#39; [integrazione store](./store-integration.md). Quando viene apportata una modifica, questa influisce su tutti gli elenchi di Amazon che condividono [!DNL Amazon Seller SKU] negli archivi Amazon che vendono nella stessa area (come definito in _[!UICONTROL Amazon Marketplace Country]_durante l&#39; [integrazione degli archivi](./store-integration.md)). Una modifica apportata a una [!DNL Amazon Seller SKU] condivisa negli Stati Uniti non influisce sugli archivi Amazon impostati per un&#39;area diversa (come definito durante l&#39;integrazione dello store).

>[!NOTE]
>
>Quando un ordine viene soddisfatto da Amazon (FBA) e l’ordine viene importato, nei dettagli dell’ordine puoi visualizzare dati fittizi per alcuni campi. Consulta [Dettagli ordine Amazon](./amazon-order-details.md).

## Configurare le impostazioni [!UICONTROL Fulfilled By] {#configure-fulfilled-by-settings}

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione _[!UICONTROL Fulfilled By]_.

1. Per **[!UICONTROL Product Fulfilled By]**, scegli chi soddisfa (spedisce) l&#39;ordine:

   - `Fulfilled by Merchant` - Il commerciante adempie l&#39;ordine.

   - `Fulfilled by Amazon` - Il magazzino Amazon soddisfa l&#39;ordine.

   - `Assign Fulfilled By Using Magento Product Attribute` - Un  [!DNL Commerce] attributo indica chi soddisfa l&#39;ordine per prodotto.

      Se scelto, scegli l&#39;attributo [!DNL Commerce] da mappare in **[!UICONTROL Fulfilled by Attribute]**.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Impostazioni soddisfatte da](assets/amazon-fulfilled-by.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | Opzioni:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Scegli se esegui gli ordini. Quando un ordine viene effettuato, l&#39;inventario viene detratto dal catalogo [!DNL Commerce]. Quando viene creato un nuovo prodotto, viene assegnato il metodo di esecuzione di Merchant Fulfill.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Scegli se Amazon soddisfa gli ordini. Con questo metodo di evasione, l&#39;inventario dei prodotti non viene detratto dal catalogo [!DNL Commerce] quando viene effettuato un ordine. Quando un prodotto viene creato, viene creato con _[!UICONTROL Fulfilled by Amazon (FBA)]_come tipo di evasione. Assicurati che i tuoi prodotti siano idonei per la conformità FBA all&#39;interno del tuo account [!DNL Amazon Seller Central] . L’inventario FBA viene gestito direttamente anche tramite il tuo account [!DNL Amazon Seller Central] . Con questo metodo di evasione, gli aggiornamenti di quantità non vengono inviati rispetto al catalogo [!DNL Commerce], pertanto non è possibile utilizzare alcuni degli strumenti di marketing descritti in [Impostazioni stock/quantità](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Scegli se disponi di un  [!DNL Commerce] attributo esistente che determina se è soddisfatto dal commerciante o soddisfatto da Amazon. Se scelto, l&#39;opzione **[!UICONTROL Fulfilled by Attribute]** abilita.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Scegli l&#39;attributo [!DNL Commerce] utilizzato per determinare il metodo di evasione.<br><br>Ad esempio, se l&#39;attributo è  _Eseguito_ da e si sceglie il valore dell&#39;attributo come  _[!UICONTROL Fulfilled By Merchant]_o_[!UICONTROL Fulfilled By Amazon (FBA)]_, il sistema utilizza tale valore come tipo di evasione per un nuovo prodotto. In qualità di commerciante, è necessario assicurarsi che i prodotti siano idonei per l&#39;adempimento FBA all&#39;interno del tuo account [!DNL Amazon Seller Central]. L&#39;inventario FBA viene gestito direttamente anche tramite il tuo account Amazon Seller.<br><br>Le opzioni dipendono dagli attributi impostati per i prodotti Amazon. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
