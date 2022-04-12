---
title: Gestire gli ordini di Marketplace Walmart
description: Visualizza e gestisci [!DNL Walmart Marketplace] ordini con [!DNL Channel Manager] per Adobe Commerce e Magenti Open Source.
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 70f8b5487cf1c6507ce8e3cbaec91f4fc883d683
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gestire gli ordini di Marketplace Walmart

[!DNL Walmart Marketplace] ordini [!DNL Commerce] gli elenchi dei prodotti si sincronizzano automaticamente con [!DNL Channel Manager] dopo che Walmart elabora l&#39;ordine. Al termine della sincronizzazione, puoi visualizzare le informazioni sull’ordine selezionando **[!UICONTROL Orders]** dalla visualizzazione dell&#39;archivio canali collegata in [!DNL Channel Manager].

![Vista Ordini di Channel Manager per gestire gli ordini di Walmart Marketplace](assets/orders-dashboard-view.png)

>[!NOTE]
>
>Può richiedere fino a 35 minuti per un [!DNL Walmart Marketplace] per visualizzare nel [!DNL Channel Manager] elenco ordini. [!DNL Walmart] richiede circa 30 minuti per elaborare gli ordini in arrivo e inviarli a [!DNL Channel Manager].  Dopo che Channel Manager ha ricevuto l’ordine, ci vogliono altri 5 minuti per creare e visualizzare l’ordine in Adobe Commerce o Magento Open Source.

## Ordini di revisione

1. Dall’amministratore, seleziona **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** per aprire [!UICONTROL Channel Manager Marketplace Stores] pagina.

1. Apri la vista Store selezionando l&#39;icona a forma di matita in una riga di voce dello store.

1. Per visualizzare le informazioni sull&#39;ordine, selezionare *[!UICONTROL *Orders]**

## Visualizza dettagli ordine

Dopo aver ricevuto un ordine dal marketplace e importato in Adobe Commerce o nel Magento Open Source, utilizza [!DNL Commerce] ID ordine per visualizzare l’ordine in Adobe Commerce.

Da **[!UICONTROL Orders]**, seleziona [!UICONTROL Commerce Order Number] per aprire [!DNL Commerce]  dettaglio dell&#39;ordine.

![Visualizzazione dettagli ordine di Commerce per un ordine Marketplace Walmart](assets/order-detail-with-external-order-id.png)

### Controlli sugli ordini e descrizioni delle colonne

Le tabelle seguenti descrivono i controlli e le colonne disponibili per Ordini.

**Controlli per[!UICONTROL Orders]**
| **Controllo**                    | **Descrizione**                                                                                                                                               | |—|—| | [!UICONTROL Filter orders]     | Ordinare la visualizzazione selezionando una delle [!UICONTROL Order Status] carte.                                                                                        | | Dettagli messaggio di errore | Passa il puntatore del mouse [!UICONTROL Error Status] per visualizzare il messaggio di errore dettagliato.                                                                      | | [!UICONTROL View order detail] | Per visualizzare i dettagli dell&#39;ordine, seleziona la [!DNL Commerce] numero d&#39;ordine nel [!UICONTROL Order] tabella. Quindi, utilizza [!DNL Commerce] opzioni di ordine per elaborare l&#39;ordine. |

**Descrizioni delle colonne**

| Campo | Descrizione |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL  Walmart Order Number] | Numero dell&#39;ordine di acquisto assegnato all&#39;ordine nel [!DNL Walmart Marketplace]. Quando un ordine viene inizialmente importato in [!DNL Channel Manager], viene visualizzato solo il numero di ordine Walmart. Quando il [!DNL Commerce] l&#39;ordine viene creato, [!DNL Walmart] il numero dell&#39;ordine è memorizzato nel [!UICONTROL External ID] attributo di prodotto. |
| [!DNL Commerce]  Numero ordine | Il numero assegnato al [!DNL Commerce]  ordine creato da [!DNL Walmart Marketplace] ordine. |
| Elementi | Numero di elementi ordinati il [!DNL Walmart Marketplace]. |
| [!UICONTROL Order Value] | Costo totale degli articoli ordinati. |
| [!UICONTROL Date Created] | La data di creazione dell&#39;ordine nel [!DNL Walmart Marketplace]. |
| [!UICONTROL Ship By Date] | Data in cui l&#39;ordine deve essere spedito per soddisfare [!DNL Walmart Marketplace] requisiti. |
| [!UICONTROL Order Status] | Indica lo stato corrente dell&#39;ordine nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando abbini i prodotti [!DNL Walmart Marketplace]. Se un&#39;operazione non riesce, nell&#39;elenco viene visualizzato lo stato Error. Dopo aver corretto l&#39;errore, [!DNL Channel Manager] prova nuovamente l&#39;operazione e aggiorna lo stato. |

### Informazioni sullo stato dell’ordine

[!UICONTROL Order Status] fornisce informazioni sullo stato corrente di [!DNL Walmart Marketplace] ordini gestiti da Adobe Commerce o Magenti Open Source. Gli aggiornamenti dello stato dell&#39;ordine si verificano quando [!DNL Channel Manager] riceve informazioni aggiornate sull&#39;ordine da [!DNL Walmart Marketplace] o [!DNL Commerce] sistema d&#39;ordine. Gli ordini possono avere i seguenti stati:

* **[!UICONTROL Open]**-Ordini ricevuti da [!DNL Walmart Marketplace] pronto per essere rivisto ed elaborato in Adobe Commerce o Magenti Open Source.

   Dopo che un cliente ordina un prodotto dal [!DNL Walmart Marketplace], potrebbero essere necessari fino a 35 minuti perché l&#39;ordine aperto venga visualizzato nell&#39;area di lavoro dell&#39;ordine per il canale connesso. [!DNL Commerce] richiede circa 30 minuti per elaborare gli ordini in arrivo e inviarli a [!DNL Channel Manager]. Dopo che Channel Manager ha ricevuto l&#39;ordine, ci vogliono altri 5 minuti per creare e visualizzare il [!DNL Commerce] ordine.

* **[!UICONTROL Processed]**- Ordini spediti, annullati o rimborsati dal [!DNL Commerce] archiviare.

   Per visualizzare tutti gli ordini spediti, annullati e rimborsati, selezionare la **Elaborato** scheda di stato.

* **[!UICONTROL Canceled]**- Ordini annullati dal [!DNL Commerce] archiviare.

   Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace].

* **[!UICONTROL Refunded]**- Ordini rimborsati dal [!DNL Commerce] archiviare.

   Al termine del rimborso, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli rimborsati. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace].

* **[!UICONTROL Error]**- Ordini che non sono stati importati nell’archivio ordini a causa di informazioni mancanti o altri problemi.

   Per visualizzare i dettagli del messaggio di errore, passa il puntatore del mouse sul pulsante *[!UICONTROL Error]* indicatore di stato. Dopo aver risolto l’errore, l’ordine si aggiorna automaticamente per visualizzare le informazioni e lo stato correnti.
