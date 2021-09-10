---
title: Gestisci ordini
description: Puoi abilitare l’importazione degli ordini nelle Impostazioni ordine per gestire più facilmente gli ordini Amazon dal tuo amministratore Commerce.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Gestire gli ordini

Puoi visualizzare le informazioni sull&#39;ordine Amazon, come ricevuto da Amazon, nella sezione _[!UICONTROL Recent Orders]_del [dashboard dell&#39;archivio](./amazon-store-dashboard.md) o nella pagina_[!UICONTROL Amazon orders]_ (detta anche visualizzazione _[!UICONTROL All Orders]_).

La modalità di gestione degli ordini di Amazon dipende dall&#39;abilitazione o meno dell&#39;importazione degli ordini in [Impostazioni ordine](./order-settings.md#configure-order-settings).

## Con importazione ordine abilitata

Dopo l&#39; [integrazione store](./store-integration.md), l&#39;impostazione [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) è `Enabled` per impostazione predefinita. Con questa impostazione, gli ordini [!DNL Commerce] corrispondenti vengono creati per i tuoi ordini Amazon e possono essere gestiti nel flusso di lavoro [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Indipendentemente dalle impostazioni di importazione dell&#39;ordine, gli ordini Amazon presenti nel tuo account [!DNL Amazon Seller Central] prima dell&#39; [integrazione store](./store-integration.md) non vengono importati.

Gli ordini Amazon importati vengono gestiti nel flusso di lavoro [[!DNL Commerce] Ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, proprio come gli altri archivi [!DNL Commerce]. Fai clic sul numero dell&#39;ordine Amazon nella colonna *[!UICONTROL Order Number]* per aprire l&#39;ordine nel processo [[!DNL Commerce] order](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}. Consulta [Visualizza ordini Amazon](./amazon-orders-all.md).

### Processo di importazione degli ordini

Quando un ordine viene inserito in Amazon e [order import](./order-settings.md) è abilitato, inizia il seguente processo.

| Modifica | Azioni |
|---|---|
| Viene effettuato un ordine su Amazon. | <ul><li>Amazon imposta lo stato dell’ordine su `Pending`.</li><li>Le informazioni sull&#39;ordine vengono inviate a [!DNL Commerce].</li><li>L&#39;ordine viene aggiunto alla tabella [_Ordini Amazon_](./amazon-orders-all.md) con uno stato `Pending` .</li></ul> |
| Amazon modifica lo stato dell’ordine in `Unshipped`. | <ul><li>La modifica dello stato viene inviata a [!DNL Commerce].</li><li>Nella tabella [_Ordini Amazon_](./amazon-orders-all.md), lo stato dell&#39;ordine cambia in `Unshipped`.</li><li>Nel flusso di lavoro [[!DNL Commerce] ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} viene creato un ordine [!DNL Commerce] corrispondente con uno stato `Processing`.</li></ul> |
| In [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}, l&#39;ordine [!DNL Commerce] viene elaborato e lo stato cambia in `Shipped`. | <ul><li>Nella tabella [_Ordini Amazon_](./amazon-orders-all.md), lo stato dell&#39;ordine cambia in `Shipped`.</li><li>Nel processo cron successivo, lo stato dell&#39;ordine cambia in `Complete` nel [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.</li></ul> |

### Blocchi per la creazione di ordini

Esistono alcuni scenari che impediscono la creazione dell&#39;ordine corrispondente [!DNL Commerce]. [!DNL Commerce] gli ordini non vengono creati per gli ordini ricevuti quando si verifica uno dei seguenti problemi.

| Scenario | Soluzione |
|---|---|
| L&#39;elemento non esiste nel catalogo [!DNL Commerce]. | [Crea la ](./creating-assigning-catalog-products.md) produzione del  [!DNL Commerce] catalogo e la  [corrispondenza ](./creating-assigning-catalog-products.md) manuale con il prodotto. |
| L&#39;elemento nel catalogo è disabilitato. | Assicurati che lo [stato del prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} sia abilitato. |
| L&#39;articolo ordinato è esaurito. | Aggiorna o configura le [opzioni prodotto](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} per la quantità e l&#39;origine. |

Quando gli ordini non possono essere importati, nella parte superiore dello schermo viene visualizzato un messaggio di sistema simile al seguente:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Quando il problema viene risolto, l&#39;ordine [!DNL Commerce] viene creato nella sincronizzazione successiva.

## Con importazione ordine disattivata

Se non desideri importare e gestire gli ordini Amazon in [!DNL Commerce], puoi modificare l&#39;impostazione [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) in `Disabled`. Questa impostazione significa che quando nuovi ordini vengono ricevuti da Amazon, gli ordini corrispondenti [!DNL Commerce] non vengono creati.

Se disabilitata, le informazioni sull&#39;ordine ricevute da Amazon vengono visualizzate nella sezione _[!UICONTROL Recent Orders]_del dashboard dello store e nella vista_[!UICONTROL All Orders]_. Queste informazioni sull&#39;ordine sono di sola visualizzazione e devi gestire questi ordini in [!DNL Amazon Seller Central]. Per aprire i dettagli dell&#39;ordine in [!DNL Amazon Seller Central], fai clic sul numero dell&#39;ordine Amazon nella colonna _[!UICONTROL Order Number]_.

Consulta anche [Visualizza ordini Amazon](./amazon-orders-all.md), [Visualizza dettagli ordini Amazon](./amazon-order-details.md) e [Attività di elaborazione ordini comuni](./common-order-processing.md).
