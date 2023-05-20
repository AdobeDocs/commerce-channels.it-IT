---
title: 'Visualizza e gestisci ordini da [!DNL Channel Manager]'
description: '''Visualizza e gestisci [!DNL Walmart Marketplace] ordini con [!DNL Channel Manager] per Adobe Commerce e Magenti Open Source."'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Visualizza e traccia ordini da [!DNL Channel Manager]

[!DNL Walmart Marketplace] dati ordine per [!DNL Commerce] prodotti sincronizzati automaticamente con [!DNL Channel Manager] dopo [!DNL Walmart] elabora l’ordine.

Il giorno [!DNL Commerce] una sincronizzazione corretta attiva le azioni seguenti:

- [!DNL Channel Manager] invia una conferma dell&#39;ordine a Walmart.

- Una corrispondente [!DNL Commerce] L&#39;ordine viene creato dall&#39;ordine Walmart.

- Le informazioni aggiornate sull’ordine vengono visualizzate nel [!DNL Channel Manager] Dashboard ordini.

Nell’amministratore della vetrina, puoi visualizzare i dati dell’ordine da [!DNL Channel Manager] aprendo il negozio del canale di vendita e selezionando **[!UICONTROL Orders]**.

![Visualizzazione Ordini di Channel Manager da gestire [!DNL Walmart Marketplace] ordini](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Possono essere necessari fino a 35 minuti per [!DNL Walmart Marketplace] ordine di visualizzazione in [!DNL Channel Manager] elenco ordini. [!DNL Walmart] richiede circa 30 minuti per elaborare gli ordini in arrivo e inviarli a [!DNL Channel Manager]. Dopo aver ricevuto l’ordine, la creazione e la visualizzazione dell’ordine in Adobe Commerce o Magenti Open Source richiede circa altri cinque minuti.

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
<td>Ordinare la visualizzazione selezionando una delle opzioni [!UICONTROL Order Status] schede.</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Fornisce informazioni sugli errori degli ordini e sulle richieste di restituzione. Per visualizzare le informazioni sulla restituzione e lo stato del rimborso per un ordine, selezionare <strong>[!UICONTROL Return requested]</strong> testo per aprire [!UICONTROL Returns] dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell’ordine, seleziona la [!DNL Commerce] numero di ordine in [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni ordine per elaborare l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, seleziona Credenziali di connessione Walmart del canale, attributi mappati o identificatori di spedizione, impostazioni seleziona la [!DNL Commerce] numero di ordine in [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni ordine per elaborare l'ordine.</td>
</tr>
</table>


**Descrizioni delle colonne**

<table>
<tr>
<td>Campo</td>
<td>Descrizione</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>Numero dell'ordine di acquisto assegnato all'ordine nel [!DNL Walmart Marketplace]. Quando un ordine viene importato inizialmente in [!DNL Channel Manager], solo il [!DNL Walmart] viene visualizzato il numero dell’ordine. Quando [!DNL Commerce] viene creato l'ordine, il [!DNL Walmart] il numero dell'ordine è memorizzato in [!UICONTROL External ID] attributo del prodotto.</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>Numero assegnato al [!DNL Commerce] ordine creato da [!DNL Walmart Marketplace] ordine.</td>
</tr>
<tr>
<td>Elementi</td>
<td>Numero di articoli ordinati il [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>Costo totale degli articoli ordinati.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>Data in cui l'ordine è stato inviato al [!DNL Walmart Marketplace] convertito nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>Data entro la quale deve essere spedito l'ordine per soddisfare [!DNL Walmart Marketplace] requisiti convertiti nel fuso orario locale.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>Data in cui l'ordine deve essere consegnato al cliente per soddisfare [!DNL Walmart Marketplace] requisiti convertiti nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>Il [[!DNL Walmart Marketplace] Metodo di spedizione](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 selezionato per l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Timestamp che indica l’ultimo aggiornamento dei dati dell’ordine in [!DNL Channel Manager] convertito in fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indica lo stato dell'ordine corrente nel [!DNL Commerce] flusso di lavoro dell’ordine. Stato iniziale di un ordine importato da [!DNL Walmart Marketplace] è _Open_. Ulteriori aggiornamenti dello stato si verificano quando [!DNL Commerce] gli ordini vengono elaborati e [!DNL Channel Manager] sincronizza correttamente gli aggiornamenti di spedizione, spedizione parziale e annullamento in [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Fornisce informazioni più dettagliate sugli ordini con errori o richieste di rimborso.</td>
</tr>
</table>

## Stato ordine

[!UICONTROL Order Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] ordini gestiti da Adobe Commerce o Magenti Open Source. Gli aggiornamenti dello stato dell’ordine si verificano quando [!DNL Channel Manager] riceve informazioni aggiornate sull&#39;ordine da [!DNL Walmart Marketplace] o [!DNL Commerce] sistema di ordinazione. Gli ordini possono avere i seguenti stati:

- **[!UICONTROL Shipped]**- Ordini spediti dal [!DNL Commerce] archiviare. Quando l&#39;ordine viene spedito, [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione su Walmart e fornire il numero di registrazione dell&#39;ordine per la spedizione. Dopo la spedizione di un ordine, gli articoli dell&#39;ordine possono essere parzialmente o completamente rimborsati se Walmart emette un modulo di autorizzazione per la restituzione del materiale promozionale. Consulta [Restituzioni e restituzioni](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**- Ordini per i quali alcuni articoli sono contrassegnati come spediti e altri in attesa di essere spediti. Quando gli articoli nell&#39;ordine vengono spediti [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione in _[!DNL Partially Shipped]_su Walmart e fornire il numero di registrazione dell&#39;ordine per la spedizione.

- **[!UICONTROL Canceled]**- Ordini annullati dal [!DNL Commerce] archiviare.

   Al termine dell’annullamento dell’ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**- Se Walmart Marketplace richiede una restituzione per gli articoli dell&#39;ordine che sono stati spediti, `Return requested` il collegamento viene visualizzato in [!UICONTROL Status details] colonna. Selezionando il collegamento si apre [!UICONTROL Returns] per visualizzare la restituzione e gestire il processo di rimborso.

- **[!UICONTROL Error]**- Ordini con errori. Possono verificarsi errori quando un&#39;operazione di aggiornamento dell&#39;ordine non riesce. Ad esempio, si verificano degli errori se [!DNL Channel Manager] non può ricevere un nuovo ordine da Walmart. Possono verificarsi anche se [!DNL Channel Manager] non può inviare un aggiornamento di spedizione o annullamento dell&#39;ordine al [!DNL Walmart Marketplace]. Se un&#39;operazione non riesce, nella pagina Ordini viene visualizzata una _Errore_ stato dell&#39;ordine. Per ulteriori informazioni, consulta [Correggi errori ordine](errore process-orders.md#fix-shipping-and-cancel).

- **[!UICONTROL Status details]**-Fornisce ulteriori informazioni sugli errori dell&#39;ordine che si verificano a causa di problemi quali informazioni mancanti o valori non validi, dettagli di spedizione errati o un annullamento dell&#39;ordine non riuscito. La descrizione consente di determinare se si è verificato un errore in [!DNL Commerce] istanza o sul [!DNL Walmart Marketplace].

>[!NOTE]
>
>Se gli articoli dell&#39;ordine vengono inviati in più spedizioni, lo stato dell&#39;ordine in [!DNL Channel Manager] riflette l’ultimo stato dell’ordine disponibile. Ad esempio, se il primo articolo viene spedito e non vengono restituiti errori quando gli aggiornamenti dell’ordine vengono sincronizzati con [!DNL Channel Manager] e [!DNL Walmart Marketplace], il [!DNL Channel Manager] lo stato dell&#39;ordine è _[!UICONTROL Partially Shipped]_. Se viene spedito un secondo articolo e [!DNL Channel Manager] restituisce un errore, lo stato dell’ordine viene aggiornato a_[!UICONTROL Error]_.

## Ordini di revisione

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Aprire la visualizzazione punto vendita selezionando l&#39;icona a forma di occhio in una riga della voce del negozio.

1. Per visualizzare le informazioni sull’ordine, seleziona *[!UICONTROL *Orders]**.

1. Ottieni informazioni sull’ordine e determina i passaggi successivi controllando **[Stato](#order-status)** colonna.

## Rivedi dettagli ordine

Dopo aver ricevuto un ordine dal marketplace e averlo importato nel tuo negozio di canali di vendita, utilizza [!DNL Commerce] ID ordine per visualizzare i dettagli dell’ordine in Adobe Commerce.

Da **[!UICONTROL Orders]**, seleziona la **[!UICONTROL Commerce Order Number]** per aprire [!DNL Commerce] dettagli ordine.

![Visualizzazione dettagli ordine Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-detail-with-external-order-id.png)

Nella vetrina Commerce, gli ordini importati da [!DNL Walmart Marketplace] includere nei dati dell’ordine le seguenti informazioni aggiuntive:

- **Informazioni sul pagamento e metodo di spedizione**-Gli ordini importati da Walmart includono i seguenti valori per i campi di pagamento e spedizione:

   - **[!UICONTROL Offline Channel Payment]**- Indica che il pagamento dell&#39;ordine viene elaborato offline da [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**- Visualizza la [!DNL Walmart Marketplace] numero d&#39;ordine.

   - **[!UICONTROL Channel Shipping - Value]**- Indica che le spese di spedizione vengono gestite tramite [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**-Questo campo viene visualizzato solo se un ordine importato da [!DNL Walmart Marketplace] è annullato. I motivi di annullamento includono:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Elementi ordinati**- In questa sezione vengono elencati gli articoli dell&#39;ordine in tutti gli ordini di Commerce. Il [!UICONTROL Qty] fornisce la cronologia dello stato per gli elementi dell&#39;ordine. Ad esempio, se un ordine è stato fatturato, spedito e rimborsato, è possibile visualizzare le transizioni di stato.

   ![Dettagli ordine cronologia stato articoli ordinati [!DNL Walmart Marketplace] ordini](assets/order-detail-status-history.png)

Visualizzare i dettagli della fattura articolo e del rimborso selezionando [!UICONTROL Invoice] e [!UICONTROL Credit Memo] dal menu di navigazione. È inoltre possibile accedere alla nota di credito direttamente dal [[!UICONTROL Returns]](return-refund-orders.md) dashboard nel tuo negozio del canale di vendita.
