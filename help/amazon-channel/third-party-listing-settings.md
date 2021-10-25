---
title: Elenco di terze parti
description: Aggiorna le impostazioni dell’elenco di terze parti per determinare se il catalogo Commerce importa prodotti dagli elenchi Amazon Seller Central esistenti.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Elenco di terze parti

Le impostazioni di elenco di terze parti fanno parte delle impostazioni di elenco degli archivi. Le impostazioni dell’elenco sono accessibili dal [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni determinano se le [!DNL Commerce] il catalogo importa i prodotti dalla cartella esistente [!DNL Amazon Seller Central] elenchi. È consigliabile importare gli elenchi da Amazon per garantire che tutti gli elenchi corrispondano [!DNL Commerce] prodotti. Quando le tue inserzioni fanno parte del tuo [!DNL Commerce] catalogo, puoi gestire tutti i tuoi prodotti da un unico catalogo e utilizzare le funzioni dei canali di vendita Amazon. Queste funzionalità includono la gestione dell&#39;evasione e dell&#39;ordine con Amazon, la revisione intelligente dei prezzi e la gestione della quantità.

Una volta configurato per importare gli elenchi Amazon, il canale di vendita Amazon importa gli elenchi Amazon nel tuo [!DNL Commerce] catalogo, tentativo di abbinarli ai prodotti esistenti. Se una corrispondenza non viene trovata automaticamente, puoi importare l’elenco Amazon come nuovo [!DNL Commerce] o abbinare manualmente l’elenco a un prodotto.

Se scegli di importare gli elenchi Amazon, scegli la [!DNL Commerce] attributi con valori per SKU venditore Amazon e ASIN Amazon. Se non hai [!DNL Commerce] [attributi del prodotto](./ob-creating-magento-attributes.md), considera la creazione e l’assegnazione di tali tag. La mappatura di questi attributi aiuta a far corrispondere correttamente gli elenchi di Amazon importati ai tuoi [!DNL Commerce] prodotti.

L&#39;importazione iniziale dell&#39;elenco viene avviata quando [integrazione store](./store-integration.md) è completo. In seguito e in base alle impostazioni del cron, [!DNL Commerce] controlla continuamente gli elenchi di Amazon appena aggiunti (non creati in Amazon Sales Channel) e aggiorna i tuoi [!DNL Commerce] catalogare in base alle impostazioni degli elenchi di terze parti.

## Configurare le impostazioni di elenco di terze parti

1. Fai clic su **[!UICONTROL Listing Settings]** sul dashboard dello store.

1. Espandi la _[!UICONTROL Third Party Listings]_sezione .

1. Per **[!UICONTROL Import Third Party Listings]** (obbligatorio), scegli un’opzione:

   - `Import Listing` - (Impostazione predefinita) Scegli quando importare le informazioni di prodotto dagli elenchi di Amazon nel tuo [!DNL Commerce] catalogo dei prodotti. Questa è l’opzione predefinita ed è consigliata.

   - `Do Not Import Listing` - Scegliere quando si desidera manualmente [creare e assegnare nuovi prodotti](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;} al tuo [!DNL Commerce] catalogo per gli elenchi Amazon.
   >[!NOTE]
   >I campi delle opzioni seguenti sono attivi solo se impostati su `Import Listing`.

1. Per **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, scegli [!DNL Commerce] che corrisponde al valore SKU del venditore di Amazon.

1. Per **[!UICONTROL Attribute That Contains Amazon ASIN]**, scegli [!DNL Commerce] Attributo creato e corrispondente ad Amazon ASIN.

   >[!NOTE]
   >Se non hai creato questi [!DNL Commerce] attributi per gli elenchi di Amazon, vedi [Creazione di attributi per Amazon Matching](./ob-creating-magento-attributes.md).

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Elenco di terzi](assets/amazon-third-party-listings.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Third Party Listings] | Obbligatorio. Opzioni:<ul><li>**[!UICONTROL Import Listing]** - (Impostazione predefinita) Scegli quando importare le informazioni di prodotto dagli elenchi di Amazon nel tuo [!DNL Commerce] catalogo dei prodotti. </li><li>**[!UICONTROL Do Not Import Listing]** - Scegliere quando si desidera manualmente [creare e assegnare nuovi prodotti](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;} al tuo [!DNL Commerce] catalogo per gli elenchi Amazon.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Solo attivo se impostato su `Import Listing`.<br>Scegli la [!DNL Commerce] come corrispondenza all’attributo Amazon per lo SKU del venditore Amazon. Se questo attributo non esiste, vedi [Creazione di attributi di prodotto Amazon per Amazon Matching](./ob-creating-magento-attributes.md). Se necessario, rivedi il tuo [!DNL Commerce] [attributes](./managing-attributes.md) e crea o modifica un attributo corrispondente a questi dati di Amazon. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Solo attivo se impostato su `Import Listing`.<br>Scegli la [!DNL Commerce] attributo corrispondente all’attributo Amazon per Amazon ASIN. Se questo attributo non esiste, vedi [Creazione di attributi di prodotto Amazon per Amazon Matching](./ob-creating-magento-attributes.md). Se necessario, rivedi il tuo [!DNL Commerce] [attributes](./managing-attributes.md) e crea o modifica un attributo corrispondente a questi dati di Amazon. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
