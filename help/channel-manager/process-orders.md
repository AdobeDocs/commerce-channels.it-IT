---
title: Elabora ordini
description: Istruzioni per la spedizione e l'annullamento [!DNL Walmart Marketplace] ordini da Adobe Commerce e Magenti Open Source.
source-git-commit: 5670639697550b2d7fee67dd29be9c6278d5782b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Elabora ordini

Se utilizzi Adobe Commerce e Gestione ordini di Magento Open Source per gestire il tuo [!DNL Commerce] vendita negozio, processo [!DNL Walmart Marketplace] ordini da Commerce tramite un flusso di lavoro simile.

Quando si elabora un ordine in Commerce, Channel Manager sincronizza gli aggiornamenti di [!DNL Walmart Marketplace]. Questo aggiornamento assicura che l’inventario dei prodotti e lo stato dell’ordine di Commerce corrisponda ai dati tracciati nel [!DNL Walmart Marketplace] e comunica a Walmart di inviare informazioni sullo stato dell&#39;ordine e sulla spedizione ai clienti.

>[!NOTE]
>
> Gli aggiornamenti dell’ordine possono essere sincronizzati in fino a cinque minuti [!DNL Walmart Marketplace]. Per controllare lo stato dell&#39;ordine, torna a [!DNL Channel Manager] Ordini.

## Spedire un ordine

Quando invii un ordine da Commerce, utilizzi la funzione [[!DNL Commerce Order Management] flusso di lavoro di spedizione](https://docs.magento.com/user-guide/sales/order-ship.html). Dopo aver inviato l&#39;ordine, gli aggiornamenti vengono sincronizzati con [!DNL Walmart Marketplace]. Successivamente, Walmart comunica ai clienti lo stato dell&#39;ordine e i dettagli di spedizione.

**Prerequisito**

Prima degli ordini di spedizione, verifica che il [impostazioni di spedizione del canale e configurazione del vettore](map-shipping-carriers.md) incontro [!DNL Walmart Marketplace requirements].

### Creazione e invio della spedizione

Quando spedisci un [!DNL Walmart Marketplace] ordine da [!DNL Commerce], devi aggiungere un numero di tracciamento. I clienti ricevono il numero di registrazione nella notifica di spedizione da cui ricevono [!DNL Walmart].

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare *[!UICONTROL *Orders]**

1. Nella tabella Ordini aprire l&#39;ordine di spedizione selezionando la **Numero ordine di Commerce**.

1. Crea e invia una spedizione per tutto o parte un ordine selezionando **[!UICONTROL Ship]**.

   - Per scegliere un vettore di spedizione e aggiungere un numero di tracciamento, selezionare **[!UICONTROL Add tracking number]**.

   - Compilare il resto del modulo di spedizione in base alle esigenze. Vedi [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) per istruzioni dettagliate.

1. Dopo aver sottomesso la spedizione, tenere traccia della [stato dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

## Annullare un ordine

Quando si annulla un [!DNL Walmart Marketplace] ordine, Walmart richiede un motivo di cancellazione. Quando la cancellazione dell&#39;ordine si aggiorna a Walmart, il motivo della cancellazione è incluso nell&#39;avviso di cancellazione inviato al cliente.

Il motivo dell&#39;annullamento viene visualizzato anche nel [!DNL Commerce] informazioni sui pagamenti degli ordini.

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare *[!UICONTROL *Orders]**

1. Nella tabella Ordini aprire la pagina dei dettagli dell’ordine selezionando la **Numero ordine di Commerce** per l&#39;ordine di annullamento.

   ![Visualizzazione dettagli ordine di Commerce per un ordine Marketplace Walmart](assets/order-detail-with-external-order-id.png)

1. Annulla l&#39;ordine.

   - Seleziona **Annulla** dal menu Dettagli ordine.

   - Nel modulo Annulla ordine, seleziona la **Motivo dell&#39;annullamento**.

      ![Visualizzazione dettagli ordine di Commerce per un ordine Marketplace Walmart](assets/order-detail-with-external-order-id.png)

   - Seleziona **Annulla ordine**.

1. Verifica che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace] controllando [stato dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager].
