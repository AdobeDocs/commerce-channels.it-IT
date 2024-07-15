---
title: Canale di vendita Amazon - Azioni regola prezzo
description: Utilizzare le azioni delle regole di prezzo per definire i calcoli di adeguamento applicati all'origine del prezzo per determinare il prezzo di listino di Amazon.
feature: Sales Channels, Price Rules
exl-id: c46bd5c2-7994-45b4-ae0c-9e473372c73a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Azioni regola prezzi

Le azioni delle regole di prezzo definiscono i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino.

## Regola prezzo standard

Una [regola di prezzo standard](./standard-price-rules.md) consente di aumentare o diminuire il prezzo di un&#39;inserzione Amazon di una percentuale specifica o di un importo fisso in dollari relativo al prezzo di catalogo [!DNL Commerce] (o all&#39;origine del prezzo).

| Sezione | Descrizione |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./standard-price-rules.md) | Imposta il tipo di regola su `Standard price rule`. |
| [[!UICONTROL Price Adjustment]](./standard-price-rules.md) | Definire i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino |

## Regola di rideterminazione prezzi intelligente

Una [regola di rideterminazione dei prezzi intelligente](./intelligent-repricing-rules.md) utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che mettono in vendita gli stessi prodotti che stai mettendo in vendita su Amazon.

| Sezione | Descrizione |
|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md) | Imposta il tipo di regola su `Intelligent repricing rule` insieme al prezzo concorrente Source e ai requisiti di feedback. |
| [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md) | Definire le varianze per le condizioni dello stesso prodotto venduto dai concorrenti. |
| [[!UICONTROL Price Adjustment]](./price-adjustment.md) | Definire i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino |
| [[!UICONTROL Floor Price]](./floor-price.md) | Definisci il prezzo più basso per un prodotto per evitare che più regole di determinazione dei prezzi impostino un prezzo di vendita troppo basso. |
| [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md) | Definisci il prezzo più alto per un prodotto in modo che i prezzi rimangano competitivi. |
