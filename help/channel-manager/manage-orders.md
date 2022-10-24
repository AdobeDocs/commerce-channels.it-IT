---
title: 'Visualizza e gestisci gli ordini da [!DNL Channel Manager]'
description: '''Visualizza e gestisci [!DNL Walmart Marketplace] ordini con [!DNL Channel Manager] per Adobe Commerce e Magenti Open Source."'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 1180c86ee8f087a2fef84d84171d77fd5b33164b
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Visualizzare e tenere traccia degli ordini da [!DNL Channel Manager]

[!DNL Walmart Marketplace] dati dell&#39;ordine per [!DNL Commerce] i prodotti si sincronizzano automaticamente con [!DNL Channel Manager] dopo [!DNL Walmart] elabora l&#39;ordine.

Sulla [!DNL Commerce] side, una sincronizzazione corretta attiva le azioni seguenti:

- [!DNL Channel Manager] invia un avviso d&#39;ordine a Walmart.

- A [!DNL Commerce] l&#39;ordine viene creato dall&#39;ordine Walmart.

- Le informazioni aggiornate sull’ordine vengono visualizzate nel [!DNL Channel Manager] Dashboard ordini.

Nell’amministratore della vetrina, puoi visualizzare i dati dell’ordine da [!DNL Channel Manager] aprendo il negozio di canali di vendita e selezionando **[!UICONTROL Orders]**.

![Vista Ordini di Channel Manager da gestire [!DNL Walmart Marketplace] ordini](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Può richiedere fino a 35 minuti per un [!DNL Walmart Marketplace] per visualizzare nel [!DNL Channel Manager] elenco ordini. [!DNL Walmart] richiede circa 30 minuti per elaborare gli ordini in arrivo e inviarli a [!DNL Channel Manager]. Dopo che Channel Manager ha ricevuto l’ordine, ci vogliono circa cinque minuti in più per creare e visualizzare l’ordine in Adobe Commerce o Magento Open Source.

## Controlli sugli ordini e descrizioni delle colonne

Le tabelle seguenti descrivono i controlli e le colonne disponibili per Ordini.

**Controlli per[!UICONTROL Orders]**

<table>
<tr>
<td><strong>Controllo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>Ordina la visualizzazione selezionando una delle [!UICONTROL Order Status] carte.</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Fornisce informazioni sugli errori dell'ordine e sulle richieste di restituzione. Per visualizzare le informazioni sulla restituzione e lo stato del rimborso di un ordine, selezionare <strong>[!UICONTROL Return requested]</strong> testo per aprire [!UICONTROL Returns] dashboard.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell’ordine, seleziona la [!DNL Commerce] numero d'ordine nel [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, selezionare le credenziali di connessione Walmart del canale, gli attributi mappati o gli identificatori di spedizione, le impostazioni selezionano [!DNL Commerce] numero d'ordine nel [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
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
<td>Numero dell'ordine di acquisto assegnato all'ordine nel [!DNL Walmart Marketplace]. Quando un ordine viene inizialmente importato in [!DNL Channel Manager], solo [!DNL Walmart] viene visualizzato il numero dell'ordine. Quando il [!DNL Commerce] l'ordine viene creato, [!DNL Walmart] il numero dell'ordine è memorizzato nel [!UICONTROL External ID] attributo di prodotto.</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>Il numero assegnato al [!DNL Commerce] ordine creato da [!DNL Walmart Marketplace] ordine.</td>
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
<td>La data in cui l'ordine è stato inviato al [!DNL Walmart Marketplace] convertito nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>Data in cui l'ordine deve essere spedito per soddisfare [!DNL Walmart Marketplace] requisiti convertiti nel fuso orario locale.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>La data in cui l'ordine deve essere consegnato al cliente per soddisfare [!DNL Walmart Marketplace] requisiti convertiti nel fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>[[!DNL Walmart Marketplace] Metodo di spedizione](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29 selezionato per l'ordine.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>Timestamp che indica l’ultima volta in cui i dati dell’ordine sono stati aggiornati [!DNL Channel Manager] convertito in fuso orario locale.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indica lo stato corrente dell'ordine nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato iniziale di un ordine importato da [!DNL Walmart Marketplace] è _Open_. Si verificano aggiornamenti di stato aggiuntivi quando [!DNL Commerce] gli ordini vengono elaborati e [!DNL Channel Manager] sincronizza con successo la spedizione, la spedizione parziale e gli aggiornamenti di annullamento alla [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Fornisce informazioni più dettagliate sugli ordini con errori o richieste di rimborso.</td>
</tr>
</table>

## Stato dell&#39;ordine

[!UICONTROL Order Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] ordini gestiti da Adobe Commerce o Magenti Open Source. Gli aggiornamenti dello stato dell&#39;ordine si verificano quando [!DNL Channel Manager] riceve informazioni aggiornate sull&#39;ordine da [!DNL Walmart Marketplace] o [!DNL Commerce] sistema d&#39;ordine. Gli ordini possono avere i seguenti stati:

- **[!UICONTROL Shipped]**- Ordini spediti da [!DNL Commerce] archiviare. Quando l&#39;ordine viene spedito, [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione su Walmart e fornire il numero di registrazione dell&#39;ordine per la spedizione. Dopo la spedizione di un ordine, gli articoli dell&#39;ordine possono essere parzialmente o completamente rimborsati se Walmart emette un modulo di autorizzazione per merce di ritorno. Vedi [Restituzioni](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**- Ordini con alcuni articoli contrassegnati come spediti e altri in attesa di spedizione. Quando gli articoli della spedizione dell&#39;ordine, [!DNL Channel Manager] invia un aggiornamento a [!DNL Walmart Marketplace] per aggiornare lo stato di spedizione a _[!DNL Partially Shipped]_su Walmart e fornire il numero di registrazione dell&#39;ordine per la spedizione.

- **[!UICONTROL Canceled]**—Ordini annullati dal [!DNL Commerce] archiviare.

   Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**- Se Walmart Marketplace richiede un reso per gli articoli d&#39;ordine spediti, un `Return requested` il collegamento viene visualizzato nel [!UICONTROL Status details] colonna. Quando si seleziona il collegamento, viene aperta la [!UICONTROL Returns] dashboard per visualizzare il ritorno e gestire il processo di rimborso.

- **[!UICONTROL Error]**- Ordini con errori. Gli errori possono verificarsi quando un’operazione di aggiornamento dell’ordine non riesce. Ad esempio, si verificano degli errori se [!DNL Channel Manager] non può ricevere un nuovo ordine da Walmart. Possono anche verificarsi se [!DNL Channel Manager] impossibile inviare un aggiornamento della spedizione o dell&#39;annullamento dell&#39;ordine al [!DNL Walmart Marketplace]. Se un’operazione non riesce, nella pagina Ordini viene visualizzata una _Errore_ stato dell&#39;ordine. Per maggiori dettagli, vedi [Correggere gli errori di ordine](errori process-orders.md#fix-shipping-and-cancel-).

- **[!UICONTROL Status details]**- Fornisce ulteriori informazioni sugli errori di ordine che si verificano a causa di problemi come informazioni mancanti o valori non validi, dettagli di spedizione errati o un annullamento dell&#39;ordine non riuscito. La descrizione aiuta a determinare se si è verificato un errore nel [!DNL Commerce] o [!DNL Walmart Marketplace].

>[!NOTE]
>
>Se gli articoli dell&#39;ordine vengono inviati in più spedizioni, lo stato dell&#39;ordine in [!DNL Channel Manager] riflette lo stato dell&#39;ultimo ordine disponibile. Ad esempio, se il primo articolo viene spedito e non vengono restituiti errori quando gli aggiornamenti dell&#39;ordine sono sincronizzati con [!DNL Channel Manager] e [!DNL Walmart Marketplace], [!DNL Channel Manager] lo stato dell&#39;ordine è _[!UICONTROL Partially Shipped]_. Se viene spedito un secondo articolo e [!DNL Channel Manager] restituisce un errore, lo stato dell&#39;ordine viene aggiornato a_[!UICONTROL Error]_.

## Ordini di revisione

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Apri la vista Store selezionando l&#39;icona dell&#39;occhio in una riga della voce store.

1. Per visualizzare le informazioni sull&#39;ordine, selezionare *[!UICONTROL *Orders]**

1. Ottenere informazioni sull&#39;ordine e determinare i passaggi successivi controllando il **[Stato](#order-status)** colonna.

## Dettaglio ordine di revisione

Dopo aver ricevuto un ordine dal marketplace e importato nel tuo negozio di canali di vendita, utilizza [!DNL Commerce] ID ordine per visualizzare i dettagli dell’ordine in Adobe Commerce.

Da **[!UICONTROL Orders]**, seleziona **[!UICONTROL Commerce Order Number]** per aprire [!DNL Commerce] dettaglio dell&#39;ordine.

![Visualizzazione dettagli ordine di Commerce per un [!DNL Walmart Marketplace] ordine](assets/order-detail-with-external-order-id.png)

Nella vetrina Commerce, gli ordini importati da [!DNL Walmart Marketplace] dispongono delle seguenti informazioni aggiuntive incluse nei dati dell’ordine:

- **Informazioni sul pagamento e metodo di spedizione**-Gli ordini importati da Walmart includono i seguenti valori per i campi di pagamento e spedizione:

   - **[!UICONTROL Offline Channel Payment]**- Indica che il pagamento dell&#39;ordine è stato elaborato offline da [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**- Visualizza il [!DNL Walmart Marketplace] numero d&#39;ordine.

   - **[!UICONTROL Channel Shipping - Value]**- Indica che le spese di spedizione vengono gestite tramite [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**- Questo campo viene visualizzato solo se un ordine è stato importato da [!DNL Walmart Marketplace] è annullato. I motivi di annullamento includono:

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **Articoli ordinati**- In questa sezione sono elencati gli elementi dell&#39;ordine in tutti gli ordini Commerce. La [!UICONTROL Qty] fornisce la cronologia dello stato per gli articoli dell&#39;ordine. Ad esempio, se un ordine è stato fatturato, spedito e rimborsato, è possibile visualizzare le transizioni di stato.

   ![Dettagli ordine - Cronologia stato articolo ordinato [!DNL Walmart Marketplace] ordini](assets/order-detail-status-history.png)

Visualizza i dettagli della fattura dell&#39;articolo e del rimborso selezionando [!UICONTROL Invoice] e [!UICONTROL Credit Memo] dal menu di navigazione. È inoltre possibile accedere alla nota di accredito direttamente dalla sezione [[!UICONTROL Returns]](return-refund-orders.md) dashboard nell&#39;archivio canali di vendita.



