---
title: Gestisci le inserzioni
description: 'Gestire le inserzioni del canale di vendita per uno store [!DNL Commerce] con Channel Manager per Adobe Commerce e Magento Open Source.'
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Gestisci le inserzioni

Gestisci gli elenchi prodotti per il canale di vendita [!DNL Walmart Marketplace] dall&#39;interfaccia utente di Channel Manager.

Lo stato di una singola inserzione indica dove si trova il prodotto nel flusso di lavoro [!DNL Channel Manager], in modo da poter determinare i passaggi successivi e risolvere eventuali errori.

![Pagina delle inserzioni per un canale di vendita connesso](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

È possibile completare le seguenti attività dalla visualizzazione Elenco.

* Visualizza le inserzioni in corso
* Ordina e filtra le inserzioni
* Aggiungi prodotti
* Corrispondenza prodotti
* Tracciare lo stato dell’inserzione
* Controlla la descrizione dell&#39;errore per le inserzioni con stato di errore

## Visualizza elenchi prodotti

1. Dall&#39;amministratore, vai a [!UICONTROL **Marketing** > **Channel Manager**].

1. Dall&#39;elenco Store, selezionare l&#39;icona a forma di occhio in una riga della voce del negozio per aprire la visualizzazione del negozio.

1. Seleziona [!UICONTROL **Inserzioni**].

1. Ordina la visualizzazione *Elenco* selezionando qualsiasi intestazione di colonna nella tabella *Elenco*.

1. Filtra la visualizzazione *Elenco* selezionando una delle schede di conteggio stato.

1. Reimpostare l&#39;ordinamento e rimuovere i filtri selezionando **Aggiorna prodotti**.

## Aggiungi [!DNL Commerce] prodotti a Channel Manager

Creare l&#39;assortimento di prodotti per il canale [!DNL Walmart Marketplace] completando le attività seguenti:

* [Aggiungi prodotti dal tuo  [!DNL Commerce] catalogo prodotti a [!DNL Channel Manager]](add-products-to-channel-store.md)

* [Mappa attributi catalogo](map-catalog-attributes.md#configure-product-attribute-settings)

## Corrispondenza prodotti su [!DNL Walmart]

Puoi creare offerte di prodotti su [!DNL Walmart Marketplace] utilizzando la corrispondenza dei prodotti o caricando manualmente gli elenchi di prodotti per i nuovi prodotti.

* **[Corrispondenza prodotti su Walmart](connect-listings-to-marketplace.md)**: collega gli elenchi di prodotti dal tuo canale a [!DNL Walmart Marketplace] aggiornando gli elenchi esistenti che vendono lo stesso prodotto. I criteri di corrispondenza sono determinati dalla [configurazione di mappatura attributi](map-catalog-attributes.md) per il tuo canale.

* **[Carica manualmente nuove inserzioni](connect-listings-to-marketplace.md#upload-new-product-listings)**. Per i prodotti che non corrispondono a un&#39;inserzione esistente in [!DNL Walmart Marketplace], utilizza un modello Excel di categoria di prodotto [!DNL Walmart] per caricare in blocco le inserzioni di prodotti.

## Controlli delle voci e descrizioni delle colonne

Nelle tabelle seguenti vengono descritti i controlli e le colonne disponibili per [!UICONTROL Listings].

**Controlli per[!UICONTROL Listings]**

| **Controllo** | **Descrizione** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Apre la pagina [!UICONTROL Admin Product Catalog] per selezionare i prodotti da aggiungere all&#39;assortimento [!DNL Walmart Marketplace] o per aggiornare gli attributi dei prodotti in modo da soddisfare i requisiti di inserzione di Walmart Marketplace. |
| [!UICONTROL Match products on Walmart] | Dopo aver selezionato uno o più prodotti nello stato [!UICONTROL Draft], selezionare [!UICONTROL Match products on Walmart] per verificare le offerte di prodotti che possono essere aggiunte a un&#39;inserzione [!DNL Walmart Marketplace] esistente. |
| [!UICONTROL Refresh products] | Aggiorna la visualizzazione con l’inserzione e lo stato più recenti. Questo controllo consente inoltre di ripristinare l&#39;ordinamento predefinito per la visualizzazione dell&#39;elenco e di rimuovere eventuali filtri. |
| [!UICONTROL Filter by *Stato*] | Mostra solo le inserzioni con uno stato specifico selezionando una delle schede di stato sopra la tabella delle inserzioni. Rimuovere il filtro selezionando **[!UICONTROL Refresh products]**. |
| [!UICONTROL Sort products] | Modifica l’ordinamento per l’inserzione selezionando un’intestazione di colonna. |


**Descrizioni colonne**

| **Campo** | **Descrizione** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Nome del prodotto dal catalogo dell&#39;archivio [!DNL Commerce]. |
| [!UICONTROL SKU (Unique ID)] | Lo SKU assegnato al prodotto nel catalogo [!DNL Commerce]. |
| [!UICONTROL  Quantity] | Quantità di scorte disponibili in Adobe Commerce o Magento Open Source. |
| [!UICONTROL Price] | Prezzo del prodotto dal catalogo dello store [!DNL Commerce]. Gli aggiornamenti dei prezzi del catalogo vengono sincronizzati in Channel Manager e quindi inviati a [!DNL Walmart Marketplace] in modo che gli elementi elencati mostrino il prezzo corrente. |
| [!UICONTROL Status] | Indica lo stato dell&#39;ordine corrente nel flusso di lavoro ordine [!DNL Commerce]. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando si abbinano prodotti sul marketplace. Se un’operazione non riesce, l’elenco mostra uno stato di errore. Dopo aver corretto l&#39;errore, [!DNL Channel Manager] ritenta l&#39;operazione e aggiorna lo stato. |
| [!UICONTROL Error Description] | Fornisce informazioni aggiuntive sull&#39;errore per i prodotti con stato `[!DNL Error]`. |

### Informazioni sullo stato delle inserzioni

Nell&#39;area di lavoro Elenco, l&#39;etichetta Stato mostra la posizione di un prodotto nel flusso di lavoro [!DNL Channel Manager], in modo da poter determinare i passaggi successivi e risolvere gli errori. Le inserzioni possono avere le seguenti etichette di stato:

* **[!UICONTROL Draft]**-Identifica prodotti che non sono stati [inviati a [!DNL Walmart] per corrispondenza](connect-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**: identifica i prodotti inviati per la corrispondenza in [!DNL Walmart Marketplace]. I prodotti rimangono nello stato *Elaborazione* finché [!DNL Walmart] non restituisce un messaggio di stato HTTP che indica se la corrispondenza è stata completata o se si è verificato un errore. Il completamento dell&#39;operazione di corrispondenza in [!DNL Walmart Marketplace] può richiedere fino a 30 minuti.

* **[!UICONTROL Match]**-Identifica i prodotti corrispondenti correttamente il [!DNL Walmart].

  Una corrispondenza si verifica quando il valore dell&#39;attributo del prodotto, ad esempio il codice UPC, corrisponde al valore UPC in un elenco [!DNL Walmart Marketplace] esistente. Quando un prodotto corrisponde, l’offerta di prodotto Commerce viene aggiunta all’elenco esistente.

  Controlla il dashboard [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) per esaminare l&#39;elenco dei prodotti aggiornato e verificare i dettagli dei prodotti, il prezzo e la quantità di magazzino.

* **[!UICONTROL Match - Match in Stage]** - Identifica i prodotti corrispondenti in [!DNL Walmart] che non possono essere connessi finché l&#39;archivio [!DNL Walmart Marketplace] non è attivo. I prodotti con questo stato si connettono automaticamente quando l&#39;archivio [!DNL Walmart Marketplace] diventa attivo.

* **[!UICONTROL Error]**: identifica i prodotti che non corrispondono a un&#39;inserzione [!DNL Walmart Marketplace] esistente.

* **[!UICONTROL Error description]** - Fornisce informazioni dettagliate sull&#39;errore dell&#39;elenco.

  Dopo aver risolto l’errore, invia nuovamente il prodotto per la corrispondenza. Consulta [Risoluzione dei problemi relativi agli errori di corrispondenza del prodotto](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
