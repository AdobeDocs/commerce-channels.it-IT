---
title: "Regola di tariffazione intelligente: seleziona tipo di regola"
description: Determina il prezzo dell’inserzione di Amazon in base ai prezzi della concorrenza creando una regola di rideterminazione intelligente dei prezzi.
feature: Sales Channels, Products, Price Rules
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Regola di tariffazione intelligente: seleziona tipo di regola

>[!IMPORTANT]
>
>Le regole di rideterminazione dei prezzi intelligenti non funzionano correttamente se l’area geografica di Amazon è impostata sullo stato `Inactive`, come avviene durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e la tua area geografica deve essere nello stato `Active` affinché le tariffe di spedizione possano essere sincronizzate da Amazon.<br><br>
>
>Per aggiornare lo stato dell’area geografica nell’account Amazon, passa a Impostazioni > Informazioni account > Impostazioni ferie. Fai riferimento a [Amazon: Stato delle inserzioni per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Una regola di rideterminazione dei prezzi intelligente utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che elencano gli stessi prodotti della tua su Amazon.

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- Seleziona tipo di regola
- [Varianze condizionali dei concorrenti](./competitor-conditional-variances.md)
- [Adeguamento prezzo](./price-adjustment.md)
- [Prezzo base](./floor-price.md)
- [Prezzo massimo opzionale](./optional-ceiling-price.md)

## Configurare il tipo di regola

Definire il tipo di regola nella sezione _[!UICONTROL Select Rule Type]_.

1. Per **[!UICONTROL Rule Type]**, scegliere `Intelligent repricing rule`.

   Questa impostazione abilita il campo _[!UICONTROL Competitor Price Source]_e le sezioni [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md) e [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md).

1. Per **[!UICONTROL Competitor Price Source]**, scegliere un&#39;opzione:

   - **[!UICONTROL Use "Buy Box" Price]** - Scegli quando adeguare i prezzi Amazon in base al prezzo di vendita di Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md). Esiste un prezzo [!DNL Buy Box] quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce il venditore [!DNL Buy Box] in base ai requisiti di prestazioni. I commercianti cercano di aggiudicarsi lo stato di venditore [!DNL Buy Box] e di offrire la massima visibilità delle loro inserzioni di prodotti.

   - **[!UICONTROL Use Lowest Competitor Price]** - Scegliere quando confrontare e adeguare il prezzo dell&#39;inserzione ai prezzi della concorrenza per lo stesso prodotto. Se scelti, i campi _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono abilitati.

1. Se attivato, scegliere un&#39;opzione per **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Scegliere quando confrontare e adeguare i prezzi in base ai prezzi di tutti i concorrenti per lo stesso prodotto.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegliere quando limitare i concorrenti a cui viene confrontato il prezzo per lo stesso prodotto. Questa impostazione restringe ulteriormente i concorrenti richiedendo che la loro inserzione abbia un minimo della percentuale scelta di feedback positivo prima di applicare la regola del prezzo più basso.

1. Se attivato, immettere un valore numerico per **[!UICONTROL Minimum Feedback Count]**.

   Questo valore numerico facoltativo riduce ulteriormente i prezzi competitivi. Ad esempio, se un commerciante ha un punteggio di feedback positivo del 95%, ma ha solo un conteggio di feedback di `20`, potrebbe non essere un concorrente su cui desideri modificare i prezzi. Tuttavia, se si immette un valore di `1000`, è necessario che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni.

>[!NOTE]
>
>Potresti utilizzare le opzioni di feedback e prezzi dei concorrenti per evitare di basare i tuoi prezzi su un concorrente che ha un feedback negativo e vende un prodotto di qualità inferiore.

![Regola di rideterminazione prezzi intelligente - seleziona tipo di regola](assets/ob-intelligent-price-rule-type.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | Seleziona un tipo di regola. Opzioni:<ul><li>**[!UICONTROL Standard price rule]** - Questo tipo di regola ti consente di aumentare o diminuire il prezzo di vendita di Amazon di una percentuale specifica o di un importo fisso in dollari rispetto a _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Questo tipo di regola ti consente di adeguare il prezzo dell&#39;inserzione di Amazon in base ai prezzi del concorrente. Se scelti, i campi _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono abilitati.</li></ul> |
| [!UICONTROL Competitor Price Source] | Seleziona l’origine del prezzo desiderata. Opzioni:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Scegliere questa opzione quando si desidera adeguare i prezzi Amazon in base al prezzo di vendita di Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md). Esiste un prezzo [!DNL Buy Box] quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce il venditore [!DNL Buy Box] in base ai requisiti di prestazioni. I commercianti cercano di aggiudicarsi lo stato di venditore [!DNL Buy Box] e di offrire la massima visibilità delle loro inserzioni di prodotti.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Scegliere questa opzione quando si desidera confrontare e adeguare il prezzo di vendita al [prezzo concorrente più basso](./lowest-competitor-pricing.md) per lo stesso prodotto. Se scelti, i campi _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono abilitati.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Attivo solo se viene scelto `Use Lowest Competitor Price`. Opzioni:<ul><li>**[!UICONTROL All Competitor's Prices]** - Scegliere quando confrontare e adeguare i prezzi in base ai prezzi di tutti i concorrenti per lo stesso prodotto.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegliere quando limitare i concorrenti a cui confrontare e adeguare i prezzi. Questa impostazione limita ulteriormente i tuoi concorrenti richiedendo che la loro inserzione abbia un minimo della percentuale scelta di feedback positivo e quindi utilizzi il prezzo più basso di quel sottoinsieme di concorrenti.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Attivo solo se viene scelto `Use Lowest Competitor Price`. Questo valore numerico facoltativo restringe ulteriormente il confronto dei prezzi competitivi. Ad esempio, se un commerciante ha un punteggio di feedback positivo del 95% ma ha solo un conteggio di feedback di `20`, potrebbe non essere un concorrente su cui vuoi modificare i prezzi. Tuttavia, se si immette un valore di `1000`, è necessario che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni. |
