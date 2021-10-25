---
title: Esempi di regole di prezzo
description: Per aiutarti a progettare le regole di determinazione dei prezzi per gli elenchi di Amazon, consulta questi esempi in base a scenari comuni.
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Esempi di regole di prezzo

## Esempi di regole di prezzo standard

### Ignora regole successive

La possibilità di ignorare le regole successive è una grande caratteristica all&#39;interno delle regole di determinazione dei prezzi che impedisce a più regole di determinazione dei prezzi di sovrapporsi e di fornire sconti aggiuntivi non intenzionali. Per eliminare le regole successive, una regola di determinazione dei prezzi deve utilizzare le priorità impostate in _[!UICONTROL Priority]_sezione [Impostazioni generali della regola di determinazione prezzi](./pricing-rule-general-settings.md).

Se **[!UICONTROL Discard Subsequent Rules]** è impostato su `Yes`, le norme con priorità inferiore (numeri più elevati) non si applicano ai prodotti ammissibili.

Ad esempio, supponiamo che ci siano tre regole di prezzo:

| Esempio | Nome della regola | Priorità | Elimina regola successiva |
|----------|----|----|----|
| 1 | 10% di prodotti in vendita | 1 | No |
| 2 | $2 prodotti in vendita | 2 | Sì |
| 3 | 5% di sconto su tutti i prodotti | 3 | No |

In questo scenario, la regola #1 e #2 si applica ai prodotti idonei. La regola n. 3 si applica solo ai prodotti idonei non inclusi nella regola n. 2 perché ha una priorità inferiore all&#39;esempio n. 2 e **[!UICONTROL Discard Subsequent Rules]** è impostato su `Yes`. Pertanto, i prodotti idonei nella categoria di vendita riceverebbero uno sconto del 10% e uno sconto di 2 dollari sul prezzo di listino di Amazon.

### Applicazione di due regole di prezzo standard

| Campo | Impostazione - Regola 1 | Impostazione - Regola 2 |
|----------|----|----|
| [!UICONTROL Rule Name] | Articolo 1 | Articolo 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Regola di prezzo standard | Regola di prezzo standard |
| [!UICONTROL Price action] | Diminuisci di | Diminuisci di |
| [!UICONTROL Apply] | Applica come percentuale | Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Prodotto 1

Prezzo: $ 45,49

Regola 1 applicata: $45,49 x (0,9) = $40,94

Regola 2 applicata: $40,94 - $10,00 = $30,94

Si applica il prezzo finale dopo l&#39;articolo 1 e l&#39;articolo 2: $ 30,94

#### Prodotto 2

Prezzo: $ 47,76

Regola 1 applicata: $47,76 x (0,9) = $42,98

Regola 2 applicata: $42,98 - $10,00 = $32,98

Si applicano il prezzo finale dopo la regola 1 e la regola 2: $ 32,98

## Esempi di regole di rideterminazione intelligente dei prezzi

### Prezzo Buy Box con prezzo base = Prezzo

| Campo | Impostazione |
|----------|----|
| [!UICONTROL Rule Name] | Articolo 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione dei prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Usa prezzo &quot;Buy Box&quot; |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Corrispondenza |

#### Prodotto 1

Prezzo: $ 15

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $ 10

Perché [Buy Box](./buy-box-competitor-pricing.md) prezzo inferiore al prezzo originale, il prodotto è elencato al prezzo originale.

Il prezzo finale dopo l&#39;applicazione della regola: $ 15

#### Prodotto 2

Prezzo: $5

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $ 10

Perché [Buy Box](./buy-box-competitor-pricing.md) il prezzo è maggiore del prezzo originale, il prodotto è elencato al [Buy Box](./buy-box-competitor-pricing.md) prezzo.

Il prezzo finale dopo l&#39;applicazione della regola: $ 10

### Prezzo Buy Box con Prezzo base Origine = Prezzo e una diminuzione del 20% del prezzo

| Campo | Impostazione |
|----------|----|
| [!UICONTROL Rule Name] | Articolo 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione dei prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Usa prezzo &quot;Buy Box&quot; |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Diminuisci di |
| [!UICONTROL Apply] | Applica come percentuale |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Prodotto 1

Prezzo: $ 20

Prezzo base calcolato: $ 16

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $ 15

Perché [Buy Box](./buy-box-competitor-pricing.md) prezzo inferiore a quello calcolato [Prezzo base](./floor-price.md), il prodotto è elencato nella sezione Calcolato [Prezzo base](./floor-price.md).

Il prezzo finale dopo l&#39;applicazione della regola: $ 16

#### Prodotto 2

Prezzo: $ 15

Calcolato [Prezzo base](./floor-price.md): $ 12

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $ 15

Perché [Buy Box](./buy-box-competitor-pricing.md) è maggiore del valore calcolato [Prezzo base](./floor-price.md), il prodotto è elencato nella [Buy Box](./buy-box-competitor-pricing.md) prezzo.

Il prezzo finale dopo l&#39;applicazione della regola: $ 15

#### Prodotto 3

Prezzo: $ 17

Prezzo base calcolato: $ 13,60

[Buy Box](./buy-box-competitor-pricing.md) prezzo da Amazon: $ 15

Perché [Buy Box](./buy-box-competitor-pricing.md) è maggiore del valore calcolato [Prezzo base](./floor-price.md), il prodotto è elencato nella [Buy Box](./buy-box-competitor-pricing.md) prezzo.

