---
title: Canale di vendita Amazon - [!UICONTROL Third-party Listings]
description: Aggiorna le impostazioni dell’inserzione di terze parti per determinare se il catalogo Commerce importa prodotti dalle inserzioni esistenti di Amazon Seller Central.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

Le impostazioni delle inserzioni di terze parti fanno parte delle impostazioni delle inserzioni del Negozio. Le impostazioni dell&#39;inserzione sono accessibili da [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni determinano se [!DNL Commerce] il catalogo importa i prodotti dal tuo esistente [!DNL Amazon Seller Central] inserzioni. È consigliabile importare le inserzioni da Amazon per assicurarsi che tutte le inserzioni corrispondano [!DNL Commerce] prodotti. Quando le tue inserzioni fanno parte del tuo [!DNL Commerce] catalogo, puoi gestire tutti i prodotti da un singolo catalogo e utilizzare le funzioni del canale di vendita Amazon. Queste funzioni includono gestione degli ordini e dell&#39;evasione con Amazon, ridefinizione intelligente dei prezzi e gestione della quantità.

Quando è configurato per importare le inserzioni Amazon, il canale di vendita Amazon importa le inserzioni Amazon nel tuo [!DNL Commerce] del catalogo, tentando di farli corrispondere a prodotti esistenti. Se non viene trovata automaticamente una corrispondenza, puoi importare l’inserzione Amazon come nuova [!DNL Commerce] o far corrispondere manualmente l’inserzione a un prodotto.

Se scegli di importare le tue inserzioni Amazon, scegli [!DNL Commerce] attributi con valori per Amazon Seller SKU e Amazon ASIN. Se non ha [!DNL Commerce] [attributi prodotto](./ob-creating-magento-attributes.md), è consigliabile crearli e assegnarli. La mappatura di questi attributi consente di abbinare correttamente le inserzioni Amazon importate al tuo [!DNL Commerce] prodotti.

L&#39;importazione iniziale dell&#39;elenco viene avviata quando [integrazione store](./store-integration.md) è stato completato. In seguito e in base alle impostazioni cron, [!DNL Commerce] controlla continuamente le nuove inserzioni Amazon aggiunte (non create in Amazon Sales Channel) e aggiorna i [!DNL Commerce] catalogo in base alle impostazioni delle inserzioni di terze parti.

## Configurare le impostazioni per l’inserzione di terze parti

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi _[!UICONTROL Third Party Listings]_sezione.

1. Per **[!UICONTROL Import Third Party Listings]** (obbligatorio), scegli un’opzione:

   - `Import Listing` - (Impostazione predefinita) Scegli quando desideri che le informazioni sui prodotti delle inserzioni Amazon vengano importate nel tuo [!DNL Commerce] catalogo dei prodotti. Questa opzione è quella predefinita ed è consigliata.

   - `Do Not Import Listing` - Scegliere quando si desidera eseguire manualmente [creare e assegnare nuovi prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) al tuo [!DNL Commerce] catalogo per le inserzioni Amazon.
   >[!NOTE]
   >I campi delle opzioni seguenti sono attivi solo se impostati su `Import Listing`.

1. Per **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, scegli il [!DNL Commerce] che corrisponde al valore SKU del venditore Amazon.

1. Per **[!UICONTROL Attribute That Contains Amazon ASIN]**, scegli il [!DNL Commerce] creato e corrisponde al codice ASIN di Amazon.

   >[!NOTE]
   >Se non li hai creati [!DNL Commerce] attributi per le inserzioni Amazon, consulta [Creazione di attributi per corrispondenza Amazon](./ob-creating-magento-attributes.md).

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Inserzioni di terze parti](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Third Party Listings] | Obbligatorio. Opzioni:<ul><li>**[!UICONTROL Import Listing]** - (Impostazione predefinita) Scegli quando desideri che le informazioni sui prodotti delle inserzioni Amazon vengano importate nel tuo [!DNL Commerce] catalogo dei prodotti. </li><li>**[!UICONTROL Do Not Import Listing]** - Scegliere quando si desidera eseguire manualmente [creare e assegnare nuovi prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) al tuo [!DNL Commerce] catalogo per le inserzioni Amazon.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Attivo solo se impostato su `Import Listing`.<br>Scegli la [!DNL Commerce] come corrispondenza con l’attributo Amazon per lo SKU del venditore Amazon. Se questo attributo non esiste, vedi [Creazione di attributi di prodotto Amazon per corrispondenza Amazon](./ob-creating-magento-attributes.md). Se necessario, rivedi [!DNL Commerce] [attributi](./managing-attributes.md) e creare o modificare un attributo che corrisponda a questi dati di Amazon. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Attivo solo se impostato su `Import Listing`.<br>Scegli la [!DNL Commerce] che corrisponde all’attributo Amazon per Amazon ASIN. Se questo attributo non esiste, vedi [Creazione di attributi di prodotto Amazon per corrispondenza Amazon](./ob-creating-magento-attributes.md). Se necessario, rivedi [!DNL Commerce] [attributi](./managing-attributes.md) e creare o modificare un attributo che corrisponda a questi dati di Amazon. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
