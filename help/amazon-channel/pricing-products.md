---
title: Gestione prezzi Amazon
description: Puoi impostare i prezzi per le tue inserzioni Amazon in modo che differiscano dal tuo Negozio Commerce utilizzando le regole di prezzo.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Gestione prezzi Amazon

Il canale di vendita Amazon ti consente di impostare le regole di prezzo, che ti consentono di impostare il prezzo dell’inserzione Amazon in modo diverso da quello definito **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md). Puoi anche impilare più regole e persino utilizzare i prezzi intelligenti per adeguare il prezzo di vendita di Amazon in base ai prezzi dei concorrenti [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo o [prezzo concorrente più basso](./lowest-competitor-pricing.md).

Esistono due tipi di regole per la determinazione dei prezzi:

- [Regola determinazione prezzi standard](./standard-price-rules.md)
- [Regola di tariffazione intelligente](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Le regole di rideterminazione dei prezzi intelligenti non funzionano correttamente se l’area geografica di Amazon è impostata su `Inactive` stato, così come si presenta durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e l&#39;area geografica deve essere compresa `Active` stato delle tariffe di spedizione da sincronizzare da Amazon.
   >
   >Per aggiornare lo stato dell’area geografica nell’account Amazon, passa a Impostazioni > Informazioni account > Impostazioni ferie. Fai riferimento a [Amazon: Elenco dello stato per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){target="_blank"} (è richiesto l&#39;accesso centrale del venditore).

Questa funzione consente di manipolare i prezzi di Amazon in modo simile al [!DNL Commerce] [regole di prezzo catalogo](https://docs.magento.com/user-guide/catalog/pricing.html){target="_blank"}. Puoi creare regole complesse che ti consentono di modificare i prezzi per prodotti specifici, prodotti all&#39;interno di categorie specifiche o anche con attributi specifici.

Puoi aggiungere le regole di prezzo per le inserzioni Amazon. Le regole di prezzo possono essere utilizzate per adeguare automaticamente i prezzi delle inserzioni, in base a una serie di condizioni definite. Le regole di prezzo vengono attivate e calcolano il prezzo adeguato prima che il prodotto venga messo in vendita su Amazon.

>[!NOTE]
>
>L&#39;origine del prezzo per le inserzioni Amazon è definita per **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. Qualsiasi calcolo di adeguamento definito nella regola di determinazione prezzi utilizza come valore iniziale l&#39;origine prezzo.

Le regole di determinazione dei prezzi consentono di impostare il prezzo dell&#39;inserzione Amazon in modo diverso dal **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. Puoi anche impilare più regole che interagiscono per regolare il prezzo.

Una regola di determinazione prezzi/rideterminazione prezzi richiede tre serie di informazioni durante l&#39;impostazione:

- [Impostazioni generali](./pricing-rule-general-settings.md): definisce il nome, la descrizione, le date attive e la priorità di una regola e imposta il comportamento delle regole successive in base all’impostazione della priorità.
- [Condizioni](./pricing-rule-conditions.md): determina quali prodotti sono idonei per la regola prezzo.
- [Azioni](./pricing-rule-actions.md): definire i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino.

Puoi creare [regole di determinazione prezzi standard](./standard-price-rules.md) che adegua automaticamente il prezzo dell’inserzione di Amazon in base al **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. Questa funzione consente di manipolare i prezzi di Amazon in modo simile al [!DNL Commerce] [regole di prezzo catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}. Puoi creare regole complesse che modificano automaticamente i prezzi per prodotti specifici, prodotti all’interno di categorie specifiche o prodotti con attributi specifici. Puoi completare le impostazioni tradizionali e rideterminare il prezzo dei prodotti per aumentarli o diminuirli in base a un importo fisso o a una percentuale.

Un altro potente strumento è [Ricarica intelligente](./intelligent-repricing-rules.md) funzione che regola il prezzo di vendita di Amazon in base alla concorrenza [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo o [Prezzo concorrente più basso](./lowest-competitor-pricing.md). Simile a [!DNL Commerce] [regole di prezzo catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}, questa funzione avanzata ti consente di manipolare i prezzi di Amazon creando regole complesse. Le regole possono definire l&#39;ambito di una modifica di prezzo per prodotti specifici, prodotti all&#39;interno di categorie specifiche o anche con attributi di prodotto specifici.

Usare un metodo di repricing intelligente per adeguare i prezzi delle inserzioni Amazon in base ai prezzi della concorrenza. Il canale di vendita Amazon ha integrato delle protezioni per consentirti di configurare in modo da proteggere i margini o evitare di abbinare i prezzi di un commerciante con un feedback basso. Utilizzo di [regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md), i prezzi delle inserzioni di Amazon possono essere manipolati automaticamente come importo fisso o percentuale (su o giù) o anche sincronizzati con [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo o [Prezzo concorrente più basso](./lowest-competitor-pricing.md) per singolo articolo. Le regole possono anche essere impilate per fornire una flessibilità illimitata.

Puoi controllare aspetti importanti delle regole, ad esempio lo stato attivo/inattivo, l’idoneità del sito web, gli intervalli di date facoltativi e i livelli di priorità facoltativi (utilizzati per lo stacking delle regole).

Ad esempio, puoi definire e impostare le condizioni per una regola di prezzo che, quando le condizioni vengono soddisfatte, adegua automaticamente il prezzo dell’inserzione prima di inviarlo ad Amazon.

Un&#39;altra opzione di prezzo è [sostituzione prezzo](./overrides.md), impostato a livello di singola inserzione. A [sostituzione prezzo](./overrides.md) può essere impostata e un’esclusione ignora/ha priorità su tutte le altre impostazioni predefinite, impostazioni e regole. Un [sostituire](./overrides.md) può essere impostato per prezzo, tempo di imballaggio, condizione e note del venditore (con alcune eccezioni).

![Regole di determinazione prezzi](assets/amazon-pricing-rules.png)

## Colonne predefinite

| Colonna | Descrizione |
|---|---|
| [!UICONTROL Name] | Nome della regola di determinazione prezzi, come impostato in [Impostazioni generali regola determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Tipo di regola, come impostato in [Azioni regole determinazione prezzi](./pricing-rule-actions.md) (Regola di prezzo standard o Regola di rideterminazione prezzi intelligente) |
| [!UICONTROL Is Active] | Se la regola è attiva, come impostato in [Impostazioni generali regola determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | La priorità rispetto ad altre condizioni di prezzo, come stabilito in [Impostazioni generali regola determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Indica se vengono elaborate ulteriori regole di prezzo per i prodotti ammissibili a questa regola, come stabilito in [impostazioni generali delle regole di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Inizio del periodo di tempo in cui la regola è attiva |
| [!UICONTROL To Date] | Fine del periodo di tempo in cui la regola è attiva |
| [!UICONTROL Action] | Elenca tutte le azioni che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** nel _[!UICONTROL Action]_colonna. Opzioni: `Edit Price Rule` / `Delete Price Rule` |
