---
title: Attività comuni di elaborazione degli ordini in Amazon
description: Utilizza i  [!DNL Commerce]  ordini corrispondenti creati per gli ordini di Amazon per gestire l'attività e l'elaborazione degli ordini nell'amministratore [!UICONTROL Commerce].
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Attività comuni di elaborazione degli ordini in Amazon

[Elaborazione ordini Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) può gestire gli ordini Amazon, inclusi l&#39;invio di e-mail all&#39;acquirente, l&#39;evasione dell&#39;ordine (spedizione), l&#39;emissione di crediti/rimborsi, l&#39;aggiunta di commenti e altro ancora. Per gestire gli ordini Amazon, l&#39;impostazione [**Importa ordini Amazon**](./order-settings.md) deve essere impostata su `Enabled` in modo che vengano creati [!DNL Commerce] ordini corrispondenti al momento della ricezione degli ordini Amazon. Le informazioni sull&#39;ordine di Amazon vengono visualizzate nella sezione *[!UICONTROL Recent Orders]* del dashboard dello store.

Quando questa opzione è attivata, vengono creati [!DNL Commerce] ordini corrispondenti per gli ordini Amazon e il numero di ordine Amazon viene visualizzato nella colonna _[!UICONTROL Order Number]_. Se viene creato un ordine [!DNL Commerce] corrispondente, fare clic sul numero dell&#39;ordine per aprirlo nella pagina [Elaborazione ordine Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). Puoi gestire l&#39;ordine come gli altri [[!DNL Commerce] ordini in elaborazione](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

Il numero di ordine [!DNL Commerce] non viene visualizzato con le informazioni _[!UICONTROL Recent Orders]_. Il numero di ordine di Commerce viene visualizzato solo quando si fa clic sul numero di ordine nel dashboard del negozio e si apre l&#39;ordine in [Elaborazione ordine di Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). Quando si visualizza l&#39;ordine [!DNL Commerce], il numero dell&#39;ordine Amazon viene visualizzato nella sezione *[!UICONTROL Payment & Shipping Method]*. Include inoltre opzioni per *[!UICONTROL View or Cancel Amazon Order]*e *[!UICONTROL View all Amazon Orders]*, a seconda dello stato di spedizione dell&#39;ordine.

Vedere [annullare un ordine non spedito](./cancel-unshipped-order.md).

![Informazioni ordine Amazon nell&#39;ordine Commerce](assets/amazon-order-number-payment-info.png){width="500"}

Durante l&#39;elaborazione di un ordine Amazon, il canale di vendita Amazon aggiorna e sincronizza le informazioni sull&#39;ordine con l&#39;account [!DNL Amazon Seller Central]. Le impostazioni cron determinano la frequenza con cui le informazioni sugli ordini vengono sincronizzate tra Amazon e il canale di vendita Amazon.

Le [attività comuni di elaborazione ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) di Commerce includono:

- [Azioni ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Ricerca per ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Elabora un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [Visualizza un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [Elabora un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [Informazioni su ordini e account](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [Informazioni indirizzo](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [Metodo di pagamento e spedizione](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [Rivedi elementi ordinati](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Emissione di un credito/rimborso](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [evasione/spedizione di un ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Crea una fattura](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Annulla un ordine non spedito](./cancel-unshipped-order.md)

>[!NOTE]
>
>Se un ordine è nello stato `Unshipped`, è possibile [annullare un ordine Amazon](./cancel-unshipped-order.md) nella pagina [[!UICONTROL Amazon Order Details]](./amazon-order-details.md). Se un ordine è stato spedito, non può essere annullato.

Consulta [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
