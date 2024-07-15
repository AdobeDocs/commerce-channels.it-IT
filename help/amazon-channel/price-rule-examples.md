---
title: Canale di vendita Amazon - Esempi di regole di prezzo
description: Per aiutarti a progettare le regole di prezzo per le inserzioni Amazon, rivedi questi esempi in base a scenari comuni.
feature: Sales Channels, Price Rules
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# Esempi di regole di prezzo

## Esempi di regole di prezzo standard

### Elimina regole successive

La possibilità di scartare le regole successive è un&#39;ottima caratteristica all&#39;interno delle regole di determinazione dei prezzi che impedisce a più regole di determinazione dei prezzi di sovrapporsi e di fornire sconti aggiuntivi non intenzionali. Per ignorare le regole successive, una regola di determinazione dei prezzi deve utilizzare le priorità impostate nella sezione _[!UICONTROL Priority]_delle [Impostazioni generali regola determinazione prezzi](./pricing-rule-general-settings.md).

Se **[!UICONTROL Discard Subsequent Rules]** è impostato su `Yes`, le regole con priorità inferiore (numeri più alti) non si applicano ai prodotti idonei.

Ad esempio, supponiamo che ci siano tre regole di prezzo:

| Esempio | Nome regola | Priorità | Elimina regola successiva |
|---------|-----------------------|----------|-------------------------|
| 1 | 10% di sconto sui prodotti | 1 | No |
| 2 | Prodotti di sconto di $2 | 2 | Sì |
| 3 | 5% di sconto su tutti i prodotti | 3 | No |

In questo scenario, le regole #1 e #2 si applicano ai prodotti idonei. Il #3 di regole si applica solo ai prodotti idonei non contenuti nel #2 di regole perché ha una priorità inferiore rispetto al #2 di esempio e **[!UICONTROL Discard Subsequent Rules]** è impostato su `Yes`. Pertanto, i prodotti idonei nella categoria di vendita riceverebbero uno sconto del 10% e uno sconto di 2 dollari sul prezzo di vendita di Amazon.

### Applicazione di due regole di prezzo standard

| Campo | Impostazione - Regola 1 | Impostazione - Regola 2 |
|--------------------------------|---------------------|-----------------------|
| [!UICONTROL Rule Name] | Regola-1 | Articolo 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Regola prezzo standard | Regola prezzo standard |
| [!UICONTROL Price action] | Diminuisci di | Diminuisci di |
| [!UICONTROL Apply] | Applica come percentuale | Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Prodotto 1

Prezzo: $ 45,49

Regola 1 applicata: $45,49 x (0,9) = $40,94

Regola 2 applicata: $40,94 - $10,00 = $30,94

Viene applicato il prezzo finale dopo la regola 1 e la regola 2: $ 30,94

#### Prodotto 2

Prezzo: $ 47,76

Regola 1 applicata: $47,76 x (0,9) = $42,98

Regola 2 applicata: $42,98 - $10,00 = $32,98

Viene applicato il prezzo finale dopo la regola 1 e la regola 2: $ 32,98

## Esempi di regole di rideterminazione dei prezzi intelligenti

### Prezzo Buy Box con prezzo base Source = Prezzo

| Campo | Impostazione |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | Regola-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Usa prezzo &quot;Buy Box&quot; |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Corrispondenza |

#### Prodotto 1

Prezzo: $15

Prezzo [Buy Box](./buy-box-competitor-pricing.md) da Amazon: $10

Poiché il prezzo di [Buy Box](./buy-box-competitor-pricing.md) è inferiore al prezzo originale, il prodotto viene elencato al prezzo originale.

Il prezzo finale dopo l&#39;applicazione della regola: $15

#### Prodotto 2

Prezzo: $5

Prezzo [Buy Box](./buy-box-competitor-pricing.md) da Amazon: $10

Poiché il prezzo di [Buy Box](./buy-box-competitor-pricing.md) è maggiore del prezzo originale, il prodotto è elencato al prezzo di [Buy Box](./buy-box-competitor-pricing.md).

Prezzo finale dopo l&#39;applicazione della regola: $10

### Prezzo Buy Box con prezzo base Source = Prezzo e riduzione del prezzo del 20%

| Campo | Impostazione |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | Regola-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Usa prezzo &quot;Buy Box&quot; |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Diminuisci di |
| [!UICONTROL Apply] | Applica come percentuale |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Prodotto 1

Prezzo: $20

Prezzo base calcolato: $16

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $15

Poiché il prezzo di [Buy Box](./buy-box-competitor-pricing.md) è inferiore al prezzo di [base](./floor-price.md) calcolato, il prodotto è elencato al prezzo di [base](./floor-price.md) calcolato.

Il prezzo finale dopo l&#39;applicazione della regola: $16

#### Prodotto 2

Prezzo: $15

[Prezzo minimo](./floor-price.md) calcolato: $12

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $15

Poiché il prezzo di [Buy Box](./buy-box-competitor-pricing.md) è maggiore del prezzo di [base](./floor-price.md) calcolato, il prodotto è elencato al prezzo di [Buy Box](./buy-box-competitor-pricing.md).

Il prezzo finale dopo l&#39;applicazione della regola: $15

#### Prodotto 3

Prezzo: $17

Prezzo base calcolato: $13,60

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $15

