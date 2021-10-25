---
title: Attività di elaborazione ordine comune
description: Utilizza il corrispondente [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Amministratore.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Attività comuni di elaborazione degli ordini

[[!DNL Commerce] elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} può gestire i tuoi ordini Amazon, tra cui l&#39;invio di e-mail all&#39;acquirente, il rispetto dell&#39;ordine (spedizione), l&#39;emissione di crediti/rimborsi, l&#39;aggiunta di commenti e altro ancora. Per gestire i tuoi ordini Amazon, [**Importa ordini Amazon**](./order-settings.md) deve essere impostato su `Enabled` in modo che [!DNL Commerce] Gli ordini vengono creati quando vengono ricevuti gli ordini di Amazon. Le informazioni sull’ordine di Amazon vengono visualizzate nella *[!UICONTROL Recent Orders]* della dashboard del negozio.

Quando abilitato, corrisponde [!DNL Commerce] gli ordini vengono creati per gli ordini Amazon e il numero di ordine Amazon viene visualizzato nella _[!UICONTROL Order Number]_colonna. Se [!DNL Commerce] l&#39;ordine viene creato, fare clic sul numero dell&#39;ordine per aprire l&#39;ordine nel [!DNL Commerce] [elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html)pagina {target=&quot;_blank&quot;}. Puoi gestire l&#39;ordine come fai con gli altri [[!DNL Commerce] elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

La [!DNL Commerce] il numero dell&#39;ordine non viene visualizzato con _[!UICONTROL Recent Orders]_informazioni. La [!DNL Commerce] il numero dell&#39;ordine viene visualizzato solo quando si fa clic sul numero dell&#39;ordine sul dashboard del negozio e si apre l&#39;ordine in [[!DNL Commerce] elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. Quando visualizzi la [!DNL Commerce] nell’ordine, il numero dell’ordine di Amazon viene visualizzato nella *[!UICONTROL Payment & Shipping Method]*sezione . Include inoltre le opzioni per *[!UICONTROL View or Cancel Amazon Order]*e *[!UICONTROL View all Amazon Orders]*, a seconda dello stato di spedizione dell’ordine.

Vedi [annullare un ordine non spedito](./cancel-unshipped-order.md).

![Informazioni ordine Amazon nell’ordine Commerce](assets/amazon-order-number-payment-info.png)

Durante l&#39;elaborazione di un ordine Amazon, il canale di vendita Amazon aggiorna e sincronizza le informazioni sull&#39;ordine con il tuo [!DNL Amazon Seller Central] conto. Le impostazioni cron determinano la frequenza con cui le informazioni sull’ordine vengono sincronizzate tra il canale di vendita Amazon e Amazon.

Comune [!DNL Commerce] [elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} attività includono:

- [Azioni ordine](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [Ricerca ordini](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Elaborazione di un ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [Visualizzare un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [Elaborazione di un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [Informazioni sull&#39;ordine e sull&#39;account](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Informazioni indirizzo](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Metodo di pagamento e spedizione](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [Articoli di revisione ordinati](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [Emissione di un credito/rimborso](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [Soddisfare/spedire un ordine](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [Crea una fattura](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [Annullare un ordine non spedito](./cancel-unshipped-order.md)

>[!NOTE]
>
>Se un ordine è in `Unshipped` stato, è possibile [annullare un ordine Amazon](./cancel-unshipped-order.md) sulla [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) pagina. Se un ordine è stato spedito, non può essere annullato.

Vedi [Gestione ordini di Commerce](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
