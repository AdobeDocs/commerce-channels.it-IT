---
title: Azioni della regola di prezzo standard
description: Utilizza le azioni delle regole di prezzo standard per aumentare o diminuire un prezzo di listino di Amazon relativo al prezzo di catalogo (o all’origine del prezzo) Commerce.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Azioni standard sulle regole di prezzo

Un’azione standard di regola del prezzo ti consente di aumentare o diminuire un prezzo di listino Amazon di una percentuale specifica o di un importo fisso del dollaro rispetto a [!DNL Commerce] prezzo di catalogo (o fonte di prezzo).

Le sezioni di un&#39;azione standard di regola dei prezzi includono:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Configurare le azioni relative alle regole di prezzo

1. Per **[!UICONTROL Rule Type]**, scegli `Standard price rule`.

   Questa opzione disattiva gli altri campi nel _[!UICONTROL Select Rule Type]_sezione .

1. Espandi la _[!UICONTROL Price Adjustment]_se necessario.

1. Per **[!UICONTROL Price Action]**, scegli un’opzione per determinare come modificare la *[!UICONTROL Magento Price Source]* (definito nella [Prezzo di listino](./listing-price.md)).

   - `Decrease By` - Scegli quando vuoi che il valore venga ridotto prima di essere inserito nell’elenco di Amazon.

   - `Increase By` - Scegli quando aumentare il valore prima di inserirlo in Amazon.

1. Per **[!UICONTROL Apply]**, scegli un&#39;opzione e un&#39;opzione per determinare come vuoi definire *[!UICONTROL Magento Price Source]* definiti nella [Prezzo di listino](./listing-price.md) valore da rettificare:

   - `Apply as percentage` - Scegli quando vuoi definire *[!UICONTROL Magento Price Source]* definiti nella [Prezzo di listino](./listing-price.md) valore rettificato in percentuale

   - `Apply as fixed amount` - Scegli quando vuoi definire *[!UICONTROL Magento Price Source]* definiti nella [Prezzo di listino](./listing-price.md) valore rettificato da un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), immettere il valore numerico per l&#39;adeguamento del prezzo.

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as percentage`, inserisci il valore percentuale (esempio: enter `25` per un aggiustamento dei prezzi del 25%).

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as fixed amount`, immettere il valore numerico dell&#39;importo fisso (ad esempio: enter `25` per un adeguamento a prezzo fisso di 25 $).

1. Al termine, fai clic su **[!UICONTROL Save pricing rule]**.

![Regola di prezzo standard](assets/ob-price-rule-action-standard-example.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Rule Type] | Seleziona `Standard price rule`. |
| [!UICONTROL Price Action] | Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi definire [!DNL Commerce] il valore della fonte del prezzo da ridurre prima di inserirlo in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando vuoi definire [!DNL Commerce] valore della fonte del prezzo da aumentare prima di inserirlo in Amazon.</li></ul> |
| [!UICONTROL Apply] | Opzioni:<ul><li>**[!UICONTROL Apply as percentage]** - Scegli quando vuoi definire [!DNL Commerce] valore alla fonte del prezzo rettificato in percentuale.</li><li>**[!UICONTROL Apply as fixed amount]** - Scegli quando vuoi definire [!DNL Commerce] valore di origine del prezzo rettificato da un importo fisso.</li></ul> |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br><br>Se scegli `Apply as percentage` per *[!UICONTROL Apply]*, inserisci il valore percentuale (esempio: enter `25` per un aggiustamento del 25%).<br><br>Se hai scelto `Apply as fixed amount` per *[!UICONTROL Apply]*, immettere il valore numerico dell&#39;importo fisso (ad esempio: enter `25` per un adeguamento fisso da $ 25). |
