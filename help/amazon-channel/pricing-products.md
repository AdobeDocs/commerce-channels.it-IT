---
title: Gestire i prezzi di Amazon
description: Puoi impostare i prezzi per le inserzioni Amazon in modo che differiscano dal tuo Negozio Commerce utilizzando le regole di prezzo.
feature: Sales Channels, Price Rules
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Gestire i prezzi di Amazon

Il canale di vendita Amazon ti consente di impostare le regole di determinazione dei prezzi, che ti consentono di impostare il prezzo dell&#39;inserzione Amazon in modo diverso da **[!UICONTROL Magento Price Source]** definito nel [prezzo dell&#39;inserzione](./listing-price.md). Puoi anche impilare più regole e persino utilizzare i prezzi intelligenti per regolare il prezzo di vendita di Amazon in base al prezzo [[!DNL Buy Box]](./buy-box-competitor-pricing.md) dei concorrenti o al [prezzo più basso del concorrente](./lowest-competitor-pricing.md).

Esistono due tipi di regole per la determinazione dei prezzi:

- [Regola determinazione prezzi standard](./standard-price-rules.md)
- [Regola di tariffazione intelligente](./intelligent-repricing-rules.md)

  >[!IMPORTANT]
  >
  >Le regole di rideterminazione dei prezzi intelligenti non funzionano correttamente se l’area geografica di Amazon è impostata sullo stato `Inactive`, come avviene durante l’onboarding. I calcoli dei prezzi dipendono dalle tariffe di spedizione e la tua area geografica deve essere nello stato `Active` affinché le tariffe di spedizione possano essere sincronizzate da Amazon.
  >
  >Per aggiornare lo stato dell’area geografica nell’account Amazon, passa a Impostazioni > Informazioni account > Impostazioni ferie. Fai riferimento a [Amazon: Stato inserzione per le vacanze](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (accesso centrale del venditore richiesto).

Questa funzionalità consente di modificare i prezzi di Amazon in modo simile alle [!DNL Commerce] [regole prezzi catalogo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html). Puoi creare regole complesse che ti consentono di modificare i prezzi per prodotti specifici, prodotti all&#39;interno di categorie specifiche o anche con attributi specifici.

Puoi aggiungere le regole di prezzo per le inserzioni Amazon. Le regole di prezzo possono essere utilizzate per adeguare automaticamente i prezzi delle inserzioni, in base a una serie di condizioni definite. Le regole di prezzo vengono attivate e calcolano il prezzo adeguato prima che il prodotto venga messo in vendita su Amazon.

>[!NOTE]
>
>L&#39;origine del prezzo per le tue inserzioni Amazon è definita per **[!UICONTROL Magento Price Source]** nelle impostazioni del [prezzo](./listing-price.md). Qualsiasi calcolo di adeguamento definito nella regola di determinazione prezzi utilizza come valore iniziale l&#39;origine prezzo.

Le regole di determinazione prezzi consentono di impostare il prezzo dell&#39;inserzione Amazon in modo diverso da **[!UICONTROL Magento Price Source]** nelle impostazioni del [prezzo dell&#39;inserzione](./listing-price.md). Puoi anche impilare più regole che interagiscono per regolare il prezzo.

Una regola di determinazione prezzi/rideterminazione prezzi richiede tre serie di informazioni durante l&#39;impostazione:

- [Impostazioni generali](./pricing-rule-general-settings.md): definisce il nome, la descrizione, le date di attivazione e la priorità di una regola e imposta il comportamento delle regole successive in base all&#39;impostazione di priorità.
- [Condizioni](./pricing-rule-conditions.md): determinare quali prodotti sono idonei per la regola prezzi.
- [Azioni](./pricing-rule-actions.md): definire i calcoli di adeguamento applicati all&#39;origine del prezzo per determinare il prezzo di listino.

Puoi creare [regole di determinazione prezzi standard](./standard-price-rules.md) che modificano automaticamente il prezzo di messa in vendita di Amazon in relazione al **[!UICONTROL Magento Price Source]** selezionato nelle impostazioni del [prezzo di messa in vendita](./listing-price.md). Questa funzionalità consente di modificare i prezzi di Amazon in modo simile alle [!DNL Commerce] [regole prezzi catalogo](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html). Puoi creare regole complesse che modificano automaticamente i prezzi per prodotti specifici, prodotti all’interno di categorie specifiche o prodotti con attributi specifici. Puoi completare le impostazioni tradizionali e rideterminare il prezzo dei prodotti per aumentarli o diminuirli in base a un importo fisso o a una percentuale.

Un altro potente strumento è la funzionalità [Rimborso intelligente](./intelligent-repricing-rules.md) che regola il prezzo di vendita di Amazon in base al prezzo del concorrente [[!DNL Buy Box]](./buy-box-competitor-pricing.md) o al [prezzo del concorrente più basso](./lowest-competitor-pricing.md). Simile alle [!DNL Commerce] [regole del prezzo di catalogo](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html), questa funzione avanzata ti consente di manipolare i prezzi di Amazon creando regole complesse. Le regole possono definire l&#39;ambito di una modifica di prezzo per prodotti specifici, prodotti all&#39;interno di categorie specifiche o anche con attributi di prodotto specifici.

Usare un metodo di repricing intelligente per adeguare i prezzi delle inserzioni Amazon in base ai prezzi della concorrenza. Il canale di vendita Amazon ha integrato delle protezioni per consentirti di configurare in modo da proteggere i margini o evitare di abbinare i prezzi di un commerciante con un feedback basso. Utilizzando [regole di rideterminazione dei prezzi intelligenti](./intelligent-repricing-rules.md), i prezzi delle inserzioni di Amazon possono essere manipolati automaticamente come importo fisso o percentuale (su o giù) o anche sincronizzati con il prezzo [[!DNL Buy Box]](./buy-box-competitor-pricing.md) o con il [prezzo concorrente più basso](./lowest-competitor-pricing.md) per articolo. Le regole possono anche essere impilate per fornire una flessibilità illimitata.

Puoi controllare aspetti importanti delle regole, ad esempio lo stato attivo/inattivo, l’idoneità del sito web, gli intervalli di date facoltativi e i livelli di priorità facoltativi (utilizzati per lo stacking delle regole).

Ad esempio, puoi definire e impostare le condizioni per una regola di prezzo che, quando le condizioni vengono soddisfatte, adegua automaticamente il prezzo dell’inserzione prima di inviarlo ad Amazon.

Un&#39;altra opzione di prezzo è una [sostituzione prezzo](./overrides.md), impostata a livello di singola inserzione. È possibile impostare una [sostituzione prezzo](./overrides.md) e una sostituzione ignora/ha la priorità su tutte le altre impostazioni, impostazioni e regole. È possibile impostare una [sostituzione](./overrides.md) per prezzo, tempi di gestione, condizioni e note del venditore (con alcune eccezioni).

![Regole di determinazione prezzi](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Colonne predefinite

| Colonna | Descrizione |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Name] | Il nome della regola di determinazione prezzi, come impostato in [Impostazioni generali regola di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Tipo di regola, come impostato in [Azioni delle regole di determinazione prezzi](./pricing-rule-actions.md) (regola di determinazione prezzi standard o regola di rideterminazione prezzi intelligente) |
| [!UICONTROL Is Active] | Indica se la regola è attiva, come impostato in [Impostazioni generali regola determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | Priorità rispetto ad altre condizioni di determinazione prezzi, come impostato in [Impostazioni generali regole determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Indica se vengono elaborate ulteriori regole di prezzo per i prodotti idonei per questa regola, come impostato nelle [impostazioni generali della regola di determinazione prezzi](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Inizio del periodo di tempo in cui la regola è attiva |
| [!UICONTROL To Date] | Fine del periodo di tempo in cui la regola è attiva |
| [!UICONTROL Action] | Elenca tutte le azioni che possono essere applicate a un elenco specifico. Per applicare un&#39;azione, fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_. Opzioni: `Edit Price Rule` / `Delete Price Rule` |
