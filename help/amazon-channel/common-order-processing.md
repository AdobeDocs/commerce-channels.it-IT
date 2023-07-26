---
title: Attività comuni di elaborazione degli ordini in Amazon
description: Utilizza il corrispondente [!DNL Commerce] ordini creati per gli ordini di Amazon per gestire l'attività e l'elaborazione degli ordini in [!UICONTROL Commerce] Amministratore
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Attività comuni di elaborazione degli ordini in Amazon

[Elaborazione ordini commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) può gestire i tuoi ordini Amazon, tra cui l’invio di e-mail all’acquirente, l’esecuzione dell’ordine (spedizione), l’emissione di crediti/rimborsi, l’aggiunta di commenti e altro ancora. Per gestire gli ordini di Amazon, [**Importa ordini Amazon**](./order-settings.md) deve essere impostato su `Enabled` in modo che corrisponda [!DNL Commerce] gli ordini vengono creati quando si ricevono gli ordini di Amazon. Le informazioni sull’ordine di Amazon vengono visualizzate nel *[!UICONTROL Recent Orders]* sezione del dashboard del negozio.

Se attivato, corrisponde a [!DNL Commerce] vengono creati gli ordini per gli ordini di Amazon e il numero di ordine di Amazon viene visualizzato nel _[!UICONTROL Order Number]_colonna. Se un corrispondente [!DNL Commerce] dell&#39;ordine, fare clic sul numero dell&#39;ordine per aprire l&#39;ordine in [Elaborazione ordini commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) pagina. Puoi gestire l’ordine come fai con gli altri [[!DNL Commerce] elaborazione dell’ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

Il [!DNL Commerce] il numero dell&#39;ordine non viene visualizzato con _[!UICONTROL Recent Orders]_informazioni. Il numero di ordine di Commerce viene visualizzato solo quando si fa clic sul numero di ordine nel dashboard del negozio e si apre l’ordine in [Elaborazione ordini commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). Quando si visualizza [!DNL Commerce] nell&#39;ordine, il numero dell&#39;ordine di Amazon viene visualizzato nel *[!UICONTROL Payment & Shipping Method]*sezione. Include inoltre le opzioni per *[!UICONTROL View or Cancel Amazon Order]*e *[!UICONTROL View all Amazon Orders]*, a seconda dello stato di spedizione dell&#39;ordine.

Consulta [annullare un ordine non spedito](./cancel-unshipped-order.md).

![Informazioni sull’ordine di Amazon nell’ordine Commerce](assets/amazon-order-number-payment-info.png){width="500"}

Durante l’elaborazione di un ordine Amazon, il canale di vendita Amazon aggiorna e sincronizza le informazioni sull’ordine con il [!DNL Amazon Seller Central] account. Le impostazioni cron determinano la frequenza con cui le informazioni sugli ordini vengono sincronizzate tra Amazon e il canale di vendita Amazon.

Common Commerce [elaborazione dell’ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) le attività includono:

- [Azioni ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Ricerca per ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Elabora un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [Visualizza un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [Elabora un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [Informazioni su ordini e account](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [Informazioni indirizzo](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [Metodo di pagamento e spedizione](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [Rivedi articoli ordinati](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Emissione di un accredito/rimborso](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [Esecuzione/spedizione di un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Crea una fattura](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Annulla un ordine non spedito](./cancel-unshipped-order.md)

>[!NOTE]
>
>Se un ordine è in `Unshipped` stato, è possibile [annullare un ordine Amazon](./cancel-unshipped-order.md) il [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina. Se un ordine è stato spedito, non può essere annullato.

Consulta [Gestione ordini Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
