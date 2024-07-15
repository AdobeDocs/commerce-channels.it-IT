---
title: Annulla un ordine Amazon non spedito
description: Annulla un ordine in sospeso o parzialmente spedito (non spedito) tramite il tuo account Amazon [!DNL Seller Central] .
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Annulla un ordine Amazon non spedito

Gli ordini di Amazon possono essere annullati solo se si trovano nello stato `Unshipped`. Se l&#39;ordine è in sospeso o parzialmente spedito (non spedito), è possibile annullarlo solo tramite il proprio account [!DNL Amazon Seller Central]. Se l&#39;oggetto è stato spedito, anche le restituzioni e gli scambi devono essere gestiti nell&#39;account [!DNL Amazon Seller Central].

>[!NOTE]
>
>Per le attività diverse dall&#39;annullamento di un ordine:
>
>- Se hai abilitato [importazione ordini](./order-settings.md), gli ordini vengono gestiti nel [[!DNL Commerce] flusso di lavoro ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).
>- Se [importazione ordini](./order-settings.md) è disabilitata, è necessario gestire gli ordini in [!DNL Amazon Seller Central].

## Annulla un ordine nello stato `Unshipped`

1. Fare clic su **[!UICONTROL View Store]** sulla scheda dello store.

1. Nella sezione _[!UICONTROL Recent Orders]_del dashboard dell&#39;archivio fare clic su un numero di ordine.

   Viene visualizzata la pagina _[!UICONTROL Amazon Order Details]_.

1. Fare clic su **[!UICONTROL Cancel Order]** nella barra dell&#39;intestazione.

   Questa opzione è disponibile solo per gli ordini con stato `Unshipped`.

1. Per **[!UICONTROL Reason for cancellation]**, scegliere un&#39;opzione.

1. Fare clic su **[!UICONTROL Confirm]**.

   L&#39;ordine è stato annullato e lo stato è aggiornato a `Canceled` nei dettagli dell&#39;ordine.

La notifica di annullamento viene inviata al tuo account [!DNL Amazon Seller Central] e viene inviata anche al cliente associato all&#39;ordine. Lo stato dell&#39;ordine [!DNL Commerce] corrispondente, se presente, cambia in `Complete`.
