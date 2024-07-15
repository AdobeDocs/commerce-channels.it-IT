---
title: Mappa vettori di spedizione
description: 'Mappa attributi per corrispondenza [DNL! Commerce] prodotti alle  [!DNL Walmart Marketplace] inserzioni esistenti e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart].'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Mappa vettori di spedizione

Prima di [elaborare spedizioni ordini](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappare i vettori di spedizione preferiti di Walmart al vettore corrispondente in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I gestori Commerce che non eseguono il mapping a un gestore preferito sono etichettati come *[!UICONTROL Other Carrier]* il [!DNL Walmart].

**Prerequisiti**

Prima di effettuare la mappatura dei vettori di spedizione, effettuare le seguenti operazioni:

1. Rivedi [Metodi e best practice di spedizione per la consegna puntuale](https://sellerhelp.walmart.com/s/guide?article=000009473) per [!DNL Walmart Marketplace].

1. Verificare la configurazione di [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) e [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) nell&#39;archivio di [!DNL Commerce] per assicurarsi di aver ottimizzato la configurazione per [!DNL Walmart Marketplace sales].

## Mappa vettori di spedizione

1. Dalla pagina **[!UICONTROL Listings]** o **[!UICONTROL Orders]**, selezionare **[!UICONTROL Channel Settings]**.

1. In **[!UICONTROL Channel Settings]**, selezionare **[!UICONTROL Shipping Carriers]**.

   ![Mappa vettori di spedizione](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. Per ogni vettore preferito [!DNL Walmart] elencato, selezionare il nome del vettore [!DNL Commerce] dal menu a discesa se il vettore è disponibile.

1. Selezionare **[!UICONTROL Save]** per applicare la configurazione.