Il prezzo finale dopo l&#39;applicazione della regola: $ 15

### Prezzo più basso con tutti i prezzi della concorrenza e utilizzare tutte le condizioni di prodotto della concorrenza

| Campo | Impostazione |
|----------|-----|
| [!UICONTROL Rule Name] | Articolo 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Regola di rideterminazione dei prezzi intelligente |
| [!UICONTROL Competitor Price Source] | Utilizza il prezzo più basso della concorrenza |
| [!UICONTROL Minimum Positive Feedback] | Tutti i prezzi della concorrenza |
| [!UICONTROL Conditional Variance] | Utilizza tutte le condizioni di prodotto della concorrenza |
| [!UICONTROL Price Action] | Confronta prezzo concorrente |
| [!UICONTROL Floor Price Source] | Prezzo |
| [!UICONTROL Floor Price Action] | Corrispondenza |

| Prezzo | Condizione |
|----------|----|
| $ 17 | Nuovo |
| $ 15 | Nuovo |
| $ 14 | Utilizzato; Molto buono |
| $ 13 | Utilizzato; Buono |

#### Prodotto 1

Prezzo: $ 10

Condizione: Nuovo

Poiché il prezzo più basso della concorrenza per la nuova condizione è $15, il prodotto è elencato a $15.

Il prezzo finale dopo l&#39;applicazione della regola: $ 15

#### Prodotto 2

Prezzo: $ 10

Condizione: Utilizzato; Accettabile

Perché [prezzo concorrente più basso](./lowest-competitor-pricing.md) per la condizione Utilizzato è $13, il prodotto è elencato a $13.

Il prezzo finale dopo l&#39;applicazione della regola: $ 13

### Regola di rideterminazione intelligente dei prezzi che combina prezzo massimo, conversione della valuta e IVA

| Campo | Impostazione |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $ 10 |
| [!UICONTROL Currency conversion] | 1,25Euro:1USD |

[Prezzo massimo](./optional-ceiling-price.md) sul mercato europeo (IVA): $ 10 x 1,25 = $ 12,50

Quando il [prezzo massimo](./optional-ceiling-price.md) nel mercato europeo (IVA) è colpita, l&#39;IVA è calcolata e aggiunta.

Prezzo finale al netto dell&#39;IVA: $ 12,50 x (1,1) = $ 13,75

### Combinazione di più regole di prezzo, prezzo massimo, conversione di valuta e IVA

#### Regola di prezzo intelligente (dall&#39;esempio precedente)

| Campo | Impostazione |
|----------|----|
| Priorità | 1 |
| IVA | 10% |
| Prezzo a soffitto | $ 10 |
| Conversione in valuta | 1,25Euro:1USD |

[Prezzo massimo](./optional-ceiling-price.md) sul mercato europeo (IVA): $ 10 x 1,25 = $ 12,50

Prezzo finale al netto dell&#39;IVA: $ 12,50 x (1,1) = $ 13,75

#### Regola di prezzi standard

| Campo | Impostazione |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Aumenta di |
| [!UICONTROL Apply] | Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | $ 5,00 |

Quando il [prezzo massimo](./optional-ceiling-price.md) viene colpita, la regola di prezzo standard viene applicata oltre alla regola di prezzo intelligente.

Prezzo finale dopo l&#39;applicazione della regola di prezzo standard: $13,75 + $5,00 = $18,75

### Adeguamento del prezzo

In questo esempio, il prezzo più competitivo è definito guardando ad Amazon [il prezzo più basso del concorrente](./lowest-competitor-pricing.md) con un feedback positivo del 95% e un feedback minimo di 1.000 recensioni dei commercianti.

![Esempio di aggiustamento dei prezzi](assets/amazon-price-adjustment-example.png)

Dopo aver eseguito questa ricerca basata su questi parametri, il prezzo competitivo torna a $25.

Da qui ci sono tre diversi [azione della regola del prezzo](./pricing-rule-actions.md) scelte basate su questo prezzo più basso.

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Price Action] | Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Questa opzione diminuisce il prezzo di listino rispetto al [prezzo concorrente più basso](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - Questa opzione aumenta il prezzo dell&#39;inserzione rispetto al [prezzo concorrente più basso](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Questa opzione modifica il prezzo di listino di Amazon in modo che corrisponda al prezzo più basso in base ai parametri. Nell’esempio, il prezzo di listino di Amazon è di $25.</li></ul> |
| [!UICONTROL Apply] | Opzioni: Applica come percentuale / Applica come importo fisso |
| [!UICONTROL Adjustment Amount] | Valore numerico per definire la percentuale o l’importo fisso dello sconto da applicare. <br>Queste selezioni si traducono in prendere il prezzo più basso e impostarlo a $ 0,01 in meno. |

### Prezzo a virgola mobile

| Campo | Impostazione |
|----------|----|
| [!UICONTROL Floor Price Source] | Costo = $5 |
| [!UICONTROL Floor Price Action] | Aumenta di |
| [!UICONTROL Apply] | Applica come percentuale |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Prezzo a virgola mobile](./floor-price.md) calcolo = Origine prezzo base `$5` x Importo adeguamento piano `5%` = $5,25

Quando viene applicata la regola di prezzo intelligente, consente che il prezzo di listino sia inferiore a 5,25 $ per questo prodotto specifico quando il costo è di 5 $.
