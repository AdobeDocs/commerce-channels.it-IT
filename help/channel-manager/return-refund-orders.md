---
title: Ordini di restituzione e di rimborso
description: Istruzioni per l'emissione di rimborsi completi o parziali per le richieste di rimpatrio ricevute da [!DNL Walmart Marketplace] da [!DNL Channel Manager] per Adobe Commerce e Magento Open Source.
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# Ordini di restituzione e di rimborso

Quando un acquirente richiede una restituzione per gli articoli dell&#39;ordine acquistati tramite [!DNL Walmart Marketplace], Walmart crea una richiesta di reso. [!DNL Channel Manager] monitora il canale del marketplace per queste richieste e sincronizza automaticamente le informazioni sulla richiesta di ritorno a Channel Manager.

Sul lato Commerce, la richiesta di ritorno avvia il seguente flusso di lavoro:

1. Channel Manager crea una richiesta di ritorno corrispondente con lo stato ricevuto e aggiunge il numero ID restituito ([!UICONTROL RMA #]) al [!UICONTROL Returns] dashboard. Il giorno [!DNL Orders] dashboard, i dettagli dello stato per l&#39;ordine associato agli aggiornamenti di restituzione per includere un [!UICONTROL Return requested] per visualizzare ed elaborare il reso.

1. I commercianti elaborano il rimborso associato alla restituzione creando una nota di credito dopo la [Flusso di lavoro di rimborso di Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html). Tutti i rimborsi vengono elaborati utilizzando il metodo offline.

1. [!DNL Channel Manager] invia un aggiornamento del rimborso a Walmart marketplace in modo che lo stato di restituzione possa essere aggiornato per riflettere il rimborso completato da Adobe Commerce.

In amministrazione vetrina, puoi visualizzare ed elaborare i resi da Channel Manager aprendo il negozio del canale di vendita e selezionando **[!UICONTROL Returns]**.

![Il dashboard Restituzioni di Channel Manager consente di elaborare i rimborsi per le richieste di restituzione ricevute da [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>È possibile elaborare i rimborsi solo per gli ordini spediti. In entrata [!DNL Channel Manager], lo stato dell&#39;ordine deve essere [!UICONTROL Shipped]. In entrata [!DNL Walmart Marketplace] Account del venditore, l&#39;ordine deve essere [!UICONTROL Delivered].

## Restituisce i controlli e le descrizioni delle colonne

Nelle tabelle seguenti vengono descritti i controlli e le colonne disponibili per [!DNL Channel Manager] restituisce.

**Controlli per[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Controllo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filtrare la visualizzazione selezionando una delle opzioni [!UICONTROL Return Status] schede.</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Per le voci di ritorno con [!UICONTROL Received] o [!UICONTROL Refunded] stato, è possibile creare o visualizzare la nota di accredito per il rimborso selezionando il testo collegato nella colonna Dettagli stato.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell’ordine, seleziona la [!DNL Commerce] numero di ordine in [!UICONTROL Order] tabella per aprire l’ordine Commerce.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, seleziona Credenziali di connessione Walmart del canale, attributi mappati o identificatori di spedizione, impostazioni seleziona la [!DNL Commerce] numero di ordine in [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni ordine per elaborare l'ordine.</td>
</tr>
</table>

**Descrizioni delle colonne**

<table>
<tr>
<td><strong>Campo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>Il numero di autorizzazione per la restituzione del materiale promozionale associato alla richiesta di restituzione ricevuta da [!DNL Walmart Marketplace]. Questo numero è generato da Walmart Marketplace [!UICONTROL Returns] quando viene avviato il processo di restituzione.</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>Il [!DNL Commerce] numero di ordine associato agli elementi inclusi nella richiesta di reso da Walmart Marketplace. Visualizzare i dettagli dell'ordine selezionando il numero dell'ordine.</td>
</tr>
<tr>
<td>Richiesto</td>
<td>Data della richiesta di restituzione in data [!DNL Walmart Marketplace]
convertito nell’ora locale.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>Data entro la quale deve essere rimborsata la restituzione per soddisfare [!DNL Walmart Marketplace] [requisiti](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) convertiti in ora locale.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>Elenca lo SKU e la quantità per ogni articolo elencato nella restituzione.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>Il valore totale da rimborsare per gli articoli restituiti.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indica lo stato corrente della restituzione nel [!DNL Commerce] flusso di lavoro di ritorno-<i>Ricevuto</i>, <i>Rimborsato</i>, o <i>Errore</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Per le voci di restituzione ricevute e rimborsate, i dettagli sullo stato forniscono un collegamento per accedere alla nota di credito per l'elaborazione del rimborso. Se si verifica un errore durante la [!DNL Channel Manager] processo di sincronizzazione tra Adobe Commerce e [!DNL Walmart marketplace], questo campo fornisce la descrizione dell’errore.</td>
</tr>
</table>

## Stato di ritorno

[!UICONTROL Return Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] richieste di restituzione gestite da Adobe Commerce o Magento Open Source.

Gli aggiornamenti dello stato di ritorno si verificano quando [!DNL Channel Manager] riceve una richiesta di ritorno da [!DNL Walmart Marketplace] o quando [!DNL Commerce] viene creata una nota di credito per elaborare il rimborso per gli articoli restituiti.

Le restituzioni possono avere i seguenti stati:

* **[!UICONTROL Received]**-Questo è lo stato iniziale della richiesta di ritorno ricevuta dal [!DNL Walmart Marketplace] archiviare. Il commerciante può elaborare il rimborso per la restituzione selezionando **[!UICONTROL Create credit memo]** nel [!UICONTROL Status details].

* **[!UICONTROL Refunded]**- Indica che è stata creata una nota di accredito per emettere un rimborso per gli articoli restituiti. Gli esercenti possono visualizzare le informazioni sul rimborso selezionando **[!UICONTROL View credit memo]** nel [!UICONTROL Status details].

* **[!UICONTROL Error]**- Restituisci le richieste che presentano errori. Possono verificarsi errori quando la richiesta di ritorno da Walmart contiene dati mancanti o errati. Oppure, se [!DNL Channel Manager] non può inviare la notifica di aggiornamento del rimborso a Walmart.

## Scenari di ritorno

Gli scenari seguenti descrivono come emettere rimborsi per diversi tipi di richieste di rimpatrio da [!DNL Channel Manager].

* **Ritorno completo**- Se la richiesta di restituzione di Walmart Marketplace riguarda tutti gli articoli dell&#39;ordine, aggiornare la quantità della nota di credito per rimborsare tutti gli articoli.

* **Restituzione parziale**-Se la richiesta di restituzione di Walmart Marketplace riguarda solo alcuni articoli dell&#39;ordine, aggiornare la quantità della nota di credito solo per gli articoli da rimborsare.

* **Restituzioni già rimborsate tramite Walmart Marketplace**-In alcuni casi, un rimborso viene elaborato il [!DNL Walmart Marketplace] prima di elaborare il reso in Channel Manager. Ad esempio, se un ordine Commerce non viene rimborsato entro la finestra di elaborazione del rimborso di 48 ore richiesta da Walmart, quest&#39;ultimo lo rimborsa automaticamente. In questo caso, Channel Manager sincronizza ancora la richiesta di restituzione con Adobe Commerce in modo da poter elaborare la restituzione e emettere la nota di credito. Questo flusso di lavoro garantisce che i dettagli dell’ordine in [!DNL Commerce] corrisponde alle informazioni sull&#39;ordine in Walmart Marketplace.

>[!NOTE]
>
> La sincronizzazione degli aggiornamenti dei rimborsi con può richiedere fino a cinque minuti [!DNL Walmart Marketplace]. Puoi controllare lo stato corrente della restituzione dalla sezione [!DNL Channel Manager] [!UICONTROL Returns] dashboard.

## Elabora una richiesta di rimborso

1. Apri [!UICONTROL Returns] dashboard per il tuo negozio del canale di vendita.

   * Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

   * È possibile esaminare le restituzioni selezionando la **[!UICONTROL Returns]** scheda.

     È inoltre possibile accedere alle informazioni di ritorno da [!UICONTROL Orders] pagina. Cerca [!UICONTROL Shipped] ordini con una richiesta di reso. Quindi, seleziona la `Return requested` collegamento in [!UICONTROL Status Details] per visualizzare ed elaborare la richiesta.

1. Nella tabella Restituzioni, trovare un risultato con il *[!UICONTROL Received]* stato.

1. Nella colonna Articoli esaminare l&#39;elenco degli articoli dell&#39;ordine e la quantità da rimborsare.

1. Elaborare il rimborso emettendo una nota di accredito.

   * Dalla sezione [!UICONTROL Status Details] colonna, seleziona **[!UICONTROL Create credit memo]** per aprire la pagina dei dettagli dell&#39;ordine in [!DNL Commerce].

     Se l&#39;ordine non è stato fatturato, nella pagina Dettagli ordine viene visualizzato un messaggio di errore che richiede di crearne uno. Seleziona **[!UICONTROL Create invoice]**. Allora, [crea e salva la fattura](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * Nella pagina dei dettagli dell&#39;ordine selezionare **[!UICONTROL Credit Memo]**.

   * In entrata [!UICONTROL Items to Refund] sezione del [!UICONTROL Credit Memo], aggiorna **[!UICONTROL Qty to refund]** e **[!UICONTROL Return to Stock]** informazioni relative agli elementi inclusi nella richiesta di reso.

     Assicurati di restituire solo gli elementi elencati nella richiesta di restituzione.

   * Per aggiungere un commento, immettere il testo nel **[!UICONTROL Credit Memo Comments]**

   * Seleziona **[!UICONTROL Refund Offline]**.

Dopo aver completato la restituzione, [!DNL Channel Manager] aggiorna lo stato di ritorno in [!UICONTROL Returns] dashboard a [!UICONTROL Refunded] e sincronizza l’aggiornamento con Walmart per aggiornare lo stato di ritorno nel marketplace.


## Visualizza informazioni sul rimborso per una restituzione

È possibile visualizzare informazioni sulle richieste di restituzione e sull&#39;elaborazione dei rimborsi dal [!UICONTROL Returns] dashboard.

1. Apri il dashboard Restituzioni per il tuo negozio del canale di vendita.

   * Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

   * Seleziona **[!UICONTROL Returns]**.

1. Visualizzare gli ordini rimborsati selezionando **[!UICONTROL Refunded]** scheda di stato.

1. Visualizzare i dettagli del rimborso per una restituzione selezionando **[!UICONTROL View credit memo]**.

   ![Nota di accredito per il rimborso di articoli restituiti per un [!DNL Walmart Marketplace] ordine](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Dopo il rimborso di un ordine, [!UICONTROL Orders] la dashboard non mostra le informazioni di ritorno. Per visualizzare le informazioni sulla restituzione, utilizzare [!DNL Channel Manager] Restituisce il dashboard. Informazioni più dettagliate sulla restituzione e sul rimborso sono disponibili anche nella pagina dei dettagli dell&#39;ordine.

## Correggere gli errori di ritorno

Possono verificarsi errori quando le informazioni di ritorno vengono ricevute da [!DNL Walmart Marketplace], o quando [!DNL Channel Manager] sincronizza gli aggiornamenti dello stato da [!DNL Commerce] a [!DNL Walmart Marketplace].

Se l&#39;operazione di sincronizzazione per un aggiornamento di ritorno non riesce, il [!DNL Channel Manager] La dashboard di Restituisce mostra un valore *[!UICONTROL Error]* stato della voce di ritorno. Per garantire che le informazioni relative alla restituzione e al rimborso vengano riportate in modo accurato nell&#39;account di Walmart Marketplace, aggiornare manualmente l&#39;ordine nel [!DNL Walmart Marketplace] archiviare.
