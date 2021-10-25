---
title: Condizioni della regola del prezzo
description: Utilizza le condizioni della regola del prezzo per determinare quali prodotti sono idonei per la regola del prezzo di listino.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Condizioni della regola del prezzo

Le condizioni determinano quali prodotti sono ammissibili alla regola del prezzo. La definizione delle condizioni per le regole di determinazione dei prezzi di Amazon segue la stessa logica e lo stesso processo utilizzato per definire le condizioni per [Regole del prezzo del carrello](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} in [!DNL Commerce].

>[!IMPORTANT]
>
>Se la regola del prezzo si applica a tutti i prodotti nel tuo [!DNL Commerce] catalogo, quindi lasciare vuota questa sezione.

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

## Esempio: creare una condizione di regola del prezzo

Questo processo può essere semplice o dettagliato, a seconda della configurazione del catalogo. Puoi definire le tue condizioni in modo che quando `ALL` o `ANY` delle condizioni `TRUE` o `FALSE` per un prodotto, il prodotto è idoneo per la regola di prezzo da applicare.

Le condizioni sono basate sulle [attributi del prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Per applicare la regola a tutti i prodotti, lascia vuota la sezione condizioni.

>[!NOTE]
>
>Se desideri definire una condizione basata su un attributo di prodotto specifico, **Usa per le condizioni della regola promozionale** per l&#39;attributo deve essere impostato su `Yes` nel tuo [Proprietà Storefront](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;} per l&#39;attributo.

![Condizione della regola del prezzo - riga 1](assets/ob-price-rules-condition-1.png)

Questo esempio definisce una regola che applica uno sconto del 25% a tutti i prodotti definiti nella `Books` categoria.

L’istruzione della regola dispone di due collegamenti in grassetto, che, quando viene fatto clic su di essa, mostrano le opzioni per quella parte dell’istruzione della condizione. Se salvi la condizione senza modificare un’opzione in grassetto, la regola si applica a tutti i tuoi prodotti.

- Fai clic su **[!UICONTROL ALL]** e scegli `ALL` o `ANY`.
- Fai clic su **[!UICONTROL TRUE]**, e scegli `TRUE` o `FALSE`.
- Per applicare la regola a tutti i prodotti, lasciare invariata la condizione.

È possibile creare condizioni diverse modificando la combinazione di questi valori. Per questo esempio, viene utilizzata la seguente condizione:

`If ALL of these conditions are TRUE:`

1. Per visualizzare gli attributi disponibili per i quali si applica la condizione, fare clic sul pulsante Aggiungi (![Icona Aggiungi](assets/btn-add-grn.png)) all’inizio della riga della condizione e seleziona un attributo su cui basare la condizione.

   **[!UICONTROL Conditions Combination]** - Scegliere di creare un altro set di `All/Any` e `True/False` condizioni all&#39;interno della condizione esistente.

   ![Combinazione delle condizioni della regola del prezzo](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - Gli attributi di prodotto disponibili dipendono dal [impostazione dell&#39;attributo](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}. Affinché un attributo venga visualizzato nell&#39;elenco, *[!UICONTROL Use for Promo Rule Conditions]* per l&#39;attributo deve essere impostato su `Yes` nel tuo [proprietà della vetrina](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}.

   - Per **[!UICONTROL Product Attribute]**, scegli l’attributo da definire come base della condizione. In questo esempio, la condizione selezionata è `Category`.

      ![Condizione della regola del prezzo - linea 2, parte 2](assets/ob-price-rule-condition-2.png)

      La condizione selezionata viene visualizzata nell’istruzione, seguita da altri due collegamenti in grassetto. Le opzioni variano a seconda dell’attributo di prodotto selezionato.

      Dopo aver impostato l&#39;attributo, non è possibile modificarlo. Per modificare l’attributo, devi eliminare la riga e aggiungere il nuovo attributo. Per eliminare una riga di condizione, fai clic su Elimina (![Icona Elimina](assets/btn-del-red.png) alla fine della riga.

   - Fai clic su **[!UICONTROL is]** e scegli l’operatore di confronto che descrive la condizione per i prodotti da soddisfare.

      In questo esempio, l’operatore di confronto è `is`. Le opzioni disponibili dipendono dall’attributo selezionato nel passaggio precedente e possono includere opzioni di confronto diverse. Le opzioni possono includere valori corrispondenti, esclusi o inclusi almeno uno dei valori, e maggiore di, uguale o inferiore a un importo numerico. In questo esempio, le opzioni sono `is` e `is not`.

   - Fai clic su **[!UICONTROL ...]** e scegli il valore dell’attributo su cui si basa la condizione. Le opzioni dipendono dalla configurazione dell’attributo.

      Potrebbe essere richiesto di selezionare un’opzione o di immettere un valore per la condizione. In questo esempio, il campo viene visualizzato vuoto. Per selezionare le categorie per la regola, fai clic sull’icona del selettore (![Icona del selettore](assets/btn-chooser.png)) per visualizzare le opzioni di selezione. Questa regola è valida per _Libri_, seleziona **[!UICONTROL Books]** casella di controllo. Il numero della categoria viene compilato. Per accettare le selezioni della categoria, fai clic sull’icona del segno di spunta verde (![Icona a forma di segno di spunta](assets/btn-check-mark-green.png)).

      ![Condizione della regola del prezzo - linea 2, parte 3](assets/ob-price-rule-condition-3.png)

      L’elemento selezionato viene visualizzato nell’istruzione per completare la condizione.

      ![Condizione della regola del prezzo - linea 2, parte 4](assets/ob-price-rule-condition-4.png)

      Questa condizione di esempio è completa. Come indicato, questa condizione significa che qualsiasi prodotto nel tuo [!DNL Commerce] catalogo con una categoria definita di Libri (`4`) è idonea a questa regola di prezzo. Puoi aggiungere altre linee di condizione per limitare ulteriormente i prodotti idonei.

1. Per aggiungere un’altra riga di condizione all’istruzione, tornare al passaggio 1 e ripetere il processo fino al completamento di tutte le condizioni desiderate.

   È possibile eliminare una riga dell’istruzione della condizione in qualsiasi momento facendo clic su Elimina (![Icona Elimina](assets/btn-del-red.png)) alla fine della riga.
