---
title: 'Introduzione a [!DNL Channel Manager]'
description: '''Scopri come installare e utilizzare [!DNL Channel Manager] per integrare Adobe Commerce e i negozi di Magento Open Source con Walmart Marketplace e creare un canale di vendita per gestire gli elenchi di mercati, i prezzi, le scorte e le vendite direttamente dal tuo amministratore Commerce."'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Introduzione a [!DNL Channel Manager]

[!DNL Channel Manager] aiuta i commercianti ad aumentare le vendite, raggiungere nuovi clienti, semplificare le operazioni di vendita e risparmiare tempo integrando un catalogo di prodotti Adobe Commerce o Magento Open Source con [!DNL Walmart Marketplace].

![[!DNL Channel Manager] vista amministratore dell&#39;estensione](assets/channel-manager-home.png)

[!DNL Channel Manager] supporta Adobe Commerce o i commercianti di Magenti Open Source che desiderano vendere su [!DNL Walmart Marketplace] estendendo [!DNL Commerce] Amministratore. Con [!DNL Channel Manager] installati, gli amministratori dei negozi e il personale operativo possono gestire [!DNL Walmart Marketplace] vendita, inventario e prezzi dei prodotti direttamente dall&#39;ambiente Commerce.

L&#39;amministratore esteso ottimizza le operazioni perché i commercianti possono utilizzare gli stessi flussi di lavoro e gli stessi processi per gestire le vendite da entrambi [!DNL Commerce] vetrine e il mercato Walmart.

Dopo l’installazione e la configurazione [!DNL Channel Manager], puoi utilizzare le seguenti funzionalità per gestire gli ordini di vendita di Walmart Marketplace:

* **Gestione dell&#39;elenco**- Facile connessione degli elenchi dei prodotti mediante l&#39;abbinamento dei prodotti [!DNL Commerce] catalogo a esistente [!DNL Walmart Marketplace] elenchi.

* **Inventory management**-Gli articoli nel conto del venditore del marketplace del commerciante vengono automaticamente sincronizzati e aggiornati da [!DNL Commerce] garantire livelli di inventario precisi.

* **Aggiornamenti dei prezzi**- Mantenere prezzi accurati per gli elenchi di marketplace con sincronizzazione automatica dei prezzi. Quando un prezzo cambia in Adobe Commerce, le modifiche si riflettono sul mercato.

* **Gestione degli ordini**- Quando vengono creati nuovi ordini sul mercato, [!DNL Channel Manager] sincronizza gli ordini con Adobe Commerce e invia le convalide degli ordini al marketplace. Questa conferma assicura che l&#39;inventario sia riservato per ogni ordine. Il passaggio finale consiste nel creare gli ordini corrispondenti nel [!DNL Commerce] Sistema di gestione degli ordini per l&#39;elaborazione.

* **Gestione della spedizione**- Quando gli ordini sono contrassegnati come spediti in Adobe Commerce, l&#39;aggiornamento della spedizione viene inviato al [!DNL Walmart Marketplace]. Questa notifica assicura che i venditori soddisfino i loro requisiti SLA e che i clienti ricevano notifiche di aggiornamento della spedizione per i loro ordini correnti.

* **Cancellazioni**- Quando gli ordini vengono annullati in Adobe Commerce, [!DNL Channel Manager] invia informazioni aggiornate sull’ordine al marketplace per replicare l’azione per l’ordine di marketplace corrispondente. Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] gli aggiornamenti della quantità di magazzino per riflettere gli articoli restituiti e gli aggiornamenti delle scorte vengono sincronizzati automaticamente in [!DNL Walmart Marketplace].

* **Restituzioni**- Quando Walmart Marketplace richiede un ritorno per gli articoli ordinati attraverso il canale di vendita Adobe Commerce o Magento Open Source, [!DNL Channel Manager] invia le informazioni sulla richiesta di restituzione all&#39;archivio dei canali di vendita Commerce per replicare la richiesta di restituzione. Poi, il rimborso può essere elaborato utilizzando il [!DNL Commerce] [workflow di rimborso](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow), metodo offline . Al termine del rimborso, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart in modo che lo stato di ritorno nell&#39;account del venditore del marketplace possa essere aggiornato per riflettere il rimborso.

## Latenza prevista per [!DNL Channel Manager] operazioni

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e collegati [!DNL Walmart Marketplace] archiviare richiede un po&#39; di tempo per completare. Esamina il tempo di elaborazione previsto per [!DNL Channel Manager] operazioni che consentono di pianificare il funzionamento dei canali di vendita.

**Latenza stimata per [!DNL Channel Manager] operazioni**

| **Funzionamento** | **Descrizione** | **Ritardo previsto** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a [!DNL Channel Manager] | Seleziona i prodotti dal menu [!DNL Commerce] catalogo dei prodotti e importarli in [!DNL Channel Manager]. | **Fino a cinque minuti**- Se selezioni molti prodotti, ad esempio un intero catalogo di prodotti, il processo di importazione richiede più tempo. |
| Confronta prodotti su [!DNL Walmart Marketplace] | Seleziona gli elenchi dei prodotti in [!DNL Channel Manager] e inviare a Walmart per la corrispondenza. | **Fino a 30 minuti**- Se selezioni molti prodotti, il processo di corrispondenza richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti dell&#39;inventario | Quando la quantità di inventario cambia in Commerce, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando cambia il prezzo di un prodotto, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart. | **Fino a cinque minuti** |
| Ordina sincronizzazioni da Walmart a [!DNL Commerce] | Ordini cliente a [!DNL Commerce] prodotto sul mercato Walmart. Walmart invia l&#39;ordine a [!DNL Channel Manager]. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in [!DNL Commerce] Gestione degli ordini | [!DNL Channel Manager] crea [!DNL Commerce] l&#39;ordine di Walmart e aggiorna il dashboard dell&#39;ordine in modo da includere il [!DNL Commerce] numero d&#39;ordine. | **Fino a cinque minuti** |
| Aggiornamento dello stato della spedizione in [!DNL Commerce] Gestione degli ordini | Quando un ordine viene spedito da Commerce, [!DNL Channel Manager] aggiorna lo stato di spedizione nel dashboard dell&#39;ordine e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa essere informato. | **Fino a cinque minuti** |
| Aggiornamento dell&#39;annullamento dell&#39;ordine in Gestione ordini di Commerce | Quando un ordine viene annullato da Commerce, [!DNL Channel Manager] aggiorna lo stato dell&#39;ordine nel dashboard dell&#39;ordine e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa ricevere notifiche. Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. | **Fino a cinque minuti** |


