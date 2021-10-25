---
title: Gestire i prezzi di Amazon
description: È possibile impostare i prezzi per gli annunci Amazon in modo che differiscano dall'archivio COmmerce utilizzando le regole di prezzo.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gestire i prezzi di Amazon

Il canale di vendita di Amazon ti consente di impostare le regole di prezzo, che ti consentono di impostare il prezzo di listino di Amazon diverso da quello definito **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md). Puoi anche impilare più regole e persino utilizzare i prezzi intelligenti per regolare il prezzo di listino di Amazon in base ai concorrenti&#39; [[!DNL Buy Box]](./buy-box-competitor-pricing.md) il prezzo [prezzo concorrente più basso](./lowest-competitor-pricing.md).

Esistono due tipi di regole di prezzo:

- [Regola prezzi standard](./standard-price-rules.md)
- [Regola di rideterminazione dei prezzi intelligente](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Le regole di rideterminazione intelligente dei prezzi non funzionano correttamente se l’area geografica di Amazon è impostata su `Inactive` stato, come durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e l&#39;area geografica deve essere compresa `Active` stato delle tariffe di spedizione da sincronizzare da Amazon.
   >
   >Per aggiornare lo stato della tua regione nel tuo account Amazon, vai a Impostazioni > Informazioni account > Impostazioni delle vacanze. Fai riferimento a [Amazon: Stato dell&#39;elenco per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){target=&quot;_blank&quot;} (accesso al centro rivenditori richiesto).

Questa funzione ti consente di manipolare i prezzi Amazon in modo simile al [!DNL Commerce] [regole sui prezzi di catalogo](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}. Puoi creare regole complesse che ti consentono di modificare i prezzi di prodotti specifici, prodotti all’interno di categorie specifiche o anche con attributi specifici.

Puoi aggiungere regole di prezzo per gli elenchi Amazon. Le regole sui prezzi possono essere utilizzate per regolare automaticamente i prezzi delle inserzioni, in base a una serie di condizioni definite. Le regole sui prezzi vengono attivate e calcolano il prezzo corretto prima che il prodotto venga elencato in Amazon.

>[!NOTE]
>
>L&#39;origine del prezzo per le inserzioni Amazon è definita per **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. Tutti i calcoli di adeguamento definiti nella regola di determinazione dei prezzi utilizzano l&#39;origine dei prezzi come valore iniziale.

Le regole di determinazione dei prezzi ti consentono di impostare un prezzo di vendita diverso da quello di Amazon **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. È inoltre possibile sovrapporre più regole che lavorano insieme per regolare il prezzo.

Una regola di determinazione prezzi/prezzi richiede tre serie di informazioni durante la configurazione:

- [Impostazioni generali](./pricing-rule-general-settings.md): Definisce il nome, la descrizione, le date attive e la priorità di una regola e imposta il comportamento delle regole successive in base all&#39;impostazione di priorità.
- [Condizioni](./pricing-rule-conditions.md): Determinare quali prodotti sono idonei per la regola del prezzo.
- [Azioni](./pricing-rule-actions.md): Definire i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino.

Puoi creare [regole di prezzo standard](./standard-price-rules.md) che regola automaticamente il prezzo dell&#39;inserzione di Amazon rispetto al valore selezionato **[!UICONTROL Magento Price Source]** nel tuo [prezzo di listino](./listing-price.md) impostazioni. Questa funzione ti consente di manipolare i prezzi Amazon in modo simile al [!DNL Commerce] [regole sui prezzi di catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;}. Puoi creare regole complesse che modificano automaticamente i prezzi per prodotti specifici, prodotti all’interno di categorie specifiche o prodotti con attributi specifici. Puoi completare le impostazioni tradizionali e riassegnare i prezzi ai tuoi prodotti per aumentare o diminuire in base a una quantità fissa o a una percentuale.

Un altro potente strumento è il [Repricing intelligente](./intelligent-repricing-rules.md) funzionalità che regola il prezzo di listino di Amazon in base alla concorrenza [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo o [Prezzo più basso](./lowest-competitor-pricing.md). Simile al [!DNL Commerce] [regole sui prezzi di catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;}, questa funzionalità avanzata ti consente di manipolare i prezzi di Amazon creando regole complesse. Le regole possono definire la possibilità di una variazione di prezzo per prodotti specifici, prodotti all&#39;interno di categorie specifiche o anche con attributi di prodotto specifici.

Utilizzo di un sistema intelligente di rideterminazione dei prezzi per adeguare i prezzi delle inserzioni Amazon in base ai prezzi dei concorrenti. Il canale di vendita Amazon ha creato delle protezioni per proteggere i margini o evitare di abbinare i prezzi di un commerciante con feedback contenuti. Utilizzo [regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md), i prezzi di listino di Amazon possono essere manipolati automaticamente come importo fisso o percentuale (su o giù) o anche sincronizzati con [[!DNL Buy Box]](./buy-box-competitor-pricing.md) prezzo o [Prezzo più basso](./lowest-competitor-pricing.md) per voce. Le regole possono anche essere impilate per fornire flessibilità illimitata.

Puoi controllare aspetti importanti delle regole, come lo stato attivo/inattivo, l’idoneità del sito web, gli intervalli di date facoltativi e i livelli di priorità facoltativi (utilizzati per lo stack delle regole).

Ad esempio, puoi definire e impostare le condizioni per una regola di prezzo che, una volta soddisfatte le condizioni, regola automaticamente il prezzo di listino prima che venga inviato ad Amazon.

Un&#39;altra opzione di prezzo è [sostituzione del prezzo](./overrides.md), che è impostato a livello di singolo elenco. A [sostituzione del prezzo](./overrides.md) può essere impostato e un override ignora/considera la priorità rispetto a tutti gli altri valori predefiniti, impostazioni e regole. Un [override](./overrides.md) può essere impostato per il prezzo, il tempo di gestione, la condizione e le note di vendita (con alcune eccezioni).

![Regole di determinazione prezzi](assets/amazon-pricing-rules.png)

## Colonne predefinite

| Colonna | Descrizione |
|---|---|
| [!UICONTROL Name] | Nome della regola di determinazione dei prezzi, come impostato in [Impostazioni generali della regola di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Il tipo di regola, come impostato in [Azioni sulle regole di determinazione dei prezzi](./pricing-rule-actions.md) (regola di prezzo standard o regola di prezzo intelligente) |
| [!UICONTROL Is Active] | Se la regola è attiva, come impostato in [Impostazioni generali della regola di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | La priorità rispetto ad altre condizioni di determinazione dei prezzi, come stabilito [Impostazioni generali della regola di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Indica se vengono elaborate ulteriori regole di prezzo per i prodotti ammissibili a questa regola, come stabilito in [impostazioni generali delle regole di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | L&#39;inizio del periodo di tempo in cui la regola è attiva |
| [!UICONTROL To Date] | Fine del periodo di tempo in cui la regola è attiva |
| [!UICONTROL Action] | Elenca tutte le azioni che possono essere applicate a un elenco specifico. Per applicare un’azione, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_colonna. Opzioni: `Edit Price Rule` / `Delete Price Rule` |
