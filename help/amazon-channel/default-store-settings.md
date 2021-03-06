---
title: Impostazioni store predefinite
description: Modifica le impostazioni Commerce predefinite per personalizzare il Sales Channel Amazon per il tuo negozio.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Impostazioni store predefinite

Dopo aver connesso l&#39;archivio e aver impostato la prima regola di elenco, la sincronizzazione dei dati tra Amazon e [!DNL Commerce] inizia. Esistono diversi tipi di impostazioni store che consentono di personalizzare lo store in base alle proprie esigenze. Le impostazioni dello store sono accessibili nello store [dashboard](./amazon-store-dashboard.md).

Le impostazioni store includono:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Controllare il modo in cui il catalogo dei prodotti interagisce con [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Controllare la modalità di gestione degli ordini Amazon.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definisci quali prodotti di catalogo possono essere elencati in Amazon.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Definire la modalità di modifica del prezzo di listino di Amazon per gli elenchi qualificati.

- **[!UICONTROL Store reports]** - [Analisi dei prezzi competitiva](./competitive-price-analysis.md) e [elenco dei miglioramenti](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Modifiche all&#39;elenco](./listing-changes-log.md) e [errori di comunicazione](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Rivedi le impostazioni del nome dell&#39;archivio dei canali di vendita e-mail e Amazon nella sezione [!DNL Commerce] Amministratore.

## Alcune importanti impostazioni predefinite

| Impostazione | Predefinito | Descrizione | Posizione |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | Crea corrispondenti [!DNL Commerce] gli ordini ricevuti da Amazon in caso di nuovi ordini, che consentono di gestire gli ordini nel [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html)Flusso di lavoro {target=&quot;_blank&quot;}. Quando `Disabled`, Amazon ordina le informazioni sull’ordine di importazione per la revisione, ma gli ordini devono essere gestiti nel tuo [!DNL Amazon Seller Central] conto. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | I dati dei clienti provenienti da ordini Amazon non vengono importati nel tuo [!DNL Commerce] database. Gli ordini Amazon importati vengono elaborati come pagamento guest. Se desideri creare la tua [!DNL Commerce] database del cliente, è necessario modificare questa impostazione in `Build New Customer Account`. | [Impostazioni ordine](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] prodotti di catalogo (che soddisfano i requisiti di idoneità di Amazon) per pubblicare automaticamente in Amazon e creare annunci Amazon. Per rivedere e pubblicare manualmente i prodotti, modifica questa impostazione in `Do Not Automatically List Eligible Products`. I prodotti in attesa di pubblicazione manuale compaiono sul [_Pronto per l&#39;elenco_](./ready-to-list.md) scheda . | [Azioni di elenco dei prodotti](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definisce l&#39;attributo dell&#39;origine del prezzo utilizzato come base per gli elenchi Amazon. Se non desideri utilizzare il [!DNL Commerce] `Price` attribuisci come prezzo di base a cui si basano le regole di determinazione dei prezzi, devi modificare questa impostazione in un attributo diverso. | [Prezzo di listino](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Il commerciante adempie tutti gli ordini. Se utilizzi Fulfillment by Amazon o utilizzi una combinazione di metodi di evasione, devi modificare questa impostazione. | [Completato da](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Se tutti i prodotti presentano la stessa condizione, puoi selezionare una delle opzioni di condizione di Amazon per rappresentare tutti i prodotti. Se il catalogo contiene prodotti in condizioni diverse (ad esempio Nuovo, Utilizzato e Aggiornato), è necessario modificare questa impostazione in `Assign Condition Using Product Attribute` e mappa il [!DNL Commerce] attributi di condizione per le condizioni di elenco di Amazon. | [Condizione dell’elenco dei prodotti](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | nessuno | Definisci le regole utilizzate per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici e complesse per includere o escludere i prodotti come elenchi. | [Regole di elenco](./listing-rules.md) |
| Regole di determinazione prezzi | nessuno | Definisci l’attributo del prezzo di listino di Amazon diverso da quello definito _[!UICONTROL Magento Price Source]_nel tuo [Prezzo di listino](./listing-price.md). Per regolare il prezzo dell&#39;inserzione (su o giù) rispetto al_[!UICONTROL Magento Price Source]_ impostazione, creare regole. | [Regole di determinazione prezzi](./pricing-products.md) |

Per ulteriori informazioni, consulta [Impostazioni store](./ob-store-review.md).
