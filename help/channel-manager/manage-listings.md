---
title: Gestisci elenchi
description: Gestire gli elenchi dei canali di vendita per un [!DNL Commerce] archiviare con Channel Manager per Adobe Commerce e Magenti Open Source.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 71ad5e3bc9ff6b909943a161472e4db7d375683f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# Gestire gli elenchi

Gestire gli elenchi dei prodotti per [!DNL Walmart Marketplace] canale di vendita dal [!UICONTROL Listings] nella visualizzazione archivio canali. Lo stato di un singolo elenco indica dove si trova il prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere eventuali errori.

Lo stato di un singolo elenco indica dove si trova il prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere eventuali errori.

![Pagina inserzioni per un canale di vendita connesso](assets/product-listing-landing.png)

È possibile completare le seguenti attività dalla vista Elenco.

* Visualizza elenchi correnti
* Ordinare e filtrare gli elenchi
* Aggiungi prodotti
* Prodotti abbinati
* Tracciare lo stato dell’elenco

## Visualizza elenchi prodotti

1. Dall’amministratore, vai a [!UICONTROL **Marketing** > Canali > **Channel Manager**].

1. Dall&#39;elenco Store canali, seleziona l&#39;icona a forma di matita in una riga di voce dello store per aprire la visualizzazione store.

1. Seleziona [!UICONTROL **Elenco**].

1. Ordinare *Elenco* seleziona un’intestazione di colonna nel *Elenco* tabella.

1. Filtrare *Elenco* seleziona una delle schede del conteggio di stato.

1. Ripristinare l’ordinamento e rimuovere i filtri selezionando **Aggiorna prodotti**.

## Aggiungere prodotti Commerce a Channel Manager

Crea l&#39;assortimento di prodotti per il canale Marketplace Walmart completando le seguenti attività:

* [Aggiungere prodotti dal catalogo di prodotti Commerce a Channel Manager](add-products-to-channel-store.md)

