---
title: "Regola di determinazione prezzi intelligente: prezzo massimo opzionale"
description: Utilizza le impostazioni opzionali del prezzo massimo per proteggere il prezzo più alto del prodotto dalle regole di prezzo intelligenti che gestiscono le inserzioni Amazon.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Regola di tariffazione intelligente: prezzo limite opzionale

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- [Seleziona tipo di regola](./intelligent-repricing-rules.md)
- [Varianze condizionali dei concorrenti](./competitor-conditional-variances.md)
- [Adeguamento prezzo](./price-adjustment.md)
- [Prezzo base](./floor-price.md)
- Prezzo massimo opzionale

Le impostazioni automatizzate per il prezzo del soffitto proteggono automaticamente il prezzo più alto del prodotto dalle regole di prezzo intelligenti, consentendo di impostare un tetto (prezzo più alto) per le regole di prezzo intelligenti.

## Configura prezzo massimo opzionale

Definisci le impostazioni facoltative del prezzo più alto nella sezione _[!UICONTROL Optional Ceiling Price]_.

1. Per **[!UICONTROL Ceiling Price Source]**, scegliere un attributo.

   Seleziona l&#39;[!DNL Commerce] [attributo prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) che indica il limite massimo relativo. Se ad esempio non vuoi che il prezzo dell&#39;inserzione Amazon superi il prezzo massimo di vendita dell&#39;oggetto, scegli l&#39;attributo `Manufacturer's Suggested Retail Price`.

1. Per **[!UICONTROL Ceiling Price Action]**, scegliere un&#39;opzione.

   - `Decrease By` - Scegliere quando si desidera che il valore _[!UICONTROL Ceiling Price Source]_definito venga ridotto, creando un prezzo massimo inferiore per la regola, prima di eseguire l&#39;inserzione in Amazon.

   - `Increase By` - Scegliere quando adeguare il valore _[!UICONTROL Ceiling Price Source]_definito, creando un prezzo massimo più alto per la regola, prima di mettere in vendita l&#39;oggetto ad Amazon.

   - `Match` - Scegliere quando non si desidera che il prezzo di vendita fluttui al di sopra del valore definito _[!UICONTROL Ceiling Price Source]_. Se impostato su `Match`, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_sono disabilitati.

1. Lascia **[!UICONTROL Apply]** predefinito come `Apply as percentage`.

1. Per **[!UICONTROL Ceiling Adjustment Price]**, immetti il valore numerico della percentuale per regolare il valore _[!UICONTROL Ceiling Price Source]_.

In questo esempio, il prezzo massimo è impostato su un valore inferiore del 2% rispetto al prezzo minimo all’importazione dell’articolo.

![Regola di rideterminazione prezzi intelligente - prezzo massimo opzionale](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | Scegli l&#39;[!DNL Commerce] [attributo prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) che indica il limite massimo relativo. Ad esempio, se non desideri che il prezzo di vendita del prodotto superi il prezzo consigliato per l&#39;oggetto, scegli l&#39;attributo `Manufacturer's Suggested Retail Price`. |
| [!UICONTROL Ceiling Price Action] | Scegliere un&#39;azione di adeguamento della determinazione prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegliere quando si desidera che il valore _[!UICONTROL Ceiling Price Source]_definito venga ridotto, creando un prezzo massimo inferiore per la regola, prima di eseguire l&#39;inserzione in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegliere quando adeguare il valore _[!UICONTROL Ceiling Price Source]_definito, creando un prezzo massimo più alto per la regola, prima di mettere in vendita l&#39;oggetto ad Amazon.</li><li>**[!UICONTROL Match]** - Scegliere quando non si desidera che il prezzo di vendita fluttui al di sopra del valore definito _[!UICONTROL Ceiling Price Source]_. Se impostato su `Match`, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_sono disabilitati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un adeguamento percentuale relativo al valore _[!UICONTROL Ceiling Price Source]_. |
| [!UICONTROL Ceiling Price Adjustment] | Immettere il valore numerico della percentuale per regolare il valore _[!UICONTROL Ceiling Price Source]_. |