Poiché il prezzo di [Buy Box](./buy-box-competitor-pricing.md) è maggiore del prezzo di [base](./floor-price.md) calcolato, il prodotto è elencato al prezzo di [Buy Box](./buy-box-competitor-pricing.md).

Il prezzo finale dopo l&#39;applicazione della regola: $15

### Prezzo più basso con tutti i prezzi della concorrenza e utilizzare tutte le condizioni di prodotto della concorrenza

| Campo | Impostazione |
|----------------------------------------|-----------------------------------------|
| [!UICONTROL Rule Name] | Regola-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Utilizza il prezzo concorrente più basso |
| [!UICONTROL Minimum Positive Feedback] | Tutti i prezzi della concorrenza |
| [!UICONTROL Conditional Variance] | Utilizzare tutte le condizioni di prodotto della concorrenza |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Corrispondenza |

| Prezzo | Condizione |
|-------|-----------------|
| $ 17 | Nuovo |
| $ 15 | Nuovo |
| $ 14 | Usato; Molto buono |
| $ 13 | Usato; buono |

#### Prodotto 1

Prezzo: $10

Condizione: nuova

Poiché il prezzo concorrente più basso per la nuova condizione è di 15 dollari, il prodotto è elencato a 15 dollari.

Il prezzo finale dopo l&#39;applicazione della regola: $15

#### Prodotto 2

Prezzo: $10

Condizione: Utilizzato; Accettabile

Poiché il [prezzo concorrente più basso](./lowest-competitor-pricing.md) per la condizione Usato è $13, il prodotto è elencato $13.

Il prezzo finale dopo l&#39;applicazione della regola: $13

### Regola di rideterminazione prezzi intelligente che combina prezzo massimo, conversione valuta e IVA

| Campo | Impostazione |
|-----------------------------------|---------------|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $ 10 |
| [!UICONTROL Currency conversion] | 1,25Euro:1USD |

[Prezzo massimo](./optional-ceiling-price.md) nel mercato europeo (IVA): $10 x 1,25 = $12,50

Quando viene raggiunto il [prezzo massimo](./optional-ceiling-price.md) nel mercato europeo (IVA), l&#39;IVA viene calcolata e aggiunta.

Prezzo finale al netto dell&#39;IVA: $12,50 x (1,1) = $13,75

### Combinazione di più regole di determinazione prezzi, prezzo massimo, conversione valuta e IVA

#### Regola di determinazione prezzi intelligente (dall’esempio precedente)

| Campo | Impostazione |
|----------------------|---------------|
| Priorità | 1 |
| IVA | 10% |
| Origine prezzo massimo | $ 10 |
| Conversione valuta | 1,25Euro:1USD |

[Prezzo massimo](./optional-ceiling-price.md) nel mercato europeo (IVA): $10 x 1,25 = $12,50

Prezzo finale al netto dell&#39;IVA: $12,50 x (1,1) = $13,75

#### Regola di determinazione prezzi standard

| Campo | Impostazione |
|--------------------------------|-----------------------|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Aumenta di |
| [!UICONTROL Apply] | Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | 5,00 $ |

Quando viene raggiunto il [prezzo massimo](./optional-ceiling-price.md), la regola di determinazione prezzi standard viene applicata in aggiunta alla regola di determinazione prezzi intelligente.

Prezzo finale dopo l&#39;applicazione della regola di determinazione prezzi standard: $13,75 + $5,00 = $18,75

### Rettifica prezzo

In questo esempio, il prezzo più competitivo viene definito osservando il [prezzo più basso del concorrente](./lowest-competitor-pricing.md) Amazon con un feedback positivo del 95% e un numero minimo di feedback pari a 1.000 recensioni.

![Esempio di rettifica prezzo](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

Dopo aver eseguito questa ricerca in base a questi parametri, il prezzo competitivo torna a 25 $.

Da qui, ci sono tre diverse [azioni regola prezzo](./pricing-rule-actions.md) scelte in base a questo prezzo più basso.

| Campo | Descrizione |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Questa opzione consente di diminuire il prezzo di vendita rispetto al [prezzo concorrente più basso](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - Questa opzione aumenta il prezzo di vendita rispetto al [prezzo concorrente più basso](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Questa opzione consente di modificare il prezzo di vendita di Amazon in modo che corrisponda al prezzo più basso in base ai parametri. Nell’esempio, il prezzo di vendita di Amazon è di $25.</li></ul> |
| [!UICONTROL Apply] | Opzioni: Applica come percentuale / Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | Valore numerico per definire la percentuale o l&#39;importo fisso per lo sconto da applicare. <br>Con queste selezioni si ottiene il prezzo più basso e si imposta il prezzo inferiore di $0,01. |

### Prezzo base

| Campo | Impostazione |
|--------------------------------------|---------------------|
| [!UICONTROL Floor Price Source] | Costo = $5 |
| [!UICONTROL Floor Price Action] | Aumenta di |
| [!UICONTROL Apply] | Applica come percentuale |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Calcolo prezzo minimo](./floor-price.md) = prezzo minimo Source `$5` x importo adeguamento minimo `5%` = $5,25

Quando viene applicata la regola di determinazione prezzi intelligente, il prezzo di listino non può essere inferiore a 5,25 $ per questo prodotto specifico quando il costo è di 5 $.
