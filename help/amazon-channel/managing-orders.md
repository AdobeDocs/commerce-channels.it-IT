---
title: Gestisci ordini
description: Puoi abilitare l’importazione degli ordini nelle Impostazioni ordine per gestire più facilmente gli ordini di Amazon dall’amministratore di Commerce.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Gestisci ordini

È possibile visualizzare le informazioni sull’ordine di Amazon ricevute da Amazon nel _[!UICONTROL Recent Orders]_sezione del [dashboard store](./amazon-store-dashboard.md) o il_[!UICONTROL Amazon orders]_ pagina (denominata anche _[!UICONTROL All Orders]_view).

La modalità di gestione degli ordini di Amazon dipende dall’abilitazione o meno dell’importazione negli [Impostazioni ordine](./order-settings.md#configure-order-settings).

## Con importazione ordine abilitata

Dopo [integrazione store](./store-integration.md), il [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) impostazione è `Enabled` per impostazione predefinita. Con questa impostazione, corrispondente [!DNL Commerce] gli ordini vengono creati per gli ordini Amazon e possono essere gestiti in [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} flusso di lavoro.

>[!NOTE]
>
>Indipendentemente dalle impostazioni di importazione degli ordini, gli ordini Amazon presenti nel tuo [!DNL Amazon Seller Central] account prima del [integrazione store](./store-integration.md) non vengono importati.

Gli ordini Amazon importati vengono gestiti in [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workflow, just like your other [!DNL Commerce] stores. Click the Amazon order number in the *[!UICONTROL Order Number]* column to open the order in the [[!DNL Commerce] order process](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target="_blank"}. Consulta [Visualizza ordini Amazon](./amazon-orders-all.md).

### Processo di importazione degli ordini

Quando un ordine viene effettuato su Amazon e [importazione ordine](./order-settings.md) è attivato, inizia il seguente processo.

| Cambia | Azioni |
|---|---|
| Un ordine viene effettuato su Amazon. | <ul><li>Amazon imposta lo stato dell’ordine su `Pending`.</li><li>Le informazioni sull’ordine vengono inviate a [!DNL Commerce].</li><li>L&#39;ordine viene aggiunto a [_Ordini Amazon_ tabella](./amazon-orders-all.md) con un `Pending` stato.</li></ul> |
| Amazon modifica lo stato dell’ordine in `Unshipped`. | <ul><li>La modifica dello stato viene inviata a [!DNL Commerce].</li><li>In [_Ordini Amazon_ tabella](./amazon-orders-all.md), lo stato dell’ordine diventa `Unshipped`.</li><li>In [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}, un corrispondente [!DNL Commerce] l’ordine viene creato con un `Processing` stato.</li></ul> |
| In entrata [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}, il [!DNL Commerce] l&#39;ordine viene elaborato e lo stato cambia in `Shipped`. | <ul><li>In [_Ordini Amazon_ tabella](./amazon-orders-all.md), lo stato dell’ordine diventa `Shipped`.</li><li>Al successivo job cron, lo stato dell&#39;ordine cambia in `Complete` nel [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}.</li></ul> |

### Blocchi della creazione degli ordini

Esistono alcuni scenari che impediscono la creazione del corrispondente [!DNL Commerce] ordine. [!DNL Commerce] gli ordini non vengono creati per gli ordini ricevuti quando si verifica uno dei seguenti problemi.

| Scenario | Soluzione |
|---|---|
| L&#39;elemento non esiste in [!DNL Commerce] catalogo. | [Creare il prodotto](./creating-assigning-catalog-products.md) nel tuo [!DNL Commerce] catalogo e [corrispondenza manuale](./creating-assigning-catalog-products.md) al prodotto. |
| L&#39;elemento nel catalogo è disabilitato. | Assicurati che il [stato del prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} è abilitato. |
| L&#39;articolo ordinato è esaurito. | Aggiornare o configurare il [opzioni prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} per quantità e origine. |

Quando gli ordini non possono essere importati, nella parte superiore dello schermo viene visualizzato un messaggio di sistema simile al seguente:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Quando il problema viene risolto, il [!DNL Commerce] l&#39;ordine viene creato alla sincronizzazione successiva.

## Con importazione ordine disabilitata

Se non desideri importare e gestire gli ordini di Amazon in [!DNL Commerce], è possibile modificare [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) impostazione su `Disabled`. Ciò significa che, quando si ricevono nuovi ordini da Amazon, i corrispondenti [!DNL Commerce] gli ordini non vengono creati.

Se l&#39;opzione è disabilitata, le informazioni sugli ordini ricevute da Amazon vengono visualizzate nel _[!UICONTROL Recent Orders]_sezione del dashboard del negozio e nella sezione_[!UICONTROL All Orders]_ visualizzazione. Queste informazioni sull&#39;ordine sono di sola visualizzazione e occorre gestire questi ordini in [!DNL Amazon Seller Central]. Per aprire i dettagli dell&#39;ordine in [!DNL Amazon Seller Central], fai clic sul numero di ordine di Amazon in _[!UICONTROL Order Number]_colonna.

Vedi anche [Visualizza ordini Amazon](./amazon-orders-all.md), [Visualizza dettagli ordine Amazon](./amazon-order-details.md), e [Attività comuni di elaborazione degli ordini](./common-order-processing.md).
