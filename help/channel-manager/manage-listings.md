---
title: Gestisci ordini
description: Gestire gli elenchi dei canali di vendita per un [!DNL Commerce] archiviare con Channel Manager per Adobe Commerce e Magenti Open Source.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: f1a42dab1dbbc629ba01a4fcd8ade1052697d5a5
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Gestisci elenchi

Gestire gli elenchi di prodotti per un canale connesso da[!UICONTROL Listings] nella visualizzazione archivio canali.

L’area di lavoro Elenchi include i prodotti da elencare su Walmart Marketplace e fornisce gli strumenti per gestire gli elenchi. Lo stato di un singolo elenco mostra dove si trova il prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere gli errori.

![Pagina inserzioni per un canale di vendita connesso](assets/products-submit-for-matching.png)

## Visualizza elenchi

1. Dall’amministratore, vai a [!UICONTROL **Marketing** > Canali > **Channel Manager**].

1. Dall&#39;elenco Store canali, seleziona l&#39;icona a forma di matita in una riga di voce dello store per aprire la visualizzazione store.

1. Seleziona [!UICONTROL **Elenco**].


## Pubblicare prodotti su Walmart

Puoi creare offerte di prodotti su Walmart Marketplace utilizzando la corrispondenza dei prodotti o caricando manualmente gli elenchi di prodotti per i nuovi prodotti. Per istruzioni, consulta [Pubblicare annunci su Walmart Marketplace](publish-listings-to-marketplace.md) come descritto nei seguenti argomenti:

* **[Prodotti abbinati su Walmart](publish-listings-to-marketplace.md)**- Pubblica gli elenchi dei prodotti dal tuo canale su [!DNL Walmart Marketplace] aggiornando gli elenchi esistenti che vendono lo stesso prodotto. I criteri di corrispondenza sono determinati dal [configurazione della mappatura degli attributi](map-product-attributes-for-matching.md) per il tuo canale.

* **Carica manualmente le nuove inserzioni**- Per i prodotti che non corrispondono a un elenco esistente su Walmart Marketplace, utilizza un modello Excel di categoria di prodotti Walmart per caricare in massa gli elenchi di prodotti.

## Informazioni e controlli dell’elenco

**Controlli per[!UICONTROL Listings]**

| **Attributo** | **Livello del requisito** |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aggiorna prodotti | Aggiorna la visualizzazione con l&#39;elenco e i dati di stato più recenti. |
| Aggiungi prodotti | Apre la [!UICONTROL  Admin Product Catalog] per selezionare i prodotti da aggiungere al tuo [!DNL Walmart Marketplace] assortimento o per aggiornare gli attributi di prodotto per soddisfare i requisiti di elenchi di Walmart Marketplace. |
| Prodotti abbinati su Walmart | Dopo aver selezionato uno o più prodotti in stato Bozza, seleziona Confronta prodotti su Walmart per verificare la presenza di offerte di prodotti che possono essere aggiunte a un esistente[!DNL Walmart Marketplace] elenco. |


**Descrizioni delle colonne**

| **Campo** | **Descrizione** |
|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nome del prodotto | Nome del prodotto dal [!DNL Commerce] memorizzare il catalogo. |
| SKU (ID univoco) | L’attributo mappato utilizzato per abbinare i prodotti sul marketplace. Il nome del campo varia a seconda della configurazione dell&#39;attributo mappata per [!DNL Channel Manager] elenchi. In questo caso, l’operazione di corrispondenza del prodotto utilizza la SKU del prodotto dal [!DNL Commerce] catalogo per trovare un [!DNL Walmart Marketplace]  Elenco con un valore SKU corrispondente al valore SKU degli attributi di prodotto Commerce. |
| Quantità | Quantità di scorte disponibili in Adobe Commerce o Magento Open Source. |
| Prezzo | Il prezzo del prodotto dal [!DNL Commerce] memorizzare il catalogo. Gli aggiornamenti dei prezzi del catalogo vengono sincronizzati in Channel Manager e quindi inviati a [!DNL Walmart Marketplace]  in modo che gli articoli elencati mostrino il prezzo corrente. |
| Stato | Indica lo stato corrente dell&#39;ordine nel [!DNL Commerce] flusso di lavoro dell’ordine. Lo stato viene aggiornato quando si aggiungono correttamente prodotti a [!DNL Channel Manager] e quando abbini prodotti sul mercato. Se un&#39;operazione non riesce, nell&#39;elenco viene visualizzato lo stato Error. Dopo aver corretto l&#39;errore, [!DNL Channel Manager] prova nuovamente l&#39;operazione e aggiorna lo stato. |


### Informazioni sullo stato dell’elenco

Nell’area di lavoro Elenco, l’etichetta Stato mostra dove si trova un prodotto [!DNL Channel Manager] flusso di lavoro per determinare i passaggi successivi e risolvere gli errori. Stato del prodotto*.

* **[!UICONTROL Draft]**- Identifica i prodotti che non sono stati [presentata [!DNL Walmart] per corrispondenza](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**- Identifica i prodotti inviati per la corrispondenza sul [!DNL Walmart Marketplace]. I prodotti rimangono in *Elaborazione* fino al [!DNL Walmart Marketplace] restituisce un messaggio di stato HTTP che indica se la corrispondenza è avvenuta correttamente o se si è verificato un errore. Possono essere necessari fino a 30 minuti per completare l&#39;operazione della partita sul [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifica i prodotti che sono stati confrontati con successo su Walmart.

   Una corrispondenza si verifica quando il valore dell&#39;attributo del prodotto - Codice UPC per esempio - corrisponde al valore UPC in un[!DNL Walmart Marketplace] elenco. Quando un prodotto corrisponde, l’offerta Commerce viene aggiunta all’elenco esistente di Walmart.

   Controlla la [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) dashboard per esaminare l&#39;elenco dei prodotti aggiornato e verificare i dettagli dei prodotti, il prezzo e la quantità di scorte.


* **[!UICONTROL Error]**- Identifica i prodotti che non corrispondono a un esistente [!DNL Walmart Marketplace] elenco. Visualizzare i dettagli dell’errore passando il mouse sopra *Errore* etichetta di stato.

   Dopo aver risolto l’errore, invia nuovamente il prodotto per la corrispondenza. Vedi [Risolvere i problemi relativi agli errori di corrispondenza del prodotto](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.sz6eji8z9vzy).

* **[!UICONTROL Error - Match in Stage]**- Identifica i prodotti a cui corrispondono [!DNL Walmart] che non possono essere pubblicati fino al [!DNL Walmart Marketplace] il negozio è in diretta. I prodotti con questo stato vengono pubblicati automaticamente quando [!DNL Walmart Marketplace] il negozio va in diretta.
