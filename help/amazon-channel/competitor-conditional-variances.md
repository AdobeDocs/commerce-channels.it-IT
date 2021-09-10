---
title: '''Regola di rideterminazione intelligente dei prezzi: Varianze condizionali della concorrenza'
description: Determina il prezzo di listino di Amazon in base ai prezzi e alle condizioni della concorrenza del prodotto creando una regola di rideterminazione dei prezzi intelligente.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Regola di prezzo intelligente: varianze condizionali del concorrente

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Una regola di rideterminazione intelligente dei prezzi utilizza i prezzi dei concorrenti Amazon per determinare il prezzo del tuo annuncio. I concorrenti sono altri venditori che elencano gli stessi prodotti che stai inserendo in Amazon.

Se un prodotto esiste con la stessa condizione, il prezzo di corrispondenza di base è il prezzo [concorrente più basso](./lowest-competitor-pricing.md) con la stessa condizione. Se nessun prodotto concorrente corrisponde alla tua condizione, il prezzo di corrispondenza di base passa attraverso altre condizioni concorrenti disponibili a partire da Nuovo, Rinnovato e proseguendo nelle condizioni disponibili. Una volta trovata una condizione, il prezzo di corrispondenza di base sarà il prezzo più basso in quella condizione.

Se hai un prodotto elencato con la condizione `Used; Good` e il prezzo di corrispondenza di base, e un concorrente ha lo stesso prodotto nella stessa condizione a un prezzo inferiore, viene utilizzato il prezzo del concorrente. Se un concorrente non esiste con la stessa condizione, il sistema controlla un concorrente con la condizione successiva, che è `New`. Se un concorrente viene trovato con quella condizione, viene utilizzato il prezzo più basso.

## Configurare le varianze condizionali della concorrenza

Definisci le varianze di condizione nella sezione _[!UICONTROL Competitor Conditional Variances]_.

Per **[!UICONTROL Conditional Variance]**, scegli un’opzione:

- `Use all competitor's product conditions` - (Impostazione predefinita) Scegli quando desideri che il prodotto venga confrontato con qualsiasi condizione disponibile (se non esiste una corrispondenza per la condizione che stai inserendo).

- `Use Only Matching Competitor's Product Condition` - Scegli quando vuoi che il tuo prodotto venga confrontato solo con i prodotti della concorrenza nella stessa condizione. Se non esiste alcuna corrispondenza, il prezzo del prodotto è il _Prezzo Magento Origine_ definito nel [Prezzo di listino](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Scegli di provare prima a confrontare con la tua condizione di prodotto corrispondente. Se non esiste alcuna condizione di corrispondenza, viene applicata una varianza (in percentuale) relativa alla condizione del prodotto e alla condizione del concorrente più basso.

   Quando si seleziona la funzione _[!UICONTROL Apply Variance]_, vengono visualizzati campi di varianza aggiuntivi per ciascuna delle condizioni di Amazon. Questa funzione ti consente di utilizzare regole di rideterminazione dei prezzi intelligenti quando offri prodotti che si trovano in condizioni diverse da quelle dei tuoi concorrenti. Per comprendere il calcolo alla base della varianza condizionale, è innanzitutto necessario comprendere che tutta la varianza è determinata da un prezzo di corrispondenza di base.

   Le opzioni di varianza condizionale visualizzate si basano sulle impostazioni di elenco per `Condition` mappate ai valori di condizione utilizzando un [!DNL Commerce] [attributo di prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Per tutte le condizioni mappate, puoi definire una percentuale di varianza di 1-100. L&#39;eccezione è rappresentata dai collettori, nel qual caso può essere applicata una percentuale superiore a 100.

![Regola di rideterminazione intelligente dei prezzi - varianze condizionali dei concorrenti](assets/amazon-competitor-cond-variances.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | Opzioni: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Se non esiste una corrispondenza per la condizione con cui stai inserendo il prodotto, questa opzione corrisponde a qualsiasi condizione disponibile. In primo luogo tenta di corrispondere alla condizione e quindi si sposta dalla condizione `New` a `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Questa opzione corrisponde alle condizioni del prodotto. Se non esiste alcuna corrispondenza, i prezzi del prodotto sono fissati a _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Questa opzione cerca prima di tutto di corrispondere alla condizione del prodotto. Se non esiste alcuna condizione di corrispondenza, applica una varianza (in percentuale) relativa alla condizione del prodotto e alla condizione del concorrente più basso.</li></ul><br><br>Le opzioni di varianza condizionale visualizzate in base alle impostazioni di elenco per Condition mappate ai valori di condizione utilizzando un attributo  [!DNL Commerce] [prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. Per tutte le condizioni mappate, puoi indicare una percentuale di varianza di 1-100. L&#39;eccezione è rappresentata dai collettori, nel qual caso può essere applicata una percentuale superiore a 100.<br><br>Questa funzione ti consente di utilizzare regole di rideterminazione dei prezzi intelligenti quando offri prodotti che si trovano in condizioni diverse da quelle dei tuoi concorrenti. Per comprendere il calcolo alla base della varianza condizionale, è innanzitutto necessario comprendere che tutta la varianza è determinata da un prezzo di corrispondenza di base. |

## Calcolare la base della varianza condizionale

- BMC (Base Match Condition Variance) = La varianza per la condizione del tuo concorrente del prezzo di corrispondenza di base. Utilizzando l’esempio precedente, BMC è la varianza per la condizione `New` .
- Varianza condizione commerciante (MCV) = varianza per la condizione del prodotto. Utilizzando l’esempio precedente, MCV = la varianza per la condizione `Used; Good` .
- Base Match Price (BMP) = $7,99 (spiegato sopra)

La formula per calcolare la base della varianza condizionale è la seguente:

![formula di calcolo della base della varianza condizionale](assets/amazon-cond-variance-calc-1.png)

## Esempio

Le impostazioni di varianza condizionale sono le seguenti:

![impostazioni di varianza condizionale di esempio](assets/amazon-cond-variances.png)

- BMC = 100 (Concorrenza condizione = Nuovo)
- MCV = 80 (condizione del commerciante = Utilizzato; Bene)
- BMP = $7,99 (Prezzo di corrispondenza di base = Il prezzo più basso della condizione di concorrenza abbinata)

![esempio di calcolo della base della varianza condizionale](assets/amazon-cond-variance-calc-2.png)

Utilizzando il calcolo della base della varianza condizionale di cui sopra, la base della varianza condizionale = $6,39. Questo calcolo è l&#39;origine del prezzo concorrente utilizzata per le azioni della regola del prezzo, spiegato ulteriormente in [Adeguamento del prezzo](./price-adjustment.md).
