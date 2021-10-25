---
title: Dettagli ordine Amazon
description: Visualizza i dettagli degli ordini di Amazon Marketplace in Adobe Commerce o nell’amministratore di Magento Open Source.
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Dettagli dell’ordine Amazon

![Dettagli dell’ordine Amazon](assets/amazon-order-details-header.png)

## Visualizza dettagli ordine Amazon

1. Fai clic su **[!UICONTROL View Store]** sulla scheda del negozio.

1. In _[!UICONTROL Recent Orders]_fare clic su un numero di ordine.

   La _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina .

>[!NOTE]
>
>Se l’importazione dell’ordine è abilitata nella [Impostazioni ordine](./order-settings.md) e l&#39;ordine è [soddisfatto da Amazon (FBA)](./fulfilled-by.md), potrebbero essere visualizzati dati fittizi per alcuni campi nei dettagli dell’ordine. Amazon non invia i seguenti dati per gli ordini FBA.
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

La _[!UICONTROL Order and Shipping Details]_La scheda mostra informazioni dettagliate sull’ordine, come ricevuto da Amazon.

>[!IMPORTANT]
>
>Amazon accetta informazioni sull’indirizzo non standard che non possono essere importate nel canale di vendita Amazon, impedendo in tal modo l’aggiornamento corretto dei codici di stato/paese per alcuni ordini. Per correggere gli errori di indirizzo, i campi seguenti sono modificabili nei dettagli dell’ordine:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`

>
>Non dimenticare di fare clic **Salva ordine** dopo aver apportato le modifiche.

![Dettagli ordine e spedizione](assets/amazon-order-details.png)

### Scheda Articoli ordine

La _[!UICONTROL Order Items]_La scheda mostra tutti gli elementi associati all’ordine Amazon, come ricevuti da Amazon.

![Dettagli articolo ordine](assets/amazon-order-item-details.png)

### Scheda Tracking

La _[!UICONTROL Tracking]_La scheda mostra le informazioni di tracciamento associate all’ordine Amazon.

![Dettagli di tracciamento](assets/amazon-order-tracking-details.png)
