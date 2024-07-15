---
title: "Esempio: definire una condizione per le regole di elenco di Amazon"
description: Durante la creazione delle regole di inserzione, definisci le condizioni per identificare i prodotti del catalogo Commerce da elencare sul Marketplace Amazon.
feature: Sales Channels, Products, Configuration
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Esempio: definire una condizione

## Condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

**Non aggiungere condizioni se tutti i prodotti all&#39;interno del sito Web selezionato sono idonei.**

>[!NOTE]
>
>Esiste un set complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che stai tentando di elencare e a quanto potrebbero essere occupati i sistemi di Amazon (ad esempio il Black Friday), potrebbe volerci del tempo perché i tuoi elementi vengano elencati su Amazon.

Consulta la sezione Condizioni di [Creazione di una regola prezzo carrello](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html).

## Definire una condizione

Questo processo può essere semplice o dettagliato, a seconda della configurazione del catalogo. È possibile impostare le condizioni in modo che, quando `ALL` o `ANY` delle condizioni definite sono `TRUE` o `FALSE` per un prodotto, il prodotto sia idoneo per essere elencato in Amazon.

Le condizioni si basano sui valori degli attributi del prodotto esistenti. Per applicare la regola a tutti i prodotti, lascia vuota la sezione condizioni.

>[!NOTE]
>
>Per definire una condizione basata su un attributo di prodotto specifico, impostare l&#39;impostazione **[!UICONTROL Use for Promo Rule Conditions]** per l&#39;attributo su `Yes`. Puoi accedere a questa impostazione nella pagina [Proprietà storefront](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) dell&#39;attributo.

![Condizione - riga 1](assets/ob-listing-rule-conditions-start.png){width="500"}

La regola in questo esempio definisce una regola che imposta l&#39;idoneità di Amazon per tutti i prodotti del catalogo con l&#39;attributo _Amazon FBA_ impostato su `Yes`.

L&#39;istruzione della regola dispone di due collegamenti in grassetto che, se selezionati, consentono di visualizzare le opzioni per quella parte dell&#39;istruzione. Se salvi la condizione senza modificare un’opzione in grassetto, la regola si applica a tutti i prodotti.

- Fare clic su **[!UICONTROL ALL]** e scegliere `ALL` o `ANY`.
- Fare clic su **[!UICONTROL TRUE]** e scegliere `TRUE` o `FALSE`.
- Per applicare la regola a tutti i prodotti, lascia invariata la condizione.

È possibile creare condizioni diverse modificando la combinazione di questi valori. In questo esempio, viene utilizzata la seguente condizione:

`If ALL of these conditions are TRUE:`

1. Fare clic sull&#39;icona Aggiungi (![icona Aggiungi](assets/btn-add-grn.png)) all&#39;inizio della riga della condizione e selezionare un attributo su cui basare la condizione, ad esempio una combinazione di condizioni o un attributo di prodotto.

   - **[!UICONTROL Conditions Combination]** - Consente di creare un altro set di condizioni `All/Any` e `True/False` all&#39;interno del set esistente.

     ![Combinazione di condizioni](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - Gli attributi del prodotto dipendono dalla configurazione dell&#39;attributo. Affinché un attributo venga visualizzato nell’elenco, deve essere configurato per l’utilizzo nelle condizioni della regola promozionale. Vedi _Utilizza per le condizioni della regola promozionale_ in [Attributi del prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

     Nell&#39;elenco in **[!UICONTROL Product Attribute]**, scegliere l&#39;attributo che si desidera utilizzare come base della condizione. Per questo esempio, la condizione selezionata è `Amazon FBA`.

     ![Riga di condizione 2, parte 2](assets/ob-condition-attribute-dropdown.png){width="350"}

     La condizione selezionata viene visualizzata nell&#39;istruzione, seguita da altri due collegamenti in grassetto. Le opzioni variano a seconda dell’attributo di prodotto selezionato.

     L&#39;attributo impostato non può essere modificato. Per modificare l&#39;attributo, eliminare la riga e aggiungere il nuovo attributo. È possibile eliminare una riga di condizione facendo clic sull&#39;icona Elimina (![icona Elimina](assets/btn-del-red.png)) alla fine della riga.

      1. Fare clic su **[!UICONTROL is]** e scegliere l&#39;operatore di confronto che descrive la condizione per i prodotti da soddisfare.

         In questo esempio, l&#39;operatore di confronto è `is`. Le opzioni disponibili dipendono dall’attributo selezionato nel passaggio precedente. Le opzioni possono includere diverse opzioni di confronto, ad esempio valori corrispondenti, che non includono o includono almeno uno di un valore, maggiore di, uguale e inferiore a un importo numerico. In questo esempio, le opzioni sono `is` e `is not`.

      1. Fare clic su **[!UICONTROL ...]** e scegliere il valore di attributo su cui si basa la condizione.

         Le opzioni dipendono dalla configurazione dell’attributo. È possibile che venga richiesto di selezionare un&#39;opzione o di immettere testo o valori numerici per la condizione. In questo esempio, la selezione è `Yes`.

         L&#39;elemento selezionato viene visualizzato nell&#39;istruzione per completare la condizione.

         ![Riga di condizione 2, parte 3](assets/ob-listing-rule-condition-is.png){width="500"}

   Questa condizione è stata completata. Come indicato, questa condizione significa che qualsiasi prodotto nel catalogo [!DNL Commerce] con l&#39;attributo FBA di Amazon impostato su un valore di `Yes` può essere inserito nell&#39;elenco di Amazon per l&#39;area geografica e lo store. Puoi aggiungere altre righe di condizione per restringere ulteriormente i prodotti idonei.

1, Per aggiungere un&#39;altra riga di condizione all&#39;istruzione, tornare al passaggio 1 e ripetere il processo fino al completamento di tutte le condizioni desiderate.

È possibile eliminare una riga dell&#39;istruzione di condizione in qualsiasi momento facendo clic sull&#39;icona Elimina (![icona Elimina](assets/btn-del-red.png)) alla fine della riga.
