---
title: Annullare un ordine non spedito
description: Annulla un ordine in sospeso o parzialmente spedito (non spedito) tramite il tuo account Amazon [!DNL Seller Central] .
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Annullare un ordine non spedito

Gli ordini Amazon possono essere annullati solo se sono nello stato `Unshipped` . Se l&#39;ordine è in sospeso o parzialmente spedito (non spedito), l&#39;ordine può essere annullato solo tramite il tuo account [!DNL Amazon Seller Central]. Se l&#39;articolo è stato spedito, i resi e gli scambi devono essere gestiti anche nel tuo account [!DNL Amazon Seller Central].

>[!NOTE]
>
>Per attività diverse dall&#39;annullamento di un ordine:
>
>- Se è abilitato [order import](./order-settings.md), gli ordini vengono gestiti nel flusso di lavoro [[!DNL Commerce] ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.
>- Se [order import](./order-settings.md) è disattivato, è necessario gestire gli ordini in [!DNL Amazon Seller Central].


## Annullare un ordine nello stato `Unshipped`

1. Fai clic su **[!UICONTROL View Store]** nella scheda del negozio.

1. Nella sezione _[!UICONTROL Recent Orders]_del dashboard dell&#39;archivio fare clic su un numero di ordine.

   Viene visualizzata la pagina _[!UICONTROL Amazon Order Details]_.

1. Fai clic su **[!UICONTROL Cancel Order]** nella barra dell’intestazione.

   Questa opzione viene visualizzata solo per gli ordini nello stato `Unshipped` .

1. Per **[!UICONTROL Reason for cancellation]**, scegli un’opzione.

1. Fare clic su **[!UICONTROL Confirm]**.

   L&#39;ordine viene annullato e lo stato viene aggiornato a `Canceled` nei dettagli dell&#39;ordine.

La notifica di annullamento viene inviata al tuo account [!DNL Amazon Seller Central] e anche il cliente associato all&#39;ordine viene informato. Lo stato dell&#39;eventuale ordine [!DNL Commerce] corrispondente cambia in `Complete`.
