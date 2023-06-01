---
title: Aggiungere regole di determinazione prezzi di Amazon
description: Utilizza le regole di determinazione prezzi per gestire i prezzi di inserzione sul Marketplace Amazon per il catalogo prodotti Commerce.
exl-id: 37ecf25a-7b47-4f6d-a4bb-2f306f7b5997
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Aggiungere regole di determinazione prezzi di Amazon

Le regole di determinazione prezzi possono essere configurate o modificate in qualsiasi momento dopo l&#39;integrazione del negozio. Le regole di determinazione prezzi fanno parte di [Impostazioni elenco](./listing-settings.md) e sono accessibili nel [dashboard store](./amazon-store-dashboard.md).

## Regola prezzo standard

Un’azione di regola di prezzo standard ti consente di aumentare o diminuire un prezzo di inserzione di Amazon di una percentuale specifica o di un importo in dollari fisso relativo al **[!UICONTROL Magento Price Source*]* definito nel [Prezzo di vendita](./listing-price.md).

### Aggiungere una regola di determinazione prezzi standard

1. Clic **[!UICONTROL Pricing rules]** nel dashboard del negozio.

1. Clic **[!UICONTROL Add new pricing rule]**.

1. Completa il **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)** per la regola.

1. Completa il **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)** per la regola.

1. Completa il **[[!UICONTROL Price Rule Actions]](./standard-price-rules.md)** per la regola.

1. Al termine, fai clic su **[!UICONTROL Save pricing rule]**.

## Regola di rideterminazione prezzi intelligente

Una regola di rideterminazione dei prezzi intelligente utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che mettono in vendita gli stessi prodotti che stai mettendo in vendita su Amazon.

### Aggiungere una regola di rideterminazione prezzi intelligente

1. Clic **[!UICONTROL Pricing rules]** nel dashboard del negozio.

1. Clic **[!UICONTROL Add new pricing rule]**.

1. Completa il **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)** per la regola.

1. Completa il **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)** per la regola.

1. Completa il **[!UICONTROL Price Rule Actions]** per la regola.

   - [[!UICONTROL Select Rule Typ]e](./intelligent-repricing-rules.md)

   - [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)

   - [[!UICONTROL Price Adjustment]](./price-adjustment.md)

   - [[!UICONTROL Floor Price]](./floor-price.md)

   - [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

1. Al termine, fai clic su **[!UICONTROL Save pricing rule]**.
