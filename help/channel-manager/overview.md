---
title: '"Introduzione a [!DNL Channel Manager]'''
description: "Scopri come installare e utilizzare [!DNL Channel Manager] integrare Adobe Commerce e i negozi di Magento Open Source con Walmart Marketplace e creare un canale di vendita per gestire in modo semplice le inserzioni, i prezzi, l’inventario e le vendite nel marketplace dal proprio amministratore Commerce."
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# Introduzione a [!DNL Channel Manager]

[!DNL Channel Manager] consente ai commercianti di aumentare le vendite, raggiungere nuovi clienti, semplificare le operazioni di vendita e risparmiare tempo integrando un catalogo di prodotti Adobe Commerce o Magenti Open Source con [!DNL Walmart Marketplace].

![[!DNL Channel Manager] visualizzazione amministrazione dell’estensione](assets/channel-manager-home.png)

[!DNL Channel Manager] supporta i commercianti Adobe Commerce o di Magento Open Source che desiderano vendere su [!DNL Walmart Marketplace] estendendo il [!DNL Commerce] Amministratore Con [!DNL Channel Manager] installate, gli amministratori dei negozi e il personale operativo possono gestire [!DNL Walmart Marketplace] vendite, inventario e prezzi dei prodotti direttamente dall’ambiente Commerce.

L’amministratore esteso semplifica le operazioni perché gli esercenti possono utilizzare gli stessi flussi di lavoro e gli stessi processi per gestire le vendite da entrambi [!DNL Commerce] vetrine e Walmart Marketplace.

Dopo aver installato e configurato [!DNL Channel Manager], è possibile utilizzare le funzionalità seguenti per gestire gli ordini di vendita di Walmart Marketplace:

* **Gestione elenchi**- Facile connessione degli elenchi di prodotti grazie alla corrispondenza dei prodotti [!DNL Commerce] catalogo a esistente [!DNL Walmart Marketplace] inserzioni.

* **Inventory management**-Gli oggetti nel conto del venditore del marketplace del commerciante vengono automaticamente sincronizzati e aggiornati da [!DNL Commerce] per garantire livelli di inventario accurati.

* **Aggiornamenti dei prezzi**- Gestisce la determinazione dei prezzi accurata per le inserzioni sul marketplace con la sincronizzazione automatica dei prezzi. Quando un prezzo cambia in Adobe Commerce, le modifiche si riflettono sul marketplace.

* **Gestione ordini**- Quando vengono creati nuovi ordini sul mercato, [!DNL Channel Manager] sincronizza gli ordini con Adobe Commerce e invia le conferme degli ordini al marketplace. Questa conferma garantisce che l&#39;inventario sia prenotato per ogni ordine. Il passaggio finale consiste nel creare gli ordini corrispondenti nel [!DNL Commerce] Sistema Order Management per l&#39;elaborazione.

* **Gestione spedizione**- Quando gli ordini vengono contrassegnati come spediti in Adobe Commerce, l&#39;aggiornamento della spedizione viene inviato al [!DNL Walmart Marketplace]. Questa notifica garantisce che i venditori soddisfino i requisiti SLA e che i clienti ricevano le notifiche di aggiornamento della spedizione per gli ordini correnti.

* **Annullamenti**- Quando gli ordini vengono annullati in Adobe Commerce, [!DNL Channel Manager] invia informazioni aggiornate sull’ordine al marketplace per replicare l’azione per l’ordine di marketplace corrispondente. Al termine dell’annullamento dell’ordine, il [!DNL Commerce] gli aggiornamenti della quantità di magazzino per riflettere gli articoli restituiti e gli aggiornamenti del magazzino vengono sincronizzati automaticamente con [!DNL Walmart Marketplace].

* **Restituzioni e restituzioni**- Quando Walmart Marketplace richiede una restituzione per gli articoli ordinati tramite il canale di vendita Adobe Commerce o Magenti Open Source, [!DNL Channel Manager] invia le informazioni sulla richiesta di reso all’archivio dei canali di vendita Commerce per replicare la richiesta di reso. Quindi, il rimborso può essere elaborato utilizzando [!DNL Commerce] [flusso di lavoro di rimborso](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow), metodo offline. Al termine del rimborso, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart in modo che lo stato di restituzione nell&#39;account del venditore del marketplace possa essere aggiornato per riflettere il rimborso.

## Latenza prevista per [!DNL Channel Manager] operazioni

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e un collegamento [!DNL Walmart Marketplace] richiedono un po’ di tempo per il completamento. Esamina il tempo di elaborazione previsto per [!DNL Channel Manager] operazioni che consentono di pianificare il funzionamento delle operazioni del canale di vendita.

**Latenza stimata per [!DNL Channel Manager] operazioni**

| **Operazione** | **Descrizione** | **Ritardo previsto** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a [!DNL Channel Manager] | Seleziona prodotti da [!DNL Commerce] catalogo dei prodotti e importarli in [!DNL Channel Manager]. | **Fino a cinque minuti**-Se si selezionano molti prodotti, ad esempio un intero catalogo prodotti, il processo di importazione richiede più tempo. |
| Corrispondenza prodotti su [!DNL Walmart Marketplace] | Seleziona elenchi prodotti in [!DNL Channel Manager] e inviarli a Walmart per la corrispondenza. | **Fino a 30 minuti**-Se si selezionano molti prodotti, il processo di abbinamento richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti inventario | Quando la quantità in magazzino cambia in Commerce, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando cambia il prezzo di un prodotto, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart. | **Fino a cinque minuti** |
| Ordina sincronizzazioni da Walmart a [!DNL Commerce] | Il cliente ordina un [!DNL Commerce] prodotto sul Walmart Marketplace. Walmart invia l’ordine a [!DNL Channel Manager]. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in [!DNL Commerce] Gestione ordini | [!DNL Channel Manager] crea il [!DNL Commerce] ordina da Walmart e aggiorna il dashboard dell&#39;ordine in modo da includere [!DNL Commerce] numero d&#39;ordine. | **Fino a cinque minuti** |
| Aggiornamento dello stato della spedizione in [!DNL Commerce] Gestione ordini | Quando un ordine viene spedito da Commerce, [!DNL Channel Manager] aggiorna lo stato di spedizione nel dashboard degli ordini e invia l&#39;aggiornamento a Walmart marketplace in modo che possa essere inviata una notifica al cliente. | **Fino a cinque minuti** |
| Aggiornamento dell’annullamento di un ordine in Commerce Order Management | Quando un ordine viene annullato da Commerce, [!DNL Channel Manager] aggiorna lo stato dell&#39;ordine nel dashboard degli ordini e invia l&#39;aggiornamento a Walmart marketplace in modo che possa essere inviata una notifica al cliente. Al termine dell’annullamento dell’ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. | **Fino a cinque minuti** |


