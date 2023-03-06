---
title: Attività comuni di elaborazione degli ordini
description: Utilizza il corrispondente [!DNL Commerce] ordini creati per gli ordini di Amazon per gestire l'attività e l'elaborazione degli ordini in [!UICONTROL Commerce] Amministratore
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Attività comuni di elaborazione degli ordini

[[!DNL Commerce] elaborazione dell’ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} può gestire i tuoi ordini Amazon, tra cui l’invio di e-mail all’acquirente, l’esecuzione dell’ordine (spedizione), l’emissione di crediti/rimborsi, l’aggiunta di commenti e altro ancora. Per gestire gli ordini di Amazon, [**Importa ordini Amazon**](./order-settings.md) deve essere impostato su `Enabled` in modo che corrisponda [!DNL Commerce] gli ordini vengono creati quando si ricevono gli ordini di Amazon. Le informazioni sull’ordine di Amazon vengono visualizzate nel *[!UICONTROL Recent Orders]* sezione del dashboard del negozio.

Se attivato, corrisponde a [!DNL Commerce] vengono creati gli ordini per gli ordini di Amazon e il numero di ordine di Amazon viene visualizzato nel _[!UICONTROL Order Number]_colonna. Se un corrispondente [!DNL Commerce] dell&#39;ordine, fare clic sul numero dell&#39;ordine per aprire l&#39;ordine in [!DNL Commerce] [elaborazione dell’ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

Il [!DNL Commerce] il numero dell&#39;ordine non viene visualizzato con _[!UICONTROL Recent Orders]_informazioni. Il [!DNL Commerce] numero ordine viene visualizzato solo quando si fa clic sul numero di ordine nel dashboard del negozio e si apre l&#39;ordine in [[!DNL Commerce] elaborazione dell’ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}. Quando si visualizza [!DNL Commerce] nell&#39;ordine, il numero dell&#39;ordine di Amazon viene visualizzato nel *[!UICONTROL Payment & Shipping Method]*sezione. Include inoltre le opzioni per *[!UICONTROL View or Cancel Amazon Order]*e *[!UICONTROL View all Amazon Orders]*, a seconda dello stato di spedizione dell&#39;ordine.

Consulta [annullare un ordine non spedito](./cancel-unshipped-order.md).

![Informazioni sull’ordine di Amazon nell’ordine Commerce](assets/amazon-order-number-payment-info.png)

Durante l’elaborazione di un ordine Amazon, il canale di vendita Amazon aggiorna e sincronizza le informazioni sull’ordine con il [!DNL Amazon Seller Central] account. Le impostazioni cron determinano la frequenza con cui le informazioni sugli ordini vengono sincronizzate tra Amazon e il canale di vendita Amazon.

Comune [!DNL Commerce] [elaborazione dell’ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} le attività includono:

- [Azioni ordine](https://docs.magento.com/user-guide/sales/order-actions.html){target="_blank"}
- [Ricerca per ordine](https://docs.magento.com/user-guide/sales/orders-search.html){target="_blank"}
- [Elabora un ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}
   - [Visualizza un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target="_blank"}
   - [Elabora un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target="_blank"}
   - [Informazioni su ordini e account](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target="_blank"}
   - [Informazioni indirizzo](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target="_blank"}
   - [Metodo di pagamento e spedizione](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target="_blank"}
   - [Rivedi articoli ordinati](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target="_blank"}
- [Emissione di un accredito/rimborso](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target="_blank"}
- [Esecuzione/spedizione di un ordine](https://docs.magento.com/user-guide/sales/shipments-create.html){target="_blank"}
- [Crea una fattura](https://docs.magento.com/user-guide/sales/invoice-create.html){target="_blank"}
- [Annulla un ordine non spedito](./cancel-unshipped-order.md)

>[!NOTE]
>
>Se un ordine è in `Unshipped` stato, è possibile [annullare un ordine Amazon](./cancel-unshipped-order.md) il [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina. Se un ordine è stato spedito, non può essere annullato.

Consulta [Gestione ordini Commerce](https://docs.magento.com/user-guide/sales/order-management.html){target="_blank"}.
