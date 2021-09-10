---
title: '''Regola di rideterminazione intelligente dei prezzi: Prezzo base"'
description: Utilizza le impostazioni del prezzo minimo per determinare il prezzo più basso per una regola di prezzo intelligente per gestire gli annunci Amazon.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Regola di prezzo intelligente: prezzo base

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Le impostazioni [Prezzo base](./floor-price.md) proteggono automaticamente il prezzo più basso del prodotto dalle regole di prezzo intelligenti. Utilizza queste impostazioni per impostare un prezzo minimo (al prezzo più basso) per le tue regole di prezzo intelligenti, assicurandoti che i tuoi prodotti non siano elencati al di sotto di un prezzo desiderato.

Gli attributi del prezzo base si basano sull&#39;ambito del sito web se il tuo [!DNL Commerce] negozio utilizza l&#39;ambito del prezzo del sito web. Vedere [Campo di applicazione del prezzo](./price-scope.md).

Il prezzo base viene utilizzato solo quando **[!UICONTROL Rule Type]** è impostato su `Intelligent repricing rule`.

## Configura il prezzo minimo

Definisci l&#39;impostazione del prezzo più basso nella sezione _[!UICONTROL Floor Price]_.

1. Per **[!UICONTROL Floor Price Source]**, scegli un attributo di origine del prezzo.

   Scegli l&#39; [!DNL Commerce] [attributo di prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} che indica il limite di pavimento relativo. Ad esempio, se non desideri che il prezzo di listino di Amazon scenda al di sotto del costo dell&#39;articolo, scegli l&#39;attributo *Cost* .

1. Per **[!UICONTROL Floor Price Action]**, scegli un’opzione.

   - `Decrease By` - Scegli quando vuoi che il  _[!UICONTROL Floor Price Source]_valore definito sia regolato verso il basso, creando un prezzo minimo più basso per la regola, prima di inserirlo in Amazon.

   - `Increase By` - Scegli quando modificare il  _[!UICONTROL Floor Price Source]_valore definito, creando un prezzo minimo più alto per la regola, prima di inserirla in Amazon.

   - `Match` - Scegliere il momento in cui non si desidera che il prezzo di listino oscilli al di sotto del  _[!UICONTROL Floor Price Source]_valore definito. Quando è impostato su `Match`, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_sono disabilitati.

1. Lascia il valore predefinito **[!UICONTROL Apply]** come `Apply as percentage`.

1. Per **[!UICONTROL Floor Adjustment Price]**, immettere il valore numerico della percentuale per regolare il valore _[!UICONTROL Floor Price Source]_.

In questo esempio, il prezzo minimo è impostato a un 3% superiore al costo dell&#39;articolo.

![Esempio di regola di rideterminazione intelligente dei prezzi: prezzo base](assets/ob-intelligent-pricde-rule-floor-price.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Floor Price Source] | Scegli l&#39;attributo [!DNL Commerce] che indica il limite relativo del pavimento (prezzo più basso). Ad esempio, se non desideri che il prezzo di listino di Amazon scenda al di sotto del costo dell’articolo, scegli l’attributo `Cost` . |
| [!UICONTROL Floor Price Action] | Scegliere un&#39;azione di adeguamento dei prezzi. Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegli quando vuoi che il  _[!UICONTROL Floor Price Source]_valore definito sia regolato verso il basso, creando un prezzo minimo più basso per la regola, prima di inserirlo in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegli quando modificare il  _[!UICONTROL Floor Price Source]_valore definito, creando un prezzo minimo più alto per la regola, prima di inserirla in Amazon.</li><li>**[!UICONTROL Match]** - Scegliere il momento in cui non si desidera che il prezzo di listino oscilli al di sotto del  _[!UICONTROL Floor Price Source]_valore definito. Quando viene selezionato, i campi_[!UICONTROL Apply]_ e _[!UICONTROL Floor Adjustment Amount]_sono disabilitati.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Un aggiustamento percentuale relativo al  _[!UICONTROL Floor Price Source]_valore. |
| [!UICONTROL Floor Adjustment Amount] | Immetti il valore numerico della percentuale per regolare il valore _[!UICONTROL Floor Price Source]_. |
