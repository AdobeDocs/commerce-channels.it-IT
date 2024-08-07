---
title: Canale di vendita Amazon - [!UICONTROL Overrides]
description: Il Sales Channel Amazon fornisce la scheda Sostituzioni per aiutarti a identificare e gestire le modalità di applicazione delle sostituzioni nelle inserzioni Amazon.
feature: Sales Channels, Price Rules
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# [!UICONTROL Overrides]

La scheda _[!UICONTROL Overrides]_mostra le tue inserzioni Amazon alle quali hai applicato una sostituzione. Una sostituzione è un&#39;impostazione specifica dell&#39;elenco che può essere utilizzata per impostare un valore definito su un elenco. Un override applicato a un elenco definisce l&#39;impostazione per l&#39;elenco, indipendentemente da altre impostazioni o regole definite per l&#39;elenco per le quali l&#39;elenco è idoneo. Quando si applica una sostituzione a un&#39;inserzione, questa viene visualizzata nella scheda_[!UICONTROL Overrides]_. Il valore definito nella sostituzione viene visualizzato nella colonna appropriata per l&#39;elenco. È possibile applicare quattro tipi di sostituzioni: prezzo, tempo di gestione, condizione e note del venditore.

## Tipi di sostituzioni

| Tipo | Descrizione |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Prezzo | Sostituzione che imposta il prezzo dell&#39;inserzione, ignorando tutte le altre impostazioni relative al prezzo dell&#39;inserzione. <br><br>**Esempio**: hai definito una regola di prezzo di sconto del 20% che si applica a tutti i prodotti in una categoria specifica del catalogo. Hai un prodotto nuovo per il mercato e la domanda è elevata, quindi non desideri applicare il prezzo scontato all&#39;inserzione anche se il prodotto si trova in quella categoria. È possibile selezionare l&#39;inserzione, [creare una sostituzione del prezzo](./creating-editing-overrides.md#edit-override-single-listing) e definire il prezzo di vendita in una sostituzione del prezzo. |
| Tempo di imballaggio | Sostituzione che imposta il tempo di gestione per un&#39;inserzione, ignorando il tempo di gestione predefinito impostato nelle impostazioni dell&#39;inserzione.<br><br>**Esempio**: il tuo tempo di gestione predefinito per le inserzioni è impostato su 2 giorni. Hai un prodotto che è fragile e richiede un giorno in più per garantire il suo imballaggio speciale per la spedizione. È possibile visualizzare l&#39;elenco, [creare una sostituzione del tempo di gestione](./creating-editing-overrides.md#edit-override-single-listing) e definire il tempo di gestione in tre giorni.<br><br>**Nota:** non disponibile per i prodotti impostati su `Fulfilled by Amazon`. |
| Condizione | Sostituzione che imposta il valore della condizione di un elenco, indipendentemente dall&#39;attributo della condizione assegnato all&#39;elenco.<br><br>**Esempio**: la maggior parte dei prodotti nel catalogo è Nuova condizione, ma il prodotto è in stato Rinnovato. Puoi visualizzare l&#39;inserzione, [creare una sostituzione di condizione](./creating-editing-overrides.md#edit-override-single-listing) e definire la condizione Rinnovata per l&#39;inserzione.<br><br>**Nota:** non disponibile per i prodotti impostati su `Fulfilled by Amazon`. |
| Note del venditore | Sostituzione che definisce la sezione _Note del venditore_ dell&#39;inserzione. Questo campo può essere utilizzato per aggiungere informazioni aggiuntive relative al prodotto o alla sostituzione applicata, in genere utilizzata per descrivere la condizione di prodotti &quot;non nuovi&quot;. Il testo in questo campo viene visualizzato con l’elenco dell’acquirente. Impossibile aggiungere le note del venditore per un&#39;inserzione con valore di condizione `New`. <br><br>**Esempio**: un prodotto si trova nella condizione `Refurbished`. Normalmente i prodotti in queste condizioni non includono manuali o documenti, ma si dispone di un fornitore diverso per questo prodotto che include un manuale. Puoi visualizzare l&#39;inserzione, [creare una sostituzione delle note del venditore](./creating-editing-overrides.md#edit-override-single-listing), e aggiungere la tua nota di testo univoca a questa inserzione sul manuale in modo che l&#39;acquirente sappia che è incluso.<br><br>**Nota**: se un prodotto presenta una condizione definita di `New`, è possibile immettere una sostituzione delle note del venditore, ma Amazon non visualizza le note del venditore per un prodotto `New`. |

