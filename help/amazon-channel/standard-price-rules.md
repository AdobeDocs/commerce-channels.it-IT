---
title: 'Canale di vendita Amazon: azioni della regola di prezzo standard'
description: Utilizzare le azioni delle regole di prezzo standard per aumentare o diminuire un prezzo di listino di Amazon rispetto al prezzo di catalogo Commerce (o origine prezzo).
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Azioni della regola di prezzo standard

Un&#39;azione di una regola di prezzo standard consente di aumentare o diminuire un prezzo di vendita Amazon di una percentuale specifica o di un importo fisso in dollari relativo al prezzo di catalogo [!DNL Commerce] (o all&#39;origine del prezzo).

Le sezioni di un&#39;azione di una regola di prezzo standard includono:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Configurare le azioni delle regole di prezzo

1. Per **[!UICONTROL Rule Type]**, scegliere `Standard price rule`.

   Questa opzione disattiva gli altri campi della sezione _[!UICONTROL Select Rule Type]_.

1. Espandere la sezione _[!UICONTROL Price Adjustment]_, se necessario.

1. Per **[!UICONTROL Price Action]**, scegli un&#39;opzione per determinare come modificare il valore di *[!UICONTROL Magento Price Source]* (definito nel [Prezzo d&#39;inserzione](./listing-price.md)).

   - `Decrease By` - Scegli quando vuoi ridurre il valore prima di inserirlo in Amazon.

   - `Increase By` - Scegli quando desideri che il valore venga aumentato prima di inserirlo nell&#39;elenco di Amazon.

1. Per **[!UICONTROL Apply]**, scegli un&#39;opzione per determinare come regolare il *[!UICONTROL Magento Price Source]* definito nel [prezzo d&#39;inserzione](./listing-price.md):

   - `Apply as percentage` - Scegliere quando si desidera che il *[!UICONTROL Magento Price Source]* definito nel valore [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di una percentuale

   - `Apply as fixed amount` - Scegliere quando si desidera che il *[!UICONTROL Magento Price Source]* definito nel valore [Prezzo d&#39;inserzione](./listing-price.md) venga adeguato di un importo fisso.

1. Per **[!UICONTROL Adjustment Amount]** (obbligatorio), immettere il valore numerico per l&#39;adeguamento del prezzo.

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as percentage`, immettere il valore percentuale (ad esempio: immettere `25` per un adeguamento del prezzo percentuale del 25%).

   - Quando *[!UICONTROL Apply]* è impostato su `Apply as fixed amount`, immettere il valore numerico per l&#39;importo fisso (ad esempio, immettere `25` per un adeguamento del prezzo fisso di 25 $).

1. Al termine, fare clic su **[!UICONTROL Save pricing rule]**.

![Regola prezzo standard](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | Selezionare `Standard price rule`. |
| [!UICONTROL Price Action] | Opzioni:<ul><li>**[!UICONTROL Decrease By]** - Scegliere quando ridurre il valore dell&#39;origine prezzo [!DNL Commerce] definito prima di inserirlo in Amazon.</li><li>**[!UICONTROL Increase By]** - Scegliere quando aumentare il valore dell&#39;origine prezzo [!DNL Commerce] definito prima di eseguire l&#39;inserzione in Amazon.</li></ul> |
| [!UICONTROL Apply] | Opzioni:<ul><li>**[!UICONTROL Apply as percentage]** - Scegliere quando si desidera che il valore dell&#39;origine prezzo [!DNL Commerce] definito venga adeguato di una percentuale.</li><li>**[!UICONTROL Apply as fixed amount]** - Scegliere quando si desidera che il valore dell&#39;origine prezzo [!DNL Commerce] definito venga adeguato di un importo fisso.</li></ul> |
| [!UICONTROL Adjustment Amount] | Obbligatorio.<br><br>Se si sceglie `Apply as percentage` per *[!UICONTROL Apply]*, immettere il valore percentuale, ad esempio `25` per un adeguamento del 25%.<br><br>Se si sceglie `Apply as fixed amount` per *[!UICONTROL Apply]*, immettere il valore numerico per l&#39;importo fisso (ad esempio, immettere `25` per un adeguamento fisso di 25 dollari). |
