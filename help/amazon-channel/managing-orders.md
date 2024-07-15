---
title: Gestire gli ordini di Amazon
description: Puoi abilitare l’importazione degli ordini nelle Impostazioni ordine per gestire più facilmente gli ordini di Amazon dal tuo amministratore Commerce.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Gestire gli ordini di Amazon

È possibile visualizzare le informazioni sull&#39;ordine di Amazon ricevute da Amazon nella sezione _[!UICONTROL Recent Orders]_del dashboard [store](./amazon-store-dashboard.md) o nella pagina_[!UICONTROL Amazon orders]_ (denominata anche visualizzazione _[!UICONTROL All Orders]_).

La modalità di gestione degli ordini di Amazon dipende dall&#39;abilitazione o meno dell&#39;importazione degli ordini nelle [Impostazioni ordine](./order-settings.md#configure-order-settings).

## Con importazione ordine abilitata

Dopo l&#39;[integrazione store](./store-integration.md), l&#39;impostazione predefinita [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) è `Enabled`. Con questa impostazione, vengono creati [!DNL Commerce] ordini corrispondenti per gli ordini Amazon e possono essere gestiti nel flusso di lavoro [[!DNL Commerce] Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).

>[!NOTE]
>
>Indipendentemente dalle impostazioni di importazione degli ordini, gli ordini Amazon esistenti nell&#39;account [!DNL Amazon Seller Central] prima dell&#39;integrazione dello [store](./store-integration.md) non vengono importati.

Gli ordini Amazon importati vengono gestiti nel flusso di lavoro [[!DNL Commerce] Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), proprio come gli altri negozi [!DNL Commerce]. Fare clic sul numero di ordine Amazon nella colonna *[!UICONTROL Order Number]* per aprire l&#39;ordine nel [[!DNL Commerce] processo ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions). Vedi [Visualizza ordini Amazon](./amazon-orders-all.md).

### Processo di importazione degli ordini

Quando un ordine viene effettuato su Amazon e l&#39;importazione [ordine](./order-settings.md) è abilitata, inizia il seguente processo.

| Cambia | Azioni |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Un ordine viene effettuato su Amazon. | <ul><li>Amazon imposta lo stato dell&#39;ordine su `Pending`.</li><li>Informazioni sull&#39;ordine inviate a [!DNL Commerce].</li><li>Ordine aggiunto a [_ordini Amazon_ tabella](./amazon-orders-all.md) con stato `Pending`.</li></ul> |
| Amazon modifica lo stato dell&#39;ordine in `Unshipped`. | <ul><li>La modifica dello stato viene inviata a [!DNL Commerce].</li><li>Nella tabella [_Ordini Amazon_](./amazon-orders-all.md), lo stato dell&#39;ordine cambia in `Unshipped`.</li><li>Nel flusso di lavoro [[!DNL Commerce] ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), viene creato un ordine [!DNL Commerce] corrispondente con stato `Processing`.</li></ul> |
| In [[!DNL Commerce] flusso di lavoro ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), l&#39;ordine [!DNL Commerce] viene elaborato e lo stato cambia in `Shipped`. | <ul><li>Nella tabella [_Ordini Amazon_](./amazon-orders-all.md), lo stato dell&#39;ordine cambia in `Shipped`.</li><li>Nel successivo processo cron, lo stato dell&#39;ordine cambia in `Complete` nel [[!DNL Commerce] flusso di lavoro ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul> |

### Blocchi della creazione degli ordini

Esistono alcuni scenari che impediscono la creazione dell&#39;ordine [!DNL Commerce] corrispondente. [!DNL Commerce] ordini non creati per gli ordini ricevuti quando si verifica uno dei seguenti problemi.

| Scenario | Soluzione |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Elemento inesistente nel catalogo [!DNL Commerce]. | [Crea il prodotto](./creating-assigning-catalog-products.md) nel catalogo [!DNL Commerce] e [abbina manualmente](./creating-assigning-catalog-products.md) al prodotto. |
| L&#39;elemento nel catalogo è disabilitato. | Verificare che lo stato del [prodotto](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) sia abilitato. |
| L&#39;articolo ordinato è esaurito. | Aggiorna o configura le [opzioni prodotto](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) per quantità e origine. |

Quando gli ordini non possono essere importati, nella parte superiore dello schermo viene visualizzato un messaggio di sistema simile al seguente:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Quando il problema viene risolto, l&#39;ordine [!DNL Commerce] viene creato alla sincronizzazione successiva.

## Con importazione ordine disabilitata

Se non desideri importare e gestire gli ordini Amazon in [!DNL Commerce], puoi modificare l&#39;impostazione [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) in `Disabled`. Ciò significa che quando si ricevono nuovi ordini da Amazon, non vengono creati [!DNL Commerce] ordini corrispondenti.

Se disabilitata, le informazioni sull&#39;ordine ricevute da Amazon vengono visualizzate nella sezione _[!UICONTROL Recent Orders]_del dashboard dell&#39;archivio e nella visualizzazione_[!UICONTROL All Orders]_. Le informazioni sull&#39;ordine sono di sola visualizzazione e sarà necessario gestire questi ordini in [!DNL Amazon Seller Central]. Per aprire i dettagli dell&#39;ordine in [!DNL Amazon Seller Central], fare clic sul numero dell&#39;ordine Amazon nella colonna _[!UICONTROL Order Number]_.

Vedi anche [Visualizza ordini Amazon](./amazon-orders-all.md), [Visualizza dettagli ordine Amazon](./amazon-order-details.md) e [Attività comuni di elaborazione ordine](./common-order-processing.md).
