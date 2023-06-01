---
title: "Regola di tariffazione intelligente: seleziona tipo di regola"
description: Determina il prezzo dell’inserzione di Amazon in base ai prezzi della concorrenza creando una regola di rideterminazione intelligente dei prezzi.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Regola di tariffazione intelligente: seleziona tipo di regola

>[!IMPORTANT]
>
>Le regole di rideterminazione dei prezzi intelligenti non funzionano correttamente se l’area geografica di Amazon è impostata su `Inactive` stato, così come si presenta durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e l&#39;area geografica deve essere compresa `Active` stato delle tariffe di spedizione da sincronizzare da Amazon.<br><br>
>
>Per aggiornare lo stato dell’area geografica nell’account Amazon, passa a Impostazioni > Informazioni account > Impostazioni ferie. Fai riferimento a [Amazon: Elenco dello stato per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Una regola di rideterminazione dei prezzi intelligente utilizza i prezzi dei concorrenti di Amazon per determinare il prezzo dell&#39;inserzione. I concorrenti sono altri venditori che elencano gli stessi prodotti della tua su Amazon.

Le sezioni di una regola di rideterminazione dei prezzi intelligente includono:

- Seleziona tipo di regola
- [Varianze condizionali dei concorrenti](./competitor-conditional-variances.md)
- [Adeguamento prezzo](./price-adjustment.md)
- [Prezzo base](./floor-price.md)
- [Prezzo massimo opzionale](./optional-ceiling-price.md)

## Configurare il tipo di regola

Definisci il tipo di regola in _[!UICONTROL Select Rule Type]_sezione.

1. Per **[!UICONTROL Rule Type]**, scegli `Intelligent repricing rule`.

   Questa impostazione abilita _[!UICONTROL Competitor Price Source]_e [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md), e [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) sezioni.

1. Per **[!UICONTROL Competitor Price Source]**, scegli un’opzione:

   - **[!UICONTROL Use "Buy Box" Price]** - Scegliere quando adeguare i prezzi di Amazon in base all&#39;Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo di vendita. A [!DNL Buy Box] il prezzo esiste quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce [!DNL Buy Box] in base ai requisiti prestazionali. I commercianti cercano di vincere [!DNL Buy Box] stato del venditore e massima visibilità delle inserzioni dei prodotti.

   - **[!UICONTROL Use Lowest Competitor Price]** - Scegli quando vuoi confrontare e adeguare il prezzo dell&#39;inserzione ai prezzi della concorrenza per lo stesso prodotto. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono attivati.

1. Se attivato, scegli un’opzione per **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Scegliere quando confrontare e adeguare i prezzi in base a tutti i prezzi della concorrenza per lo stesso prodotto.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegliere quando si desidera limitare i concorrenti a cui viene confrontato il prezzo per lo stesso prodotto. Questa impostazione restringe ulteriormente i concorrenti richiedendo che la loro inserzione abbia un minimo della percentuale scelta di feedback positivo prima di applicare la regola del prezzo più basso.

1. Se attivato, immettere un valore numerico per **[!UICONTROL Minimum Feedback Count]**.

   Questo valore numerico facoltativo riduce ulteriormente i prezzi competitivi. Ad esempio, se un commerciante ha un rating di feedback positivo del 95%, ma ha solo un conteggio di feedback pari a `20`, potrebbe non essere un concorrente su cui vuoi modificare i prezzi. Tuttavia, se si immette il valore `1000`, richiederebbe che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni.

>[!NOTE]
>
>Potresti usare le opzioni di feedback e prezzi dei concorrenti per evitare di basare i tuoi prezzi su un concorrente che ha un feedback negativo e vende un prodotto di qualità inferiore.

![Regola di rideterminazione prezzi intelligente: seleziona tipo di regola](assets/ob-intelligent-price-rule-type.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Rule Type] | Seleziona un tipo di regola. Opzioni:<ul><li>**[!UICONTROL Standard price rule]** - Questo tipo di regola ti consente di aumentare o diminuire il prezzo di inserzione di Amazon di una percentuale specifica o di un importo fisso in dollari relativo al _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Questo tipo di regola ti consente di adeguare il prezzo di inserzione di Amazon in base ai prezzi del concorrente. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono attivati.</li></ul> |
| [!UICONTROL Competitor Price Source] | Seleziona l’origine del prezzo desiderata. Opzioni:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Scegliere questa opzione quando si desidera adeguare i prezzi di Amazon in base all&#39;Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo di vendita. A [!DNL Buy Box] il prezzo esiste quando più venditori su Amazon offrono lo stesso prodotto. Amazon definisce [!DNL Buy Box] in base ai requisiti prestazionali. I commercianti cercano di vincere [!DNL Buy Box] stato del venditore e massima visibilità delle inserzioni dei prodotti.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Scegli questa opzione quando vuoi confrontare e adeguare il prezzo dell&#39;inserzione al [prezzo concorrente più basso](./lowest-competitor-pricing.md) per lo stesso prodotto. Quando viene scelto, il _[!UICONTROL Minimum Positive Feedback]_e_[!UICONTROL Minimum Feedback Count]_ sono attivati.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Attivo solo se `Use Lowest Competitor Price` viene selezionato. Opzioni:<ul><li>**[!UICONTROL All Competitor's Prices]** - Scegliere quando confrontare e adeguare i prezzi in base a tutti i prezzi della concorrenza per lo stesso prodotto.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Scegli quando vuoi limitare i concorrenti a cui confrontare e adeguare i tuoi prezzi. Questa impostazione limita ulteriormente i tuoi concorrenti richiedendo che la loro inserzione abbia un minimo della percentuale scelta di feedback positivo e quindi utilizzi il prezzo più basso di quel sottoinsieme di concorrenti.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Attivo solo se `Use Lowest Competitor Price` viene selezionato. Questo valore numerico facoltativo restringe ulteriormente il confronto dei prezzi competitivi. Ad esempio, se un commerciante ha un punteggio di feedback positivo del 95% ma ha solo un conteggio di feedback pari a `20`, potrebbe non essere un concorrente su cui vuoi modificare i prezzi. Tuttavia, se si immette il valore `1000`, richiederebbe che il commerciante abbia un feedback positivo del 95% e un minimo di 1000 recensioni. |
