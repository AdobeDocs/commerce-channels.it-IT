---
title: Gestisci connessione a Walmart Marketplace
description: '"Aggiornare le credenziali API per autorizzare la connessione tra un [DNL! Commerce] visualizza store e  [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] inserzioni prodotti e sincronizza i dati di inventario, prezzo, ordine e spedizione tra [!DNL Commerce] e Walmart.'''
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Mappa vettori di spedizione

Prima di [elaborare spedizioni ordini](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappare i vettori di spedizione preferiti di Walmart al vettore corrispondente in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I gestori Commerce che non eseguono il mapping a un gestore preferito sono etichettati come *[!UICONTROL Other Carrier]* il [!DNL Walmart].

**Prerequisiti**

Rivedi [Requisiti Walmart](walmart-requirements.md) per [!DNL Marketplace Seller account].

## Aggiorna credenziali di connessione

1. Nella pagina [!UICONTROL Listings] per il negozio del canale di vendita, selezionare **[!UICONTROL Channel Settings]**.

1. In **[!UICONTROL Channel Settings]**, selezionare **[!UICONTROL Walmart Connection]**.

1. Per modificare le credenziali, selezionare **[!UICONTROL Change Credentials]**

   ![Aggiorna le credenziali API di Walmart per autorizzare la connessione](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. Immettere **[!UICONTROL Walmart Client ID]** e **[!UICONTROL Walmart Client Secret]**.

1. Selezionare **[!UICONTROL Save]** per applicare la configurazione.
