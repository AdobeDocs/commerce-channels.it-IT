---
title: '''Regola di rideterminazione intelligente dei prezzi: Prezzo base"'
description: Utilizza le impostazioni del prezzo minimo per determinare il prezzo più basso per una regola di prezzo intelligente per gestire gli annunci Amazon.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Regola di prezzo intelligente: prezzo base

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

La [prezzo base](./floor-price.md) le impostazioni proteggono automaticamente il prezzo di prodotto più basso rispetto alle regole di prezzo intelligenti. Utilizza queste impostazioni per impostare un prezzo minimo (al prezzo più basso) per le tue regole di prezzo intelligenti, assicurandoti che i tuoi prodotti non siano elencati al di sotto di un prezzo desiderato.

Gli attributi del prezzo base sono basati sull&#39;ambito del sito web se il tuo [!DNL Commerce] il negozio utilizza l&#39;ambito di determinazione dei prezzi del sito web. Vedi [Portata del prezzo](./price-scope.md).

Il prezzo a pavimento è utilizzato solo quando **[!UICONTROL Rule Type]** è impostato su `Intelligent repricing rule`.

## Configura il prezzo minimo

Definisci l&#39;impostazione del prezzo più basso nella _[!UICONTROL Floor Price]_sezione .

1. Per **[!UICONTROL Floor Price Source]**, scegli un attributo di origine del prezzo.

   Scegli la [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} che indica il limite del pavimento relativo. Ad esempio, se non desideri che il tuo prezzo di listino Amazon scenda al di sotto del costo del tuo articolo, scegli la *Costo* attributo.

1. Per **[!UICONTROL Floor Price Action]**, scegli un’opzione.

   - `Decrease By` - Scegli quando vuoi definire _[!UICONTROL Floor Price Source]_da regolare, creando un prezzo minimo più basso per la regola, prima di inserirla in Amazon.

   - `Increase By` - Scegli quando vuoi definire _[!UICONTROL Floor Price Source]_valore da regolare, creando un prezzo minimo più alto per la regola, prima di inserirla in Amazon.

   - `Match` - Scegliere quando non si desidera che il prezzo di listino fluttui al di sotto del valore definito _[!UICONTROL Floor Price Source]_valore. Quando è impostato su `Match`,_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_i campi sono disabilitati.

1. Lascia la **[!UICONTROL Apply]** predefinito come `Apply as percentage`.

1. Per **[!UICONTROL Floor Adjustment Price]**, immetti il valore numerico della percentuale per regolare il _[!UICONTROL Floor Price Source]_valore.

In questo esempio, il prezzo minimo è impostato a un 3% superiore al costo dell&#39;articolo.

![Esempio di regola di rideterminazione intelligente dei prezzi: prezzo base](assets/ob-intelligent-pricde-rule-floor-price.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Floor Price Source] | Scegli la [!DNL Commerce] attributo che indica il limite relativo (prezzo più basso). Ad esempio, se non desideri che il tuo prezzo di listino Amazon scenda al di sotto del costo del tuo articolo, scegli la `Cost` attributo. |
| [!UICONTROL Floor Price Action] | Scegliere un&#39;azione di adeguamento dei prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi definire _[!UICONTROL Floor Price Source]_da regolare, creando un prezzo minimo più basso per la regola, prima di inserirla in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando vuoi definire _[!UICONTROL Floor Price Source]_valore da regolare, creando un prezzo minimo più alto per la regola, prima di inserirla in Amazon.</li><li>**[!UICONTROL Match]** - Scegliere quando non si desidera che il prezzo di listino fluttui al di sotto del valore definito _[!UICONTROL Floor Price Source]_valore. Quando viene scelto, il_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_i campi sono disabilitati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un aggiustamento percentuale relativo al _[!UICONTROL Floor Price Source]_valore. |
| [!UICONTROL Floor Adjustment Amount] | Immetti il valore numerico della percentuale per regolare il tuo _[!UICONTROL Floor Price Source]_valore. |
