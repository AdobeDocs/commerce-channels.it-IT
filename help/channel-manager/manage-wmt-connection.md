---
title: Gestire la connessione a Marketplace Walmart
description: '''Aggiorna le credenziali API per autorizzare la connessione tra un [DNL! Commerce] e la vista Store e [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] elenchi dei prodotti e sincronizza i dati di inventario, prezzo, ordine e spedizione tra [!DNL Commerce] e il Walmart."'
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Mappa vettori di spedizione

Prima di [spedizioni di ordini di elaborazione](process-orders.md#ship-an-order) per [!DNL Walmart Marketplace] ordini, mappare i vettori di spedizione preferiti Walmart al corrispondente vettore in [!DNL Commerce] in modo che i dati di spedizione possano essere sincronizzati tra [!DNL Walmart] e [!DNL Commerce].

I vettori commerciali che non si mappano a un vettore preferito sono etichettati come *[!UICONTROL Other Carrier]* su [!DNL Walmart].

**Prerequisiti**

Revisione [Requisiti di Walmart](walmart-requirements.md) per [!DNL Marketplace Seller account].

## Aggiorna credenziali di connessione

1. Sulla [!UICONTROL Listings] pagina per l&#39;archivio canali di vendita, seleziona **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, seleziona **[!UICONTROL Walmart Connection]**.

1. Per modificare le credenziali, seleziona **[!UICONTROL Change Credentials]**

   ![Aggiornare le credenziali API di Walmart per autorizzare la connessione](assets/update-connection-credentials.png)

1. Inserisci il **[!UICONTROL Walmart Client ID]** e **[!UICONTROL Walmart Client Secret]**.

1. Seleziona **[!UICONTROL Save]** per applicare la configurazione.
