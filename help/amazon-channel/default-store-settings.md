---
title: Impostazioni store predefinite per le inserzioni Amazon
description: Modifica le impostazioni predefinite di Commerce per personalizzare il Sales Channel Amazon per il tuo archivio.
role: Admin
feature: Sales Channels, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Impostazioni store predefinite per le inserzioni Amazon

Dopo aver connesso l&#39;archivio e aver impostato la prima regola di inserzione, viene avviata la sincronizzazione dei dati tra Amazon e [!DNL Commerce]. Esistono diversi tipi di impostazioni dello store che consentono di personalizzare lo store in base alle proprie esigenze. Accesso alle impostazioni dello store nel [dashboard](./amazon-store-dashboard.md) dello store.

Le impostazioni del Negozio includono:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Controlla la modalità di interazione del catalogo prodotti con [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Controlla la modalità di gestione degli ordini di Amazon.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definisci quali prodotti del catalogo possono essere elencati in Amazon.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Definisci come viene modificato il prezzo di listino di Amazon per le inserzioni qualificate.

- **[!UICONTROL Store reports]** - [Analisi dei prezzi competitivi](./competitive-price-analysis.md) e [miglioramenti delle inserzioni](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Modifiche all&#39;elenco](./listing-changes-log.md) e [errori di comunicazione](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Rivedi le impostazioni del nome del negozio del canale di vendita di Amazon e dell&#39;e-mail nell&#39;amministratore [!DNL Commerce].

## Alcune importanti impostazioni predefinite

| Impostazione | Predefinito | Descrizione | Posizione |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | `Enabled` | Crea [!DNL Commerce] ordini corrispondenti quando vengono ricevuti nuovi ordini da Amazon, consentendo la gestione degli ordini nel flusso di lavoro [[!DNL Commerce] Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). Quando `Disabled`, Amazon ordina di importare le informazioni dell&#39;ordine per la revisione, ma gli ordini devono essere gestiti nel tuo account [!DNL Amazon Seller Central]. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | I dati dei clienti provenienti dagli ordini di Amazon non vengono importati nel database [!DNL Commerce]. Gli ordini Amazon importati vengono elaborati come pagamento guest. Se si desidera creare il database clienti [!DNL Commerce], è necessario modificare questa impostazione in `Build New Customer Account`. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] cataloga i prodotti (che soddisfano i requisiti di idoneità di Amazon) per pubblicarli automaticamente in Amazon e creare inserzioni Amazon. Se si desidera rivedere e pubblicare manualmente i prodotti, è necessario modificare questa impostazione in `Do Not Automatically List Eligible Products`. I prodotti in attesa di pubblicazione manuale vengono visualizzati nella scheda [_Pronto per l&#39;elenco_](./ready-to-list.md). | [Azioni per l&#39;elenco dei prodotti](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definisce l&#39;attributo di origine del prezzo utilizzato come base per le inserzioni Amazon. Se non si desidera utilizzare l&#39;attributo [!DNL Commerce] `Price` come prezzo base su cui si basano le regole di determinazione prezzi, è necessario modificare questa impostazione in un attributo diverso. | [Prezzo di vendita](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Il mercante evade tutti gli ordini. Se si utilizza l&#39;evasione tramite Amazon o una combinazione di metodi di evasione, è necessario modificare questa impostazione. | [Soddisfatto da](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Se tutti i prodotti hanno la stessa condizione, puoi selezionare una delle opzioni di condizione di Amazon per rappresentare tutti i prodotti. Se il catalogo contiene prodotti in condizioni diverse (ad esempio nuovi, usati e ricondizionati), è necessario modificare questa impostazione in `Assign Condition Using Product Attribute` e mappare gli attributi della condizione [!DNL Commerce] alle condizioni dell&#39;inserzione Amazon. | [Condizione elenco prodotti](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | nessuno | Definisci le regole utilizzate per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici o complesse da includere o escludere prodotti come inserzioni. | [Regole di elenco](./listing-rules.md) |
| Regole di determinazione prezzi | nessuno | Definisci l&#39;attributo del prezzo dell&#39;inserzione Amazon diverso da _[!UICONTROL Magento Price Source]_definito nel [Prezzo dell&#39;inserzione](./listing-price.md). Per modificare il prezzo dell&#39;inserzione (su o giù) in base all&#39;impostazione_[!UICONTROL Magento Price Source]_, creare le regole. | [Regole di determinazione prezzi](./pricing-products.md) |

Per ulteriori informazioni, vedere [Impostazioni archivio](./ob-store-review.md).
