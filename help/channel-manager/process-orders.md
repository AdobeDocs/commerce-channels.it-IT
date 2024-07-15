---
title: Elabora ordini
description: '''Istruzioni per la spedizione e l''annullamento [!DNL Walmart Marketplace] di ordini da Adobe Commerce e Magento Open Source.'''
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Elabora ordini

Dopo la conferma e l&#39;invio di [!DNL Walmart Marketplace] ordini a [!DNL Channel Manager], si utilizza [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) per elaborare l&#39;ordine.

Channel Manager sincronizza gli aggiornamenti in [!DNL Walmart Marketplace] per assicurarsi che lo stato dell&#39;ordine e le informazioni di spedizione da [!DNL Commerce] corrispondano ai dati tracciati in [!DNL Walmart Marketplace].

* **Per ordinare spedizioni**-Walmart è necessario un numero di registrazione per tutte le spedizioni. Se alcuni articoli sono esauriti, puoi creare spedizioni parziali per inviare gli articoli attualmente disponibili. Dopo l&#39;invio della spedizione, gli aggiornamenti degli ordini vengono sincronizzati con [!DNL Walmart Marketplace]. Quindi, Walmart avvisa i clienti dello stato dell&#39;ordine e dei dettagli di spedizione.

* **Annullamenti ordini**-Quando si annulla un ordine [!DNL Walmart Marketplace], Walmart richiede un motivo di annullamento incluso nell&#39;avviso di annullamento dell&#39;ordine inviato al cliente. Il motivo dell&#39;annullamento viene visualizzato anche nelle informazioni sui pagamenti dell&#39;ordine di [!DNL Commerce]. Dopo l&#39;invio dell&#39;annullamento, gli aggiornamenti dell&#39;inventario vengono sincronizzati con [!DNL Walmart Marketplace]. Quindi, Walmart avvisa i clienti dello stato dell&#39;ordine e dei dettagli di spedizione.

  Nella vetrina, devi annullare l’intero ordine. [!DNL Commerce] non consente annullamenti parziali.

* **Richiesta di rimborso**-Se per un ordine spedito è richiesta una restituzione di Walmart Marketplace, [!UICONTROL Status details] include un collegamento alla restituzione. I resi e i rimborsi sono gestiti dal dashboard [Restituzioni](return-refund-orders.md).

Quando gli ordini Commerce vengono elaborati e [!DNL Channel Manager] sincronizza correttamente gli aggiornamenti di spedizione, spedizione parziale e annullamento in [!DNL Walmart Marketplace], l&#39;elaborazione dell&#39;ordine è completata. Le richieste di restituzione e i rimborsi per gli ordini spediti vengono gestiti dal dashboard [Restituzioni](return-refund-orders.md).

>[!NOTE]
>
> La sincronizzazione degli aggiornamenti dell&#39;ordine in [!DNL Walmart Marketplace] può richiedere fino a cinque minuti. Per verificare lo stato dell&#39;ordine, tornare alla pagina Ordini [!DNL Channel Manager].

## Spedisci un ordine

1. Dall&#39;amministratore, selezionare **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare **[!UICONTROL Orders]**.

1. Nella tabella Ordini aprire l&#39;ordine da spedire selezionando **[!UICONTROL Commerce Order Number]**.

1. Creare e inviare una spedizione per un ordine o parte di esso selezionando **[!UICONTROL Ship]**.

   ![Visualizzazione dettagli ordine Commerce per un ordine [!DNL Walmart Marketplace]](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Scegliere un vettore e aggiungere un numero di registrazione selezionando **[!UICONTROL Add tracking number]**.

     ![Visualizzazione dettagli ordine Commerce per un ordine [!DNL Walmart Marketplace]](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Compilare il resto del modulo di spedizione in base alle esigenze. Per istruzioni dettagliate, vedere [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html).

1. Dopo l&#39;invio della spedizione, tenere traccia dello stato [dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

Dopo la spedizione di un ordine, è possibile elaborare rimborsi completi o parziali da [!DNL Channel Manager] per gli articoli inclusi nell&#39;ordine in base alle richieste di restituzione ricevute da [!DNL Walmart Marketplace]. Vedi [Ordini di reso e rimborso](return-refund-orders.md).

## Annullare un ordine

1. Dall&#39;amministratore, selezionare **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

1. Per visualizzare [!DNL Walmart Marketplace] ordini, selezionare *[!UICONTROL Orders]**.

1. Nella tabella Ordini aprire la [pagina dei dettagli dell&#39;ordine](manage-orders.md#view-order-detail) selezionando **[!UICONTROL Commerce Order Number]** per l&#39;ordine da annullare.

   ![Visualizzazione dettagli ordine Commerce per un[!DNL Walmart Marketplace]ordine](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Annulla l’ordine.

   * Selezionare **Annulla** dal menu Dettagli ordine.

   * Nel modulo [!UICONTROL Cancel Order], selezionare **[!UICONTROL Cancellation reason]**.

   ![Visualizzazione dettagli ordine Commerce per un ordine [!DNL Walmart Marketplace]](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Selezionare **[!UICONTROL Cancel Order]**.

1. Dopo aver inviato l&#39;annullamento, tenere traccia dello stato [dell&#39;ordine](manage-orders.md#about-order-status) in [!DNL Channel Manager] per verificare che gli aggiornamenti siano stati inviati a [!DNL Walmart Marketplace].

## Correggi errori ordine

Gli errori possono verificarsi durante il processo di sincronizzazione degli ordini da [!DNL Walmart Marketplace] o durante il processo di aggiornamento degli ordini per spedizioni, spedizioni parziali e annullamenti.

Se l&#39;operazione di sincronizzazione per un aggiornamento di spedizione, spedizione parziale o annullamento non riesce, nella pagina Ordini [!DNL Channel Manager] viene visualizzato lo stato _Errore_ per l&#39;ordine. Per garantire che le informazioni relative alla spedizione e all&#39;annullamento dell&#39;ordine vengano riportate correttamente nell&#39;account di Walmart Marketplace, aggiornare manualmente l&#39;ordine nell&#39;archivio [!DNL Walmart Marketplace].


