---
title: Impostazioni di Evasione per le inserzioni Amazon
description: Utilizza le impostazioni Evasione di per determinare come vengono evasi (spediti) gli ordini provenienti dalle inserzioni di Amazon.
feature: Sales Channels, Products
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Impostazioni di Evasione per le inserzioni Amazon

_[!UICONTROL Fulfilled By]_Le impostazioni fanno parte delle impostazioni dell&#39;inserzione del Negozio. Le impostazioni dell&#39;inserzione sono accessibili da [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni definiscono la parte che esegue (o spedisce) gli ordini. Se tutti gli ordini vengono evasi con un unico metodo, scegli tra esercente (tu) o Amazon. Se prevedi di evadere gli ordini dalle tue ubicazioni e di utilizzare Amazon, è consigliabile utilizzare la terza opzione e configurare un’ [!DNL Commerce] attributo del prodotto.

- **[!UICONTROL Fulfilled by Merchant]** - Scegli se tu, il commerciante, evade tutti gli ordini. Quando viene effettuato un ordine, le scorte vengono detratte dal [!DNL Commerce] catalogo.

- **[!UICONTROL Fulfilled by Amazon]** - Scegliere se Amazon soddisfa tutti gli ordini. Con questa opzione, l’inventario dei prodotti non viene dedotto dal tuo [!DNL Commerce] quando viene effettuato un ordine. Le scorte di magazzino per gli ordini evasi da Amazon vengono memorizzate e detratte dai magazzini. Prima di assegnare questa opzione, devi verificare nel [!DNL Amazon Seller Central] account per cui i prodotti sono idonei _Soddisfatto da Amazon_ (FBA) adempimento. L’inventario FBA viene gestito direttamente tramite il tuo [!DNL Amazon Seller Central] Account. Con questo metodo di evasione, il canale di vendita Amazon non condivide gli aggiornamenti della quantità tra [!DNL Commerce] e Amazon. Pertanto, non tutti gli strumenti di marketing descritti in Impostazioni quantità sono disponibili nel canale di vendita di Amazon.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Se i prodotti sono soddisfatti da te e da Amazon, puoi creare un’ [!DNL Commerce] attributo del prodotto con valori per Evaso da commerciante e Evaso da Amazon. L’impostazione di questo valore per prodotto indica chi evade gli ordini.

Il metodo di evasione è un attributo regionale e si basa sul **[!UICONTROL Amazon Marketplace Country]** impostazione definita durante [integrazione store](./store-integration.md). Quando viene apportata una modifica, questa interessa tutte le inserzioni di Amazon che condividono [!DNL Amazon Seller SKU] nei negozi Amazon che vendono nella stessa area geografica (come definito in _[!UICONTROL Amazon Marketplace Country]_durante [integrazione store](./store-integration.md)). Una modifica a una condivisione [!DNL Amazon Seller SKU] negli Stati Uniti non influisce sugli store Amazon impostati per un’area geografica diversa (come definito durante l’integrazione dello store).

>[!NOTE]
>
>Quando un ordine viene evaso da Amazon (FBA) e l’ordine viene importato, nei dettagli dell’ordine potrebbero essere visualizzati dei dati fittizi per alcuni campi. Consulta [Dettagli ordine Amazon](./amazon-order-details.md).

## Configurare [!UICONTROL Fulfilled By] impostazioni {#configure-fulfilled-by-settings}

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi _[!UICONTROL Fulfilled By]_sezione.

1. Per **[!UICONTROL Product Fulfilled By]**, scegli chi esegue (spedisce) l’ordine:

   - `Fulfilled by Merchant` - Il commerciante evade l&#39;ordine.

   - `Fulfilled by Amazon` - Amazon warehouse evade l&#39;ordine.

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] l&#39;attributo indica chi esegue l&#39;ordine per prodotto.

     Se è stato scelto, scegliere [!DNL Commerce] attributo da mappare in **[!UICONTROL Fulfilled by Attribute]**.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Impostazioni di Evasione da](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| Campo | Descrizione |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | Opzioni:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Scegli se evadere gli ordini. Quando viene effettuato un ordine, le scorte vengono detratte dal [!DNL Commerce] catalogo. Quando viene creato un nuovo prodotto, viene assegnato il metodo di evasione dell&#39;esercente evaso.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Scegli se Amazon evade gli ordini. Con questo metodo di evasione, l&#39;inventario dei prodotti non viene dedotto dal [!DNL Commerce] quando viene effettuato un ordine. Quando viene creato un prodotto, questo viene creato con _[!UICONTROL Fulfilled by Amazon (FBA)]_come tipo di adempimento. Assicurati che i tuoi prodotti siano idonei per l&#39;adempimento FBA all&#39;interno del tuo [!DNL Amazon Seller Central] account. L’inventario FBA viene gestito direttamente anche tramite [!DNL Amazon Seller Central] account. Con questo metodo di evasione, gli aggiornamenti della quantità non vengono inviati in relazione al [!DNL Commerce] , pertanto non è possibile utilizzare alcuni degli strumenti di marketing descritti in [Impostazioni scorte/quantità](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Scegli se disponi di un [!DNL Commerce] attributo che determina se è soddisfatto dall’esercente o da Amazon. Quando viene scelto, **[!UICONTROL Fulfilled by Attribute]** abilita.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Scegli la [!DNL Commerce] attributo utilizzato per determinare il metodo di adempimento.<br><br>Ad esempio, se l’attributo è _Soddisfatto da_ e scegli il valore attributo come `Fulfilled By Merchant` o `Fulfilled By Amazon (FBA)`, il sistema utilizza tale valore come tipo di adempimento per un nuovo prodotto. In qualità di commerciante, devi assicurarti che i tuoi prodotti siano idonei per l’adempimento FBA all’interno del tuo [!DNL Amazon Seller Central] account. L’inventario FBA viene gestito direttamente anche tramite il tuo account Amazon Seller.<br><br>Le opzioni dipendono dagli attributi impostati per i prodotti Amazon. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
