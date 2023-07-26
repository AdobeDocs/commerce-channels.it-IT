---
title: Mappa vettori di spedizione
description: '''Mappa attributi per corrispondenza [DNL! Prodotti Commerce] a esistenti [!DNL Walmart Marketplace] elenchi e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart]."'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Mappa vettori di spedizione

Prima di [elabora spedizioni ordine](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappa i vettori di spedizione preferiti di Walmart al vettore corrispondente in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I vettori commerciali che non mappano su un vettore preferito sono etichettati come *[!UICONTROL Other Carrier]* il [!DNL Walmart].

**Prerequisiti**

Prima di effettuare la mappatura dei vettori di spedizione, effettuare le seguenti operazioni:

1. Rivedi [Metodi di trasporto e best practice per la consegna puntuale](https://sellerhelp.walmart.com/s/guide?article=000009473) per [!DNL Walmart Marketplace].

1. Verificare la [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) e [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) configurazione nel tuo [!DNL Commerce] archiviare per essere certi di aver ottimizzato la configurazione per [!DNL Walmart Marketplace sales].

## Mappa vettori di spedizione

1. Dalla sezione **[!UICONTROL Listings]** o **[!UICONTROL Orders]** pagina, seleziona **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, seleziona **[!UICONTROL Shipping Carriers]**.

   ![Mappa vettori di spedizione](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. Per ogni [!DNL Walmart] vettore preferito elencato, seleziona il [!DNL Commerce] nome del gestore dal menu a discesa, se il gestore è disponibile.

1. Seleziona **[!UICONTROL Save]** per applicare la configurazione.

