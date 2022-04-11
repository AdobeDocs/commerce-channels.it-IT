---
title: Gestire gli elenchi
description: Gestire gli elenchi dei canali di vendita per un [!DNL Commerce] archiviare con Channel Manager per Adobe Commerce e Magenti Open Source.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Gestisci elenchi

Gestire gli elenchi di prodotti per un canale connesso da [!UICONTROL Listings] nella visualizzazione archivio canali.

Utilizza la *[!UICONTROL Listings]* per gestire [!DNL Commerce] prodotti offerti in vendita su Walmart Marketplace. Lo stato di un singolo elenco indica dove si trova il prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere eventuali errori.

![Pagina inserzioni per un canale di vendita connesso](assets/products-submit-for-matching.png)

## Visualizza elenchi

1. Dall’amministratore, vai a [!UICONTROL **Marketing** > Canali > **Channel Manager**].

1. Dall&#39;elenco Store canali, seleziona l&#39;icona a forma di matita in una riga di voce dello store per aprire la visualizzazione store.

1. Seleziona [!UICONTROL **Elenco**].

## Aggiungere prodotti Commerce a Channel Manager

Completa le seguenti attività per creare l’assortimento di prodotti per il canale Marketplace Walmart:

* [Aggiungere prodotti dal catalogo di prodotti Commerce a Channel Manager](add-products-to-connected-channel.md)

* [Configurare la corrispondenza dei prodotti](map-product-attributes-for-matching.md#configure-product-attribute-settings)

## Pubblicare prodotti su Walmart

Puoi creare offerte di prodotti su Walmart Marketplace utilizzando la corrispondenza dei prodotti o caricando manualmente gli elenchi di prodotti per i nuovi prodotti. Per istruzioni, consulta [Pubblicare annunci su Walmart Marketplace](publish-listings-to-marketplace.md) come descritto nei seguenti argomenti:

* **[Prodotti abbinati su Walmart](publish-listings-to-marketplace.md)**- Pubblica gli elenchi dei prodotti dal tuo canale su [!DNL Walmart Marketplace] aggiornando gli elenchi esistenti che vendono lo stesso prodotto. I criteri di corrispondenza sono determinati dal [configurazione della mappatura degli attributi](map-product-attributes-for-matching.md) per il tuo canale.

* **[Carica manualmente le nuove inserzioni](publish-listings-to-marketplace.md#upload-new-product-listings)-**- Per i prodotti che non corrispondono a un elenco esistente su Walmart Marketplace, utilizza un modello Excel di categoria di prodotti Walmart per caricare in massa gli elenchi di prodotti.

## Controlli elenco e descrizioni dei campi

Le tabelle seguenti descrivono i controlli e i campi disponibili nel [!UICONTROL Listings] pagina.

**Controlli per[!UICONTROL Listings]**

| **Attributo** | **Livello del requisito** |
|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Refresh products] | Aggiorna la visualizzazione con l&#39;elenco e lo stato più aggiornati |
| [!UICONTROL Add Products ] | Apre la [!UICONTROL  Admin Product Catalog] per selezionare i prodotti da aggiungere al tuo [!DNL Walmart Marketplace] assortimento o per aggiornare gli attributi di prodotto per soddisfare i requisiti di elenchi di Walmart Marketplace. |
| [!UICONTROL Match products on Walmart] | Dopo aver selezionato uno o più prodotti in stato Bozza, seleziona [!UICONTROL Match products on Walmart] per verificare le offerte di prodotti che possono essere aggiunte a un [!DNL Walmart Marketplace] elenco. |


**Descrizioni delle colonne**

| **Campo** | **Descrizione** |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Nome del prodotto dal [!DNL Commerce] memorizzare il catalogo. |
| [!UICONTROL SKU (Unique ID)] | L’attributo mappato utilizzato per abbinare i prodotti sul marketplace. Il nome del campo varia a seconda della configurazione dell&#39;attributo mappata per [!DNL Channel Manager] elenchi. In questo caso, l’operazione di corrispondenza del prodotto utilizza la SKU del prodotto dal [!DNL Commerce] catalogo per trovare un [!DNL Walmart Marketplace]  Elenco con un valore SKU corrispondente al valore SKU degli attributi di prodotto Commerce. |
| [!UICONTROL  Quantity] | Quantità di scorte disponibili in Adobe Commerce o Magento Open Source. |
| [!UICONTROL Price] | Il prezzo del prodotto dal [!DNL Commerce] memorizzare il catalogo. Gli aggiornamenti dei prezzi del catalogo vengono sincronizzati in Channel Manager e quindi inviati a [!DNL Walmart Marketplace]  in modo che gli articoli elencati mostrino il prezzo corrente. |
| [!UICONTROL Status] | Indica lo stato corrente dell&#39;ordine nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando abbini prodotti sul mercato. Se un&#39;operazione non riesce, nell&#39;elenco viene visualizzato lo stato Error. Dopo aver corretto l&#39;errore, [!DNL Channel Manager] prova nuovamente l&#39;operazione e aggiorna lo stato. |


### Informazioni sullo stato dell’elenco

Nell’area di lavoro Elenco, l’etichetta Stato mostra dove si trova un prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere gli errori. Le inserzioni possono avere le seguenti etichette di stato:

* **[!UICONTROL Draft]**- Identifica i prodotti che non sono stati [presentata [!DNL Walmart] per corrispondenza](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**- Identifica i prodotti inviati per la corrispondenza sul [!DNL Walmart Marketplace]. I prodotti rimangono in *Elaborazione* fino al [!DNL Walmart] restituisce un messaggio di stato HTTP che indica se la corrispondenza è avvenuta correttamente o se si è verificato un errore. Possono essere necessari fino a 30 minuti per completare l&#39;operazione della partita sul [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifica i prodotti su cui è stata eseguita la corrispondenza [!DNL Walmart].

   Una corrispondenza si verifica quando il valore dell&#39;attributo del prodotto - Codice UPC per esempio - corrisponde al valore UPC in un[!DNL Walmart Marketplace] elenco. Quando un prodotto corrisponde, l’offerta Commerce viene aggiunta all’elenco esistente di Walmart.

   Controlla la [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard per esaminare l&#39;elenco dei prodotti aggiornato e verificare i dettagli dei prodotti, il prezzo e la quantità di scorte.


* **[!UICONTROL Error]**- Identifica i prodotti che non corrispondono a un esistente [!DNL Walmart Marketplace] elenco. Visualizzare i dettagli dell’errore passando il mouse sopra *Errore* etichetta di stato.

   Dopo aver risolto l’errore, invia nuovamente il prodotto per la corrispondenza. Vedi [Risolvere i problemi relativi agli errori di corrispondenza del prodotto](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.sz6eji8z9vzy).

* **[!UICONTROL Error - Match in Stage]**- Identifica i prodotti a cui corrispondono [!DNL Walmart] che non possono essere pubblicati fino al [!DNL Walmart Marketplace] il negozio è in diretta. I prodotti con questo stato vengono pubblicati automaticamente quando [!DNL Walmart Marketplace] il negozio va in diretta.
