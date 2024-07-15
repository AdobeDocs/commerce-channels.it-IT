---
title: Sales Channel Amazon - [!UICONTROL Third-party Listings]
description: Aggiorna le impostazioni delle inserzioni di terze parti per determinare se il catalogo Commerce importa prodotti dalle inserzioni esistenti di Amazon Seller Central.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

Le impostazioni delle inserzioni di terze parti fanno parte delle impostazioni delle inserzioni del Negozio. Le impostazioni dell&#39;inserzione sono accessibili dal [dashboard dell&#39;archivio](./amazon-store-dashboard.md).

Queste impostazioni determinano se il catalogo [!DNL Commerce] importa prodotti dalle inserzioni [!DNL Amazon Seller Central] esistenti. È consigliabile importare le inserzioni da Amazon per assicurarsi che tutte le inserzioni abbiano prodotti [!DNL Commerce] corrispondenti. Quando le tue inserzioni fanno parte del catalogo [!DNL Commerce], puoi gestire tutti i tuoi prodotti da un singolo catalogo e utilizzare le funzionalità del canale di vendita Amazon. Queste funzioni includono gestione degli ordini e dell&#39;evasione con Amazon, ridefinizione intelligente dei prezzi e gestione della quantità.

Se configurato per importare le tue inserzioni Amazon, il canale di vendita Amazon importa le tue inserzioni Amazon nel catalogo [!DNL Commerce], tentando di farle corrispondere ai prodotti esistenti. Se non viene trovata automaticamente una corrispondenza, puoi importare l&#39;inserzione di Amazon come nuovo prodotto [!DNL Commerce] o abbinare manualmente l&#39;inserzione a un prodotto.

Se scegli di importare le tue inserzioni Amazon, scegli gli attributi [!DNL Commerce] con i valori per Amazon Seller SKU e Amazon ASIN. Se non disponi di [!DNL Commerce] [attributi di prodotto](./ob-creating-magento-attributes.md), puoi crearli e assegnarli. La mappatura di questi attributi consente di associare correttamente le inserzioni Amazon importate ai prodotti [!DNL Commerce].

L&#39;importazione iniziale dell&#39;elenco viene avviata quando [viene completata l&#39;integrazione dell&#39;archivio](./store-integration.md). In seguito e in base alle impostazioni cron, [!DNL Commerce] controlla continuamente le inserzioni Amazon appena aggiunte (non create nel Sales Channel Amazon) e aggiorna il catalogo [!DNL Commerce] in base alle impostazioni delle inserzioni di terze parti.

## Configurare le impostazioni per l’inserzione di terze parti

1. Fare clic su **[!UICONTROL Listing Settings]** nel dashboard dell&#39;archivio.

1. Espandere la sezione _[!UICONTROL Third Party Listings]_.

1. Per **[!UICONTROL Import Third Party Listings]** (obbligatorio), scegliere un&#39;opzione:

   - `Import Listing` - (Predefinito) Scegli quando vuoi che le informazioni sui prodotti delle tue inserzioni Amazon vengano importate nel catalogo prodotti [!DNL Commerce]. Questa opzione è quella predefinita ed è consigliata.

   - `Do Not Import Listing` - Scegli quando desideri [creare e assegnare manualmente nuovi prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) al catalogo [!DNL Commerce] per le tue inserzioni Amazon.

   >[!NOTE]
   >I campi delle opzioni seguenti sono attivi solo se impostati su `Import Listing`.

1. Per **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, scegli l&#39;attributo [!DNL Commerce] che corrisponde al valore SKU del venditore Amazon.

1. Per **[!UICONTROL Attribute That Contains Amazon ASIN]**, scegliere l&#39;attributo [!DNL Commerce] creato e confrontarlo con il codice ASIN di Amazon.

   >[!NOTE]
   >Se non hai creato questi [!DNL Commerce] attributi per le tue inserzioni Amazon, consulta [Creazione di attributi per corrispondenza Amazon](./ob-creating-magento-attributes.md).

1. Al termine, fare clic su **[!UICONTROL Save listing settings]**.

![Inserzioni di terze parti](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | Obbligatorio. Opzioni:<ul><li>**[!UICONTROL Import Listing]** - (Predefinito) Scegli quando vuoi che le informazioni sui prodotti delle tue inserzioni Amazon vengano importate nel catalogo prodotti [!DNL Commerce]. </li><li>**[!UICONTROL Do Not Import Listing]** - Scegli quando desideri [creare e assegnare manualmente nuovi prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) al catalogo [!DNL Commerce] per le tue inserzioni Amazon.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Attivo solo se impostato su `Import Listing`.<br>Scegli l&#39;attributo [!DNL Commerce] come corrispondenza con l&#39;attributo Amazon per lo SKU del venditore Amazon. Se questo attributo non esiste, vedere [Creazione di attributi di prodotto Amazon per la corrispondenza Amazon](./ob-creating-magento-attributes.md). Se necessario, controlla [!DNL Commerce] [attributi](./managing-attributes.md) e crea o modifica un attributo che corrisponda a questi dati di Amazon. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Attivo solo se impostato su `Import Listing`.<br>Scegliere l&#39;attributo [!DNL Commerce] corrispondente all&#39;attributo Amazon per Amazon ASIN. Se questo attributo non esiste, vedere [Creazione di attributi di prodotto Amazon per la corrispondenza Amazon](./ob-creating-magento-attributes.md). Se necessario, controlla [!DNL Commerce] [attributi](./managing-attributes.md) e crea o modifica un attributo che corrisponda a questi dati di Amazon. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
