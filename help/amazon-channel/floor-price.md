---
title: "Regola di tariffazione intelligente: prezzo minimo"
description: Utilizza le impostazioni del prezzo base per determinare il prezzo più basso per una regola di determinazione prezzi intelligente per gestire le tue inserzioni Amazon.
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Regola di tariffazione intelligente: prezzo base

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Le impostazioni del [prezzo base](./floor-price.md) proteggono automaticamente il prezzo del prodotto più basso dalle regole di prezzo intelligenti. Utilizza queste impostazioni per impostare un prezzo minimo per le tue regole di prezzo intelligenti, assicurandoti che i tuoi prodotti non siano elencati al di sotto di un prezzo desiderato.

Gli attributi del prezzo base si basano sull&#39;ambito del sito Web se lo store [!DNL Commerce] utilizza l&#39;ambito di determinazione prezzi del sito Web. Vedi [Ambito prezzo](./price-scope.md).

Il prezzo minimo viene utilizzato solo quando **[!UICONTROL Rule Type]** è impostato su `Intelligent repricing rule`.

## Configura prezzo minimo

Definire il prezzo più basso nella sezione _[!UICONTROL Floor Price]_.

1. Per **[!UICONTROL Floor Price Source]**, scegliere un attributo origine prezzo.

   Scegli l&#39;[!DNL Commerce] [attributo di prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) che indica il limite di soglia relativo. Ad esempio, se non vuoi che il prezzo dell&#39;inserzione Amazon scenda sotto il costo del tuo oggetto, scegli l&#39;attributo *Costo*.

1. Per **[!UICONTROL Floor Price Action]**, scegliere un&#39;opzione.

   - `Decrease By` - Scegliere quando si desidera che il valore _[!UICONTROL Floor Price Source]_definito venga ridotto, creando un prezzo minimo inferiore per la regola, prima di eseguire l&#39;inserzione in Amazon.

   - `Increase By` - Scegliere quando adeguare il valore _[!UICONTROL Floor Price Source]_definito, creando un prezzo minimo più alto per la regola, prima di mettere in vendita l&#39;oggetto ad Amazon.

   - `Match` - Scegliere se non si desidera che il prezzo di vendita fluttui al di sotto del valore definito _[!UICONTROL Floor Price Source]_. Se impostato su `Match`, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_sono disabilitati.

1. Lascia **[!UICONTROL Apply]** predefinito come `Apply as percentage`.

1. Per **[!UICONTROL Floor Adjustment Price]**, immetti il valore numerico della percentuale per regolare il valore _[!UICONTROL Floor Price Source]_.

In questo esempio, il prezzo minimo è impostato per essere superiore del 3% al costo dell&#39;articolo.

![Esempio di regola di rideterminazione prezzi intelligente - prezzo minimo](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source] | Scegliere l&#39;attributo [!DNL Commerce] che indica il limite minimo relativo (prezzo più basso). Se ad esempio non vuoi che il prezzo dell&#39;inserzione Amazon scenda sotto il costo dell&#39;oggetto, scegli l&#39;attributo `Cost`. |
| [!UICONTROL Floor Price Action] | Scegliere un&#39;azione di adeguamento della determinazione prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegliere quando si desidera che il valore _[!UICONTROL Floor Price Source]_definito venga ridotto, creando un prezzo minimo inferiore per la regola, prima di eseguire l&#39;inserzione in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegliere quando adeguare il valore _[!UICONTROL Floor Price Source]_definito, creando un prezzo minimo più alto per la regola, prima di mettere in vendita l&#39;oggetto ad Amazon.</li><li>**[!UICONTROL Match]** - Scegliere se non si desidera che il prezzo di vendita fluttui al di sotto del valore definito _[!UICONTROL Floor Price Source]_. Se scelti, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_sono disabilitati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un adeguamento percentuale relativo al valore _[!UICONTROL Floor Price Source]_. |
| [!UICONTROL Floor Adjustment Amount] | Immettere il valore numerico della percentuale per regolare il valore _[!UICONTROL Floor Price Source]_. |
