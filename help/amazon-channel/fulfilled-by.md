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

Le impostazioni di _[!UICONTROL Fulfilled By]_fanno parte delle impostazioni dell&#39;inserzione dello store. Le impostazioni dell&#39;inserzione sono accessibili dal [dashboard dell&#39;archivio](./amazon-store-dashboard.md).

Queste impostazioni definiscono la parte che esegue (o spedisce) gli ordini. Se tutti gli ordini vengono evasi con un unico metodo, scegli tra esercente (tu) o Amazon. Se si prevede di evadere gli ordini dalle proprie sedi e di utilizzare Amazon, è consigliabile utilizzare la terza opzione e configurare un attributo di prodotto [!DNL Commerce].

- **[!UICONTROL Fulfilled by Merchant]** - Scegli se tu, il commerciante, evade tutti gli ordini. Quando viene effettuato un ordine, le scorte vengono detratte dal catalogo [!DNL Commerce].

- **[!UICONTROL Fulfilled by Amazon]** - Scegli se Amazon soddisfa tutti gli ordini. Con questa opzione, l&#39;inventario dei prodotti non viene detratto dal catalogo [!DNL Commerce] quando viene effettuato un ordine. Le scorte di magazzino per gli ordini evasi da Amazon vengono memorizzate e detratte dai magazzini. Prima di assegnare questa opzione, è necessario verificare nell&#39;account [!DNL Amazon Seller Central] che i prodotti siano idonei per il _adempimento da parte di Amazon_ (FBA). L&#39;inventario FBA è gestito direttamente tramite l&#39;account [!DNL Amazon Seller Central]. Con questo metodo di evasione, il canale di vendita Amazon non condivide gli aggiornamenti di quantità tra [!DNL Commerce] e Amazon. Pertanto, non tutti gli strumenti di marketing descritti in Impostazioni quantità sono disponibili nel canale di vendita di Amazon.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Se i tuoi prodotti possono essere soddisfatti da te e da Amazon, puoi creare un attributo di prodotto [!DNL Commerce] con valori per Evasione da parte del commerciante e Evasione da parte di Amazon. L’impostazione di questo valore per prodotto indica chi evade gli ordini.

Il metodo di evasione è un attributo regionale e si basa sull&#39;impostazione **[!UICONTROL Amazon Marketplace Country]** definita durante l&#39;[integrazione archivio](./store-integration.md). Quando viene apportata una modifica, questa interessa tutte le inserzioni di Amazon che condividono [!DNL Amazon Seller SKU] nei tuoi Amazon store e vendono nella stessa area (come definito in _[!UICONTROL Amazon Marketplace Country]_durante l&#39;[integrazione dello store](./store-integration.md)). Una modifica a un [!DNL Amazon Seller SKU] condiviso negli Stati Uniti non influisce sugli store Amazon impostati per un&#39;area diversa (come definito durante l&#39;integrazione dello store).

>[!NOTE]
>
>Quando un ordine viene evaso da Amazon (FBA) e l’ordine viene importato, nei dettagli dell’ordine potrebbero essere visualizzati dei dati fittizi per alcuni campi. Consulta [Dettagli ordine Amazon](./amazon-order-details.md).

## Configura le impostazioni di [!UICONTROL Fulfilled By] {#configure-fulfilled-by-settings}

1. Fare clic su **[!UICONTROL Listing Settings]** nel dashboard dell&#39;archivio.

1. Espandere la sezione _[!UICONTROL Fulfilled By]_.

1. Per **[!UICONTROL Product Fulfilled By]**, scegliere chi esegue (invia) l&#39;ordine:

   - `Fulfilled by Merchant` - Il commerciante evade l&#39;ordine.

   - `Fulfilled by Amazon` - Amazon warehouse evade l&#39;ordine.

   - `Assign Fulfilled By Using Magento Product Attribute` - Un attributo [!DNL Commerce] indica chi soddisfa l&#39;ordine per prodotto.

     Se scelto, scegliere l&#39;attributo [!DNL Commerce] da mappare in **[!UICONTROL Fulfilled by Attribute]**.

1. Al termine, fare clic su **[!UICONTROL Save listing settings]**.

![Soddisfatto dalle impostazioni](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| Campo | Descrizione |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | Opzioni:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Scegliere se si eseguono gli ordini. Quando viene effettuato un ordine, le scorte vengono detratte dal catalogo [!DNL Commerce]. Quando viene creato un nuovo prodotto, viene assegnato il metodo di evasione dell&#39;esercente evaso.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Scegli se Amazon soddisfa gli ordini. Con questo metodo di evasione, l&#39;inventario dei prodotti non viene detratto dal catalogo [!DNL Commerce] quando viene effettuato un ordine. Quando viene creato un prodotto, viene creato con _[!UICONTROL Fulfilled by Amazon (FBA)]_come tipo di evasione. Assicurati che i tuoi prodotti siano idonei per l&#39;evasione FBA nel tuo account [!DNL Amazon Seller Central]. L&#39;inventario FBA viene gestito direttamente anche tramite l&#39;account [!DNL Amazon Seller Central]. Con questo metodo di evasione, gli aggiornamenti della quantità non vengono inviati relativamente al catalogo [!DNL Commerce], pertanto non puoi utilizzare alcuni degli strumenti di marketing descritti in [Impostazioni magazzino/quantità](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Scegli se hai un attributo [!DNL Commerce] esistente che determina se è soddisfatto dal commerciante o da Amazon. Se scelto, **[!UICONTROL Fulfilled by Attribute]** abilita.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Scegliere l&#39;attributo [!DNL Commerce] utilizzato per determinare il metodo di adempimento.<br><br>Ad esempio, se l&#39;attributo è _Evaso da_ e si sceglie il valore dell&#39;attributo come `Fulfilled By Merchant` o `Fulfilled By Amazon (FBA)`, il sistema utilizza tale valore come tipo di evasione per un nuovo prodotto. In qualità di commerciante, devi assicurarti che i tuoi prodotti siano idonei per l&#39;adempimento FBA all&#39;interno del tuo account [!DNL Amazon Seller Central]. L’inventario FBA viene gestito direttamente anche tramite il tuo account Amazon Seller.<br><br>Le opzioni dipendono dagli attributi impostati per i prodotti Amazon. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
