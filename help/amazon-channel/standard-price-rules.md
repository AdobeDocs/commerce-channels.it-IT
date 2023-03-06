---
title: Azioni di regole di prezzo standard
description: Utilizza le azioni della regola di prezzo standard per aumentare o diminuire un prezzo di listino di Amazon relativo al prezzo di catalogo Commerce (o origine prezzo).
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Azioni di regole di prezzo standard

Un&#39;azione di regola di prezzo standard ti consente di aumentare o diminuire un prezzo di inserzione di Amazon di una percentuale specifica o di un importo in dollari fisso relativo al [!DNL Commerce] prezzo di catalogo (o origine prezzo).

Le sezioni di un&#39;azione di una regola di prezzo standard includono:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Configurare le azioni delle regole di prezzo

1. Per **[!UICONTROL Rule Type]**, scegli `Standard price rule`.

   Questa opzione disattiva gli altri campi nel _[!UICONTROL Select Rule Type]_sezione.

1. Espandi _[!UICONTROL Price Adjustment]_sezione, se necessario.

1. Per **[!UICONTROL Price Action]**, scegli un’opzione per determinare come desideri modificare il *[!UICONTROL Magento Price Source]* (definito nel [Prezzo di vendita](./listing-price.md)).

   - `Decrease By` : scegli quando vuoi ridurre il valore prima di inserirlo nell’elenco di Amazon.

   - `Increase By` : scegli quando desideri che il valore venga aumentato prima di inserirlo nell’elenco di Amazon.

1. Per **[!UICONTROL Apply]**, scegli un’opzione e un’opzione per determinare come definire *[!UICONTROL Magento Price Source]* definito nel [Prezzo di vendita](./listing-price.md) valore da regolare:

   - `Apply as percentage` - Scegli quando vuoi definire *[!UICONTROL Magento Price Source]* definito nel [Prezzo di vendita](./listing-price.md) valore adeguato di una percentuale

   - `Apply as fixed amount` - Scegli quando vuoi definire *[!UICONTROL Magento Price Source]* definito nel [Prezzo di vendita](./listing-price.md) valore rettificato da un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), inserire il valore numerico per l&#39;adeguamento del prezzo.

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as percentage`, inserisci il valore percentuale (esempio: invio `25` per un adeguamento di prezzo del 25%).

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as fixed amount`, immettere il valore numerico per l&#39;importo fisso (ad esempio: invio `25` per un adeguamento del prezzo fisso di 25 dollari).

1. Al termine, fai clic su **[!UICONTROL Save pricing rule]**.

![Regola prezzo standard](assets/ob-price-rule-action-standard-example.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Rule Type] | Seleziona `Standard price rule`. |
| [!UICONTROL Price Action] | Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi definire [!DNL Commerce] il valore dell’origine del prezzo deve essere diminuito prima di essere inserito nell’elenco di Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando vuoi definire [!DNL Commerce] valore di origine del prezzo da aumentare prima di inserirlo in Amazon.</li></ul> |
| [!UICONTROL Apply] | Opzioni:<ul><li>**[!UICONTROL Apply as percentage]** - Scegli quando vuoi definire [!DNL Commerce] valore origine prezzo rettificato in percentuale.</li><li>**[!UICONTROL Apply as fixed amount]** - Scegli quando vuoi definire [!DNL Commerce] valore origine prezzo rettificato da un importo fisso.</li></ul> |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br><br>Se si sceglie `Apply as percentage` per *[!UICONTROL Apply]*, inserisci il valore percentuale (esempio: invio `25` per un adeguamento del 25%).<br><br>Se si sceglie `Apply as fixed amount` per *[!UICONTROL Apply]*, immettere il valore numerico per l&#39;importo fisso (ad esempio: invio `25` per un adeguamento fisso di 25 dollari). |
