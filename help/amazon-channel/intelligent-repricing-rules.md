---
title: '''Regola di rideterminazione intelligente dei prezzi: Seleziona tipo di regola'''
description: Determina il tuo prezzo di listino Amazon in base ai prezzi della concorrenza creando una regola di rideterminazione intelligente dei prezzi.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Regola di prezzo intelligente: seleziona tipo di regola

>[!IMPORTANT]
>
>Le regole di rideterminazione intelligente dei prezzi non funzionano correttamente se l’area geografica di Amazon è impostata su `Inactive` stato, come durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e l&#39;area geografica deve essere compresa `Active` stato delle tariffe di spedizione da sincronizzare da Amazon.<br><br>
>
>Per aggiornare lo stato della tua regione nel tuo account Amazon, vai a Impostazioni > Informazioni account > Impostazioni delle vacanze. Fai riferimento a [Amazon: Stato dell&#39;elenco per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Una regola di rideterminazione intelligente dei prezzi utilizza i prezzi dei concorrenti Amazon per determinare il prezzo del tuo annuncio. I concorrenti sono altri venditori che elencano gli stessi prodotti della tua su Amazon.

Le sezioni di una regola di rideterminazione intelligente dei prezzi includono:

- Seleziona tipo di regola
- [Varianze condizionali della concorrenza](./competitor-conditional-variances.md)
- [Adeguamento del prezzo](./price-adjustment.md)
- [Prezzo base](./floor-price.md)
- [Prezzo a soffitto opzionale](./optional-ceiling-price.md)

## Configurare il tipo di regola

Definisci il tipo di regola nel _[!UICONTROL Select Rule Type]_sezione .

1. Per **[!UICONTROL Rule Type]**, scegli `Intelligent repricing rule`.

   Questa impostazione abilita _[!UICONTROL Competitor Price Source]_e [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md)e [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) sezioni.

1. Per **[!UICONTROL Competitor Price Source]**, scegli un’opzione:

   - **[!UICONTROL Use "Buy Box" Price]** - Scegli quando vuoi modificare i prezzi di Amazon in base ad Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo di vendita. A [!DNL Buy Box] il prezzo esiste quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce il [!DNL Buy Box] in base ai requisiti di prestazioni. I commercianti cercano di vincere [!DNL Buy Box] lo stato del venditore e offrire la massima visibilità dei loro elenchi di prodotti.

   - **[!UICONTROL Use Lowest Competitor Price]** - Scegli quando confrontare e adeguare il prezzo dell&#39;inserzione al prezzo concorrente per lo stesso prodotto. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ i campi sono abilitati.

1. Se abilitata, scegli un’opzione per **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Scegli quando confrontare e adeguare i prezzi in base a tutti i prezzi concorrenti per lo stesso prodotto.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegliere quando si desidera limitare i concorrenti a cui viene confrontato il prezzo per lo stesso prodotto. Questa impostazione restringe ulteriormente i concorrenti richiedendo che la loro quotazione abbia un minimo della percentuale di feedback positivo prescelta prima di applicare la regola del prezzo più basso.

1. Se attivato, immetti un valore numerico per **[!UICONTROL Minimum Feedback Count]**.

   Questo valore numerico facoltativo riduce ulteriormente il prezzo competitivo. Ad esempio, se un commerciante ha un rating di feedback positivo del 95%, ma ha solo un conteggio di feedback di `20`, potrebbe non essere un concorrente su cui desideri modificare i prezzi. Tuttavia, se immetti un valore di `1000`, richiederebbe che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni dei commercianti.

>[!NOTE]
>
>Potresti utilizzare queste opzioni di prezzo e feedback dei concorrenti per evitare di basare i tuoi prezzi su un concorrente che ha un feedback scadente e sta vendendo un prodotto di qualità inferiore.

![Regola di rideterminazione intelligente dei prezzi: seleziona il tipo di regola](assets/ob-intelligent-price-rule-type.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Rule Type] | Seleziona un tipo di regola. Opzioni:<ul><li>**[!UICONTROL Standard price rule]** - Questo tipo di regola ti consente di aumentare o ridurre il prezzo di listino di Amazon di una percentuale specifica o di un importo fisso in dollari rispetto al _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Questo tipo di regola ti consente di regolare il prezzo di listino di Amazon in base ai prezzi della concorrenza. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ i campi sono abilitati.</li></ul> |
| [!UICONTROL Competitor Price Source] | Selezionare la fonte di prezzo desiderata. Opzioni:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Scegli questa opzione quando vuoi modificare i prezzi di Amazon in base all&#39;Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo di vendita. A [!DNL Buy Box] il prezzo esiste quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce il [!DNL Buy Box] in base ai requisiti di prestazioni. I commercianti cercano di vincere [!DNL Buy Box] lo stato del venditore e offrire la massima visibilità dei loro elenchi di prodotti.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Scegliere questa opzione quando si desidera confrontare e regolare il prezzo dell&#39;inserzione in [prezzo concorrente più basso](./lowest-competitor-pricing.md) per lo stesso prodotto. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ i campi sono abilitati.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Solo attivo se `Use Lowest Competitor Price` è scelto. Opzioni:<ul><li>**[!UICONTROL All Competitor's Prices]** - Scegli quando confrontare e adeguare i prezzi in base a tutti i prezzi concorrenti per lo stesso prodotto.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegli quando limitare i concorrenti ai quali confrontare e adeguare i prezzi. Questa impostazione restringe ulteriormente i tuoi concorrenti richiedendo che la loro quotazione abbia un minimo della percentuale di feedback positivo scelta e poi utilizzare il prezzo più basso di quel sottoinsieme di concorrenti.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Solo attivo se `Use Lowest Competitor Price` è scelto. Questo valore numerico facoltativo restringe ulteriormente il confronto competitivo dei prezzi. Ad esempio, se un commerciante ha un punteggio di feedback positivo del 95% ma ha solo un conteggio di feedback di `20`, potrebbe non essere un concorrente su cui desideri modificare i prezzi. Tuttavia, se immetti un valore di `1000`, richiederebbe che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni dei commercianti. |
