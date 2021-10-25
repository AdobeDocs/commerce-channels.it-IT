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
>La sezione Adeguamento dei prezzi è leggermente diversa per le regole di rideterminazione dei prezzi standard e intelligenti. **[!UICONTROL Match Competitor Price]** è disponibile solo in _[!UICONTROL Price Action]_quando **[!UICONTROL Rule Type]**è impostato su `Intelligent repricing rule`.

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [Seleziona tipo di regola](./intelligent-repricing-rules.md)
- [Varianze condizionali della concorrenza](./competitor-conditional-variances.md)
- Adeguamento del prezzo
- [Prezzo base](./floor-price.md)
- [Prezzo a soffitto opzionale](./optional-ceiling-price.md)

L&#39;aggiustamento del prezzo definisce il calcolo del prezzo quando si è identificato l&#39;origine del prezzo concorrente.

## Configurare la regolazione del prezzo

Definire l&#39;adeguamento dei prezzi nel _[!UICONTROL Price Adjustment]_sezione .

1. Per **[!UICONTROL Price Action]**, scegli un’opzione:

   - `Decrease By` - Scegli quando vuoi che il valore della fonte del prezzo definito sia regolato verso il basso, creando un prezzo più basso per la regola, prima di inserirlo in Amazon.

   - `Increase By` - Scegli quando vuoi che il valore della fonte del prezzo definito sia regolato, creando un prezzo più alto per la regola, prima di inserirlo in Amazon.

   - `Match Competitor Price` - (Solo regola di prezzo intelligente) Scegli quando vuoi cambiare il prezzo dell&#39;inserzione di Amazon in modo che corrisponda al [concorrente più basso](./lowest-competitor-pricing.md) prezzo, in base ai parametri di feedback e varianza del tuo concorrente. Quando è impostato su `Match Competitor Price`, _[!UICONTROL Apply]_e_[!UICONTROL Adjustment Amount]_ i campi vengono rimossi.

1. Per **[!UICONTROL Apply]**, scegli un’opzione:

   - `Apply as percentage` - Scegli quando vuoi definire **[!UICONTROL Magento Price Source]** definiti nella [Prezzo di listino](./listing-price.md) adeguati in percentuale.

   - `Apply as fixed amount` - Scegli quando vuoi definire **[!UICONTROL Magento Price Source]** definiti nella [Prezzo di listino](./listing-price.md) adeguati di un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), immettere il valore numerico per l&#39;adeguamento del prezzo.

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as percentage`, inserisci il valore percentuale (esempio: enter `25` per un aggiustamento del 25%).

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as fixed amount`, immettere il valore numerico dell&#39;importo fisso (ad esempio: enter `25` per un adeguamento fisso da $ 25).

![Regola di rideterminazione intelligente dei prezzi - adeguamento dei prezzi](assets/amazon-price-adjustment.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Price Action] | Scegliere un&#39;azione di adeguamento dei prezzi. Opzioni:<br>**[!UICONTROL Decrease By]**- Scegli quando vuoi definire _[!UICONTROL Magento Price Source]_definiti nella [Prezzo di listino](./listing-price.md) da regolare, creando un prezzo più basso per la regola, prima di inserirla in Amazon.<br>**[!UICONTROL Increase By]**- Scegli quando vuoi definire_[!UICONTROL Magento Price Source]_ definiti nella [Prezzo di listino](./listing-price.md) da regolare, creando un prezzo più alto per la regola, prima di inserirla in Amazon.<br>**[!UICONTROL Match Competitor Price]**- (Solo regola di prezzo intelligente) Scegli quando vuoi cambiare il prezzo dell&#39;inserzione di Amazon in modo che corrisponda al [concorrente più basso](./lowest-competitor-pricing.md) prezzo, in base ai parametri di feedback e varianza del tuo concorrente. Quando viene scelto, il _Applica_ e _Importo adeguamento_ i campi vengono rimossi. |
| [!UICONTROL Apply] | Opzioni:<br>**[!UICONTROL Apply as percentage]**- Scegli quando vuoi definire _[!UICONTROL Magento Price Source]_definiti nella [Prezzo di listino](./listing-price.md) adeguati in percentuale.<br>**[!UICONTROL Apply as fixed amount]**- Scegli quando vuoi definire_[!UICONTROL Magento Price Source]_ definiti nella [Prezzo di listino](./listing-price.md) adeguati di un importo fisso. |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br>Se hai scelto `Apply as percentage` per **[!UICONTROL Apply]**, inserisci il valore percentuale (esempio: enter `25` per un aggiustamento del 25%).<br>Se hai scelto `Apply as fixed amount` per **[!UICONTROL Apply]**, immettere il valore numerico dell&#39;importo fisso (ad esempio: enter `25` per un adeguamento fisso da $ 25). |
