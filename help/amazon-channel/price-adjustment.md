---
title: Adeguamento prezzo
description: Configurare gli adeguamenti di prezzo per definire il calcolo del prezzo dopo aver identificato l'origine del prezzo del concorrente Amazon.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Adeguamento prezzo

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

Definire l&#39;adeguamento dei prezzi in _[!UICONTROL Price Adjustment]_sezione.

1. Per **[!UICONTROL Price Action]**, scegli un’opzione:

   - `Decrease By` - Scegliere quando si desidera che il valore dell&#39;origine del prezzo definito venga adeguato verso il basso, creando un prezzo inferiore per la regola, prima di eseguire l&#39;inserzione in Amazon.

   - `Increase By` - Scegliere quando si desidera adeguare il valore dell&#39;origine del prezzo definito, creando un prezzo più alto per la regola, prima di mettere in vendita il prodotto in Amazon.

   - `Match Competitor Price` - (Solo regola di rideterminazione dei prezzi intelligente) Scegli quando desideri modificare il prezzo dell’inserzione Amazon in modo che corrisponda al [concorrente più basso](./lowest-competitor-pricing.md) prezzo, in base al feedback del concorrente e ai parametri di varianza. Se impostato su `Match Competitor Price`, il _[!UICONTROL Apply]_e_[!UICONTROL Adjustment Amount]_ vengono rimossi.

1. Per **[!UICONTROL Apply]**, scegli un’opzione:

   - `Apply as percentage` - Scegli quando vuoi definire **[!UICONTROL Magento Price Source]** definito nel [Prezzo di vendita](./listing-price.md) adeguato di una percentuale.

   - `Apply as fixed amount` - Scegli quando vuoi definire **[!UICONTROL Magento Price Source]** definito nel [Prezzo di vendita](./listing-price.md) adeguato di un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), inserire il valore numerico per l&#39;adeguamento del prezzo.

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as percentage`, inserisci il valore percentuale (esempio: invio `25` per un adeguamento del 25%).

   - Quando **[!UICONTROL Apply]** è impostato su `Apply as fixed amount`, immettere il valore numerico per l&#39;importo fisso (ad esempio: invio `25` per un adeguamento fisso di 25 dollari).

![Regola di rideterminazione prezzi intelligente - Adeguamento prezzo](assets/amazon-price-adjustment.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Price Action] | Scegliere un&#39;azione di adeguamento della determinazione prezzi. Opzioni:<br>**[!UICONTROL Decrease By]**- Scegli quando vuoi definire _[!UICONTROL Magento Price Source]_definito nel [Prezzo di vendita](./listing-price.md) per essere adeguato, creando un prezzo più basso per la regola, prima di mettere in vendita ad Amazon.<br>**[!UICONTROL Increase By]**- Scegli quando vuoi definire_[!UICONTROL Magento Price Source]_ definito nel [Prezzo di vendita](./listing-price.md) per essere adeguato, creando un prezzo più alto per la regola, prima di mettere in vendita ad Amazon.<br>**[!UICONTROL Match Competitor Price]**- (Solo regola di rideterminazione dei prezzi intelligente) Scegli quando desideri modificare il prezzo dell’inserzione Amazon in modo che corrisponda al [concorrente più basso](./lowest-competitor-pricing.md) prezzo, in base al feedback del concorrente e ai parametri di varianza. Quando viene scelto, il _Applica_ e _Importo rettifica_ vengono rimossi. |
| [!UICONTROL Apply] | Opzioni:<br>**[!UICONTROL Apply as percentage]**- Scegli quando vuoi definire _[!UICONTROL Magento Price Source]_definito nel [Prezzo di vendita](./listing-price.md) adeguato di una percentuale.<br>**[!UICONTROL Apply as fixed amount]**- Scegli quando vuoi definire_[!UICONTROL Magento Price Source]_ definito nel [Prezzo di vendita](./listing-price.md) adeguato di un importo fisso. |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br>Se si sceglie `Apply as percentage` per **[!UICONTROL Apply]**, inserisci il valore percentuale (esempio: invio `25` per un adeguamento del 25%).<br>Se si sceglie `Apply as fixed amount` per **[!UICONTROL Apply]**, immettere il valore numerico per l&#39;importo fisso (ad esempio: invio `25` per un adeguamento fisso di 25 dollari). |
