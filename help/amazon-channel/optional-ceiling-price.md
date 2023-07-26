---
title: "Regola di determinazione prezzi intelligente: prezzo massimo opzionale"
description: Utilizza le impostazioni opzionali del prezzo massimo per proteggere il prezzo più alto del prodotto dalle regole di prezzo intelligenti che gestiscono le inserzioni Amazon.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '387'
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

Definisci le impostazioni opzionali del prezzo più alto in _[!UICONTROL Optional Ceiling Price]_sezione.

1. Per **[!UICONTROL Ceiling Price Source]**, scegli un attributo.

   Seleziona il [!DNL Commerce] [attributo prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) che indica il limite massimo relativo. Ad esempio, se non desideri che il prezzo dell’inserzione Amazon superi il prezzo consigliato per l’oggetto, scegli il `Manufacturer's Suggested Retail Price` attributo.

1. Per **[!UICONTROL Ceiling Price Action]**, scegli un’opzione.

   - `Decrease By` - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da regolare verso il basso, creando un prezzo limite inferiore per la regola, prima di inserirlo nell’elenco di Amazon.

   - `Increase By` - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da adeguare, creando un prezzo massimo più alto per la regola, prima di inserirlo nell’elenco di Amazon.

   - `Match` - Scegliere quando non si desidera che il prezzo di vendita fluttui al di sopra del _[!UICONTROL Ceiling Price Source]_valore. Se impostato su `Match`, il_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_campi sono disattivati.

1. Lascia **[!UICONTROL Apply]** predefinito come `Apply as percentage`.

1. Per **[!UICONTROL Ceiling Adjustment Price]**, immettere il valore numerico per la percentuale di adeguamento _[!UICONTROL Ceiling Price Source]_valore.

In questo esempio, il prezzo massimo è impostato su un valore inferiore del 2% rispetto al prezzo minimo all’importazione dell’articolo.

![Regola di rideterminazione intelligente dei prezzi: prezzo massimo opzionale](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | Scegli la [!DNL Commerce] [attributo prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) che indica il limite massimo relativo. Ad esempio, se non vuoi che il prezzo di vendita del prodotto superi il prezzo consigliato per l&#39;inserzione, scegli `Manufacturer's Suggested Retail Price` attributo. |
| [!UICONTROL Ceiling Price Action] | Scegliere un&#39;azione di adeguamento della determinazione prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da regolare verso il basso, creando un prezzo limite inferiore per la regola, prima di inserirlo nell’elenco di Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando vuoi definire _[!UICONTROL Ceiling Price Source]_valore da adeguare, creando un prezzo massimo più alto per la regola, prima di inserirlo nell’elenco di Amazon.</li><li>**[!UICONTROL Match]** - Scegliere quando non si desidera che il prezzo di vendita fluttui al di sopra del _[!UICONTROL Ceiling Price Source]_valore. Se impostato su `Match`, il_[!UICONTROL Apply]_ e _[!UICONTROL Ceiling Adjustment Amount]_campi sono disattivati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un adeguamento percentuale relativo al _[!UICONTROL Ceiling Price Source]_valore. |
| [!UICONTROL Ceiling Price Adjustment] | Immettere il valore numerico per la percentuale di adeguamento _[!UICONTROL Ceiling Price Source]_valore. |
