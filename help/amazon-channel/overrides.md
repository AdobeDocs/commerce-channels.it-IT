---
title: Sostituzioni
description: Amazon Sales Channel fornisce la scheda Ignorare per identificare e gestire in modo più efficace l’applicazione delle sostituzioni negli elenchi Amazon.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Sostituzioni

La scheda _[!UICONTROL Overrides]_mostra gli elenchi Amazon a cui è stata applicata una sostituzione. Una sostituzione è un’impostazione specifica per un elenco che può essere utilizzata per impostare un valore definito su un elenco. Una sostituzione applicata a un elenco definisce l’impostazione per l’elenco, indipendentemente da altre impostazioni o regole di elenco definite per le quali l’elenco è idoneo. Quando a un elenco viene applicata una sostituzione, l’elenco viene visualizzato nella scheda_[!UICONTROL Overrides]_ . Il valore definito nella sostituzione viene visualizzato nella colonna appropriata per l’elenco. È possibile applicare quattro tipi di sostituzioni: Prezzo, tempo di gestione, condizioni e note del venditore.

## Tipi di sostituzioni

| Tipo | Descrizione |
|---|---|
| Prezzo | Sostituzione che imposta il prezzo dell&#39;inserzione, ignorando tutte le altre impostazioni di prezzo per l&#39;inserzione. <br><br>**Esempio**: Hai definito una regola del prezzo di sconto del 20% che si applica a tutti i prodotti in una categoria specifica del tuo catalogo. Hai un prodotto che è nuovo sul mercato e la domanda è alta, quindi non vuoi il prezzo scontato applicato alla quotazione anche se il prodotto è in quella categoria. È possibile selezionare l&#39;inserzione, [creare un prezzo alternativo](./creating-editing-overrides.md#edit-override-single-listing) e definire il prezzo dell&#39;inserzione in un prezzo alternativo. |
| Tempo di gestione | Sostituzione che imposta il tempo di gestione per un elenco, ignorando il tempo di gestione predefinito impostato nelle impostazioni di elenco.<br><br>**Esempio**: Il tempo di gestione predefinito per le inserzioni è impostato su 2 giorni. Hai un prodotto che è fragile e richiede un giorno extra per garantire il suo imballaggio speciale per la spedizione. È possibile visualizzare l&#39;elenco, [creare un override del tempo di gestione](./creating-editing-overrides.md#edit-override-single-listing) e definire il tempo di gestione in tre giorni.<br><br>**Nota:** non disponibile per i prodotti impostati su  `Fulfilled by Amazon`. |
| Condizione | Sostituzione che imposta il valore della condizione di un elenco, indipendentemente dall&#39;attributo della condizione assegnato all&#39;elenco.<br><br>**Esempio**: La maggior parte dei prodotti nel catalogo sono condizione Nuova, ma si dispone di un prodotto in condizioni Rinnovato. È possibile visualizzare l&#39;elenco, [creare una condizione override](./creating-editing-overrides.md#edit-override-single-listing) e definire la condizione Rinnovato per l&#39;elenco.<br><br>**Nota:** non disponibile per i prodotti impostati su  `Fulfilled by Amazon`. |
| Note sul venditore | Sostituzione che definisce la sezione _Note venditore_ dell&#39;elenco. Questo campo può essere utilizzato per aggiungere informazioni aggiuntive relative al prodotto o alla sostituzione applicata, generalmente utilizzato per descrivere la condizione dei prodotti &quot;non nuovi&quot;. Il testo in questo campo viene visualizzato insieme all&#39;elenco per l&#39;acquirente. Non è possibile aggiungere note per un annuncio con un valore di condizione `New`. <br><br>**Esempio**: Hai un prodotto in  `Refurbished` condizioni. Normalmente i prodotti in questa condizione non includono manuali o documenti, ma si dispone di un fornitore diverso per questo prodotto che include un manuale. È possibile visualizzare l&#39;elenco, [creare una nota di vendita override](./creating-editing-overrides.md#edit-override-single-listing) e aggiungere la nota di testo univoca a questa inserzione sul manuale in modo che l&#39;acquirente sappia che è incluso.<br><br>**Nota**: Se un prodotto presenta una condizione definita di  `New`, puoi immettere una sostituzione delle note di vendita, ma Amazon non visualizza le note di vendita per un  `New` prodotto. |

