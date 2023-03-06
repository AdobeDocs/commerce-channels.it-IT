---
title: Impostazioni store predefinite
description: Modifica le impostazioni predefinite di Commerce per personalizzare il Sales Channel Amazon per il tuo archivio.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Impostazioni store predefinite

Dopo aver connesso l’archivio e aver impostato la prima regola di inserzione, la sincronizzazione dei dati tra Amazon e [!DNL Commerce] inizia. Esistono diversi tipi di impostazioni dello store che consentono di personalizzare lo store in base alle proprie esigenze. Le impostazioni del Negozio sono accessibili nel Negozio [dashboard](./amazon-store-dashboard.md).

Le impostazioni del Negozio includono:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Controllare l&#39;interazione del catalogo dei prodotti con [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) : controlla come vengono gestiti gli ordini di Amazon.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) : definisci quali prodotti del catalogo possono essere elencati in Amazon.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) : definisci in che modo viene modificato il prezzo di listino di Amazon per le inserzioni qualificate.

- **[!UICONTROL Store reports]** - [Analisi dei prezzi competitivi](./competitive-price-analysis.md) e [miglioramenti alle inserzioni](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Modifiche all’elenco](./listing-changes-log.md) e [errori di comunicazione](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Controlla le impostazioni delle e-mail e del nome del negozio del canale di vendita Amazon nella [!DNL Commerce] Amministratore

## Alcune importanti impostazioni predefinite

| Impostazione | Predefinito | Descrizione | Posizione |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | Crea corrispondenti [!DNL Commerce] ordini quando vengono ricevuti nuovi ordini da Amazon, consentendo la gestione degli ordini in [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} flusso di lavoro. Quando `Disabled`, Amazon ordina le informazioni sugli ordini di importazione per la revisione, ma gli ordini devono essere gestiti nel [!DNL Amazon Seller Central] account. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | I dati dei clienti provenienti dagli ordini di Amazon non vengono importati nel tuo [!DNL Commerce] database. Gli ordini Amazon importati vengono elaborati come pagamento guest. Se desideri creare il [!DNL Commerce] database del cliente, è necessario modificare questa impostazione in `Build New Customer Account`. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] catalogare i prodotti (che soddisfano i requisiti di idoneità di Amazon) per pubblicarli automaticamente in Amazon e creare inserzioni Amazon. Se desideri rivedere e pubblicare manualmente i prodotti, devi modificare questa impostazione in `Do Not Automatically List Eligible Products`. I prodotti in attesa di pubblicazione manuale vengono visualizzati nel [_Pronto per l&#39;elenco_](./ready-to-list.md) scheda. | [Azioni per l’elenco dei prodotti](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definisce l&#39;attributo di origine del prezzo utilizzato come base per le inserzioni Amazon. Se non si desidera utilizzare il [!DNL Commerce] `Price` come prezzo base su cui si basano le regole di determinazione prezzi, è necessario modificare questa impostazione in un attributo diverso. | [Prezzo di vendita](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Il mercante evade tutti gli ordini. Se si utilizza l&#39;evasione tramite Amazon o una combinazione di metodi di evasione, è necessario modificare questa impostazione. | [Soddisfatto da](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Se tutti i prodotti hanno la stessa condizione, puoi selezionare una delle opzioni di condizione di Amazon per rappresentare tutti i prodotti. Se il catalogo contiene prodotti in condizioni diverse (ad esempio nuovi, usati e ricondizionati), è necessario modificare questa impostazione in `Assign Condition Using Product Attribute` e mappare [!DNL Commerce] gli attributi della condizione alle condizioni dell’inserzione Amazon. | [Condizione elenco prodotti](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | nessuno | Definisci le regole utilizzate per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici o complesse da includere o escludere prodotti come inserzioni. | [Regole di inserzione](./listing-rules.md) |
| Regole di determinazione prezzi | nessuno | Definisci un attributo di prezzo dell’inserzione Amazon diverso da quello definito _[!UICONTROL Magento Price Source]_nel tuo [Prezzo di vendita](./listing-price.md). Per regolare il prezzo dell&#39;inserzione (su o giù) in base al_[!UICONTROL Magento Price Source]_ , creare regole. | [Regole di determinazione prezzi](./pricing-products.md) |

Per ulteriori informazioni, consulta [Impostazioni store](./ob-store-review.md).
