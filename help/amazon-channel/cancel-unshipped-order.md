---
title: Annulla un ordine non spedito
description: Annullare un ordine in sospeso o parzialmente spedito (non spedito) tramite Amazon [!DNL Seller Central] account.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Annulla un ordine non spedito

Gli ordini di Amazon possono essere annullati solo se si trovano in un `Unshipped` stato. Se l&#39;ordine è in sospeso o parzialmente spedito (non spedito), l&#39;ordine può essere annullato solo tramite [!DNL Amazon Seller Central] account. Se l&#39;oggetto è stato spedito, le restituzioni e gli scambi devono essere gestiti anche nel tuo [!DNL Amazon Seller Central] Account.

>[!NOTE]
>
>Per le attività diverse dall&#39;annullamento di un ordine:
>
>- Se è stato [importazione ordine](./order-settings.md) abilitato, gli ordini vengono gestiti in [[!DNL Commerce] flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}.
>- Se [importazione ordine](./order-settings.md) è disabilitato, devi gestire i tuoi ordini in [!DNL Amazon Seller Central].


## Annullare un ordine in `Unshipped` stato

1. Clic **[!UICONTROL View Store]** sulla scheda del negozio.

1. In _[!UICONTROL Recent Orders]_sezione del dashboard del negozio, fai clic su un numero di ordine.

   Il _[!UICONTROL Amazon Order Details]_viene visualizzata.

1. Clic **[!UICONTROL Cancel Order]** nella barra dell’intestazione.

   Questa opzione è disponibile solo per gli ordini in `Unshipped` stato.

1. Per **[!UICONTROL Reason for cancellation]**, scegli un’opzione.

1. Clic **[!UICONTROL Confirm]**.

   L’ordine viene annullato e lo stato viene aggiornato a `Canceled` nei dettagli dell’ordine.

La notifica di cancellazione viene inviata al tuo indirizzo [!DNL Amazon Seller Central] e il cliente associato all&#39;ordine. Stato del corrispondente [!DNL Commerce] l&#39;ordine, se del caso, delle modifiche `Complete`.
