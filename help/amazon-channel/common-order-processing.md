---
title: Attività di elaborazione ordine comune
description: Utilizza l'amministratore corrispondente [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Attività comuni di elaborazione degli ordini

[[!DNL Commerce] l&#39;elaborazione degli ordini](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} può gestire gli ordini Amazon, tra cui l&#39;invio tramite e-mail all&#39;acquirente, il rispetto dell&#39;ordine (spedizione), l&#39;emissione di crediti/rimborsi, l&#39;aggiunta di commenti e altro ancora. Per gestire gli ordini Amazon, l&#39;impostazione [**Importa ordini Amazon**](./order-settings.md) deve essere impostata su `Enabled` in modo che gli ordini [!DNL Commerce] corrispondenti vengano creati quando vengono ricevuti gli ordini Amazon. Le informazioni sull&#39;ordine di Amazon vengono visualizzate nella sezione *[!UICONTROL Recent Orders]* del dashboard del negozio.

Quando abilitato, gli ordini [!DNL Commerce] corrispondenti vengono creati per gli ordini Amazon e il numero di ordine Amazon viene visualizzato nella colonna _[!UICONTROL Order Number]_. Se viene creato un ordine [!DNL Commerce] corrispondente, fare clic sul numero dell&#39;ordine per aprire l&#39;ordine nella pagina [!DNL Commerce] [elaborazione ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. Puoi gestire l&#39;ordine come fai con l&#39;altra [[!DNL Commerce] elaborazione dell&#39;ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

Il numero dell&#39;ordine [!DNL Commerce] non viene visualizzato con le informazioni _[!UICONTROL Recent Orders]_. Il numero dell&#39;ordine [!DNL Commerce] viene visualizzato solo quando si fa clic sul numero dell&#39;ordine sul dashboard dell&#39;archivio e si apre l&#39;ordine in [[!DNL Commerce] elaborazione dell&#39;ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. Quando si visualizza l&#39;ordine [!DNL Commerce], il numero dell&#39;ordine Amazon viene visualizzato nella sezione *[!UICONTROL Payment & Shipping Method]*. Include inoltre opzioni per *[!UICONTROL View or Cancel Amazon Order]*e *[!UICONTROL View all Amazon Orders]*, a seconda dello stato di spedizione dell&#39;ordine.

Vedere [annullare un ordine non spedito](./cancel-unshipped-order.md).

![Informazioni ordine Amazon nell’ordine Commerce](assets/amazon-order-number-payment-info.png)

Durante l&#39;elaborazione di un ordine Amazon, il canale di vendita Amazon aggiorna e sincronizza le informazioni sull&#39;ordine con il tuo account [!DNL Amazon Seller Central]. Le impostazioni cron determinano la frequenza con cui le informazioni sull’ordine vengono sincronizzate tra il canale di vendita Amazon e Amazon.

Le attività comuni [!DNL Commerce] [elaborazione ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} includono:

- [Azioni ordine](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [Ricerca ordine](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Elabora un ordine](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [Visualizza un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [Elabora un ordine](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [Informazioni sull&#39;ordine e sull&#39;account](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Informazioni indirizzo](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Metodo](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method) di pagamento e spedizione{target=&quot;_blank&quot;}
   - [Rivedi gli articoli ordinati](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [Emissione di un credito/rimborso](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [Esecuzione/spedizione di un ordine](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [Crea una fattura](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [Annullare un ordine non spedito](./cancel-unshipped-order.md)

>[!NOTE]
>
>Se un ordine è nello stato `Unshipped`, è possibile [annullare un ordine Amazon](./cancel-unshipped-order.md) nella pagina [[!UICONTROL Amazon Order Details]](./amazon-order-details.md). Se un ordine è stato spedito, non può essere annullato.

Vedere [Gestione ordini di commercio](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
