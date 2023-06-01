---
title: Canale di vendita Amazon - Condizioni della regola di prezzo
description: Utilizzare le condizioni della regola del prezzo per determinare quali prodotti sono idonei per la regola del prezzo di listino.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Condizioni della regola di prezzo

Le condizioni determinano quali prodotti sono idonei per la regola del prezzo. La definizione delle condizioni per le regole di determinazione dei prezzi di Amazon segue la stessa logica e la stessa procedura utilizzata per definire le condizioni per [Regole prezzo carrello](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) in [!DNL Commerce].

>[!IMPORTANT]
>
>Se la regola dei prezzi si applica a tutti i prodotti nel [!DNL Commerce] , quindi lascia vuota questa sezione.

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

## Esempio: creare una condizione di regola di prezzo

Questo processo può essere semplice o dettagliato, a seconda della configurazione del catalogo. È possibile definire le condizioni in modo che quando `ALL` o `ANY` delle condizioni sono: `TRUE` o `FALSE` per un prodotto, il prodotto è idoneo per la regola di prezzo da applicare.

Le condizioni si basano su [attributi prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). Per applicare la regola a tutti i prodotti, lascia vuota la sezione condizioni.

>[!NOTE]
>
>Se desideri definire una condizione in base a un attributo di prodotto specifico, **Usa per condizioni regola promozionale** per l’attributo deve essere impostato su `Yes` nel tuo [Proprietà vetrina](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html) per l’attributo.

![Condizione regola prezzo - riga 1](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

Questo esempio definisce una regola che applica uno sconto del 25% a tutti i prodotti definiti nel `Books` categoria.

L’istruzione della regola dispone di due collegamenti in grassetto che, se cliccati, mostrano le opzioni per quella parte dell’istruzione della condizione. Se salvi la condizione senza modificare un’opzione in grassetto, la regola si applica a tutti i prodotti.

- Clic **[!UICONTROL ALL]** e scegliere `ALL` o `ANY`.
- Clic **[!UICONTROL TRUE]**, e scegliere `TRUE` o `FALSE`.
- Per applicare la regola a tutti i prodotti, lascia invariata la condizione.

È possibile creare condizioni diverse modificando la combinazione di questi valori. In questo esempio, viene utilizzata la seguente condizione:

`If ALL of these conditions are TRUE:`

1. Per visualizzare gli attributi disponibili a cui si applica la condizione, fare clic sul pulsante Aggiungi (![Icona Aggiungi](assets/btn-add-grn.png)) all&#39;inizio della riga della condizione e selezionare un attributo su cui basare la condizione.

   **[!UICONTROL Conditions Combination]** - Scegli di creare un altro set di `All/Any` e `True/False` condizioni all&#39;interno della condizione esistente.

   ![Combinazione di condizioni della regola di prezzo](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** : gli attributi di prodotto disponibili dipendono dal [impostazione dell’attributo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html). Per visualizzare un attributo nell&#39;elenco: *[!UICONTROL Use for Promo Rule Conditions]* per l’attributo deve essere impostato su `Yes` nelle proprietà della vetrina.

   - Per **[!UICONTROL Product Attribute]**, scegli l’attributo che desideri definire come base della condizione. Per questo esempio, la condizione selezionata è `Category`.

      ![Condizione regola prezzo - riga 2, parte 2](assets/ob-price-rule-condition-2.png){width="500"}

      La condizione selezionata viene visualizzata nell&#39;istruzione, seguita da altri due collegamenti in grassetto. Le opzioni variano a seconda dell’attributo di prodotto selezionato.

      Dopo aver impostato l&#39;attributo, non è possibile modificarlo. Per modificare l&#39;attributo, eliminare la riga e aggiungere il nuovo attributo. È possibile eliminare una riga di condizione facendo clic su Elimina (![Icona Elimina](assets/btn-del-red.png) alla fine della riga.

   - Clic **[!UICONTROL is]** e scegli l’operatore di confronto che descrive la condizione che i prodotti devono soddisfare.

      In questo esempio, l’operatore di confronto è `is`. Le opzioni disponibili dipendono dall’attributo selezionato nel passaggio precedente e possono includere diverse opzioni di confronto. Le opzioni possono includere valori corrispondenti, non includendo o includendo almeno uno di un valore, maggiore di, uguale e inferiore a un importo numerico. In questo esempio, le opzioni sono `is` e `is not`.

   - Clic **[!UICONTROL ...]** e scegliere il valore di attributo su cui si basa la condizione. Le opzioni dipendono dalla configurazione dell’attributo.

      Potrebbe essere richiesto di selezionare un&#39;opzione o di immettere un valore per la condizione. In questo esempio, il campo viene visualizzato vuoto. Per selezionare le categorie per la regola, fai clic sull’icona del selettore (![Icona selettore](assets/btn-chooser.png)) per visualizzare le opzioni selezionate. Questa regola è per _Libri_, seleziona la **[!UICONTROL Books]** casella di controllo. Il numero di categoria viene popolato. Per accettare le selezioni della categoria, fai clic sull’icona del segno di spunta verde (![Icona segno di spunta](assets/btn-check-mark-green.png)).

      ![Condizione regola prezzo - riga 2, parte 3](assets/ob-price-rule-condition-3.png){width="500"}

      L&#39;elemento selezionato viene visualizzato nell&#39;istruzione per completare la condizione.

      ![Condizione regola prezzo - riga 2, parte 4](assets/ob-price-rule-condition-4.png){width="500"}

      Questa condizione di esempio è completa. Come indicato, questa condizione significa che qualsiasi prodotto nel [!DNL Commerce] catalogo con una categoria di libri definita (`4`) è idoneo per questa regola tariffaria. Puoi aggiungere altre righe di condizione per restringere ulteriormente i prodotti idonei.

1. Per aggiungere un&#39;altra linea di condizione all&#39;istruzione, tornare al passo 1 e ripetere il processo fino al completamento di tutte le condizioni desiderate.

   È possibile eliminare una riga dell&#39;istruzione di condizione in qualsiasi momento facendo clic sul pulsante Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.