* [Mappare gli attributi del catalogo](map-catalog-attributes.md#configure-product-attribute-settings)

## Pubblicare prodotti su Walmart

Puoi creare offerte di prodotti su Walmart Marketplace utilizzando la corrispondenza dei prodotti o caricando manualmente gli elenchi di prodotti per i nuovi prodotti.

* **[Prodotti abbinati su Walmart](publish-listings-to-marketplace.md)**- Pubblica gli elenchi dei prodotti dal tuo canale su [!DNL Walmart Marketplace] aggiornando gli elenchi esistenti che vendono lo stesso prodotto. I criteri di corrispondenza sono determinati dal [configurazione di mappatura degli attributi](map-catalog-attributes.md) per il tuo canale.

* **[Carica manualmente le nuove inserzioni](publish-listings-to-marketplace.md#upload-new-product-listings)**- Per i prodotti che non corrispondono a un elenco esistente su Walmart Marketplace, utilizza un modello Excel di categoria di prodotti Walmart per caricare in massa gli elenchi di prodotti.

## Controlli elenco e descrizioni a colonne

Le tabelle seguenti descrivono i controlli e le colonne disponibili per [!UICONTROL Listings].

**Controlli per[!UICONTROL Listings]**

| **Controllo** | **Descrizione** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Apre la [!UICONTROL Admin Product Catalog] per selezionare i prodotti da aggiungere al tuo [!DNL Walmart Marketplace] assortimento o per aggiornare gli attributi di prodotto per soddisfare i requisiti di elenchi di Walmart Marketplace. |
| [!UICONTROL Match products on Walmart] | Dopo aver selezionato uno o più prodotti in stato Bozza, seleziona Confronta prodotti su Walmart per verificare la presenza di offerte di prodotti che possono essere aggiunte a un esistente [!DNL Walmart Marketplace] elenco. |
| [!UICONTROL Refresh products] | Aggiorna la visualizzazione con l&#39;elenco e lo stato più aggiornati. Questo controllo ripristina inoltre l&#39;ordinamento predefinito della visualizzazione elenco e rimuove eventuali filtri. |
| [!UICONTROL Filter by *Stato*] | Mostra solo gli elenchi con uno stato specifico selezionando una delle schede del conteggio di stato sopra la tabella Elenco. Utilizza la *Aggiorna prodotti* per rimuovere il filtro. |
| [!UICONTROL Sort products] | Per modificare l’ordinamento dell’elenco, seleziona un’intestazione di colonna. |


**Descrizioni delle colonne**

| **Campo** | **Descrizione** |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Nome del prodotto dal [!DNL Commerce] memorizzare il catalogo. |
| [!UICONTROL SKU (Unique ID)] | L’attributo mappato utilizzato per abbinare i prodotti sul marketplace. Il nome del campo varia a seconda della configurazione dell&#39;attributo mappata per [!DNL Channel Manager] elenchi. In questo caso, l’operazione di corrispondenza del prodotto utilizza la SKU del prodotto dal [!DNL Commerce] catalogo per trovare un [!DNL Walmart Marketplace]  Elenco con un valore SKU che corrisponde al valore SKU del [!DNL Commerce] attributi del prodotto. |
| [!UICONTROL  Quantity] | Quantità di scorte disponibili in Adobe Commerce o Magento Open Source. |
| [!UICONTROL Price] | Il prezzo del prodotto dal [!DNL Commerce] memorizzare il catalogo. Gli aggiornamenti dei prezzi del catalogo vengono sincronizzati in Channel Manager e quindi inviati a [!DNL Walmart Marketplace]  in modo che gli articoli elencati mostrino il prezzo corrente. |
| [!UICONTROL Status] | Indica lo stato corrente dell&#39;ordine nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando abbini prodotti sul mercato. Se un&#39;operazione non riesce, nell&#39;elenco viene visualizzato uno stato di errore. Dopo aver corretto l&#39;errore, [!DNL Channel Manager] prova nuovamente l&#39;operazione e aggiorna lo stato. |
| [!UICONTROL Status Detail] | Fornisce informazioni aggiuntive sui prodotti con *Errore* o *Corrispondenza* stato. |

### Informazioni sullo stato dell’elenco

Nell’area di lavoro Elenco, l’etichetta Stato mostra dove si trova un prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere gli errori. Le inserzioni possono avere le seguenti etichette di stato:

* **[!UICONTROL Draft]**- Identifica i prodotti che non sono stati [presentata [!DNL Walmart] per corrispondenza](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**- Identifica i prodotti presentati per la corrispondenza [!DNL Walmart Marketplace]. I prodotti rimangono in *Elaborazione* fino al [!DNL Walmart] restituisce un messaggio di stato HTTP che indica se la corrispondenza è avvenuta correttamente o se si è verificato un errore. Possono essere necessari fino a 30 minuti per completare l&#39;operazione della partita sul [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifica i prodotti su cui è stata eseguita la corrispondenza [!DNL Walmart].

   Una corrispondenza si verifica quando il valore dell&#39;attributo del prodotto, ad esempio il codice UPC, corrisponde al valore UPC in un[!DNL Walmart Marketplace] elenco. Quando un prodotto corrisponde, l’offerta Commerce viene aggiunta all’elenco esistente di Walmart.

   Controlla la [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard per esaminare l&#39;elenco dei prodotti aggiornato e verificare i dettagli dei prodotti, il prezzo e la quantità di scorte.

* **[!UICONTROL Match - Match in Stage]**- Identifica i prodotti a cui corrispondono [!DNL Walmart] che non possono essere pubblicati fino al [!DNL Walmart Marketplace] il negozio è in diretta. I prodotti con questo stato vengono pubblicati automaticamente quando [!DNL Walmart Marketplace] il negozio va in diretta.

* **[!UICONTROL Error]**- Identifica i prodotti che non sono stati confrontati con un esistente [!DNL Walmart Marketplace] elenco.

* **[!UICONTROL Error description]**- Fornisce informazioni dettagliate sull&#39;errore di inserimento nell&#39;elenco.

   Dopo aver risolto l’errore, invia nuovamente il prodotto per la corrispondenza. Vedi [Risolvere i problemi relativi agli errori di corrispondenza del prodotto](publish-listings-to-marketplace.md#troubleshoot-product-match-errors).
