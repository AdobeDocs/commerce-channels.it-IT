---
title: Gestisci ordini
description: Puoi abilitare l’importazione degli ordini nelle Impostazioni ordine per gestire più facilmente gli ordini Amazon dal tuo amministratore Commerce.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 1d1b888db4de4f6e3658af768cd6f5cf30828788
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gestire gli ordini

Puoi visualizzare le informazioni sull’ordine Amazon, come ricevuto da Amazon, nella _[!UICONTROL Recent Orders]_della sezione [dashboard store](./amazon-store-dashboard.md) o_[!UICONTROL Amazon orders]_ (o _[!UICONTROL All Orders]_vista).

La modalità di gestione degli ordini di Amazon dipende dall’abilitazione o meno dell’importazione dell’ordine nel [Impostazioni ordine](./order-settings.md#configure-order-settings).

## Con importazione ordine abilitata

Dopo [integrazione store](./store-integration.md), [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) impostazione `Enabled` per impostazione predefinita. Con questa impostazione, corrispondente [!DNL Commerce] gli ordini vengono creati per i tuoi ordini Amazon e possono essere gestiti nel [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html)Flusso di lavoro {target=&quot;_blank&quot;}.

>[!NOTE]
>
>Indipendentemente dalle impostazioni di importazione dell’ordine, gli ordini Amazon presenti nel [!DNL Amazon Seller Central] prima del [integrazione store](./store-integration.md) non vengono importati.

Gli ordini Amazon importati vengono gestiti nel [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html)flusso di lavoro {target=&quot;_blank&quot;}, proprio come l&#39;altro [!DNL Commerce] negozi. Fai clic sul numero dell’ordine di Amazon nel *[!UICONTROL Order Number]* per aprire l’ordine nel [[!DNL Commerce] processo dell&#39;ordine](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}. Vedi [Visualizza ordini Amazon](./amazon-orders-all.md).

### Processo di importazione degli ordini

Quando un ordine viene effettuato su Amazon e [importazione ordini](./order-settings.md) è attivato, inizia il seguente processo.

| Modifica | Azioni |
|---|---|
| Viene effettuato un ordine su Amazon. | <ul><li>Amazon imposta lo stato dell’ordine su `Pending`.</li><li>Le informazioni sull’ordine vengono inviate a [!DNL Commerce].</li><li>L’ordine viene aggiunto a [_Ordini Amazon_ tabella](./amazon-orders-all.md) con `Pending` stato.</li></ul> |
| Amazon modifica lo stato dell’ordine in `Unshipped`. | <ul><li>La modifica dello stato viene inviata a [!DNL Commerce].</li><li>In [_Ordini Amazon_ tabella](./amazon-orders-all.md), lo stato dell’ordine cambia in `Unshipped`.</li><li>In [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, un [!DNL Commerce] viene creato con un `Processing` stato.</li></ul> |
| In [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, il [!DNL Commerce] l&#39;ordine viene elaborato e lo stato cambia in `Shipped`. | <ul><li>In [_Ordini Amazon_ tabella](./amazon-orders-all.md), lo stato dell’ordine cambia in `Shipped`.</li><li>Nel successivo processo cron, lo stato dell&#39;ordine cambia in `Complete` in [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.</li></ul> |

### Blocchi per la creazione di ordini

Esistono alcuni scenari che impediscono la creazione dei corrispondenti [!DNL Commerce] ordine. [!DNL Commerce] gli ordini non vengono creati per gli ordini ricevuti quando si verifica uno dei seguenti problemi.

| Scenario | Soluzione |
|---|---|
| L&#39;elemento non esiste nel [!DNL Commerce] catalogo. | [Creare il prodotto](./creating-assigning-catalog-products.md) nel tuo [!DNL Commerce] catalogo e [corrispondenza manuale](./creating-assigning-catalog-products.md) al prodotto. |
| L&#39;elemento nel catalogo è disabilitato. | Assicurati che il [stato del prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target=&quot;_blank&quot;} è abilitato. |
| L&#39;articolo ordinato è esaurito. | Aggiorna o configura la [opzioni di prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target=&quot;_blank&quot;} per quantità e origine. |

Quando gli ordini non possono essere importati, nella parte superiore dello schermo viene visualizzato un messaggio di sistema simile al seguente:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Quando il problema viene risolto, il [!DNL Commerce] l&#39;ordine viene creato nella sincronizzazione successiva.

## Con importazione ordine disattivata

Se non desideri importare e gestire gli ordini Amazon in [!DNL Commerce], è possibile modificare le [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) impostazione su `Disabled`. Questa impostazione significa che quando vengono ricevuti nuovi ordini da Amazon, i corrispondenti [!DNL Commerce] gli ordini non vengono creati.

Se disabilitata, le informazioni sull’ordine ricevute da Amazon vengono visualizzate nella sezione _[!UICONTROL Recent Orders]_della dashboard del negozio e nella_[!UICONTROL All Orders]_ visualizza. Queste informazioni sull&#39;ordine sono di sola visualizzazione e devi gestire questi ordini in [!DNL Amazon Seller Central]. Per aprire i dettagli dell’ordine in [!DNL Amazon Seller Central], fai clic sul numero dell’ordine Amazon nel _[!UICONTROL Order Number]_colonna.

Vedi anche [Visualizza ordini Amazon](./amazon-orders-all.md), [Visualizza dettagli ordine Amazon](./amazon-order-details.md)e [Attività di elaborazione ordine comune](./common-order-processing.md).
