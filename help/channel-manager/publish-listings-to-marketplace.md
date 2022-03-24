---
title: Pubblicare annunci su Walmart
description: Pubblica annunci per i prodotti Commerce su Walmart Marketplace per iniziare a vendere.
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Pubblicare annunci su Walmart

Come altri mercati, Walmart consente ai venditori di terze parti di elencare gli articoli venduti da altri.

La piattaforma utilizza identificatori di prodotto come UPC e GTIN per abbinare gli articoli già in vendita.
Per i prodotti abbinati, l’elenco esistente di Walmart Marketplace viene aggiornato per includere l’offerta per il prodotto Commerce.
Di solito, i prodotti con i prezzi più bassi compaiono prima nei risultati. Ma anche altri fattori come le recensioni influenzano il posizionamento.

## Flusso di lavoro corrispondente

Quando si confrontano i prodotti, Channel Manager invia i dati del prodotto a Walmart Marketplace per cercare gli elenchi esistenti con valori di attributo che corrispondono all’attributo di prodotto Commerce mappato.

Se viene trovata una corrispondenza, l’elenco dei prodotti esistenti viene aggiornato per aggiungere la tua offerta.

## Prerequisiti

Prima di eseguire la corrispondenza con i prodotti, verifica che i valori degli attributi del catalogo dei prodotti soddisfino i requisiti di Walmart e configura le impostazioni degli attributi. Vedi [Configurare la corrispondenza dei prodotti](map-product-attributes-for-matching.md)

## Selezionare e abbinare i prodotti

1. Apri un canale di vendita collegato.

1. Da **[!UICONTROL Listings]**, seleziona i prodotti per la corrispondenza in *[!UICONTROL Draft]* stato.

   ![Seleziona i prodotti da inserzioni e invia per la corrispondenza](assets/products-in-marketplace-sales-channel.png)

1. Seleziona **[!UICONTROL Match Products]**.

   Un messaggio indica il numero di prodotti inviati per la corrispondenza.

   ![Inviare prodotti al canale di vendita collegato](assets/products-submit-for-matching.png)

   Per completare l&#39;operazione di match, Walmart Marketplace può richiedere fino a 30 minuti.

   Lo stato dei prodotti selezionati viene modificato in *[!UICONTROL Processing]* fino al completamento delle operazioni di abbinamento. Per completare l&#39;operazione di match, Walmart Marketplace può richiedere fino a 30 minuti.

## Verifica lo stato di corrispondenza

1. Seleziona **Aggiorna prodotti** per aggiornare lo stato del prodotto più recente.

1. Controlla lo stato del prodotto.

   Al termine della corrispondenza, lo stato può essere *Corrispondenza* o *Errore*.

   * **[!UICONTROL Match]** indica che la corrispondenza del prodotto è stata completata. L&#39;offerta di prodotto è stata pubblicata in un elenco esistente di Walmart Marketplace.

   * **[!UICONTROL Error]** indica una delle seguenti opzioni:

      * Si è verificato un errore e l&#39;operazione di corrispondenza non è riuscita.

      * Non è stata trovata alcuna corrispondenza.

      * Corrispondenza trovata, ma prodotto pubblicato come staging perché il [L&#39;archivio Marketplace non è attivo](walmart-prerequisites.md#walmart-marketplace-store-status).

## Risolvere i problemi relativi agli errori di corrispondenza del prodotto

Se l’operazione di corrispondenza del prodotto non riesce, Walmart Marketplace restituisce un codice di errore e Channel Manager visualizza lo stato di errore nelle informazioni di elenco del prodotto.

Visualizzare i dettagli dei messaggi di errore passando il mouse sopra **Errore** etichetta di stato. Gli errori comuni restituiti sono valori ID prodotto formattati in modo non corretto o attributi richiesti mancanti.

## Correggere i valori ID prodotto

| Tipo | Descrizione | Esempio |
|------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, il numero a 12 cifre, compresa la cifra di controllo.</br></br>Se l&#39;UPC ha meno di 12 cifre, ad esempio UPC-E a 8 cifre, aggiungi</br>gli zeri iniziali per soddisfare i requisiti. | Cambia da `45678912345` a `045678912345` |
| GTIN | GTIN-14, il numero a 14 cifre, compresa la cifra di controllo.</br></br>Se il valore GTIN è inferiore a 14 cifre, aggiungere zeri iniziali </br>per soddisfare il requisito. | Modifica `456789123456` a `0045678912345` |
| EAN | GTIN-13, il numero a 13 cifre, compresa la cifra di controllo.</br></br>Se l&#39;EAN ha meno di 13 cifre, aggiungi l&#39;interlinea</br>zero per soddisfare il requisito. | Cambia da `4567891234` a `0004567891234` |

Per informazioni dettagliate sui codici di errore di Walmart Marketplace, consulta la sezione [Aiuto per i venditori di Walmart](https://sellerhelp.walmart.com/s/guide?article=000005844).
