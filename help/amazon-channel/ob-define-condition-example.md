---
title: "Esempio: definire una condizione"
description: Durante la creazione delle regole di inserzione, definisci le condizioni per identificare i prodotti del catalogo Commerce da elencare nel Marketplace Amazon.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# Esempio: definire una condizione

## Condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

**Non aggiungere condizioni se tutti i prodotti all’interno del sito web selezionato sono idonei.**

>[!NOTE]
>
>Esiste un set complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che stai tentando di elencare e a quanto potrebbero essere occupati i sistemi di Amazon (ad esempio il Black Friday), potrebbe volerci del tempo perché i tuoi elementi vengano elencati su Amazon.

Consulta la sezione Condizioni di [Creazione di una regola prezzo carrello](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){target="_blank"}.

## Definire una condizione

Questo processo può essere semplice o dettagliato, a seconda della configurazione del catalogo. È possibile impostare le condizioni in modo che quando `ALL` o `ANY` delle condizioni definite sono `TRUE` o `FALSE` per un prodotto, il prodotto può essere elencato su Amazon.

Le condizioni si basano sui valori degli attributi del prodotto esistenti. Per applicare la regola a tutti i prodotti, lascia vuota la sezione condizioni.

>[!NOTE]
>
>Se desideri definire una condizione basata su un attributo di prodotto specifico, imposta **[!UICONTROL Use for Promo Rule Conditions]** impostazione dell&#39;attributo su `Yes`. Puoi accedere a questa impostazione su [Proprietà vetrina](https://docs.magento.com/user-guide/catalog/product-attributes-add.html){target="_blank"} per l&#39;attributo.

![Condizione - riga 1](assets/ob-listing-rule-conditions-start.png)

La regola di questo esempio definisce una regola che imposta l’idoneità di Amazon per tutti i prodotti di catalogo che hanno _AMAZON FBA_ attributo impostato su `Yes`.

L&#39;istruzione della regola dispone di due collegamenti in grassetto che, se selezionati, consentono di visualizzare le opzioni per quella parte dell&#39;istruzione. Se salvi la condizione senza modificare un’opzione in grassetto, la regola si applica a tutti i prodotti.

- Clic **[!UICONTROL ALL]** e ha scelto `ALL` o `ANY`.
- Clic **[!UICONTROL TRUE]** e scegliere `TRUE` o `FALSE`.
- Per applicare la regola a tutti i prodotti, lascia invariata la condizione.

È possibile creare condizioni diverse modificando la combinazione di questi valori. In questo esempio, viene utilizzata la seguente condizione:

`If ALL of these conditions are TRUE:`

1. Fai clic sul pulsante Aggiungi (![Icona Aggiungi](assets/btn-add-grn.png)) all&#39;inizio della riga della condizione e selezionare un attributo su cui basare la condizione, ad esempio una combinazione di condizioni o un attributo di prodotto.

   - **[!UICONTROL Conditions Combination]** - Scegli di consentire la creazione di un altro set di `All/Any` e `True/False` all&#39;interno del set esistente.

      ![Combinazione di condizioni](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - Gli attributi del prodotto dipendono dall’impostazione dell’attributo. Affinché un attributo venga visualizzato nell’elenco, deve essere configurato per l’utilizzo nelle condizioni della regola promozionale. Consulta la _Usa per condizioni regola promozionale_ in [Attributi del prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"}.

      Nell’elenco in **[!UICONTROL Product Attribute]**, scegli l’attributo che desideri utilizzare come base della condizione. Per questo esempio, la condizione selezionata è `Amazon FBA`.

      ![Condizione riga 2, parte 2](assets/ob-condition-attribute-dropdown.png)

      La condizione selezionata viene visualizzata nell&#39;istruzione, seguita da altri due collegamenti in grassetto. Le opzioni variano a seconda dell’attributo di prodotto selezionato.

      L&#39;attributo impostato non può essere modificato. Per modificare l&#39;attributo, eliminare la riga e aggiungere il nuovo attributo. È possibile eliminare una riga di condizione facendo clic su Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.

      1. Clic **[!UICONTROL is]** e scegli l’operatore di confronto che descrive la condizione che i prodotti devono soddisfare.

         In questo esempio, l’operatore di confronto è `is`. Le opzioni disponibili dipendono dall’attributo selezionato nel passaggio precedente. Le opzioni possono includere diverse opzioni di confronto, ad esempio valori corrispondenti, che non includono o includono almeno uno di un valore, maggiore di, uguale e inferiore a un importo numerico. In questo esempio, le opzioni sono `is` e `is not`.

      1. Clic **[!UICONTROL ...]** e scegliere il valore di attributo su cui si basa la condizione.

         Le opzioni dipendono dalla configurazione dell’attributo. È possibile che venga richiesto di selezionare un&#39;opzione o di immettere testo o valori numerici per la condizione. In questo esempio, la selezione è `Yes`.

         L&#39;elemento selezionato viene visualizzato nell&#39;istruzione per completare la condizione.

         ![Condizione riga 2, parte 3](assets/ob-listing-rule-condition-is.png)
   Questa condizione è stata completata. Come indicato, questa condizione significa che qualsiasi prodotto nel [!DNL Commerce] catalogo con l’attributo FBA di Amazon impostato sul valore `Yes` può essere inserito nell’elenco di Amazon per la regione e il negozio. Puoi aggiungere altre righe di condizione per restringere ulteriormente i prodotti idonei.

1, Per aggiungere un&#39;altra riga di condizione all&#39;istruzione, tornare al passaggio 1 e ripetere il processo fino al completamento di tutte le condizioni desiderate.

È possibile eliminare una riga dell&#39;istruzione di condizione in qualsiasi momento facendo clic sul pulsante Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.
