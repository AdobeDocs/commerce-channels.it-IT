---
title: Adeguamento del prezzo
description: Configura gli adeguamenti dei prezzi per definire il calcolo del prezzo quando hai identificato l'origine dei prezzi della concorrenza Amazon.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Adeguamento del prezzo

>[!NOTE]
>
>La sezione Adeguamento dei prezzi è leggermente diversa per le regole di rideterminazione dei prezzi standard e intelligenti. **[!UICONTROL Match Competitor Price]** è disponibile solo in  _[!UICONTROL Price Action]_quando **[!UICONTROL Rule Type]**è impostato su  `Intelligent repricing rule`.

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [Seleziona tipo di regola](./intelligent-repricing-rules.md)
- [Varianze condizionali della concorrenza](./competitor-conditional-variances.md)
- Adeguamento del prezzo
- [Prezzo base](./floor-price.md)
- [Prezzo a soffitto opzionale](./optional-ceiling-price.md)

L&#39;aggiustamento del prezzo definisce il calcolo del prezzo quando si è identificato l&#39;origine del prezzo concorrente.

## Configurare la regolazione del prezzo

Definisci la regolazione dei prezzi nella sezione _[!UICONTROL Price Adjustment]_.

1. Per **[!UICONTROL Price Action]**, scegli un’opzione:

   - `Decrease By` - Scegli quando vuoi che il valore della fonte del prezzo definito sia regolato verso il basso, creando un prezzo più basso per la regola, prima di inserirlo in Amazon.

   - `Increase By` - Scegli quando vuoi che il valore della fonte del prezzo definito sia regolato, creando un prezzo più alto per la regola, prima di inserirlo in Amazon.

   - `Match Competitor Price` - (Solo regola di prezzo intelligente) Scegli quando vuoi cambiare il prezzo dell&#39;inserzione di Amazon in modo che corrisponda al prezzo  [più basso ](./lowest-competitor-pricing.md) della concorrenza, in base ai tuoi parametri di feedback e varianza della concorrenza. Quando è impostato su `Match Competitor Price`, i campi _[!UICONTROL Apply]_e_[!UICONTROL Adjustment Amount]_ vengono rimossi.

1. Per **[!UICONTROL Apply]**, scegli un’opzione:

   - `Apply as percentage` - Scegliere quando si desidera che il valore definito  **[!UICONTROL Magento Price Source]** definito nel  [listino ](./listing-price.md) Prezzi sia corretto di una percentuale.

   - `Apply as fixed amount` - Scegliere quando si desidera che il valore definito  **[!UICONTROL Magento Price Source]** definito nell&#39; [elenco ](./listing-price.md) del prezzo sia corretto di un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), immettere il valore numerico per l&#39;adeguamento del prezzo.

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as percentage`, immettere il valore percentuale (esempio: immettere `25` per una regolazione del 25%).

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as fixed amount`, immettere il valore numerico per l&#39;importo fisso (ad esempio: immettere `25` per un adeguamento fisso da $ 25).

![Regola di rideterminazione intelligente dei prezzi - adeguamento dei prezzi](assets/amazon-price-adjustment.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Price Action] | Scegliere un&#39;azione di adeguamento dei prezzi. Opzioni:<br>**[!UICONTROL Decrease By]**- Scegliere quando si desidera che il _[!UICONTROL Magento Price Source]_definito nel [Prezzo di listino](./listing-price.md) sia regolato verso il basso, creando un prezzo più basso per la regola, prima di inserirlo in Amazon.<br>**[!UICONTROL Increase By]**- Scegliere quando si desidera che il_[!UICONTROL Magento Price Source]_ prezzo definito nel  [listino ](./listing-price.md) sia regolato, creando un prezzo più alto per la regola, prima di inserirlo in Amazon.<br>**[!UICONTROL Match Competitor Price]**- (Solo regola di prezzo intelligente) Scegli quando vuoi cambiare il prezzo dell&#39;inserzione di Amazon in modo che corrisponda al prezzo  [più basso ](./lowest-competitor-pricing.md) della concorrenza, in base ai tuoi parametri di feedback e varianza della concorrenza. Quando scelto, i campi _Apply_ e _Adjustment Amount_ vengono rimossi. |
| [!UICONTROL Apply] | Opzioni:<br>**[!UICONTROL Apply as percentage]**- Scegli quando vuoi che il _[!UICONTROL Magento Price Source]_definito nel tuo [Prezzo di listino](./listing-price.md) sia regolato da una percentuale.<br>**[!UICONTROL Apply as fixed amount]**- Scegliere quando si desidera che il valore definito_[!UICONTROL Magento Price Source]_ definito nell&#39; [elenco ](./listing-price.md) del prezzo sia corretto di un importo fisso. |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br>Se hai scelto  `Apply as percentage` per  **[!UICONTROL Apply]**, immetti il valore percentuale (esempio: inserire  `25` un adeguamento del 25%).<br>Se si sceglie  `Apply as fixed amount` per  **[!UICONTROL Apply]**, immettere il valore numerico per l&#39;importo fisso (ad esempio: inserire  `25` un adeguamento fisso da $ 25). |
