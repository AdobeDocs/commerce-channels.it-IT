---
title: Gestisci le inserzioni
description: '''Gestire le inserzioni del canale di vendita per un [!DNL Commerce] archiviare con Channel Manager per Adobe Commerce e Magenti Open Source."'
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# Gestisci le inserzioni

Gestire gli elenchi di prodotti per [!DNL Walmart Marketplace] canale di vendita dall’interfaccia utente di Channel Manager.

Lo stato di una singola inserzione indica dove si trova il prodotto nel [!DNL Channel Manager] in modo da poter determinare i passaggi successivi e risolvere eventuali errori.

![Pagina delle inserzioni per un canale di vendita connesso](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

È possibile completare le seguenti attività dalla visualizzazione Elenco.

* Visualizza le inserzioni in corso
* Ordina e filtra le inserzioni
* Aggiungi prodotti
* Corrispondenza prodotti
* Tracciare lo stato dell’inserzione
* Controlla la descrizione dell&#39;errore per le inserzioni con stato di errore

## Visualizza elenchi prodotti

1. Dall’amministratore, vai a [!UICONTROL **Marketing** > **Channel Manager**].

1. Dall&#39;elenco Store, selezionare l&#39;icona a forma di occhio in una riga della voce del negozio per aprire la visualizzazione del negozio.

1. Seleziona [!UICONTROL **Inserzioni**].

1. Ordina *Elenco* visualizzare selezionando un&#39;intestazione di colonna nel *Elenco* tabella.

1. Filtra il *Elenco* visualizzare selezionando una delle schede di conteggio dello stato.

1. Reimpostare l&#39;ordinamento e rimuovere i filtri selezionando **Aggiorna prodotti**.

## Aggiungi [!DNL Commerce] prodotti per Channel Manager

Crea l’assortimento di prodotti per [!DNL Walmart Marketplace] canale completando le seguenti attività:

* [Aggiungi prodotti dal tuo [!DNL Commerce] catalogo prodotti a [!DNL Channel Manager]](add-products-to-channel-store.md)

* [Mappa attributi catalogo](map-catalog-attributes.md#configure-product-attribute-settings)

## Corrispondenza prodotti su [!DNL Walmart]

Puoi creare offerte di prodotti su [!DNL Walmart Marketplace] utilizzando la corrispondenza del prodotto o caricando manualmente gli elenchi di prodotti per i nuovi prodotti.

* **[Corrispondenza prodotti su Walmart](connect-listings-to-marketplace.md)**: collega gli elenchi di prodotti dal tuo canale a [!DNL Walmart Marketplace] aggiornando le inserzioni esistenti che vendono lo stesso prodotto. I criteri di corrispondenza sono determinati dal [configurazione mapping attributi](map-catalog-attributes.md) per il tuo canale.

* **[Carica manualmente le nuove inserzioni](connect-listings-to-marketplace.md#upload-new-product-listings)**- Per i prodotti che non corrispondono a un&#39;inserzione esistente [!DNL Walmart Marketplace], utilizza un [!DNL Walmart] modello di Excel della categoria di prodotti per caricare in blocco gli elenchi di prodotti.

## Controlli delle voci e descrizioni delle colonne

Nelle tabelle seguenti vengono descritti i controlli e le colonne disponibili per [!UICONTROL Listings].

**Controlli per[!UICONTROL Listings]**

| **Controllo** | **Descrizione** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Apre il [!UICONTROL Admin Product Catalog] pagina per selezionare i prodotti da aggiungere al [!DNL Walmart Marketplace] o per aggiornare gli attributi del prodotto in modo da soddisfare i requisiti di quotazione di Walmart Marketplace. |
| [!UICONTROL Match products on Walmart] | Dopo aver selezionato uno o più prodotti in [!UICONTROL Draft] stato, seleziona [!UICONTROL Match products on Walmart] per verificare la presenza di offerte di prodotti che possono essere aggiunte a un [!DNL Walmart Marketplace] elenco. |
| [!UICONTROL Refresh products] | Aggiorna la visualizzazione con l’inserzione e lo stato più recenti. Questo controllo consente inoltre di ripristinare l&#39;ordinamento predefinito per la visualizzazione dell&#39;elenco e di rimuovere eventuali filtri. |
| [!UICONTROL Filter by *Stato*] | Mostra solo le inserzioni con uno stato specifico selezionando una delle schede di stato sopra la tabella delle inserzioni. Rimuovere il filtro selezionando **[!UICONTROL Refresh products]**. |
| [!UICONTROL Sort products] | Modifica l’ordinamento per l’inserzione selezionando un’intestazione di colonna. |


**Descrizioni delle colonne**

| **Campo** | **Descrizione** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Nome del prodotto da [!DNL Commerce] catalogo del negozio. |
| [!UICONTROL SKU (Unique ID)] | Lo SKU assegnato al prodotto nel [!DNL Commerce] catalogo. |
| [!UICONTROL  Quantity] | Quantità di scorte disponibili in Adobe Commerce o Magenti Open Source. |
| [!UICONTROL Price] | Il prezzo del prodotto dal [!DNL Commerce] catalogo del negozio. Gli aggiornamenti dei prezzi del catalogo vengono sincronizzati in Channel Manager e quindi inviati a [!DNL Walmart Marketplace]  in modo che gli articoli elencati mostrino il prezzo corrente. |
| [!UICONTROL Status] | Indica lo stato dell&#39;ordine corrente nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando i prodotti si abbinano sul mercato. Se un’operazione non riesce, l’elenco mostra uno stato di errore. Dopo aver corretto l’errore, [!DNL Channel Manager] ritenta l&#39;operazione e aggiorna lo stato. |
| [!UICONTROL Error Description] | Fornisce informazioni di errore aggiuntive per i prodotti con `[!DNL Error]` stato. |

### Informazioni sullo stato delle inserzioni

Nell’area di lavoro dell’inserzione, l’etichetta Stato mostra la posizione di un prodotto nell’area [!DNL Channel Manager] in modo da poter determinare i passaggi successivi e risolvere gli errori. Le inserzioni possono avere le seguenti etichette di stato:

* **[!UICONTROL Draft]**-Identifica i prodotti che non sono stati [inviato a [!DNL Walmart] per corrispondenza](connect-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**- Identifica i prodotti inviati per l&#39;abbinamento nel [!DNL Walmart Marketplace]. I prodotti rimangono in *Elaborazione* fino al [!DNL Walmart] restituisce un messaggio di stato HTTP che indica se la corrispondenza è stata stabilita correttamente o se si è verificato un errore. Il completamento dell&#39;operazione di abbinamento sul [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**-Identifica i prodotti con corrispondenza riuscita il [!DNL Walmart].

  Una corrispondenza si verifica quando il valore dell’attributo del prodotto, ad esempio il codice UPC, corrisponde al valore UPC in un [!DNL Walmart Marketplace] elenco. Quando un prodotto corrisponde a, l’offerta di prodotto Commerce viene aggiunta all’elenco esistente.

  Controlla la [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard per esaminare l’elenco dei prodotti aggiornato e verificare i dettagli dei prodotti, il prezzo e la quantità di magazzino.

* **[!UICONTROL Match - Match in Stage]**- Identifica i prodotti con corrispondenza [!DNL Walmart] che non può essere connesso fino al [!DNL Walmart Marketplace] il negozio è in diretta. I prodotti con questo stato si connettono automaticamente quando [!DNL Walmart Marketplace] il negozio entra in funzione.

* **[!UICONTROL Error]**- Identifica i prodotti che non corrispondono a un [!DNL Walmart Marketplace] elenco.

* **[!UICONTROL Error description]**- Fornisce informazioni dettagliate sull&#39;errore dell&#39;elenco.

  Dopo aver risolto l’errore, invia nuovamente il prodotto per la corrispondenza. Consulta [Risolvere i problemi relativi agli errori di corrispondenza prodotto](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
