---
title: Visualizza ordini Amazon
description: Visualizza gli ordini di Amazon Marketplace in Adobe Commerce o nell’amministratore di Magento Open Source.
feature: Sales Channels, Orders
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Visualizza ordini Amazon

Esistono due modi per visualizzare gli ordini Amazon: _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_.

Entrambe le opzioni mostrano le informazioni di base sull’ordine ricevute da Amazon, tra cui:

- Data di acquisto
- Numero ordine
- Stato
- Nome dell&#39;acquirente
- Totale complessivo
- Note ordine

La visualizzazione _[!UICONTROL All Orders]_aggiunge opzioni di filtro per le ricerche degli ordini.

>[!NOTE]
>
>Ad eccezione della colonna _[!UICONTROL Order Notes]_, la tabella_[!UICONTROL Amazon orders]_ viene compilata con le informazioni sull&#39;ordine ricevute da Amazon. La colonna _Note ordine_ è stata aggiornata da [!DNL Commerce] durante l&#39;elaborazione dell&#39;ordine.

## Ordini recenti

Puoi visualizzare gli ordini più recenti nella sezione _[!UICONTROL Recent Orders]_del [dashboard dello store](./amazon-store-dashboard.md).

![Ordini recenti](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### Visualizza gli ordini recenti di Amazon

1. Fare clic su **[!UICONTROL View Store]** su una scheda dello store.

1. Visualizza gli ordini nella sezione _[!UICONTROL Recent Orders]_.

1. Per visualizzare i dettagli dell&#39;ordine, fare clic sul numero dell&#39;ordine Amazon nella colonna _[!UICONTROL Order Number]_.

   Viene aperta la pagina _[!UICONTROL Amazon Order Details]_per l&#39;ordine.

## Visualizza tutti gli ordini

Puoi visualizzare tutti gli ordini Amazon nella pagina _[!UICONTROL Amazon orders]_(denominata anche visualizzazione_[!UICONTROL All Orders]_). La tabella Ordini di Amazon è simile alla sezione _[!UICONTROL Recent Orders]_del dashboard del negozio, ma consente di visualizzare tutti gli ordini di Amazon e di restringere l&#39;elenco degli ordini con le seguenti opzioni di filtro:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Ordini Amazon](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### Visualizza tutti gli ordini Amazon

1. Fare clic su **[!UICONTROL View Store]** su una scheda dello store.

1. Fare clic su **[!UICONTROL All Orders]** nella sezione _[!UICONTROL Recent Orders]_.

1. Per limitare l&#39;elenco o cercare un numero di ordine specifico, completare i parametri **[!UICONTROL Filter by]** e fare clic su **[!UICONTROL Apply filters]**.

1. Per visualizzare i dettagli dell&#39;ordine, fare clic sul numero dell&#39;ordine Amazon nella colonna _[!UICONTROL Order Number]_.

   Viene aperta la pagina _[!UICONTROL Amazon Order Details]_per l&#39;ordine.

## Utilizzo dei filtri

È possibile applicare i filtri all&#39;elenco ordini nella sezione _[!UICONTROL Filter by]_. Effettuare le selezioni e fare clic su **[!UICONTROL Apply filters]**. I filtri applicati vengono visualizzati sopra la griglia degli ordini.

![Filtri per la visualizzazione degli ordini di Amazon](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### Modifica dei filtri applicati

- È possibile aggiungere o modificare i filtri nella sezione _[!UICONTROL Filter by]_. Fare clic su **[!UICONTROL Apply filters]**per aggiornare l&#39;elenco degli ordini e le opzioni di filtro visualizzate sopra la griglia degli ordini.

- È possibile rimuovere i filtri, uno alla volta facendo clic su `x` per il filtro oppure tutti contemporaneamente facendo clic su **[!UICONTROL Clear all filters]**. La rimozione di un filtro aggiorna l&#39;elenco degli ordini e le opzioni di filtro visualizzate sopra la griglia degli ordini.

- Se l&#39;elenco degli ordini è lungo, è possibile utilizzare i controlli di impaginazione sotto la griglia per visualizzare più ordini.

>[!TIP]
>
>Alcuni suggerimenti sulla visualizzazione degli ordini:
>
>- Se disponi di più integrazioni di store Amazon, potrebbe essere necessario aggiornare la visualizzazione della pagina quando si passa da una visualizzazione all’altra per aggiornare sia l’elenco degli ordini che le visualizzazioni di impaginazione per il store corrente.
>- Quando si ordina per colonna, l’ordinamento viene applicato solo alla vista a elenco corrente. È consigliabile filtrare l’elenco e quindi ordinare la pagina visualizzata.
>- A seconda della larghezza della finestra di visualizzazione, è possibile che il testo delle colonne si sovrapponga. Per espandere le colonne del testo da disporre, allargare la visualizzazione della finestra.
>- Quando si filtra per _[!UICONTROL Total]_, filtrare per numeri interi. L&#39;immissione di un importo decimale può causare errori nei risultati.

### Colonne predefinite

| Colonna | Descrizione |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Filter by] | Disponibile solo nella visualizzazione _[!UICONTROL All Orders]_.<br>Limita l&#39;elenco degli ordini in base a:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | La data dell’acquisto, ricevuta da Amazon. |
| [!UICONTROL Order Number] | Il numero di ordine generato da e ricevuto da Amazon. Per visualizzare la schermata Dettagli ordine di Amazon, fai clic sul collegamento. |
| [!UICONTROL Status] | Lo stato dell’ordine, ricevuto da Amazon. Opzioni: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Il nome della persona che ha effettuato l’ordine ricevuto da Amazon. |
| [!UICONTROL Grand Total] | Il valore totale in valuta dell’ordine, come ricevuto da Amazon. |
| [!UICONTROL Order Notes] | Azione più recente registrata per l&#39;ordine durante l&#39;elaborazione in [!DNL Commerce]. Le informazioni includono, tra l’altro, gli errori di importazione degli ordini e gli aggiornamenti dell’elaborazione degli ordini.<br>**Nota**: questo campo è stato aggiornato da [!DNL Commerce] durante l&#39;elaborazione dell&#39;ordine. |
