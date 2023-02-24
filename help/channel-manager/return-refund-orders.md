---
title: Ordini di restituzione
description: Istruzioni per il rilascio dei rimborsi completi o parziali per le richieste di rimpatrio ricevute da [!DNL Walmart Marketplace] da [!DNL Channel Manager] per Adobe Commerce e Magenti Open Source.
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ordini di restituzione

Quando un acquirente richiede un reso per gli articoli dell&#39;ordine acquistati tramite [!DNL Walmart Marketplace], Walmart crea una richiesta di restituzione. [!DNL Channel Manager] controlla il canale marketplace per queste richieste e sincronizza automaticamente le informazioni di richiesta di ritorno a Channel Manager.

Sul lato Commerce, la richiesta di ritorno avvia il seguente flusso di lavoro:

1. Channel Manager crea una richiesta di restituzione corrispondente con uno stato ricevuto e aggiunge il numero di ID restituito ([!UICONTROL RMA #]) al [!UICONTROL Returns] dashboard. Sulla [!DNL Orders] dashboard, il dettaglio dello stato dell&#39;ordine associato agli aggiornamenti di ritorno per includere un [!UICONTROL Return requested] per visualizzare ed elaborare il ritorno.

1. I commercianti elaborano il rimborso associato alla restituzione creando una nota di credito successiva alla [Flusso di lavoro di rimborso Adobe Commerce](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow). Tutti i rimborsi vengono elaborati utilizzando il metodo offline.

1. [!DNL Channel Manager] invia un aggiornamento del rimborso a Walmart marketplace in modo che lo stato di restituzione possa essere aggiornato per riflettere il rimborso completato da Adobe Commerce.

Nell&#39;amministratore della vetrina, puoi visualizzare ed elaborare i resi da Channel Manager aprendo l&#39;archivio dei canali di vendita e selezionando **[!UICONTROL Returns]**.

![Channel Manager Restituisce il dashboard per elaborare i rimborsi per le richieste di restituzione ricevute da [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>È possibile elaborare solo i rimborsi per gli ordini spediti. In [!DNL Channel Manager], lo stato dell&#39;ordine deve essere [!UICONTROL Shipped]. In [!DNL Walmart Marketplace] Conto del venditore, l&#39;ordine deve essere [!UICONTROL Delivered].

## Restituisce controlli e descrizioni a colonne

Le tabelle seguenti descrivono i controlli e le colonne disponibili per [!DNL Channel Manager] restituisce.

**Controlli per[!UICONTROL Returns]**

<table>
<tr>
<td><strong>Controllo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filtrare la visualizzazione selezionando una delle [!UICONTROL Return Status] carte.</td>
</tr>
<tr>
<td>Dettagli stato</td>
<td>Per le voci di ritorno con [!UICONTROL Received] o [!UICONTROL Refunded] è possibile creare o visualizzare la nota di credito per il rimborso selezionando il testo collegato nella colonna Dettagli stato.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>Per visualizzare i dettagli dell’ordine, seleziona la [!DNL Commerce] numero d'ordine nel [!UICONTROL Order] per aprire l’ordine Commerce.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>Per modificare la configurazione del canale, selezionare le credenziali di connessione Walmart del canale, gli attributi mappati o gli identificatori di spedizione, le impostazioni selezionano [!DNL Commerce] numero d'ordine nel [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni di ordine per elaborare l'ordine.</td>
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
<td>Numero di autorizzazione Merchandise restituito associato alla richiesta di restituzione ricevuta da [!DNL Walmart Marketplace]. Questo numero è generato da Walmart Marketplace [!UICONTROL Returns] quando viene avviato il processo di restituzione.</td>
</tr>
<tr>
<td>[!DNL Commerce] N. ordine</td>
<td>La [!DNL Commerce] numero dell'ordine associato agli elementi inclusi nella richiesta di restituzione da Walmart Marketplace. Visualizzare i dettagli dell’ordine selezionando il numero dell’ordine.</td>
</tr>
<tr>
<td>Richiesto</td>
<td>La data in cui è stato richiesto il ritorno è [!DNL Walmart Marketplace]
convertito in ora locale.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>La data entro la quale la restituzione deve essere rimborsata per soddisfare [!DNL Walmart Marketplace] [requisiti](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f) convertito in ora locale.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>Elenca lo SKU e la quantità per ogni articolo elencato nella restituzione.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>Valore totale da rimborsare per gli elementi restituiti.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indica lo stato di ritorno corrente nel [!DNL Commerce] workflow di ritorno<i>Ricevuto</i>, <i>Rimborsato</i>oppure <i>Errore</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>Per le voci di reso ricevute e rimborsate, i dettagli dello stato forniscono un collegamento per accedere alla nota di credito per l'elaborazione del rimborso. Se si verifica un errore durante la [!DNL Channel Manager] processo di sincronizzazione tra Adobe Commerce e [!DNL Walmart marketplace], questo campo fornisce la descrizione dell’errore.</td>
</tr>
</table>

## Stato di ritorno

[!UICONTROL Return Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] richieste di restituzione gestite da Adobe Commerce o Magenti Open Source.

Gli aggiornamenti dello stato di ritorno si verificano quando [!DNL Channel Manager] riceve una richiesta di ritorno da [!DNL Walmart Marketplace] o quando [!DNL Commerce] viene creata una nota di credito per elaborare il rimborso per gli articoli restituiti.

I valori restituiti possono avere i seguenti stati:

* **[!UICONTROL Received]**- Questo è lo stato iniziale della richiesta di restituzione ricevuta dal [!DNL Walmart Marketplace] archiviare. Il commerciante può elaborare il rimborso per il ritorno selezionando **[!UICONTROL Create credit memo]** in [!UICONTROL Status details].

* **[!UICONTROL Refunded]**- Indica che è stata creata una nota di credito per emettere un rimborso per gli articoli restituiti. I commercianti possono visualizzare le informazioni sui rimborsi selezionando **[!UICONTROL View credit memo]** in [!UICONTROL Status details].

* **[!UICONTROL Error]**- Restituire richieste con errori. Gli errori possono verificarsi quando la richiesta di restituzione da Walmart presenta dati mancanti o non corretti. Oppure, se [!DNL Channel Manager] impossibile inviare la notifica di aggiornamento del rimborso a Walmart.

## Scenari di ritorno

I seguenti scenari descrivono come eseguire i rimborsi per diversi tipi di richieste di restituzione da [!DNL Channel Manager].

* **Ritorno completo**- Se la richiesta di restituzione Walmart Marketplace è per tutti gli articoli nell&#39;ordine, aggiornare la quantità della nota di credito per rimborsare tutti gli articoli.

* **Ritorno parziale**- Se la richiesta di restituzione di Walmart Marketplace è solo per alcuni articoli dell&#39;ordine, aggiornare la quantità della nota di credito solo per gli articoli da rimborsare.

* **Ritorno già rimborsato tramite Walmart Marketplace**-In alcuni casi viene elaborata una restituzione [!DNL Walmart Marketplace] prima di elaborare il ritorno in Channel Manager. Ad esempio, se un ordine Commerce non viene rimborsato entro la finestra di elaborazione dei rimborsi di 48 ore richiesta da Walmart, Walmart rimborsa automaticamente l&#39;ordine. In questo caso, Channel Manager sincronizza ancora la richiesta di restituzione con Adobe Commerce in modo da poter elaborare la restituzione ed emettere la nota di credito. Questo flusso di lavoro assicura che i dettagli dell’ordine siano [!DNL Commerce] corrisponde alle informazioni sull&#39;ordine in Walmart Marketplace.

>[!NOTE]
>
> Può richiedere fino a cinque minuti per gli aggiornamenti dei rimborsi per sincronizzarsi con [!DNL Walmart Marketplace]. Puoi controllare lo stato di ritorno corrente dalla [!DNL Channel Manager] [!UICONTROL Returns] dashboard.

## Elabora una richiesta di rimborso

1. Apri [!UICONTROL Returns] dashboard per l&#39;archivio canali di vendita.

   * Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

   * Puoi rivedere i risultati selezionando la **[!UICONTROL Returns]** scheda .

      È inoltre possibile accedere alle informazioni di ritorno da [!UICONTROL Orders] pagina. Cerca [!UICONTROL Shipped] ordini che hanno una richiesta di restituzione. Quindi, seleziona la `Return requested` nel collegamento [!UICONTROL Status Details] per visualizzare ed elaborare la richiesta.

1. Dalla tabella Restituisce, trovare un ritorno con il *[!UICONTROL Received]* stato.

1. Dalla colonna Articoli, esaminare l&#39;elenco degli articoli dell&#39;ordine e la quantità da rimborsare.

1. Elaborare il rimborso emettendo una nota di credito.

   * Da [!UICONTROL Status Details] colonna, seleziona **[!UICONTROL Create credit memo]** per aprire la pagina dei dettagli Ordine in [!DNL Commerce].

      Se l&#39;ordine non è stato fatturato, nella pagina Dettagli ordine viene visualizzato un messaggio di errore che richiede di crearne uno. Seleziona **[!UICONTROL Create invoice]**. Allora, [creare e salvare la fattura](https://docs.magento.com/user-guide/sales/invoices.html).

   * Nella pagina Dettagli ordine, seleziona **[!UICONTROL Credit Memo]**.

   * In [!UICONTROL Items to Refund] della sezione [!UICONTROL Credit Memo], aggiorna **[!UICONTROL Qty to refund]** e **[!UICONTROL Return to Stock]** informazioni relative agli elementi inclusi nella richiesta di restituzione.

      Assicurati di restituire solo gli elementi elencati nella richiesta di restituzione.

   * Per aggiungere un commento, immetti il testo nel **[!UICONTROL Credit Memo Comments]**

   * Seleziona **[!UICONTROL Refund Offline]**.

Dopo aver completato il rimborso, [!DNL Channel Manager] aggiorna lo stato di ritorno in [!UICONTROL Returns] dashboard [!UICONTROL Refunded] e sincronizza l&#39;aggiornamento a Walmart per aggiornare lo stato di ritorno in marketplace.


## Visualizza informazioni sul rimborso per un reso

Puoi visualizzare informazioni sulle richieste di restituzione e sull&#39;elaborazione dei rimborsi dal [!UICONTROL Returns] dashboard.

1. Apri il dashboard Restituisce per l&#39;archivio dei canali di vendita.

   * Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Apri la vista Store selezionando l&#39;icona occhio per un negozio di canali di vendita.

   * Seleziona **[!UICONTROL Returns]**.

1. Visualizza gli ordini rimborsati selezionando la **[!UICONTROL Refunded]** scheda di stato.

1. Visualizza i dettagli del rimborso per un ritorno selezionando **[!UICONTROL View credit memo]**.

   ![Nota di credito per il rimborso degli articoli restituiti per un [!DNL Walmart Marketplace] ordine](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>Dopo il rimborso di un ordine, il [!UICONTROL Orders] il dashboard non mostra le informazioni di ritorno. Per visualizzare le informazioni di ritorno, utilizza [!DNL Channel Manager] Restituisce il dashboard. Informazioni più dettagliate su restituzione e rimborso sono disponibili anche nella pagina Dettagli ordine.

## Correggere gli errori di ritorno

Gli errori possono verificarsi quando si ricevono le informazioni di ritorno da [!DNL Walmart Marketplace]o quando [!DNL Channel Manager] sincronizza gli aggiornamenti di stato da [!DNL Commerce] a [!DNL Walmart Marketplace].

Se l&#39;operazione di sincronizzazione per un aggiornamento di ritorno non riesce, il [!DNL Channel Manager] Restituisce un dashboard *[!UICONTROL Error]* stato della voce di ritorno. Per garantire che le informazioni di restituzione e rimborso siano riportate con precisione nell&#39;account Marketplace Walmart, aggiorna manualmente l&#39;ordine nel tuo [!DNL Walmart Marketplace] archiviare.
