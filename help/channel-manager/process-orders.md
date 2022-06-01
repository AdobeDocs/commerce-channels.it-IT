---
title: Elabora ordini
description: Istruzioni per la spedizione e l'annullamento [!DNL Walmart Marketplace] ordini da Adobe Commerce e Magenti Open Source.
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: f1c37111df2f566b9673946bb9b2b282506f990c
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Elabora ordini

Dopo [!DNL Walmart Marketplace] gli ordini sono stati riconosciuti e sono stati inviati con successo a [!DNL Channel Manager], utilizza [Gestione ordini di Commerce](https://docs.magento.com/user-guide/sales/orders-workspace.html) per elaborare l&#39;ordine.

Channel Manager sincronizza gli aggiornamenti di [!DNL Walmart Marketplace] per garantire che lo stato dell’ordine e le informazioni di spedizione da Commerce corrispondano ai dati tracciati nel [!DNL Walmart Marketplace].

* **Spedizioni ordine**-Walmart richiede un numero di registrazione per tutte le spedizioni. Se alcuni articoli sono esauriti, è possibile creare spedizioni parziali per inviare gli articoli attualmente disponibili. Dopo aver inviato la spedizione, gli aggiornamenti dell&#39;ordine vengono sincronizzati con [!DNL Walmart Marketplace]. Successivamente, Walmart comunica ai clienti lo stato dell&#39;ordine e i dettagli di spedizione.

* **Annullamento dell&#39;ordine**-Quando si annulla un [!DNL Walmart Marketplace] ordine, Walmart richiede un motivo di cancellazione che è incluso nell&#39;avviso di cancellazione dell&#39;ordine inviato al cliente. Il motivo dell&#39;annullamento viene visualizzato anche nel [!DNL Commerce] informazioni sui pagamenti degli ordini.

>[!NOTE]
>
> Gli aggiornamenti dell’ordine possono essere sincronizzati con [!DNL Walmart Marketplace]. Per controllare lo stato dell&#39;ordine, torna al [!DNL Channel Manager] Pagina Ordini.

## Spedire un ordine

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare *[!UICONTROL *Orders]**

1. Nella tabella Ordini aprire l&#39;ordine di spedizione selezionando la **Numero ordine di Commerce**.

1. Crea e invia una spedizione per tutto o parte un ordine selezionando **[!UICONTROL Ship]**.

   ![Visualizzazione dettagli ordine di Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-detail-with-external-order-id.png)

   * Scegliere un vettore di spedizione e aggiungere un numero di tracciamento selezionando **[!UICONTROL Add tracking number]**.

      ![Visualizzazione dettagli ordine di Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-shipment-add-tracking-number.png)


   * Compilare il resto del modulo di spedizione in base alle esigenze. Vedi [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) per istruzioni dettagliate.

1. Dopo aver sottomesso la spedizione, tenere traccia della [stato dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

## Annullare un ordine

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare *[!UICONTROL *Orders]**

1. Nella tabella Ordini aprire la pagina dei dettagli dell’ordine selezionando la **Numero ordine di Commerce** per l&#39;ordine di annullamento.

   ![Visualizzazione dettagli ordine di Commerce per un[!DNL Walmart Marketplace]ordine](assets/order-detail-with-external-order-id.png)

1. Annulla l&#39;ordine.

   * Seleziona **Annulla** dal menu Dettagli ordine.

   * Sulla [!UICONTROL Cancel Order] selezionare il modulo **Motivo dell&#39;annullamento**.
   ![Visualizzazione dettagli ordine di Commerce per un [!DNL Walmart Marketplace] ordine](assets/cancel-order-reason-selector.png)

   * Seleziona **Annulla ordine**.


1. Dopo aver inviato l&#39;annullamento, tieni traccia della [stato dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].