Puoi creare, modificare o rimuovere un override per un [singolo elenco](./creating-editing-overrides.md#edit-override-single-listing). Nelle schede _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ e _[!UICONTROL Ineligible]_, puoi fare clic su **[!UICONTROL Select]**nella colonna_[!UICONTROL Action]_ e scegliere **[!UICONTROL Create Override]**. L’azione _[!UICONTROL Edit Overrides]_è disponibile solo quando un elenco ha un’esclusione applicata e viene visualizzato nella scheda_[!UICONTROL Overrides]_ .

È inoltre possibile creare, modificare o rimuovere un override per [più elenchi](./creating-editing-overrides.md#edit-override-multiple-listings). Nelle schede _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ e _[!UICONTROL Ineligible]_, puoi fare clic su **[!UICONTROL Select]**nella colonna_[!UICONTROL Action]_ e scegliere **[!UICONTROL Edit Listing Overrides]**.

La rimozione di una sostituzione indica all&#39;elenco di utilizzare i valori definiti dalle impostazioni e dalle regole dell&#39;elenco.

Quando definisci un override, puoi anche scegliere di immettere un singolo tipo di override o qualsiasi combinazione dei tipi.

Consulta [Creare e modificare sostituzioni](./creating-editing-overrides.md).

>[!NOTE]
>
>Se sono presenti elenchi in corso, il numero di elenchi viene visualizzato in un messaggio posto sopra le schede.

![Scheda Sostituzioni](assets/amazon-overrides.png)

Le home page del canale di vendita Amazon condividono alcuni controlli comuni [workspace](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

## Colonne predefinite

| Colonna | Descrizione |
|---|---|
| [!UICONTROL Amazon Seller SKU] | SKU (Stock Keeping Unit) assegnato da Amazon a un prodotto per identificare il prodotto, le opzioni, il prezzo e il produttore. |
| [!UICONTROL ASIN] | Un blocco univoco di 10 lettere e/o numeri che identificano gli elementi.<br><br>ASIN sta per numeri di identificazione standard Amazon. Un ASIN è un blocco univoco di 10 lettere e/o numeri che identificano gli elementi. Per i libri, l&#39;ASIN è uguale al numero ISBN, ma per tutti gli altri prodotti viene creato un nuovo ASIN quando l&#39;articolo viene caricato sul loro catalogo. Puoi trovare un articolo ASIN nella pagina dei dettagli del prodotto su Amazon, insieme a ulteriori dettagli relativi all’articolo. |
| [!UICONTROL Condition Override] | La nuova condizione definita nell&#39;override. Se la sostituzione applicata all’elenco non è una sostituzione di condizione, `Not Selected` viene visualizzata in questa colonna. |
| [!UICONTROL Product Listing Name] | Nome del prodotto. |
| [!UICONTROL Seller Notes Override] | Le nuove note sul venditore definite nella sostituzione. Se la sostituzione applicata all&#39;elenco non è questo tipo di sostituzione, questa colonna è vuota. |
| [!UICONTROL Handling Override] | Il nuovo tempo di gestione definito nell&#39;override (in giorni). Se la sostituzione applicata all&#39;elenco non è una sostituzione del tempo di gestione, questa colonna è vuota. |
| [!UICONTROL List Price Override] | Il nuovo prezzo di listino definito nella sostituzione. Se la sostituzione applicata all&#39;inserzione non è una sostituzione del prezzo, `N/A` viene visualizzata in questa colonna. |
| [!UICONTROL Action] | Elenco delle azioni disponibili che possono essere applicate a un elenco specifico. Per applicare un’azione, nella colonna _[!UICONTROL Action]_fai clic su **[!UICONTROL Select]**e scegli un’opzione:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
