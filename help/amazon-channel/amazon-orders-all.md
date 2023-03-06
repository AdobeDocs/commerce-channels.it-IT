---
title: Visualizza ordini Amazon
description: Visualizza gli ordini di Amazon Marketplace in Adobe Commerce o nell’amministratore di Magento Open Source.
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Visualizza ordini Amazon

Esistono due modi per visualizzare gli ordini di Amazon: _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_.

Entrambe le opzioni mostrano le informazioni di base sull’ordine ricevute da Amazon, tra cui:

- Data di acquisto
- Numero ordine
- Stato
- Nome dell&#39;acquirente
- Totale complessivo
- Note ordine

_[!UICONTROL All Orders]_visualizza aggiunge opzioni di filtro per le ricerche degli ordini.

>[!NOTE]
>
>Ad eccezione del _[!UICONTROL Order Notes]_, la colonna_[!UICONTROL Amazon orders]_ La tabella viene compilata con le informazioni sugli ordini ricevute da Amazon. Il _Note ordine_ la colonna è aggiornata da [!DNL Commerce] come l’ordine elabora.

## Ordini recenti

Puoi visualizzare gli ordini più recenti in _[!UICONTROL Recent Orders]_sezione del [dashboard store](./amazon-store-dashboard.md).

![Ordini recenti](assets/amazon-recent-orders-imported.png)

### Visualizza gli ordini recenti di Amazon

1. Clic **[!UICONTROL View Store]** su una carta del negozio.

1. Visualizza gli ordini in _[!UICONTROL Recent Orders]_sezione.

1. Per visualizzare i dettagli dell’ordine, fai clic sul numero dell’ordine di Amazon in _[!UICONTROL Order Number]_colonna.

   Il _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina dell’ordine.

## Visualizza tutti gli ordini

Puoi visualizzare tutti gli ordini di Amazon sulla _[!UICONTROL Amazon orders]_pagina (nota anche come_[!UICONTROL All Orders]_ view). La tabella Ordini di Amazon è simile alla _[!UICONTROL Recent Orders]_sezione del dashboard del negozio, ma consente di visualizzare tutti gli ordini di Amazon e di restringere l’elenco degli ordini con le seguenti opzioni di filtro:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Ordini Amazon](assets/amazon-orders-list-all.png)

### Visualizza tutti gli ordini Amazon

1. Clic **[!UICONTROL View Store]** su una carta del negozio.

1. Clic **[!UICONTROL All Orders]** nel _[!UICONTROL Recent Orders]_sezione.

1. Per restringere l&#39;elenco o cercare un numero di ordine specifico, completare la **[!UICONTROL Filter by]** e fai clic su **[!UICONTROL Apply filters]**.

1. Per visualizzare i dettagli dell’ordine, fai clic sul numero dell’ordine di Amazon in _[!UICONTROL Order Number]_colonna.

   Il _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina dell’ordine.

## Utilizzo dei filtri

Puoi applicare i filtri all’elenco degli ordini nel _[!UICONTROL Filter by]_sezione. Effettuare le selezioni e fare clic su **[!UICONTROL Apply filters]**. I filtri applicati vengono visualizzati sopra la griglia degli ordini.

![Filtri per visualizzare gli ordini di Amazon](assets/amazon-orders-filter-view.png)

### Modifica dei filtri applicati

- Puoi aggiungere o modificare i filtri nella sezione _[!UICONTROL Filter by]_sezione. Clic **[!UICONTROL Apply filters]**per aggiornare l&#39;elenco degli ordini e le opzioni di filtro visualizzate sopra la griglia degli ordini.

- Per rimuovere i filtri, uno alla volta, fai clic sul pulsante `x` per il filtro o tutti contemporaneamente facendo clic su **[!UICONTROL Clear all filters]**. La rimozione di un filtro aggiorna l&#39;elenco degli ordini e le opzioni di filtro visualizzate sopra la griglia degli ordini.

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
|---|---|
| [!UICONTROL Filter by] | Disponibile solo in _[!UICONTROL All Orders]_visualizzazione.<br>Limita l’elenco degli ordini in base a:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | La data dell’acquisto, ricevuta da Amazon. |
| [!UICONTROL Order Number] | Il numero di ordine generato da e ricevuto da Amazon. Per visualizzare la schermata Dettagli ordine di Amazon, fai clic sul collegamento. |
| [!UICONTROL Status] | Lo stato dell’ordine, ricevuto da Amazon. Opzioni: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Il nome della persona che ha effettuato l’ordine ricevuto da Amazon. |
| [!UICONTROL Grand Total] | Il valore totale in valuta dell’ordine, come ricevuto da Amazon. |
| [!UICONTROL Order Notes] | Azione più recente registrata per l’ordine durante l’elaborazione in [!DNL Commerce]. Le informazioni includono, tra l’altro, gli errori di importazione degli ordini e gli aggiornamenti dell’elaborazione degli ordini.<br>**Nota**: campo aggiornato da [!DNL Commerce] come l’ordine elabora. |
