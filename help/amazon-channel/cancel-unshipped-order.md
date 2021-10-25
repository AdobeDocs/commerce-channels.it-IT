---
title: Annullare un ordine non spedito
description: Annullare un ordine in sospeso o parzialmente spedito (non spedito) tramite il tuo Amazon [!DNL Seller Central] conto.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Annullare un ordine non spedito

Gli ordini di Amazon possono essere annullati solo se si trovano in un `Unshipped` stato. Se l&#39;ordine è in sospeso o parzialmente spedito (non spedito), l&#39;ordine può essere annullato solo tramite il tuo [!DNL Amazon Seller Central] conto. Se l&#39;articolo è stato spedito, i ritorni e gli scambi devono essere gestiti anche nel tuo [!DNL Amazon Seller Central] Conto.

>[!NOTE]
>
>Per attività diverse dall&#39;annullamento di un ordine:
>
>- Se [importazione ordini](./order-settings.md) abilitato, gli ordini vengono gestiti nel [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.
>- Se [importazione ordini](./order-settings.md) è disattivato, è necessario gestire gli ordini in [!DNL Amazon Seller Central].


## Annullare un ordine in `Unshipped` status

1. Fai clic su **[!UICONTROL View Store]** sulla scheda del negozio.

1. In _[!UICONTROL Recent Orders]_fare clic su un numero di ordine nella sezione del dashboard del negozio.

   La _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina .

1. Fai clic su **[!UICONTROL Cancel Order]** nella barra dell’intestazione.

   Questa opzione viene visualizzata solo per gli ordini in `Unshipped` stato.

1. Per **[!UICONTROL Reason for cancellation]**, scegli un’opzione.

1. Fai clic su **[!UICONTROL Confirm]**.

   L&#39;ordine viene annullato e lo stato viene aggiornato in `Canceled` nei dettagli dell&#39;ordine.

La notifica di cancellazione viene inviata al tuo [!DNL Amazon Seller Central] viene inoltre notificato l’account e il cliente associato all’ordine. Lo stato del corrispondente [!DNL Commerce] l&#39;eventuale modifica di `Complete`.