Puoi creare, modificare o rimuovere una sostituzione per una [singola inserzione](./creating-editing-overrides.md#edit-override-single-listing). Nelle schede _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ e _[!UICONTROL Ineligible]_è possibile fare clic su **[!UICONTROL Select]**nella colonna_[!UICONTROL Action]_ e scegliere **[!UICONTROL Create Override]**. L&#39;azione _[!UICONTROL Edit Overrides]_è disponibile solo quando a un&#39;inserzione è applicata una sostituzione ed è visualizzata nella scheda_[!UICONTROL Overrides]_.

È inoltre possibile creare, modificare o rimuovere una sostituzione per [più inserzioni](./creating-editing-overrides.md#edit-override-multiple-listings). Nelle schede _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ e _[!UICONTROL Ineligible]_è possibile fare clic su **[!UICONTROL Select]**nella colonna_[!UICONTROL Action]_ e scegliere **[!UICONTROL Edit Listing Overrides]**.

La rimozione di una sostituzione indica all’inserzione di utilizzare i valori definiti dalle impostazioni e dalle regole dell’inserzione.

Quando definite una sostituzione, potete anche scegliere di inserire un singolo tipo di sostituzione o una combinazione qualsiasi dei tipi.

Consulta [Creare e modificare le sostituzioni](./creating-editing-overrides.md).

>[!NOTE]
>
>Se sono presenti inserzioni in corso, il numero di inserzioni viene visualizzato in un messaggio sopra le schede.

![Scheda Sostituzioni](assets/amazon-overrides.png){width="600" zoomable="yes"}

Le home page del canale di vendita Amazon condividono alcuni [controlli dell&#39;area di lavoro](./workspace-controls.md) comuni che consentono di personalizzare i dati visualizzati.

## Colonne predefinite

| Colonna | Descrizione |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Lo SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN è l&#39;acronimo di Amazon Standard Identification Number. Un codice ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, il codice ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo codice ASIN al momento del caricamento dell&#39;elemento nel catalogo. Puoi trovare un codice ASIN nella pagina dei dettagli del prodotto di Amazon, insieme a ulteriori dettagli relativi all’elemento. |
| [!UICONTROL Condition Override] | La nuova condizione definita nell’override. Se la sostituzione applicata all&#39;elenco non è una sostituzione della condizione, `Not Selected` verrà visualizzato in questa colonna. |
| [!UICONTROL Product Listing Name] | Il nome del prodotto. |
| [!UICONTROL Seller Notes Override] | Le nuove note del venditore definite nella sostituzione. Se la sostituzione applicata all&#39;elenco non è di questo tipo, questa colonna è vuota. |
| [!UICONTROL Handling Override] | Il nuovo tempo di gestione definito nella sostituzione (in giorni). Se la sostituzione applicata all&#39;elenco non è una sostituzione del tempo di gestione, questa colonna è vuota. |
| [!UICONTROL List Price Override] | Il nuovo prezzo di vendita definito nella sostituzione. Se la sostituzione applicata all&#39;inserzione non è una sostituzione del prezzo, `N/A` viene visualizzato in questa colonna. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un&#39;azione, nella colonna _[!UICONTROL Action]_fare clic su **[!UICONTROL Select]**e scegliere un&#39;opzione:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
