---
title: Elabora ordini
description: "Istruzioni per la spedizione e l'annullamento [!DNL Walmart Marketplace] ordini da Adobe Commerce e Magenti Open Source."
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Elabora ordini

Dopo [!DNL Walmart Marketplace] gli ordini sono stati confermati e inviati con successo a [!DNL Channel Manager], utilizza [Gestione ordini Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) per elaborare l&#39;ordine.

Channel Manager sincronizza gli aggiornamenti in [!DNL Walmart Marketplace] per garantire che lo stato dell&#39;ordine e le informazioni di spedizione [!DNL Commerce] corrisponde ai dati tracciati in [!DNL Walmart Marketplace].

* **Spedizioni ordine**-Walmart richiede un numero di registrazione per tutte le spedizioni. Se alcuni articoli sono esauriti, puoi creare spedizioni parziali per inviare gli articoli attualmente disponibili. Dopo aver sottomesso la spedizione, gli aggiornamenti dell&#39;ordine vengono sincronizzati con [!DNL Walmart Marketplace]. Quindi, Walmart avvisa i clienti dello stato dell&#39;ordine e dei dettagli di spedizione.

* **Annullamenti ordini**-Quando si annulla una [!DNL Walmart Marketplace] ordine, Walmart richiede un motivo di annullamento che è incluso nell&#39;avviso di annullamento dell&#39;ordine inviato al cliente. Il motivo dell’annullamento viene visualizzato anche nel [!DNL Commerce] informazioni sui pagamenti degli ordini. Dopo aver sottomesso l&#39;annullamento, gli aggiornamenti dell&#39;inventario vengono sincronizzati in [!DNL Walmart Marketplace]. Quindi, Walmart avvisa i clienti dello stato dell&#39;ordine e dei dettagli di spedizione.

   Nella vetrina, devi annullare l’intero ordine. [!DNL Commerce] non consente annullamenti parziali.

* **Richiesta di rimborso**-Se per un ordine spedito viene richiesta una restituzione di Walmart Marketplace, la [!UICONTROL Status details] include un collegamento al reso. I resi e i rimborsi sono gestiti dalla [Restituisce](return-refund-orders.md) dashboard.

Quando vengono elaborati gli ordini Commerce e [!DNL Channel Manager] sincronizza correttamente gli aggiornamenti di spedizione, spedizione parziale e annullamento in [!DNL Walmart Marketplace], l’elaborazione dell’ordine è stata completata. Le richieste di restituzione e i rimborsi per gli ordini spediti vengono gestiti dalla [Restituisce](return-refund-orders.md) dashboard.

>[!NOTE]
>
> La sincronizzazione degli aggiornamenti dell&#39;ordine con può richiedere fino a cinque minuti [!DNL Walmart Marketplace]. Per controllare lo stato dell&#39;ordine, tornare al [!DNL Channel Manager] Pagina Ordini.

## Spedisci un ordine

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, seleziona **[!UICONTROL Orders]**.

1. Nella tabella Ordini aprire l&#39;ordine da spedire selezionando l&#39;opzione **[!UICONTROL Commerce Order Number]**.

1. Creare e sottomettere una spedizione per tutto o parte di un ordine selezionando **[!UICONTROL Ship]**.

   ![Visualizzazione dettagli ordine Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Scegliere un vettore di spedizione e aggiungere un numero di registrazione selezionando **[!UICONTROL Add tracking number]**.

      ![Visualizzazione dettagli ordine Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Compilare il resto del modulo di spedizione in base alle esigenze. Consulta [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) per istruzioni dettagliate.

1. Dopo aver sottomesso la spedizione, tenere traccia della [stato ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

Dopo la spedizione di un ordine, è possibile elaborare rimborsi completi o parziali da [!DNL Channel Manager] per gli articoli inclusi nell&#39;ordine in base alle richieste di restituzione ricevute da [!DNL Walmart Marketplace]. Consulta [Ordini di reso e di rimborso](return-refund-orders.md).

## Annullare un ordine

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, seleziona *[!UICONTROL Orders]**.

1. Nella tabella Ordini aprire [pagina dettagli ordine](manage-orders.md#view-order-detail) selezionando la **[!UICONTROL Commerce Order Number]** per l’ordine da annullare.

   ![Visualizzazione dettagli ordine Commerce per un[!DNL Walmart Marketplace]ordine](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Annulla l’ordine.

   * Seleziona **Annulla** dal menu Dettagli ordine.

   * Il giorno [!UICONTROL Cancel Order] , selezionare il **[!UICONTROL Cancellation reason]**.
   ![Visualizzazione dettagli ordine Commerce per un [!DNL Walmart Marketplace] ordine](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Seleziona **[!UICONTROL Cancel Order]**.


1. Dopo aver inviato l’annullamento, tieni traccia di [stato ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

## Correggi errori ordine

È possibile che si verifichino errori durante il processo di sincronizzazione degli ordini da [!DNL Walmart Marketplace]oppure durante il processo di aggiornamento degli ordini per spedizioni, spedizioni parziali e annullamenti.

Se l&#39;operazione di sincronizzazione per una spedizione, una spedizione parziale o un aggiornamento dell&#39;annullamento ha esito negativo, il [!DNL Channel Manager] La pagina Ordini mostra un _Errore_ stato dell&#39;ordine. Per garantire che le informazioni relative alla spedizione e all&#39;annullamento dell&#39;ordine vengano riportate in modo accurato nel conto di Walmart Marketplace, aggiornare manualmente l&#39;ordine nel [!DNL Walmart Marketplace] archiviare.


