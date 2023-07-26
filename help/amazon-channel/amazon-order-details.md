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

1. Clic **[!UICONTROL View Store]** sulla scheda del negozio.

1. In _[!UICONTROL Recent Orders]_, fare clic su un numero d&#39;ordine.

   Il _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina.

>[!NOTE]
>
>Se l’importazione degli ordini è abilitata nel [Impostazioni ordine](./order-settings.md) e l’ordine è [soddisfatto da Amazon (FBA)](./fulfilled-by.md), è possibile che vengano visualizzati dati fittizi per alcuni campi nei dettagli dell&#39;ordine. Amazon non invia i seguenti dati per gli ordini FBA.
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

Il _[!UICONTROL Order and Shipping Details]_Questa scheda mostra informazioni dettagliate sull’ordine, così come ricevute da Amazon.

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

Il _[!UICONTROL Order Items]_Questa scheda mostra tutti gli elementi associati all’ordine di Amazon, così come sono stati ricevuti da Amazon.

![Dettagli articolo ordine](assets/amazon-order-item-details.png){width="600" zoomable="yes"}

### Scheda Tracciamento

Il _[!UICONTROL Tracking]_Questa scheda mostra le informazioni di tracciamento associate all’ordine Amazon.

![Dettagli di tracciamento](assets/amazon-order-tracking-details.png){width="600" zoomable="yes"}
