---
title: '''Regola di rideterminazione intelligente dei prezzi: Prezzo a soffitto opzionale"'
description: Utilizza le impostazioni di prezzo a soffitto opzionali per proteggere il prezzo più elevato del prodotto dalle regole di prezzo intelligenti che gestiscono gli annunci Amazon.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Regola di prezzo intelligente: prezzo massimo facoltativo

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [Seleziona tipo di regola](./intelligent-repricing-rules.md)
- [Varianze condizionali della concorrenza](./competitor-conditional-variances.md)
- [Adeguamento del prezzo](./price-adjustment.md)
- [Prezzo base](./floor-price.md)
- Prezzo a soffitto opzionale

Le impostazioni automatizzate dei prezzi massimi proteggono automaticamente il prezzo più elevato del prodotto dalle regole di prezzo intelligenti, consentendo di impostare un tetto (il prezzo più alto) per le regole di prezzo intelligenti.

## Configura il prezzo massimo opzionale

Definisci le impostazioni di prezzo più elevate facoltative nella _[!UICONTROL Optional Ceiling Price]_sezione .

1. Per **[!UICONTROL Ceiling Price Source]**, scegli un attributo.

   Seleziona la tua [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} che indica il limite di massimale relativo. Ad esempio, se non desideri che il prezzo di listino di Amazon superi il valore MSRP dell’articolo, scegli la `Manufacturer's Suggested Retail Price` attributo.

1. Per **[!UICONTROL Ceiling Price Action]**, scegli un’opzione.

   - `Decrease By` - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_da regolare, creando un prezzo massimo più basso per la regola, prima di inserirla in Amazon.

   - `Increase By` - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da regolare, creando un prezzo massimo più alto per la regola, prima di inserirla in Amazon.

   - `Match` - Scegliere quando non si desidera che il prezzo di listino fluttui al di sopra del valore definito _[!UICONTROL Ceiling Price Source]_valore. Quando è impostato su `Match`,_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_i campi sono disabilitati.

1. Lascia la **[!UICONTROL Apply]** predefinito come `Apply as percentage`.

1. Per **[!UICONTROL Ceiling Adjustment Price]**, immetti il valore numerico della percentuale per regolare il _[!UICONTROL Ceiling Price Source]_valore.

In questo esempio, il prezzo massimo è fissato al 2% al di sotto del valore MSRP dell&#39;articolo.

![Regola di rideterminazione intelligente dei prezzi - prezzo massimo opzionale](assets/ob-intelligent-price-rule-ceiling.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Ceiling Price Source] | Scegli la [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} che indica il limite di massimale relativo. Ad esempio, se non desideri che il prezzo di listino dei prodotti superi il valore MSRP dell’articolo, scegli la `Manufacturer's Suggested Retail Price` attributo. |
| [!UICONTROL Ceiling Price Action] | Scegliere un&#39;azione di adeguamento dei prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_da regolare, creando un prezzo massimo più basso per la regola, prima di inserirla in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da regolare, creando un prezzo massimo più alto per la regola, prima di inserirla in Amazon.</li><li>**[!UICONTROL Match]** - Scegliere quando non si desidera che il prezzo di listino fluttui al di sopra del valore definito _[!UICONTROL Ceiling Price Source]_valore. Quando è impostato su `Match`,_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_i campi sono disabilitati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un aggiustamento percentuale relativo al _[!UICONTROL Ceiling Price Source]_valore. |
| [!UICONTROL Ceiling Price Adjustment] | Immetti il valore numerico della percentuale per regolare il tuo _[!UICONTROL Ceiling Price Source]_valore. |
