---
title: Gestisci connessione a Walmart Marketplace
description: '"Aggiornare le credenziali API per autorizzare la connessione tra un [DNL! Commerce] vista store e [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] elenchi di prodotti e sincronizzazione dei dati di inventario, prezzo, ordine e spedizione tra [!DNL Commerce] e il Walmart".'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Mappa vettori di spedizione

Prima di [elabora spedizioni ordine](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappa i vettori di spedizione preferiti di Walmart al vettore corrispondente in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I vettori commerciali che non mappano su un vettore preferito sono etichettati come *[!UICONTROL Other Carrier]* il [!DNL Walmart].

**Prerequisiti**

Revisione [Requisiti Walmart](walmart-requirements.md) per [!DNL Marketplace Seller account].

## Aggiorna credenziali di connessione

1. Il giorno [!UICONTROL Listings] pagina per il negozio del canale di vendita, seleziona **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, seleziona **[!UICONTROL Walmart Connection]**.

1. Per modificare le credenziali, seleziona **[!UICONTROL Change Credentials]**

   ![Aggiorna le credenziali API di Walmart per autorizzare la connessione](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. Inserisci il **[!UICONTROL Walmart Client ID]** e **[!UICONTROL Walmart Client Secret]**.

1. Seleziona **[!UICONTROL Save]** per applicare la configurazione.
