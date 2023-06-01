---
title: Canale di vendita Amazon - Impostazioni generali delle regole di determinazione prezzi
description: Utilizzare le impostazioni generali della regola prezzo per definire le caratteristiche principali di una regola prezzo di vendita.
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Impostazioni generali delle regole di determinazione prezzi

Definisci il nome, la descrizione, le date di attivazione e la priorità della regola.

## Completare la sezione Impostazioni generali regola prezzo

1. Per **[!UICONTROL Rule Name]** (obbligatorio), inserisci il nome della regola.

   Questo nome è solo a scopo di identificazione interna. Il nome della regola è tanto più descrittivo quanto migliore.

1. Per **[!UICONTROL Description]**, immettere una descrizione dettagliata della regola.

   Questa descrizione può includere informazioni sui prodotti idonei, sulle date attive, sulla formula per il calcolo del prezzo adeguato o qualsiasi altra informazione utile per modificare la regola.

1. Per **[!UICONTROL Status]**, scegli un’opzione:

   - `Active` - Scegli questa opzione quando desideri che la regola di determinazione dei prezzi venga applicata ai prodotti idonei e che adegui i prezzi delle inserzioni prima di pubblicarle su Amazon.

   - `Inactive` - Scegliere questa opzione quando non si desidera applicare la regola di determinazione prezzi ai prodotti idonei. Questa opzione verrà probabilmente utilizzata quando si modifica una regola di determinazione prezzi o si disattiva dopo una promozione limitata.

1. Per **[!UICONTROL From]** e **[!UICONTROL To]** Immettere una data di inizio e una data di fine per la regola di determinazione prezzi.

   Puoi anche fare clic sull’icona del calendario per selezionare una data dal calendario dinamico. Questa opzione di avvio e arresto automatici è utile quando si impostano promozioni a tempo limitato o stagionali con date di inizio e fine definite.

1. Per **[!UICONTROL Priority]**, immetti un valore numerico per la priorità della regola.

   Valore di priorità uguale a `1` è la priorità più alta. Se sono presenti più regole di determinazione prezzi attive, è possibile utilizzare questo valore di priorità per determinare quale regola viene applicata per prima. Questo campo è necessario per utilizzare _[!UICONTROL Discard Subsequent Rules]_funzionalità.

1. Per **[!UICONTROL Discard Subsequent Rules]**, scegli un’opzione:

   - `Yes` - Scegliere questa opzione quando non si desidera che vengano applicate altre regole di determinazione dei prezzi applicabili a un prodotto. Ignorare le regole successive significa che, se più regole di determinazione dei prezzi si applicano allo stesso prodotto, solo la regola di determinazione dei prezzi con il valore di priorità definito più alto viene applicata al prodotto. Questa opzione impedisce a più regole di determinazione dei prezzi di sovrapporsi e di offrire sconti aggiuntivi non desiderati.

   - `No` - Scegliere questa opzione quando si desidera consentire l&#39;applicazione di più regole di determinazione prezzi allo stesso prodotto. Questa opzione potrebbe comportare lo stacking e l&#39;applicazione di più sconti.

>[!NOTE]
>
>Per ignorare le regole successive, una regola di determinazione dei prezzi deve avere un valore **Priorità** valore.

![Impostazioni generali delle regole di determinazione prezzi](assets/amazon-pricing-rule-general.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|---|---|
| [!UICONTROL Rule Name] | (Obbligatorio) Immetti un nome per la regola, utilizzato a scopo di identificazione interna. Il nome della regola è tanto più descrittivo quanto migliore. Ad esempio, &quot;25% di sconto sulla vendita di libri di fine anno&quot;. |
| [!UICONTROL Description] | Immettere una descrizione dettagliata che illustri la regola (utilizzata anche per scopi interni). Ad esempio, &quot;Vendita di fine anno, 25% di sconto su tutti gli articoli della categoria Libri&quot;. |
| [!UICONTROL Status] | Opzioni:<ul><li>**[!UICONTROL Inactive]** - La regola di prezzo non si applica alle tue inserzioni. Questa opzione può essere utilizzata quando si modifica una regola di determinazione dei prezzi o si disattiva dopo una promozione limitata.</li><li>**[!UICONTROL Active]** - La regola di determinazione dei prezzi si applica alle tue inserzioni e regola i prezzi prima di pubblicarle su Amazon.</li></ul> |
| [!UICONTROL From] | Inserire la data di inizio della regola di determinazione prezzi. Ad esempio, per effettuare una vendita nell&#39;ultimo mese dell&#39;anno, devi impostare `From` data: 1 dicembre, in modo che la regola di determinazione dei prezzi venga applicata automaticamente alle tue inserzioni Amazon a partire dal 1 dicembre. |
| [!UICONTROL To] | Inserire la data di fine al termine della regola di determinazione prezzi. Continuando con l&#39;esempio precedente, per limitare la vendita all&#39;ultimo mese dell&#39;anno, è necessario impostare `To` data: 31 dicembre, quindi la regola di determinazione dei prezzi scade il 31 dicembre. |
| [!UICONTROL Priority] | Inserire un valore per la priorità della regola di determinazione prezzi. Un valore di priorità uguale a `1` è la priorità più alta. Se si dispone di più regole di determinazione prezzi, è possibile utilizzare il valore di priorità per determinare quale regola viene applicata per prima. Questo campo è necessario per utilizzare **Elimina regole successive** funzionalità. |
| [!UICONTROL Discard Subsequent Rules] | Utilizzato per consentire o impedire lo stacking di più regole di determinazione dei prezzi e per offrire sconti aggiuntivi. Per ignorare le regole successive, una regola di determinazione prezzi deve avere un valore definito per **[!UICONTROL Priority]**. Opzioni:<ul><li>**[!UICONTROL Yes]** - Scegliere quando non si desidera che vengano applicate altre regole di determinazione dei prezzi applicabili a un prodotto. Ignorare le regole successive significa che, quando più regole di determinazione dei prezzi si applicano allo stesso prodotto, viene applicata solo la regola di determinazione dei prezzi con il valore di priorità definito più alto.</li><li>**[!UICONTROL No]** - Scegliere quando si desidera consentire l&#39;applicazione di più regole di determinazione prezzi allo stesso prodotto. Questa opzione potrebbe comportare lo stacking e l&#39;applicazione di più sconti al prezzo dell&#39;inserzione.</li></ul> |
