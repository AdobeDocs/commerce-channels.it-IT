---
title: "Regola di tariffazione intelligente: varianze condizionali dei concorrenti"
description: Determina il prezzo dell’inserzione di Amazon in base ai prezzi della concorrenza e alle condizioni del prodotto creando una regola di rideterminazione intelligente dei prezzi.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Regola di tariffazione intelligente: varianze condizionali dei concorrenti

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Una regola di rideterminazione dei prezzi intelligente utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che mettono in vendita gli stessi prodotti che stai mettendo in vendita su Amazon.

Se esiste un prodotto con la stessa condizione, il prezzo di abbinamento di base è il [concorrente più basso](./lowest-competitor-pricing.md) alla stessa condizione. Se nessun prodotto concorrente soddisfa le tue condizioni, il prezzo di base della partita passa attraverso altre condizioni concorrenti disponibili a partire da Nuovo, Rinnovato e continuando verso il basso attraverso le condizioni disponibili. Una volta trovata una condizione, il prezzo di abbinamento di base sarà il prezzo più basso all&#39;interno di tale condizione.

Se hai un prodotto elencato con la condizione `Used; Good` e il prezzo base di abbinamento, e un concorrente ha lo stesso prodotto nella stessa condizione a un prezzo inferiore, viene utilizzato il prezzo concorrente. Se non esiste un concorrente con la stessa condizione, il sistema verifica la presenza di un concorrente con la condizione successiva, ovvero `New`. Se si trova un concorrente con tale condizione, viene utilizzato il prezzo più basso.

## Configurare le varianze condizionali del concorrente

Definire le varianze delle condizioni in _[!UICONTROL Competitor Conditional Variances]_sezione.

Per **[!UICONTROL Conditional Variance]**, scegli un’opzione:

- `Use all competitor's product conditions` - (Impostazione predefinita) Scegli quando vuoi che il prodotto venga confrontato con qualsiasi condizione disponibile (se non esiste una corrispondenza per la condizione che stai elencando).

- `Use Only Matching Competitor's Product Condition` - Scegliere quando si desidera che il prodotto sia confrontato solo con i prodotti della concorrenza che si trovano nella stessa condizione. Se non esiste alcuna corrispondenza, il prezzo del prodotto è fissato al _Origine prezzo Magento_ definito nel [Prezzo di vendita](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Scegli di iniziare il confronto con la condizione del prodotto corrispondente. Se non esiste alcuna condizione corrispondente, viene applicata una varianza (in percentuale) relativa alla condizione del prodotto e alla condizione del concorrente più basso.

   Quando _[!UICONTROL Apply Variance]_viene selezionata, vengono visualizzati campi di varianza aggiuntivi per ciascuna condizione Amazon. Questa funzione ti consente di utilizzare regole intelligenti di repricing quando offri prodotti in condizioni diverse da quelle della concorrenza. Per comprendere il calcolo alla base dello scostamento condizionale, è necessario innanzitutto comprendere che lo scostamento è determinato da un prezzo di abbinamento di base.

   Le opzioni di varianza condizionale visualizzate si basano sulle impostazioni dell&#39;inserzione per `Condition` mappati a valori di condizione utilizzando un [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}. Per tutte le condizioni mappate, puoi definire una percentuale di varianza da 1 a 100. L’eccezione è costituita dagli oggetti da collezione, nel qual caso può essere applicata una percentuale superiore a 100.

![Regola di rideterminazione prezzi intelligente: varianze condizionali del concorrente](assets/amazon-competitor-cond-variances.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | Opzioni: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Se non esiste una corrispondenza per la condizione con cui stai elencando il prodotto, questa opzione corrisponde a qualsiasi condizione disponibile. Tenta prima di tutto di soddisfare la tua condizione, e poi si fa strada dalla `New` condizione a `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Questa opzione corrisponde alle condizioni del prodotto. Se non esiste alcuna corrispondenza, i prezzi dei prodotti al _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Questa opzione cerca prima di impostare la condizione del prodotto. Se non esiste alcuna condizione corrispondente, applica una varianza (in percentuale) relativa alla condizione del prodotto e alla condizione del concorrente più basso.</li></ul><br><br>Le opzioni di varianza condizionale visualizzate in base alle impostazioni dell’inserzione per Condizione mappate ai valori della condizione utilizzando una [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}. Per tutte le condizioni mappate, è possibile indicare una percentuale di varianza compresa tra 1 e 100. L’eccezione è costituita dagli oggetti da collezione, nel qual caso può essere applicata una percentuale superiore a 100.<br><br>Questa funzione ti consente di utilizzare regole intelligenti di repricing quando offri prodotti in condizioni diverse da quelle della concorrenza. Per comprendere il calcolo alla base dello scostamento condizionale, è necessario innanzitutto comprendere che lo scostamento è determinato da un prezzo di abbinamento di base. |

## Calcola la base di varianza condizionale

- Scostamento condizione di corrispondenza di base (BMC) = Scostamento per la condizione del concorrente del prezzo di corrispondenza di base. Utilizzando l&#39;esempio precedente, BMC è la soluzione temporanea per `New` condizione.
- Varianza condizione commerciante (MCV) = Varianza della condizione del prodotto. Utilizzando l&#39;esempio precedente, MCV = la soluzione temporanea per `Used; Good` condizione.
- BMP = $7,99 (spiegato sopra)

La formula per il calcolo della base di varianza condizionale è la seguente:

![formula di calcolo della base per la varianza condizionale](assets/amazon-cond-variance-calc-1.png)

## Esempio

Le impostazioni della varianza condizionale sono le seguenti:

![esempio di impostazioni di varianza condizionale](assets/amazon-cond-variances.png)

- BMC = 100 (Condizione concorrente = Nuovo)
- MCV = 80 (condizione commerciante = utilizzato; buono)
- BMP = $7,99 (prezzo di abbinamento di base = prezzo più basso della condizione del concorrente corrispondente)

![esempio di calcolo base della varianza condizionale](assets/amazon-cond-variance-calc-2.png)

Utilizzando il calcolo della base di scostamento condizionale dall&#39;alto, la base di scostamento condizionale sarà pari a 6,39 dollari. Questo calcolo è l&#39;origine del prezzo del concorrente utilizzata per le azioni delle regole di prezzo, spiegata più avanti in [Adeguamento prezzo](./price-adjustment.md).
