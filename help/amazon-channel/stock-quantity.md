---
title: Stock/Quantità
description: 'Per controllare la sincronizzazione dei dettagli della quantità del prodotto dal tuo negozio Commerce al tuo account [!DNL Amazon Seller Central] , aggiorna le impostazioni Stock/Quantity.'
redirect_from: /sales-channels/asc/ob-stock-quantity.html: 
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 771
ht-degree: 0%

---

# Stock/Quantità

*[!UICONTROL Stock/Quantity]* Le impostazioni fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell&#39;elenco sono accessibili dal [dashboard del negozio](./amazon-store-dashboard.md).

Queste impostazioni vengono utilizzate per sincronizzare i dettagli della quantità del prodotto dalla vetrina [!DNL Commerce] alla quantità presente nel tuo account [!DNL Amazon Seller Central]. Questo strumento è potente e può essere utilizzato per pubblicità aggiuntiva mostrando urgenza al compratore mantenendo il vostro inventario organizzato. Ad esempio, alcuni commercianti possono avere 150 articoli di una specifica SKU in magazzino nel loro magazzino e vogliono assicurarsi che gli acquirenti Amazon possano acquistare tutto il loro inventario. Altri commercianti possono voler elencare un solo elemento alla volta per creare un senso di scarsità per l&#39;utente finale. In questo caso, imposta *[!UICONTROL Maximum Listed Quantity]* su `1`.

La quantità è un attributo regionale e si basa sull&#39;impostazione **[!UICONTROL Amazon Marketplace Country]** definita durante [l&#39;integrazione dello store](./store-integration.md). Quando viene apportata una modifica alla quantità di un prodotto, la modifica interessa tutti gli elenchi Amazon che condividono [!DNL Amazon Seller SKU] nei tuoi negozi Amazon che vendono nello stesso paese. Una modifica apportata a una [!DNL Amazon Seller SKU] condivisa negli Stati Uniti non influisce sui tuoi Amazon Store configurati per un paese diverso. Il primo archivio Amazon integrato (con la data di creazione più vecchia) controlla la priorità nelle impostazioni della quantità.

>[!NOTE]
>
>Ad Adobe, gli utenti Commerce e Magenti Open Source 2.3.x, il canale di vendita Amazon supporta l’utilizzo dell’estensione Gestione dell’inventario senza alcuna configurazione aggiuntiva. Consultare [Gestione dell&#39;inventario](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){:target=&quot;_blank&quot;}.

## Configurare le impostazioni di stock/quantità {#configure-stock--quantity-settings}

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione **[!UICONTROL Stock / Quantity]**.

1. Per **[!UICONTROL Out-of-Stock Threshold]** (obbligatorio), immetti un valore numerico per la quantità più bassa di un prodotto al fine di mantenere il prodotto idoneo per il proprio elenco Amazon.

   Il valore predefinito è `0`. Se le risorse di prodotto [!DNL Commerce] sono inferiori a questo numero, la relativa inserzione in Amazon non è idonea alle vendite tramite Amazon.

1. Per **[!UICONTROL Maximum Listed Quantity]** (obbligatorio), immetti un valore numerico per la quantità da visualizzare nell’elenco Amazon.

   Questa impostazione elenca tutti gli elenchi Amazon idonei in base al valore inserito. Quando un articolo viene venduto, la quantità dell’elenco di Amazon non cambia. La quantità di inserzione disponibile utilizza sempre questo valore, anche quando la quantità di prodotto effettivo è superiore o inferiore. Questa impostazione viene generalmente utilizzata quando non si gestisce l’inventario dei prodotti. Ad esempio, puoi avere un prodotto con una quantità di 80 nel catalogo [!DNL Commerce]. Con impostato su `10`, l’elenco Amazon visualizza sempre una quantità disponibile di `10` e non cambia quando si effettua la vendita del prodotto.

1. Per **[!UICONTROL "Do Not Manage Stock" Quantity]** (obbligatorio), immettere un valore di quantità da visualizzare per gli elenchi Amazon.

   Amazon richiede la pubblicazione di una quantità disponibile. Per i prodotti [!DNL Commerce] impostati per non gestire le scorte, ma che si desidera elencare in Amazon, l&#39;elenco viene pubblicato con la quantità disponibile inserita qui.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Impostazioni scorte/quantità](assets/amazon-stock-quantity.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Immetti un valore numerico per la quantità più bassa di un prodotto al fine di mantenere il prodotto idoneo per il suo elenco Amazon (il valore predefinito è `0`).<br><br>Se le scorte di  [!DNL Commerce] prodotto sono inferiori a questo numero, le vendite effettuate tramite Amazon non possono essere effettuate nell’elenco Amazon corrispondente. |
| [!UICONTROL Maximum Listed Quantity] | Immetti un valore numerico per la quantità da visualizzare nell’elenco Amazon.<br><br>Quando un articolo viene venduto, l&#39;elenco Amazon viene ripubblicato con la quantità inserita qui. Questa impostazione viene generalmente utilizzata quando non si gestisce l’inventario dei prodotti.<br><br>Ad esempio, puoi immettere il valore Quantità massima elencata come  `10`. La quantità effettiva per un prodotto è `80`. Poiché hai impostato questo valore su `10`, nell’elenco Amazon viene sempre visualizzata una quantità disponibile di `10`. La quantità disponibile viene sempre visualizzata con il valore definito, anche quando la quantità di scorte è inferiore. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Immetti un valore per la quantità di visualizzazione per gli elenchi Amazon.<br><br>Amazon richiede la pubblicazione di una quantità disponibile. Per i prodotti [!DNL Commerce] impostati per non gestire le scorte, ma che si desidera elencare in Amazon, l&#39;elenco viene pubblicato con la quantità disponibile del valore immesso qui. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Esempio: Quantità massima indicata

Quando un articolo viene venduto, l’elenco Amazon lo rielenca a questa quantità.

Ad esempio, se imposti *[!UICONTROL Maximum Listed Quantity]* come `12`, l’elenco Amazon mostra una quantità di 12 anche se il prodotto ha una quantità [!DNL Commerce] di 80:

![Quantità massima elencata esempio 1](assets/amazon-max-listed-quantity.png)

Se imposti *[!UICONTROL Maximum Listed Quantity]* come `1`, tutti i prodotti idonei sono elencati con una quantità di `1`. Quando un articolo viene venduto, il sistema controlla il prodotto [!DNL Commerce] e, se esiste ulteriore scorta, rielenca l&#39;articolo su Amazon con una quantità di `1`.

Questa opzione può essere utile per i prodotti ordinati normalmente a una quantità di 1. Inoltre, aumenta l’urgenza per l’acquirente quando visualizzi l’elenco di Amazon.

![Quantità massima indicata esempio 2](assets/amazon-max-listed-quantity-1.png)
