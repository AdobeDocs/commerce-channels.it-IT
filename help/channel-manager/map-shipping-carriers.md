---
title: Mappa delle navi
description: Mappa gli attributi per la corrispondenza [DNL! Prodotti Commerce a quelli esistenti [!DNL Walmart Marketplace] elenchi e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart].
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: e8c3fdc912b1e7ee4960a9a6ff66a2c9968f34f0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Mappa delle navi

Prima di [spedizioni di ordini di elaborazione](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappare i vettori di spedizione preferiti Walmart al corrispondente vettore in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I vettori commerciali che non si mappano a un vettore preferito sono etichettati come *[!UICONTROL Other Carrier]* a Walmart.

**Prerequisiti**

Prima di mappare i vettori di spedizione, completare le seguenti attività:

1. Consulta la sezione [Metodi di trasporto e best practice di spedizione per la consegna puntuale](https://sellerhelp.walmart.com/s/guide?article=000009473) per Walmart Marketplace.

1. Verifica la [[!UICONTROL Shipping Carrier]](https://docs.magento.com/user-guide/shipping/carriers.html) e [!UICONTROL Shipping Settings] nella configurazione [!DNL Commerce] per assicurarti di aver ottimizzato la configurazione per [!DNL Walmart Marketplace sales].

## Mappa delle navi

1. Sulla [!UICONTROL Listings] pagina per l&#39;archivio canali di vendita, seleziona **[!UICONTROL Settings]**.

1. Da *[!UICONTROL Map Attributes], seleziona **[!UICONTROL Shipping Carriers].

   ![Mappa delle navi](assets/map-shipping-carriers.png)

1. Per ogni [!DNL Walmart] vettore preferito elencato, selezionare [!DNL Commerce] nome del vettore dal menu a discesa, se il vettore è disponibile.

1. Seleziona **[!UICONTROL Save]** per applicare la configurazione.
