---
title: Controlli Workspace
description: Amazon Sales Channel fornisce controlli dell’area di lavoro per individuare elenchi, visualizzare informazioni e applicare facilmente le azioni.
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Controlli Workspace

Canale di vendita Amazon [home page](./amazon-sales-channel-home.md) dispone di alcuni controlli comuni dell’area di lavoro, tra cui Filtri, Vista predefinita, Colonne ed Esportazione. Non tutte le pagine dispongono delle stesse opzioni di controllo.

![Esempi di controllo dell’area di lavoro di Amazon Sales Channel](assets/amazon-workspace-controls.png)

## Azioni

La _[!UICONTROL Actions]_Il selettore fornisce un elenco di azioni disponibili per un utente per una pagina. Quando questa opzione è selezionata, l’azione viene applicata a tutti gli elementi selezionati. Per applicare un’azione a un elemento specifico, seleziona la casella di controllo nella prima colonna di ciascun elemento e scegli un’opzione in_[!UICONTROL Actions]_.

Ad esempio, quando il selettore viene visualizzato nella sezione _[!UICONTROL Attributes]_include_[!UICONTROL Re-import Product Attribute Values]_ azione. La scelta di questa azione esegue il ping del corrispondente [!DNL Amazon Seller Central] e aggiorna il [!DNL Commerce] i dati per ciascuno degli elementi dell’archivio Amazon controllati nella colonna a sinistra.

![Esempio di menu Azioni](assets/amazon-sales-channel-home-actions-option.png)

## Filtri

La _[!UICONTROL Filters]_Il controllo mostra le opzioni per la riduzione dei dati visualizzati nella tabella. Le opzioni filtro si basano sulle colonne selezionate nel controllo Colonne . Le opzioni filtro vengono visualizzate solo per le colonne abilitate nel controllo Colonne.

I controlli dei filtri possono includere calendari dinamici per limitare i dati per date specifiche, menu a discesa per colonne con selezioni predefinite e campi di testo libero che possono contenere dati personalizzati.

L’esempio seguente mostra le impostazioni per filtrare l’elenco di ordini in modo da visualizzare solo gli ordini che soddisfano i seguenti criteri:

- Ordini collocati tra il 2/01/2019 e il 2/07/2019, e
- Ordini con un acquirente denominato in `Smith`e
- Ordini con stato `Shipped`.

Quando hai impostato le opzioni di filtro, fai clic su **[!UICONTROL Apply Filters]** per filtrare i dati elencati. Fare clic su Annulla per uscire dal controllo Filtri senza applicare alcuna applicazione.

![Esempio di controllo dei filtri](assets/workspace-controls-filters.png)

Dopo aver applicato i filtri ai dati, **[!UICONTROL Active Filters]** verranno visualizzate le informazioni. Puoi fare clic su ![Icona Cancella filtri](assets/x-icon-clear-filters.png) per cancellare un’opzione di filtro specifica o fare clic su **[!UICONTROL Clear All]** per cancellare tutti i filtri applicati.

![Esempio di filtri attivi](assets/applied-filters-line.png)

## Visualizza

Il controllo Visualizza si basa sulle colonne predefinite per la pagina, quindi viene denominato Vista predefinita. È possibile aggiungere o rimuovere le colonne disponibili utilizzando il controllo Colonne . Quando si personalizzano le colonne, è quindi possibile salvare la visualizzazione come visualizzazione personalizzata nel controllo Visualizza.

Quando le colonne vengono aggiunte o rimosse dalla pagina vengono visualizzate:

1. Clic **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Immettere un nome per la visualizzazione.

1. Per salvare la visualizzazione personalizzata, fare clic sull&#39;icona a forma di freccia.

![Visualizza esempio di controllo](assets/workspace-controls-view.png)

In questo esempio, la _ID ordine_ viene aggiunta nel controllo Colonna e salvata come visualizzazione personalizzata. Dopo il salvataggio del nome della visualizzazione personalizzata, il nome della visualizzazione viene modificato da _Vista predefinita_ al nome immesso.

Per passare da una visualizzazione all’altra, seleziona la vista desiderata nel _[!UICONTROL View]_menu.

Per eliminare o modificare il nome della visualizzazione personalizzata, fai clic sull’icona a forma di matita. Puoi quindi immettere un nome diverso oppure fare clic sull’icona del cestino per eliminare la visualizzazione personalizzata. Impossibile eliminare la visualizzazione predefinita.

## Colonne

Il controllo Columns consente di aggiungere o rimuovere colonne di dati dalla visualizzazione della pagina. Ogni pagina del canale di vendita Amazon ha una combinazione preimpostata di colonne di dati, ma la maggior parte delle pagine dispone di colonne aggiuntive disponibili. Se non sono disponibili altre colonne, è comunque possibile rimuovere le colonne predefinite dalla visualizzazione.

Nell&#39;esempio seguente viene illustrato un controllo Columns. Le opzioni selezionate corrispondono alle intestazioni di colonna visualizzate nella pagina.

- Per aggiungere una colonna di dati alla pagina, seleziona la casella di controllo .
- Per rimuovere una colonna di dati dalla pagina, non selezionare la casella di controllo.

![Esempio di controllo delle colonne](assets/workspace-controls-columns.png)

Le modifiche della casella di controllo vengono visualizzate immediatamente. Se apporti modifiche e chiudi la pagina, torna alla visualizzazione della colonna predefinita. Per le modifiche apportate regolarmente, è possibile salvare le modifiche delle colonne come visualizzazione personalizzata nel controllo Visualizza. È quindi possibile attivare il controllo Visualizza senza dover aggiungere o rimuovere manualmente le colonne.

Puoi fare clic su **[!UICONTROL Reset]** per ripristinare le opzioni predefinite, oppure puoi fare clic su **[!UICONTROL Cancel]** per uscire senza apportare modifiche.

## Esporta

L’opzione Esporta consente di esportare i dati in un file di dati di quanto sia possibile importare in un software di terze parti o in un database separato. I dati esportati sono limitati ai dati visualizzati. Se necessario, assicurarsi di aggiungere o rimuovere le colonne prima di utilizzare il controllo Esporta.

Quando sei pronto per esportare i dati, scegli un’opzione di formato di esportazione e fai clic su **[!UICONTROL Export]**.

- CSV - un file di valori separati da virgole contenente dati di testo normale
- Excel XML - Formato dati foglio di calcolo basato su XML (generalmente utilizzato per gli utenti Excel)

Il file di dati generato viene salvato automaticamente nella cartella designata per i download.

![Controllo delle esportazioni](assets/workspace-controls-export.png)
