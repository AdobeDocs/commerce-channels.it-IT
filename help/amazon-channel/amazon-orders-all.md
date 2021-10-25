---
title: Visualizza ordini Amazon
description: Visualizza gli ordini di Amazon Marketplace in Adobe Commerce o nell’amministratore di Magento Open Source.
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Visualizzare gli ordini di Amazon

Esistono due modi per visualizzare gli ordini Amazon: _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_.

Entrambe le opzioni mostrano le informazioni di base sull’ordine ricevute da Amazon, tra cui:

- Data acquisto
- Numero ordine
- Stato
- Nome dell&#39;acquirente
- Totale complessivo
- Note ordine

_[!UICONTROL All Orders]_visualizza aggiunge opzioni di filtro per le ricerche nell&#39;ordine.

>[!NOTE]
>
>Ad eccezione dei _[!UICONTROL Order Notes]_la colonna_[!UICONTROL Amazon orders]_ viene compilata con le informazioni sull’ordine ricevute da Amazon. La _Note ordine_ viene aggiornata da [!DNL Commerce] come l&#39;ordine elabora.

## Ordini recenti

Puoi visualizzare gli ordini più recenti nel _[!UICONTROL Recent Orders]_della sezione [dashboard store](./amazon-store-dashboard.md).

![Ordini recenti](assets/amazon-recent-orders-imported.png)

### Visualizzare gli ordini recenti di Amazon

1. Fai clic su **[!UICONTROL View Store]** su una scheda del negozio.

1. Visualizza gli ordini nel _[!UICONTROL Recent Orders]_sezione .

1. Per visualizzare i dettagli dell’ordine, fai clic sul numero dell’ordine Amazon nel _[!UICONTROL Order Number]_colonna.

   La _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina relativa all’ordine.

## Visualizza tutti gli ordini

Puoi visualizzare tutti i tuoi ordini Amazon nella _[!UICONTROL Amazon orders]_pagina (indicata anche come_[!UICONTROL All Orders]_ vista). La tabella Ordini di Amazon è simile alla tabella _[!UICONTROL Recent Orders]_della dashboard del negozio, ma ti consente di visualizzare tutti gli ordini di Amazon e di restringere l&#39;elenco degli ordini con le seguenti opzioni di filtro:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Ordini Amazon](assets/amazon-orders-list-all.png)

### Visualizza tutti gli ordini di Amazon

1. Fai clic su **[!UICONTROL View Store]** su una scheda del negozio.

1. Fai clic su **[!UICONTROL All Orders]** in _[!UICONTROL Recent Orders]_sezione .

1. Per limitare l’elenco o cercare un numero di ordine specifico, completa il **[!UICONTROL Filter by]** e fai clic su **[!UICONTROL Apply filters]**.

1. Per visualizzare i dettagli dell’ordine, fai clic sul numero dell’ordine Amazon nel _[!UICONTROL Order Number]_colonna.

   La _[!UICONTROL Amazon Order Details]_viene visualizzata la pagina relativa all’ordine.

## Utilizzo dei filtri

Puoi applicare i filtri all’elenco degli ordini nella _[!UICONTROL Filter by]_sezione . Effettua le selezioni e fai clic su **[!UICONTROL Apply filters]**. I filtri applicati vengono visualizzati sopra la griglia degli ordini.

![Filtri per la visualizzazione degli ordini Amazon](assets/amazon-orders-filter-view.png)

### Modifica dei filtri applicati

- Puoi aggiungere o modificare i filtri nel _[!UICONTROL Filter by]_sezione . Fai clic su **[!UICONTROL Apply filters]**per aggiornare l&#39;elenco degli ordini e le opzioni filtro visualizzate sopra la griglia degli ordini.

- Puoi rimuovere i filtri uno alla volta facendo clic sul pulsante `x` per il filtro o tutti contemporaneamente facendo clic su **[!UICONTROL Clear all filters]**. La rimozione di un filtro aggiorna l’elenco degli ordini e le opzioni filtro visualizzate sopra la griglia degli ordini.

- Se l&#39;elenco degli ordini è lungo, è possibile utilizzare i controlli di impaginazione sotto la griglia per visualizzare altri ordini.

>[!TIP]
>
>Alcuni suggerimenti sulla visualizzazione degli ordini:
>
>- Se disponi di più integrazioni Amazon Store, potrebbe essere necessario aggiornare la visualizzazione della pagina quando si passa da una visualizzazione store all&#39;altra per aggiornare sia l&#39;elenco degli ordini che le visualizzazioni di impaginazione per l&#39;archivio corrente.
>- Quando si effettua l’ordinamento per colonna, questo si applica solo alla vista elenco corrente. È consigliabile filtrare l’elenco e quindi ordinare la pagina da visualizzare.
>- A seconda della larghezza della finestra di visualizzazione, è possibile che nelle colonne sia presente una sovrapposizione del testo. Per espandere le colonne del testo da mandare a capo, allargate la visualizzazione della finestra.
>- Quando si filtra _[!UICONTROL Total]_, filtra per numeri interi. L&#39;immissione di un importo decimale può causare errori nei risultati.


### Colonne predefinite

| Colonna | Descrizione |
|---|---|
| [!UICONTROL Filter by] | Disponibile solo nel _[!UICONTROL All Orders]_visualizza.<br>Limita l’elenco degli ordini in base a:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | La data dell’acquisto, come ricevuta da Amazon. |
| [!UICONTROL Order Number] | Numero dell’ordine generato da e ricevuto da Amazon. Per visualizzare la schermata Dettagli ordine di Amazon, fai clic sul collegamento . |
| [!UICONTROL Status] | Lo stato dell’ordine ricevuto da Amazon. Opzioni: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Nome della persona che ha effettuato l’ordine, come ricevuto da Amazon. |
| [!UICONTROL Grand Total] | Il valore della valuta totale dell&#39;ordine, come ricevuto da Amazon. |
| [!UICONTROL Order Notes] | L&#39;azione più recente registrata per l&#39;ordine mentre elabora in [!DNL Commerce]. Le informazioni includono, tra l’altro, errori di importazione degli ordini e aggiornamenti dell’elaborazione degli ordini.<br>**Nota**: Questo campo viene aggiornato da [!DNL Commerce] come l&#39;ordine elabora. |
