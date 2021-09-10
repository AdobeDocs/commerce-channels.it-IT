---
title: Elenco di terze parti
description: Aggiorna le impostazioni dell’elenco di terze parti per determinare se il catalogo Commerce importa prodotti dagli elenchi Amazon Seller Central esistenti.
redirect_from: /sales-channels/asc/ob-third-party-listings.html: 
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 519
ht-degree: 0%

---

# Elenco di terze parti

Le impostazioni di elenco di terze parti fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell&#39;elenco sono accessibili dal [dashboard del negozio](./amazon-store-dashboard.md).

Queste impostazioni determinano se il catalogo [!DNL Commerce] importa prodotti dagli elenchi [!DNL Amazon Seller Central] esistenti. È consigliabile importare gli elenchi da Amazon per garantire che tutti gli elenchi corrispondano ai prodotti [!DNL Commerce]. Quando gli elenchi fanno parte del catalogo [!DNL Commerce], puoi gestire tutti i prodotti da un unico catalogo e utilizzare le funzioni dei canali di vendita Amazon. Queste funzionalità includono la gestione dell&#39;evasione e dell&#39;ordine con Amazon, la revisione intelligente dei prezzi e la gestione della quantità.

Una volta configurato per importare gli elenchi Amazon, il canale di vendita Amazon importa gli elenchi Amazon nel catalogo [!DNL Commerce], tentando di farli corrispondere ai prodotti esistenti. Se una corrispondenza non viene trovata automaticamente, puoi importare l’elenco Amazon come nuovo prodotto [!DNL Commerce] oppure abbinare manualmente l’elenco a un prodotto.

Se scegli di importare le inserzioni Amazon, scegli gli attributi [!DNL Commerce] con i valori per SKU venditore Amazon e ASIN Amazon. Se non disponi di [!DNL Commerce] [attributi di prodotto](./ob-creating-magento-attributes.md), puoi crearli e assegnarli. La mappatura di questi attributi aiuta a far corrispondere correttamente gli elenchi Amazon importati ai prodotti [!DNL Commerce].

L&#39;importazione iniziale dell&#39;elenco viene avviata quando [l&#39;integrazione dell&#39;archivio](./store-integration.md) viene completata. In seguito e in base alle impostazioni cron, [!DNL Commerce] controlla continuamente gli elenchi Amazon appena aggiunti (non creati nel Sales Channel Amazon) e aggiorna il catalogo [!DNL Commerce] in base alle impostazioni degli elenchi di terze parti.

## Configurare le impostazioni di elenco di terze parti

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione _[!UICONTROL Third Party Listings]_.

1. Per **[!UICONTROL Import Third Party Listings]** (obbligatorio), scegli un’opzione:

   - `Import Listing` - (Impostazione predefinita) Scegli quando importare le informazioni di prodotto dagli elenchi Amazon nel catalogo  [!DNL Commerce] dei prodotti. Questa è l’opzione predefinita ed è consigliata.

   - `Do Not Import Listing` - Scegli quando  [creare e assegnare manualmente i nuovi prodotti](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;} al  [!DNL Commerce] catalogo per gli elenchi Amazon.
   >[!NOTE]
   >I campi delle opzioni seguenti sono attivi solo se è impostato su `Import Listing`.

1. Per **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, scegli l&#39;attributo [!DNL Commerce] che corrisponde al valore SKU del venditore di Amazon.

1. Per **[!UICONTROL Attribute That Contains Amazon ASIN]**, scegli l’attributo [!DNL Commerce] creato e lo abbini all’Amazon ASIN.

   >[!NOTE]
   >Se non hai creato questi attributi [!DNL Commerce] per gli elenchi Amazon, consulta [Creazione di attributi per Amazon Matching](./ob-creating-magento-attributes.md).

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Elenco di terzi](assets/amazon-third-party-listings.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Third Party Listings] | Obbligatorio. Opzioni:<ul><li>**[!UICONTROL Import Listing]** - (Impostazione predefinita) Scegli quando importare le informazioni di prodotto dagli elenchi Amazon nel catalogo  [!DNL Commerce] dei prodotti. </li><li>**[!UICONTROL Do Not Import Listing]** - Scegli quando  [creare e assegnare manualmente i nuovi prodotti](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;} al  [!DNL Commerce] catalogo per gli elenchi Amazon.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | È attivo solo se è impostato su `Import Listing`.<br>Scegli l’ [!DNL Commerce] attributo come corrispondenza con l’attributo Amazon per lo SKU del venditore Amazon. Se questo attributo non esiste, consulta [Creazione di attributi di prodotto Amazon per Amazon Matching](./ob-creating-magento-attributes.md). Se necessario, controlla i tuoi [!DNL Commerce] [attributi](./managing-attributes.md) e crea o modifica un attributo in modo che corrisponda a questi dati di Amazon. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | È attivo solo se è impostato su `Import Listing`.<br>Scegli l’ [!DNL Commerce] attributo che corrisponde all’attributo Amazon per Amazon ASIN. Se questo attributo non esiste, consulta [Creazione di attributi di prodotto Amazon per Amazon Matching](./ob-creating-magento-attributes.md). Se necessario, controlla i tuoi [!DNL Commerce] [attributi](./managing-attributes.md) e crea o modifica un attributo in modo che corrisponda a questi dati di Amazon. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
