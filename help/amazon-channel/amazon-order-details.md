---
title: Dettagli ordine Amazon
description: Visualizza i dettagli degli ordini di Amazon Marketplace in Adobe Commerce o nell’amministratore di Magento Open Source.
feature: Sales Channels, Orders
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Dettagli ordine Amazon

![Dettagli ordine Amazon](assets/amazon-order-details-header.png){width="600" zoomable="yes"}

## Visualizza dettagli ordine Amazon

1. Fare clic su **[!UICONTROL View Store]** sulla scheda dello store.

1. Nella sezione _[!UICONTROL Recent Orders]_fare clic su un numero di ordine.

   Verrà aperta la pagina _[!UICONTROL Amazon Order Details]_.

>[!NOTE]
>
>Se l&#39;importazione degli ordini è abilitata nelle [Impostazioni ordine](./order-settings.md) e l&#39;ordine è [evaso da Amazon (FBA)](./fulfilled-by.md), è possibile che nei dettagli dell&#39;ordine vengano visualizzati dati fittizi per alcuni campi. Amazon non invia i seguenti dati per gli ordini FBA.
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`

### Scheda Dettagli ordine e spedizione

La scheda _[!UICONTROL Order and Shipping Details]_mostra informazioni dettagliate sull&#39;ordine, così come ricevute da Amazon.

>[!IMPORTANT]
>
>Amazon accetta informazioni sull’indirizzo non standard che non possono essere importate nel canale di vendita Amazon, impedendo in tal modo l’aggiornamento corretto dei codici di stato/paese per alcuni ordini. Per correggere gli errori di indirizzo, è possibile modificare i campi seguenti nei dettagli dell&#39;ordine:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>Non dimenticare di fare clic su **Salva ordine** dopo aver apportato modifiche.

![Dettagli ordine e spedizione](assets/amazon-order-details.png){width="600" zoomable="yes"}

### Scheda Articoli ordine

La scheda _[!UICONTROL Order Items]_mostra tutti gli elementi associati all&#39;ordine Amazon, così come ricevuti da Amazon.

![Dettagli elemento ordine](assets/amazon-order-item-details.png){width="600" zoomable="yes"}

### Scheda Tracciamento

La scheda _[!UICONTROL Tracking]_mostra le informazioni di tracciamento associate all&#39;ordine Amazon.

![Dettagli di tracciamento](assets/amazon-order-tracking-details.png){width="600" zoomable="yes"}
