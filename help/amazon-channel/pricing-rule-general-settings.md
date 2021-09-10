---
title: Impostazioni generali della regola di determinazione prezzi
description: Utilizza le impostazioni generali della regola del prezzo per definire le caratteristiche principali di una regola del prezzo di listino.
redirect_from: /sales-channels/asc/ob-pricing-rules-general-settings.html: 
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 711
ht-degree: 0%

---

# Impostazioni generali della regola di determinazione prezzi

Definisci il nome, la descrizione, le date attive e la priorità della regola.

## Completa la sezione Impostazioni generali della regola del prezzo

1. Per **[!UICONTROL Rule Name]** (obbligatorio), immetti il nome della regola.

   Questo nome è solo a scopo di identificazione interno. Più descrittivo è il nome della regola, meglio sarà.

1. Per **[!UICONTROL Description]**, immetti una descrizione dettagliata della regola.

   Questa descrizione potrebbe includere informazioni sui prodotti idonei, sulle date attive, sulla formula per il calcolo del prezzo adeguato o su qualsiasi altra informazione utile per modificare la regola.

1. Per **[!UICONTROL Status]**, scegli un’opzione:

   - `Active` - Scegli questa opzione quando desideri che la regola di prezzo si applichi ai prodotti idonei e regola il prezzo dell&#39;inserzione prima della pubblicazione in Amazon.

   - `Inactive` - Scegliere questa opzione se non si desidera che la regola di determinazione dei prezzi si applichi ai prodotti idonei. Questa opzione viene utilizzata molto probabilmente quando si modifica una regola di prezzo o la si disattiva dopo una promozione limitata.

1. Per **[!UICONTROL From]** e **[!UICONTROL To]**, immettere una data di inizio e una data di fine per la regola di determinazione dei prezzi.

   Puoi anche fare clic sull’icona del calendario per selezionare una data dal calendario dinamico. Questa opzione di avvio e arresto automatico è utile quando si impostano promozioni a tempo limitato o stagionali con date di inizio e fine definite.

1. Per **[!UICONTROL Priority]**, immetti un valore numerico per la priorità della regola.

   Il valore di priorità uguale a `1` è la priorità più elevata. In presenza di più regole di determinazione dei prezzi attive, è possibile utilizzare questo valore di priorità per determinare quale regola viene applicata per prima. Questo campo è necessario per utilizzare la funzione _[!UICONTROL Discard Subsequent Rules]_.

1. Per **[!UICONTROL Discard Subsequent Rules]**, scegli un’opzione:

   - `Yes` - Scegliere questa opzione quando non si desidera applicare altre regole di determinazione prezzi applicabili a un prodotto. Se si scartano le regole successive, se al prodotto vengono applicate più regole di determinazione dei prezzi, al prodotto viene applicata solo la regola di determinazione dei prezzi con il valore di priorità definito più elevato. Questa opzione impedisce a più regole di determinazione dei prezzi di sovrapporsi e di fornire sconti aggiuntivi non intenzionali.

   - `No` - Scegliere questa opzione quando si desidera consentire l&#39;applicazione di più regole di determinazione prezzi allo stesso prodotto. Questa opzione può comportare l’impilamento e l’offerta di più sconti da applicare.

>[!NOTE]
>
>Per eliminare le regole successive, una regola di determinazione prezzi deve avere un valore definito **Priorità**.

![Impostazioni generali della regola di determinazione prezzi](assets/amazon-pricing-rule-general.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Rule Name] | (Obbligatorio) Immetti un nome per la regola, utilizzato a scopo di identificazione interna. Più descrittivo è il nome della regola, meglio sarà. Ad esempio, &quot;25% di sconto sulla vendita di libri di fine anno&quot;. |
| [!UICONTROL Description] | Immetti una descrizione dettagliata che spieghi la regola (utilizzata anche per scopi interni). Ad esempio, &quot;Vendita di fine anno, 25% di sconto su tutti gli articoli della categoria Libri&quot;. |
| [!UICONTROL Status] | Opzioni:<ul><li>**[!UICONTROL Inactive]** - La regola dei prezzi non si applica alle inserzioni. Questa opzione può essere utilizzata per modificare una regola di prezzo o disattivarla dopo una promozione limitata.</li><li>**[!UICONTROL Active]** - La regola dei prezzi si applica alle inserzioni e regola i prezzi delle inserzioni prima di pubblicarle in Amazon.</li></ul> |
| [!UICONTROL From] | Immettere la data di inizio all&#39;inizio della regola di determinazione prezzi. Ad esempio, per avere una vendita durante l’ultimo mese dell’anno, imposta la data `From` sul 1° dicembre in modo che la regola dei prezzi si applichi automaticamente alle inserzioni Amazon a partire dal 1° dicembre. |
| [!UICONTROL To] | Immettere la data di fine alla fine della regola di determinazione dei prezzi. Continuando l&#39;esempio precedente, per limitare la vendita all&#39;ultimo mese dell&#39;anno, imposterai la data `To` come 31 dicembre, quindi la regola dei prezzi scade il 31 dicembre. |
| [!UICONTROL Priority] | Immettere un valore per la priorità della regola di determinazione prezzi. Un valore di priorità uguale a `1` è la priorità più elevata. In presenza di più regole di determinazione dei prezzi, è possibile utilizzare il valore di priorità per determinare quale regola viene applicata per prima. Questo campo è necessario per utilizzare la funzione **Ignora regole successive** . |
| [!UICONTROL Discard Subsequent Rules] | Utilizzato per consentire o impedire che più regole di determinazione dei prezzi vengano sovrapposte e fornire ulteriori sconti. Per eliminare le regole successive, una regola di determinazione prezzi deve avere un valore definito per **[!UICONTROL Priority]**. Opzioni:<ul><li>**[!UICONTROL Yes]** - Scegliere il momento in cui non si desidera applicare altre regole di determinazione dei prezzi applicabili a un prodotto. Se si scartano le regole successive, quando più regole di determinazione dei prezzi si applicano allo stesso prodotto, viene applicata solo la regola di determinazione dei prezzi con il valore di priorità definito più elevato.</li><li>**[!UICONTROL No]** - Scegli quando consentire l&#39;applicazione di più regole di determinazione prezzi allo stesso prodotto. Questa opzione potrebbe comportare l’applicazione di stacking e di più sconti al prezzo dell’inserzione.</li></ul> |
