---
title: 'Visualizza e gestisci ordini da [!DNL Channel Manager]'
description: 'Visualizza e gestisci [!DNL Walmart Marketplace] ordini con [!DNL Channel Manager] per Adobe Commerce e Magento Open Source.'
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# Visualizza e traccia ordini da [!DNL Channel Manager]

I dati dell&#39;ordine [!DNL Walmart Marketplace] per i prodotti [!DNL Commerce] vengono sincronizzati automaticamente con [!DNL Channel Manager] dopo che [!DNL Walmart] elabora l&#39;ordine.

Sul lato [!DNL Commerce], una sincronizzazione riuscita attiva le azioni seguenti:

- [!DNL Channel Manager] invia una conferma dell&#39;ordine a Walmart.

- Un ordine [!DNL Commerce] corrispondente viene creato dall&#39;ordine Walmart.

- Le informazioni aggiornate sull&#39;ordine vengono visualizzate nel dashboard Ordini [!DNL Channel Manager].

Nell&#39;amministratore della vetrina è possibile visualizzare i dati dell&#39;ordine da [!DNL Channel Manager] aprendo lo store dei canali di vendita e selezionando **[!UICONTROL Orders]**.

![Visualizzazione ordini di Channel Manager per gestire [!DNL Walmart Marketplace] ordini](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>La visualizzazione di un ordine [!DNL Walmart Marketplace] nell&#39;elenco ordini [!DNL Channel Manager] può richiedere fino a 35 minuti. [!DNL Walmart] richiede circa 30 minuti per elaborare gli ordini in arrivo e inviarli a [!DNL Channel Manager]. Dopo aver ricevuto l’ordine, la creazione e la visualizzazione dell’ordine in Adobe Commerce o Magento Open Source richiede circa altri cinque minuti.

## Controlli degli ordini e descrizioni delle colonne

Nelle tabelle seguenti vengono descritti i controlli e le colonne disponibili per Ordini.

**Controlli per[!UICONTROL Orders]**

<table>
<tr>
<td><strong>Controllo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>Ordinare la visualizzazione selezionando una delle schede [!UICONTROL Order Status].</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Fornisce informazioni sugli errori degli ordini e sulle richieste di restituzione. Per visualizzare le informazioni sulla restituzione e lo stato del rimborso per un ordine, selezionare il testo <strong>[!UICONTROL Return requested]</strong> per aprire il dashboard [!UICONTROL Returns].</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell'ordine, selezionare il numero di ordine [!DNL Commerce] nella tabella [!UICONTROL Order]. Quindi utilizzare [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, selezionare le credenziali di connessione Walmart del canale, gli attributi mappati o gli identificatori di spedizione, le impostazioni selezionano il numero di ordine [!DNL Commerce] nella tabella [!UICONTROL Order]. Quindi utilizzare [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
</tr>
</table>


**Descrizioni colonne**

<table>
<tr>
<td>Campo</td>
<td>Descrizione</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>Numero dell'ordine di acquisto assegnato all'ordine in [!DNL Walmart Marketplace]. Quando un ordine viene inizialmente importato in [!DNL Channel Manager], viene visualizzato solo il numero di ordine [!DNL Walmart]. Quando viene creato l'ordine [!DNL Commerce], il numero di ordine [!DNL Walmart] viene memorizzato nell'attributo di prodotto [!UICONTROL External ID].</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>Numero assegnato all'ordine [!DNL Commerce] creato dall'ordine [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>Elementi</td>
<td>Numero di elementi ordinati il [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Costo totale degli articoli ordinati.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>Data in cui l'ordine è stato inviato a [!DNL Walmart Marketplace] convertita nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>La data in cui l'ordine deve essere spedito da per soddisfare i requisiti di [!DNL Walmart Marketplace] convertiti nel fuso orario locale.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>Data in cui l'ordine deve essere consegnato al cliente per soddisfare i requisiti [!DNL Walmart Marketplace] convertiti nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>Il [[!DNL Walmart Marketplace] metodo di spedizione](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 selezionato per l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Timestamp che indica l'ultimo aggiornamento dei dati dell'ordine in [!DNL Channel Manager] convertito nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indica lo stato dell'ordine corrente nel flusso di lavoro ordine [!DNL Commerce]. Lo stato iniziale di un ordine importato da [!DNL Walmart Marketplace] è _Open_. Ulteriori aggiornamenti dello stato si verificano quando [!DNL Commerce] ordini vengono elaborati e [!DNL Channel Manager] sincronizza correttamente gli aggiornamenti di spedizione, spedizione parziale e annullamento in [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Fornisce informazioni più dettagliate sugli ordini con errori o richieste di rimborso.</td>
</tr>
</table>

## Stato ordine

[!UICONTROL Order Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] ordini gestiti da Adobe Commerce o Magento Open Source. Gli aggiornamenti dello stato dell&#39;ordine si verificano quando [!DNL Channel Manager] riceve informazioni aggiornate sull&#39;ordine da [!DNL Walmart Marketplace] o dal sistema di ordini [!DNL Commerce]. Gli ordini possono avere i seguenti stati:

- **[!UICONTROL Shipped]** - Ordini spediti dall&#39;archivio [!DNL Commerce]. Quando l&#39;ordine viene spedito, [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione su Walmart e fornire il numero di registrazione dell&#39;ordine per la spedizione. Dopo la spedizione di un ordine, gli articoli dell&#39;ordine possono essere parzialmente o completamente rimborsati se Walmart emette un modulo di autorizzazione per la restituzione del materiale promozionale. Vedi [Restituzioni e rimborsi](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]** - Ordini con alcuni articoli contrassegnati come spediti e altri in attesa di spedizione. Quando gli articoli vengono spediti, [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione a _[!DNL Partially Shipped]_su Walmart e fornisce il numero di registrazione dell&#39;ordine per la spedizione.

- **[!UICONTROL Canceled]** - Ordini annullati dall&#39;archivio [!DNL Commerce].

  Al termine dell&#39;annullamento dell&#39;ordine, la quantità di magazzino [!DNL Commerce] viene aggiornata per riflettere gli articoli restituiti. Quindi, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]** - Se Walmart Marketplace richiede una restituzione per gli articoli dell&#39;ordine spediti, nella colonna [!UICONTROL Status details] viene visualizzato un collegamento `Return requested`. Selezionando il collegamento si apre il dashboard [!UICONTROL Returns] per visualizzare la restituzione e gestire il processo di rimborso.

- **[!UICONTROL Error]** - Ordini con errori. Possono verificarsi errori quando un&#39;operazione di aggiornamento dell&#39;ordine non riesce. Ad esempio, si verificano errori se [!DNL Channel Manager] non può ricevere un nuovo ordine da Walmart. Possono verificarsi anche se [!DNL Channel Manager] non è in grado di inviare un aggiornamento di spedizione o annullamento dell&#39;ordine a [!DNL Walmart Marketplace]. Se un&#39;operazione non riesce, nella pagina Ordini viene visualizzato lo stato _Errore_ per l&#39;ordine. Per informazioni dettagliate, vedere [Correggere gli errori dell&#39;ordine](process-orders.md#fix-shipping-and-cancel-errors).

- **[!UICONTROL Status details]** - Fornisce ulteriori informazioni sugli errori dell&#39;ordine che si verificano a causa di problemi quali informazioni mancanti o valori non validi, dettagli di spedizione errati o annullamento dell&#39;ordine non riuscito. La descrizione consente di determinare se si è verificato un errore nell&#39;istanza [!DNL Commerce] o in [!DNL Walmart Marketplace].

>[!NOTE]
>
>Se gli articoli dell&#39;ordine vengono inviati in più spedizioni, lo stato dell&#39;ordine in [!DNL Channel Manager] riflette l&#39;ultimo stato dell&#39;ordine disponibile. Ad esempio, se il primo elemento viene spedito e non vengono restituiti errori quando gli aggiornamenti dell&#39;ordine vengono sincronizzati con [!DNL Channel Manager] e [!DNL Walmart Marketplace], lo stato dell&#39;ordine [!DNL Channel Manager] è _[!UICONTROL Partially Shipped]_. Se viene spedito un secondo articolo e [!DNL Channel Manager] restituisce un errore, lo stato dell&#39;ordine viene aggiornato a_[!UICONTROL Error]_.

## Ordini di revisione

1. Dall&#39;amministratore, selezionare **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire la pagina [!UICONTROL Channel Manager Marketplace Stores].

1. Aprire la visualizzazione punto vendita selezionando l&#39;icona a forma di occhio in una riga della voce del negozio.

1. Per visualizzare le informazioni sull&#39;ordine, selezionare *[!UICONTROL *Orders]**.

1. Ottieni informazioni sull&#39;ordine e determina i passaggi successivi controllando la colonna **[Stato](#order-status)**.

## Rivedi dettagli ordine

Dopo aver ricevuto un ordine dal marketplace e importato nel tuo store dei canali di vendita, utilizza l&#39;ID ordine [!DNL Commerce] per visualizzare i dettagli dell&#39;ordine in Adobe Commerce.

Da **[!UICONTROL Orders]**, selezionare **[!UICONTROL Commerce Order Number]** per aprire i dettagli dell&#39;ordine [!DNL Commerce].

![Visualizzazione dettagli ordine Commerce per un ordine [!DNL Walmart Marketplace]](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

Nella vetrina Commerce, gli ordini importati da [!DNL Walmart Marketplace] contengono le seguenti informazioni aggiuntive:

- **Informazioni sul pagamento e metodo di spedizione**-Gli ordini importati da Walmart includono i seguenti valori per i campi di pagamento e spedizione:

   - **[!UICONTROL Offline Channel Payment]** - Indica che il pagamento dell&#39;ordine è elaborato offline da [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]** - Visualizza il numero di ordine [!DNL Walmart Marketplace].

   - **[!UICONTROL Channel Shipping - Value]**-Indica che le spese di spedizione sono gestite tramite [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]** - Questo campo viene visualizzato solo se un ordine importato da [!DNL Walmart Marketplace] è stato annullato. I motivi di annullamento includono:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Elementi ordinati** - In questa sezione vengono elencati gli elementi dell&#39;ordine in tutti gli ordini di Commerce. La colonna [!UICONTROL Qty] fornisce la cronologia dello stato per gli elementi dell&#39;ordine. Ad esempio, se un ordine è stato fatturato, spedito e rimborsato, è possibile visualizzare le transizioni di stato.

  ![Cronologia stato articoli ordinati dettagli ordine [!DNL Walmart Marketplace] ordini](assets/order-detail-status-history.png){width="600" zoomable="yes"}

Visualizzare i dettagli della fattura articolo e del rimborso selezionando le opzioni [!UICONTROL Invoice] e [!UICONTROL Credit Memo] dal menu di navigazione. È inoltre possibile accedere alla nota di credito direttamente dal dashboard [[!UICONTROL Returns]](return-refund-orders.md) nel proprio negozio del canale di vendita.
