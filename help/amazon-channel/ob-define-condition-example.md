---
title: 'Esempio: Definire una condizione'
description: Quando crei le regole di inserzione, definisci le condizioni per identificare i prodotti del catalogo Commerce da elencare in Amazon Marketplace.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Esempio: Definire una condizione

## Condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

**Non aggiungere condizioni se tutti i prodotti all’interno del sito Web selezionato sono idonei.**

>[!NOTE]
>
>Esiste un insieme complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che si sta tentando di elencare e al livello di disponibilità dei sistemi Amazon (ad esempio il Black Friday), potrebbe essere necessario del tempo per elencare gli elementi in Amazon.

Consulta la sezione Condizioni di [Creazione di una regola del prezzo del carrello](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){target=&quot;_blank&quot;}.

## Definire una condizione

Questo processo può essere semplice o dettagliato, a seconda della configurazione del catalogo. È possibile impostare le condizioni in modo che quando `ALL` o `ANY` delle condizioni definite `TRUE` o `FALSE` per un prodotto, il prodotto è idoneo per essere elencato in Amazon.

Le condizioni si basano sui valori degli attributi del prodotto esistenti. Per applicare la regola a tutti i prodotti, lascia vuota la sezione condizioni.

>[!NOTE]
>
>Se desideri definire una condizione basata su un attributo di prodotto specifico, imposta la **[!UICONTROL Use for Promo Rule Conditions]** impostazione dell&#39;attributo su `Yes`. Puoi accedere a questa impostazione nella [Proprietà Storefront](https://docs.magento.com/user-guide/catalog/product-attributes-add.html)pagina {target=&quot;_blank&quot;} per l&#39;attributo.

![Condizione - riga 1](assets/ob-listing-rule-conditions-start.png)

La regola in questo esempio definisce una regola che imposta l’idoneità di Amazon per tutti i prodotti del catalogo che hanno _Amazon FBA_ attributo impostato su `Yes`.

L’istruzione della regola dispone di due collegamenti in grassetto, che, quando viene fatto clic su di essa, visualizzano le opzioni per quella parte dell’istruzione. Se salvi la condizione senza modificare un’opzione in grassetto, la regola si applica a tutti i tuoi prodotti.

- Fai clic su **[!UICONTROL ALL]** e ha scelto `ALL` o `ANY`.
- Fai clic su **[!UICONTROL TRUE]** e scegli `TRUE` o `FALSE`.
- Per applicare la regola a tutti i prodotti, lasciare invariata la condizione.

È possibile creare condizioni diverse modificando la combinazione di questi valori. Per questo esempio, viene utilizzata la seguente condizione:

`If ALL of these conditions are TRUE:`

1. Fai clic su Aggiungi (![Icona Aggiungi](assets/btn-add-grn.png)) all’inizio della riga della condizione e seleziona un attributo su cui basare la condizione, ad esempio una combinazione di condizioni o un attributo di prodotto.

   - **[!UICONTROL Conditions Combination]** - Scegli di consentire la creazione di un altro set di `All/Any` e `True/False` condizioni all&#39;interno del set esistente.

      ![Combinazione di condizioni](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - Gli attributi del prodotto dipendono dalla configurazione dell&#39;attributo. Affinché un attributo venga visualizzato nell’elenco, deve essere configurato per l’utilizzo nelle condizioni delle regole promozionali. Consulta la sezione _Usa per le condizioni della regola promozionale_ in [Attributi del prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

      Nell&#39;elenco in **[!UICONTROL Product Attribute]**, scegli l’attributo da utilizzare come base della condizione. In questo esempio, la condizione selezionata è `Amazon FBA`.

      ![Linea condizione 2, parte 2](assets/ob-condition-attribute-dropdown.png)

      La condizione selezionata viene visualizzata nell’istruzione, seguita da altri due collegamenti in grassetto. Le opzioni variano a seconda dell’attributo di prodotto selezionato.

      Dopo aver impostato l&#39;attributo, non può essere modificato. Per modificare l’attributo, devi eliminare la riga e aggiungere il nuovo attributo. Per eliminare una riga di condizione, fai clic su Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.

      1. Fai clic su **[!UICONTROL is]** e scegli l’operatore di confronto che descrive la condizione per i prodotti da soddisfare.

         In questo esempio, l’operatore di confronto è `is`. Le opzioni disponibili dipendono dall’attributo selezionato nel passaggio precedente. Le opzioni possono includere diverse opzioni di confronto, ad esempio valori corrispondenti, senza includere o includere almeno uno di un valore, e maggiore di, uguale o inferiore a un importo numerico. In questo esempio, le opzioni sono `is` e `is not`.

      1. Fai clic su **[!UICONTROL ...]** e scegli il valore dell’attributo su cui si basa la condizione.

         Le opzioni dipendono dalla configurazione dell’attributo. È possibile che venga richiesto di selezionare un’opzione o di immettere testo o valori numerici per la condizione. Per questo esempio, la selezione è `Yes`.

         L’elemento selezionato viene visualizzato nell’istruzione per completare la condizione.

         ![Linea condizione 2, parte 3](assets/ob-listing-rule-condition-is.png)
   Questa condizione è completa. Come indicato, questa condizione significa che qualsiasi prodotto nel tuo [!DNL Commerce] catalogo con l’attributo Amazon FBA impostato su un valore di `Yes` è idoneo all’inserimento in Amazon per l’area geografica e l’archivio. Puoi aggiungere altre linee di condizione per limitare ulteriormente i prodotti idonei.

1. Per aggiungere un&#39;altra riga di condizione all&#39;istruzione, tornare al punto 1 e ripetere il processo fino a quando tutte le condizioni desiderate non sono state completate.

È possibile eliminare una riga dell’istruzione della condizione in qualsiasi momento facendo clic su Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.
