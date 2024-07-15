---
title: Aggiungere regole di determinazione prezzi di Amazon
description: Utilizza le regole di determinazione prezzi per gestire i prezzi delle inserzioni sul Marketplace Amazon per il catalogo dei prodotti Commerce.
role: Admin
feature: Sales Channels, Products, Merchandising
exl-id: 37ecf25a-7b47-4f6d-a4bb-2f306f7b5997
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Aggiungere regole di determinazione prezzi di Amazon

Le regole di determinazione prezzi possono essere configurate o modificate in qualsiasi momento dopo l&#39;integrazione del negozio. Le regole di determinazione prezzi fanno parte di [Impostazioni elenco](./listing-settings.md) e sono accessibili nel [dashboard archivio](./amazon-store-dashboard.md).

## Regola prezzo standard

Un&#39;azione di regola di prezzo standard consente di aumentare o diminuire un prezzo di vendita Amazon di una percentuale specifica o di un importo fisso in dollari relativo al **[!UICONTROL Magento Price Source*]* definito nel [Prezzo di vendita](./listing-price.md).

### Aggiungere una regola di determinazione prezzi standard

1. Fare clic su **[!UICONTROL Pricing rules]** nel dashboard dell&#39;archivio.

1. Fare clic su **[!UICONTROL Add new pricing rule]**.

1. Completare **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)** per la regola.

1. Completare **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)** per la regola.

1. Completare **[[!UICONTROL Price Rule Actions]](./standard-price-rules.md)** per la regola.

1. Al termine, fare clic su **[!UICONTROL Save pricing rule]**.

## Regola di rideterminazione prezzi intelligente

Una regola di rideterminazione dei prezzi intelligente utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che mettono in vendita gli stessi prodotti che stai mettendo in vendita su Amazon.

### Aggiungere una regola di rideterminazione prezzi intelligente

1. Fare clic su **[!UICONTROL Pricing rules]** nel dashboard dell&#39;archivio.

1. Fare clic su **[!UICONTROL Add new pricing rule]**.

1. Completare **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)** per la regola.

1. Completare **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)** per la regola.

1. Completare **[!UICONTROL Price Rule Actions]** per la regola.

   - [[!UICONTROL Select Rule Typ]e](./intelligent-repricing-rules.md)

   - [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)

   - [[!UICONTROL Price Adjustment]](./price-adjustment.md)

   - [[!UICONTROL Floor Price]](./floor-price.md)

   - [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

1. Al termine, fare clic su **[!UICONTROL Save pricing rule]**.
