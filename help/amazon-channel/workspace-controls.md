---
title: Canale di vendita Amazon - Controlli Workspace
description: Il Sales Channel Amazon fornisce controlli dell’area di lavoro che consentono di individuare le inserzioni, visualizzare le informazioni e applicare facilmente e con facilità le azioni.
feature: Sales Channels
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Controlli Workspace

Il canale di vendita Amazon [home page](./amazon-sales-channel-home.md) dispone di alcuni controlli comuni dell&#39;area di lavoro, tra cui Filtri, Visualizzazione predefinita, Colonne ed Esporta. Non tutte le pagine hanno le stesse opzioni di controllo.

![Esempi di controllo dell&#39;area di lavoro di Sales Channel di Amazon](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## Azioni

Il selettore _[!UICONTROL Actions]_fornisce un elenco di azioni disponibili per un utente per una pagina. Quando viene selezionata, l’azione viene applicata a tutti gli elementi selezionati. Per applicare un&#39;azione a un elemento specifico, selezionare la casella di controllo nella prima colonna di ogni elemento e scegliere un&#39;opzione in_[!UICONTROL Actions]_.

Ad esempio, quando il selettore viene visualizzato nella pagina _[!UICONTROL Attributes]_, include l&#39;azione_[!UICONTROL Re-import Product Attribute Values]_. La scelta di questa azione comporta il ping dell&#39;account [!DNL Amazon Seller Central] corrispondente e aggiorna i dati [!DNL Commerce] per ciascuno degli elementi dell&#39;archivio Amazon archiviati nella colonna a sinistra.

![Esempio di menu Azioni](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## Filtri

Il controllo _[!UICONTROL Filters]_mostra le opzioni per restringere i dati visualizzati nella tabella. Le opzioni filtro si basano sulle colonne selezionate nel controllo Colonne. Le opzioni di filtro vengono visualizzate solo per le colonne abilitate nel controllo Columns.

I controlli Filtri possono includere calendari dinamici per limitare i dati per date specifiche, menu a discesa per colonne con selezioni predefinite e campi di testo libero che possono contenere dati personalizzati.

Nell&#39;esempio seguente vengono illustrate le impostazioni per filtrare l&#39;elenco degli ordini in modo da visualizzare solo gli ordini che soddisfano i criteri seguenti:

- gli ordini effettuati tra il 2/01/2019 e il 2/07/2019, e
- Ordini con un buyer denominato `Smith` e
- Ordini con stato `Shipped`.

Dopo aver impostato le opzioni di filtro, fare clic su **[!UICONTROL Apply Filters]** per filtrare i dati elencati. Fare clic su Annulla per uscire dal controllo Filtri senza applicare.

![Esempio di controllo Filtri](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

Dopo aver applicato i filtri ai dati, verranno visualizzate le informazioni di **[!UICONTROL Active Filters]**. È possibile fare clic sull&#39;icona ![Cancella filtri](assets/x-icon-clear-filters.png) per cancellare un&#39;opzione di filtro specifica oppure fare clic su **[!UICONTROL Clear All]** per cancellare tutti i filtri applicati.

![Esempio di filtri attivi](assets/applied-filters-line.png){width="700"}

## Visualizza

Il controllo View si basa sulle colonne predefinite della pagina, pertanto viene denominato Default View (Visualizzazione predefinita). È possibile aggiungere o rimuovere le colonne disponibili utilizzando il controllo Colonne. Quando si personalizzano le colonne, è quindi possibile salvare la visualizzazione come visualizzazione personalizzata nel controllo Visualizzazione.

Quando hai aggiunto o rimosso le colonne dalla visualizzazione della pagina:

1. Fare clic su **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Immettere un nome per la visualizzazione.

1. Per salvare la visualizzazione personalizzata, fai clic sull’icona a forma di freccia.

![Visualizza esempio di controllo](assets/workspace-controls-view.png)

In questo esempio, la colonna _ID ordine_ viene aggiunta nel controllo Column e salvata come visualizzazione personalizzata. Dopo il salvataggio del nome della visualizzazione personalizzata, il nome della visualizzazione è cambiato da _Visualizzazione predefinita_ al nome immesso.

È possibile passare da una visualizzazione all&#39;altra selezionando la visualizzazione desiderata nel menu _[!UICONTROL View]_.

Per eliminare o modificare il nome della visualizzazione personalizzata, fare clic sull&#39;icona della matita. Puoi quindi immettere un nome diverso oppure fare clic sull’icona del cestino per eliminare la visualizzazione personalizzata. Impossibile eliminare la visualizzazione predefinita.

## Colonne

Il controllo Columns consente di aggiungere o rimuovere colonne di dati dalla visualizzazione della pagina. Ogni pagina del canale di vendita di Amazon dispone di una combinazione predefinita di colonne di dati, ma la maggior parte delle pagine dispone di colonne aggiuntive. Se non sono disponibili colonne aggiuntive, è comunque possibile rimuovere le colonne predefinite dalla visualizzazione.

Nell&#39;esempio seguente viene illustrato un controllo Columns. Le opzioni selezionate corrispondono alle intestazioni di colonna visualizzate nella pagina.

- Per aggiungere una colonna di dati alla pagina, seleziona la casella di controllo.
- Per rimuovere una colonna di dati dalla pagina, non selezionare la casella di controllo.

![Esempio di controllo Colonne](assets/workspace-controls-columns.png){width="400"}

Le modifiche apportate alla casella di controllo vengono visualizzate immediatamente. Se si apportano modifiche e si esce dalla pagina, questa ritorna alla visualizzazione di colonna predefinita. Per le modifiche apportate regolarmente, è possibile salvare le modifiche apportate alle colonne come visualizzazione personalizzata nel controllo Visualizza. È quindi possibile attivare o disattivare il controllo Visualizza senza dover aggiungere o rimuovere manualmente le colonne.

È possibile fare clic su **[!UICONTROL Reset]** per ripristinare le impostazioni predefinite oppure fare clic su **[!UICONTROL Cancel]** per uscire senza apportare modifiche.

## Esporta

L&#39;opzione Esporta consente di esportare i dati in un file di dati che può essere importato in un software di terze parti o in un database separato. I dati esportati sono limitati ai dati visualizzati. Se necessario, assicurarsi di aggiungere o rimuovere colonne prima di utilizzare il controllo Esporta.

Al termine dell&#39;esportazione dei dati, scegliere un&#39;opzione di formato di esportazione e fare clic su **[!UICONTROL Export]**.

- CSV: un file di valori separati da virgole contenente dati in testo normale
- XML di Excel: un formato di dati di foglio di calcolo basato su XML (in genere utilizzato per gli utenti di Excel)

Il file di dati generato viene salvato automaticamente nella cartella specificata per i download.

![Controllo esportazione](assets/workspace-controls-export.png){width="250"}
