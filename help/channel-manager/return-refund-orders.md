---
title: Ordini di restituzione e di rimborso
description: Istruzioni per l'emissione di rimborsi completi o parziali per le richieste di restituzione ricevute da [!DNL Walmart Marketplace] da [!DNL Channel Manager] per Adobe Commerce e Magento Open Source.
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Ordini di restituzione e di rimborso

Quando un acquirente richiede una restituzione per gli articoli dell&#39;ordine acquistati tramite [!DNL Walmart Marketplace], Walmart crea una richiesta di restituzione. [!DNL Channel Manager] monitora il canale del marketplace per queste richieste e sincronizza automaticamente le informazioni della richiesta di ritorno a Channel Manager.

Sul lato Commerce, la richiesta di ritorno avvia il seguente flusso di lavoro:

1. Channel Manager crea una richiesta di ritorno corrispondente con uno stato ricevuto e aggiunge il numero di ID restituito ([!UICONTROL RMA #]) al dashboard [!UICONTROL Returns]. Nel dashboard [!DNL Orders], i dettagli dello stato per l&#39;ordine associato agli aggiornamenti di restituzione includono un collegamento [!UICONTROL Return requested] per visualizzare ed elaborare la restituzione.

1. I commercianti elaborano il rimborso associato alla restituzione creando una nota di credito dopo il [flusso di lavoro di rimborso Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html). Tutti i rimborsi vengono elaborati utilizzando il metodo offline.

1. [!DNL Channel Manager] invia un aggiornamento di rimborso al marketplace Walmart in modo che lo stato di restituzione possa essere aggiornato per riflettere il rimborso completato da Adobe Commerce.

Nell&#39;amministratore della vetrina è possibile visualizzare ed elaborare i resi da Channel Manager aprendo lo store dei canali di vendita e selezionando **[!UICONTROL Returns]**.

![Il dashboard Restituzioni di Channel Manager consente di elaborare i rimborsi per le richieste di restituzione ricevute da [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>È possibile elaborare i rimborsi solo per gli ordini spediti. In [!DNL Channel Manager], lo stato dell&#39;ordine deve essere [!UICONTROL Shipped]. Nell&#39;account del venditore [!DNL Walmart Marketplace], l&#39;ordine deve essere [!UICONTROL Delivered].

## Restituisce i controlli e le descrizioni delle colonne

Nelle tabelle seguenti vengono descritti i controlli e le colonne disponibili per [!DNL Channel Manager] restituiti.

**Controlli per[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Controllo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filtra la visualizzazione selezionando una delle schede [!UICONTROL Return Status].</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Per le voci di restituzione con lo stato [!UICONTROL Received] o [!UICONTROL Refunded], è possibile creare o visualizzare la nota di credito per il rimborso selezionando il testo collegato nella colonna Dettagli stato.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell'ordine, selezionare il numero dell'ordine [!DNL Commerce] nella tabella [!UICONTROL Order] per aprire l'ordine Commerce.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, selezionare le credenziali di connessione Walmart del canale, gli attributi mappati o gli identificatori di spedizione, le impostazioni selezionano il numero di ordine [!DNL Commerce] nella tabella [!UICONTROL Order]. Quindi utilizzare [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
</tr>
</table>

**Descrizioni colonne**

<table>
<tr>
<td><strong>Campo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>Il numero di autorizzazione per la restituzione di merci associato alla richiesta di restituzione ricevuta da [!DNL Walmart Marketplace]. Questo numero viene generato da Walmart Marketplace [!UICONTROL Returns] all'avvio del processo di restituzione.</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>Il numero di ordine [!DNL Commerce] associato agli elementi inclusi nella richiesta di restituzione da Walmart Marketplace. Visualizzare i dettagli dell'ordine selezionando il numero dell'ordine.</td>
</tr>
<tr>
<td>Richiesto</td>
<td>Data in cui è stata richiesta la restituzione il [!DNL Walmart Marketplace]
convertito nell’ora locale.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>La data entro la quale deve essere rimborsata la restituzione per soddisfare [!DNL Walmart Marketplace] [requisiti](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) convertito nell'ora locale.</td>
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
<td>Indica lo stato corrente del reso nel flusso di lavoro di ritorno [!DNL Commerce]-<i>Ricevuto</i>, <i>Rimborsato</i> o <i>Errore</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Per le voci di restituzione ricevute e rimborsate, i dettagli sullo stato forniscono un collegamento per accedere alla nota di credito per l'elaborazione del rimborso. Se si verifica un errore durante il processo di sincronizzazione [!DNL Channel Manager] tra Adobe Commerce e [!DNL Walmart marketplace], questo campo fornisce la descrizione dell'errore.</td>
</tr>
</table>

## Stato di ritorno

[!UICONTROL Return Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] richieste di restituzione gestite da Adobe Commerce o Magento Open Source.

Gli aggiornamenti dello stato di restituzione si verificano quando [!DNL Channel Manager] riceve una richiesta di restituzione da [!DNL Walmart Marketplace] o quando viene creata la nota di credito [!DNL Commerce] per elaborare il rimborso per gli elementi restituiti.

Le restituzioni possono avere i seguenti stati:

* **[!UICONTROL Received]** - Questo è lo stato iniziale della richiesta di ritorno ricevuta dall&#39;archivio [!DNL Walmart Marketplace]. Il commerciante può elaborare il rimborso per la restituzione selezionando **[!UICONTROL Create credit memo]** in [!UICONTROL Status details].

* **[!UICONTROL Refunded]** - Indica che è stata creata una nota di credito per emettere un rimborso per gli elementi restituiti. Gli esercenti possono visualizzare le informazioni sul rimborso selezionando **[!UICONTROL View credit memo]** in [!UICONTROL Status details].

* **[!UICONTROL Error]** - Richieste restituite con errori. Possono verificarsi errori quando la richiesta di ritorno da Walmart contiene dati mancanti o errati. Oppure, se [!DNL Channel Manager] non è in grado di inviare la notifica di aggiornamento del rimborso a Walmart.

## Scenari di ritorno

Gli scenari seguenti descrivono come emettere rimborsi per diversi tipi di richieste di restituzione da [!DNL Channel Manager].

* **Restituzione completa** - Se la richiesta di restituzione di Walmart Marketplace riguarda tutti gli articoli dell&#39;ordine, aggiornare la quantità della nota di credito per rimborsare tutti gli articoli.

* **Restituzione parziale**-Se la richiesta di restituzione di Walmart Marketplace riguarda solo alcuni articoli dell&#39;ordine, aggiornare la quantità della nota di credito solo per gli articoli da rimborsare.

* **Restituzione già rimborsata tramite Walmart Marketplace**-In alcuni casi, viene elaborato un rimborso il [!DNL Walmart Marketplace] prima di elaborare la restituzione in Channel Manager. Ad esempio, se un ordine Commerce non viene rimborsato entro la finestra di elaborazione del rimborso di 48 ore richiesta da Walmart, quest&#39;ultimo lo rimborsa automaticamente. In questo caso, Channel Manager sincronizza ancora la richiesta di restituzione con Adobe Commerce in modo da poter elaborare la restituzione e emettere la nota di credito. Questo flusso di lavoro garantisce che i dettagli dell&#39;ordine in [!DNL Commerce] corrispondano alle informazioni dell&#39;ordine in Walmart Marketplace.

>[!NOTE]
>
> La sincronizzazione con [!DNL Walmart Marketplace] può richiedere fino a cinque minuti per gli aggiornamenti dei rimborsi. È possibile controllare lo stato corrente di ritorno dal dashboard [!DNL Channel Manager] [!UICONTROL Returns].

## Elabora una richiesta di rimborso

1. Apri il dashboard di [!UICONTROL Returns] per il tuo store del canale di vendita.

   * Dall&#39;amministratore, selezionare **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

   * È possibile esaminare i risultati selezionando la scheda **[!UICONTROL Returns]**.

     È inoltre possibile accedere alle informazioni di ritorno dalla pagina [!UICONTROL Orders]. Cerca [!UICONTROL Shipped] ordini con una richiesta di reso. Quindi, seleziona il collegamento `Return requested` nella colonna [!UICONTROL Status Details] per visualizzare ed elaborare la richiesta.

1. Nella tabella Restituisce trovare un risultato con lo stato *[!UICONTROL Received]*.

1. Nella colonna Articoli esaminare l&#39;elenco degli articoli dell&#39;ordine e la quantità da rimborsare.

1. Elaborare il rimborso emettendo una nota di accredito.

   * Dalla colonna [!UICONTROL Status Details], selezionare **[!UICONTROL Create credit memo]** per aprire la pagina Dettagli ordine in [!DNL Commerce].

     Se l&#39;ordine non è stato fatturato, nella pagina Dettagli ordine viene visualizzato un messaggio di errore che richiede di crearne uno. Selezionare **[!UICONTROL Create invoice]**. Quindi [crea e salva la fattura](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * Nella pagina Dettagli ordine, selezionare **[!UICONTROL Credit Memo]**.

   * Nella sezione [!UICONTROL Items to Refund] di [!UICONTROL Credit Memo], aggiornare le informazioni di **[!UICONTROL Qty to refund]** e **[!UICONTROL Return to Stock]** per gli elementi inclusi nella richiesta di ritorno.

     Assicurati di restituire solo gli elementi elencati nella richiesta di restituzione.

   * Per aggiungere un commento, immettere il testo in **[!UICONTROL Credit Memo Comments]**

   * Selezionare **[!UICONTROL Refund Offline]**.

Dopo aver completato il rimborso, [!DNL Channel Manager] aggiorna lo stato del reso nel dashboard [!UICONTROL Returns] in [!UICONTROL Refunded] e sincronizza l&#39;aggiornamento in Walmart per aggiornare lo stato del reso nel marketplace.


## Visualizza informazioni sul rimborso per una restituzione

È possibile visualizzare informazioni sulle richieste di restituzione e sull&#39;elaborazione dei rimborsi dal dashboard [!UICONTROL Returns].

1. Apri il dashboard Restituzioni per il tuo negozio del canale di vendita.

   * Dall&#39;amministratore, selezionare **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista del negozio selezionando l’icona dell’occhio per un negozio del canale di vendita.

   * Selezionare **[!UICONTROL Returns]**.

1. Visualizza ordini rimborsati selezionando la scheda di stato **[!UICONTROL Refunded]**.

1. Visualizzare i dettagli del rimborso per una restituzione selezionando **[!UICONTROL View credit memo]**.

   ![Nota di credito per il rimborso ha restituito elementi per un ordine [!DNL Walmart Marketplace]](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>Dopo il rimborso di un ordine, nel dashboard [!UICONTROL Orders] non vengono visualizzate le informazioni sulla restituzione. Per visualizzare le informazioni di ritorno, utilizzare il dashboard Restituzioni [!DNL Channel Manager]. Informazioni più dettagliate sulla restituzione e sul rimborso sono disponibili anche nella pagina dei dettagli dell&#39;ordine.

## Correggere gli errori di ritorno

Possono verificarsi errori quando le informazioni restituite vengono ricevute da [!DNL Walmart Marketplace] o quando [!DNL Channel Manager] sincronizza gli aggiornamenti dello stato da [!DNL Commerce] a [!DNL Walmart Marketplace].

Se l&#39;operazione di sincronizzazione per un aggiornamento di ritorno non riesce, il dashboard [!DNL Channel Manager] Restituisce mostra uno stato *[!UICONTROL Error]* per la voce di ritorno. Per garantire che le informazioni sulla restituzione e sul rimborso vengano riportate correttamente nell&#39;account Walmart Marketplace, aggiornare manualmente l&#39;ordine nell&#39;archivio [!DNL Walmart Marketplace].
