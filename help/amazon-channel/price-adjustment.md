---
title: Canale di vendita Amazon - [!UICONTROL Price Adjustment]
description: Configurare gli adeguamenti di prezzo per definire il calcolo del prezzo dopo aver identificato l'origine del prezzo del concorrente Amazon.
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>La sezione Adeguamento prezzo è leggermente diversa per le regole di rideterminazione dei prezzi standard e intelligenti. **[!UICONTROL Match Competitor Price]** è disponibile solo in _[!UICONTROL Price Action]_quando **[!UICONTROL Rule Type]**è impostato su `Intelligent repricing rule`.

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- [Seleziona tipo di regola](./intelligent-repricing-rules.md)
- [Varianze condizionali dei concorrenti](./competitor-conditional-variances.md)
- Adeguamento prezzo
- [Prezzo base](./floor-price.md)
- [Prezzo massimo opzionale](./optional-ceiling-price.md)

L&#39;adeguamento del prezzo definisce il calcolo del prezzo quando è stata identificata l&#39;origine del prezzo del concorrente.

## Configura rettifica prezzo

Definire l&#39;adeguamento dei prezzi nella sezione _[!UICONTROL Price Adjustment]_.

1. Per **[!UICONTROL Price Action]**, scegliere un&#39;opzione:

   - `Decrease By` - Scegliere quando adeguare il valore dell&#39;origine del prezzo definito, creando un prezzo inferiore per la regola, prima di mettere in vendita il prodotto in Amazon.

   - `Increase By` - Scegliere quando adeguare il valore dell&#39;origine del prezzo definito, creando un prezzo più alto per la regola, prima di mettere in vendita il prodotto in Amazon.

   - `Match Competitor Price` - (Solo regola di rideterminazione prezzi intelligente) Scegli quando vuoi modificare il prezzo dell&#39;inserzione Amazon in modo che corrisponda al prezzo [concorrente più basso](./lowest-competitor-pricing.md), in base al feedback del tuo concorrente e ai parametri di varianza. Se è impostato su `Match Competitor Price`, i campi _[!UICONTROL Apply]_e_[!UICONTROL Adjustment Amount]_ vengono rimossi.

1. Per **[!UICONTROL Apply]**, scegliere un&#39;opzione:

   - `Apply as percentage` - Scegli quando vuoi che il **[!UICONTROL Magento Price Source]** definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di una percentuale.

   - `Apply as fixed amount` - Scegli quando vuoi che il **[!UICONTROL Magento Price Source]** definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), immettere il valore numerico per l&#39;adeguamento del prezzo.

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as percentage`, immettere il valore percentuale (ad esempio, immettere `25` per un adeguamento percentuale del 25%).

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as fixed amount`, immettere il valore numerico per l&#39;importo fisso, ad esempio `25` per un adeguamento fisso di 25 dollari.

![Regola di rideterminazione prezzi intelligente - rettifica prezzo](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Scegliere un&#39;azione di adeguamento della determinazione prezzi. Opzioni:<br>**[!UICONTROL Decrease By]**- Scegli quando vuoi che il _[!UICONTROL Magento Price Source]_definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato verso il basso, creando un prezzo più basso per la regola, prima dell&#39;inserzione in Amazon.<br>**[!UICONTROL Increase By]**- Scegli quando vuoi che il_[!UICONTROL Magento Price Source]_ definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato, creando un prezzo più alto per la regola, prima di mettere in vendita il prodotto ad Amazon.<br>**[!UICONTROL Match Competitor Price]**- (Solo regola di rideterminazione prezzi intelligente) Scegli quando vuoi modificare il prezzo dell&#39;inserzione Amazon in modo che corrisponda al prezzo [concorrente più basso](./lowest-competitor-pricing.md), in base al feedback del tuo concorrente e ai parametri di varianza. Se scelti, i campi _Applica_ e _Importo adeguamento_ vengono rimossi. |
| [!UICONTROL Apply] | Opzioni:<br>**[!UICONTROL Apply as percentage]**- Scegliere quando si desidera che il _[!UICONTROL Magento Price Source]_definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di una percentuale.<br>**[!UICONTROL Apply as fixed amount]**- Scegli quando vuoi che il_[!UICONTROL Magento Price Source]_ definito nel [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di un importo fisso. |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br>Se si sceglie `Apply as percentage` per **[!UICONTROL Apply]**, immettere il valore percentuale (ad esempio: immettere `25` per un adeguamento del 25%).<br>Se si sceglie `Apply as fixed amount` per **[!UICONTROL Apply]**, immettere il valore numerico per l&#39;importo fisso (ad esempio, immettere `25` per un adeguamento fisso di 25 dollari). |
