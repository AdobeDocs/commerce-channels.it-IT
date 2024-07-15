---
title: 'Introduzione a [!DNL Channel Manager]'
description: '''Scopri come installare e utilizzare [!DNL Channel Manager] per integrare Adobe Commerce e i negozi di Magento Open Source con Walmart Marketplace e creare un canale di vendita per gestire senza problemi le inserzioni, i prezzi, l''inventario e le vendite nel marketplace dal tuo amministratore Commerce.'''
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---


# Introduzione a [!DNL Channel Manager]

[!DNL Channel Manager] consente ai commercianti di aumentare le vendite, raggiungere nuovi clienti, semplificare le operazioni di vendita e risparmiare tempo integrando un catalogo di prodotti Adobe Commerce o Magento Open Source con [!DNL Walmart Marketplace].

Visualizzazione amministratore dell&#39;estensione ![[!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager] supporta i commercianti Adobe Commerce o di Magento Open Source che desiderano vendere il [!DNL Walmart Marketplace] estendendo l&#39;amministratore [!DNL Commerce]. Installando [!DNL Channel Manager], gli amministratori dei negozi e il personale operativo possono gestire [!DNL Walmart Marketplace] vendite, inventario e prezzi dei prodotti direttamente dall&#39;ambiente Commerce.

L&#39;amministratore esteso semplifica le operazioni perché i commercianti possono utilizzare gli stessi flussi di lavoro e gli stessi processi per gestire le vendite sia dai punti vendita [!DNL Commerce] che da Walmart Marketplace.

Dopo aver installato e configurato [!DNL Channel Manager], è possibile utilizzare le funzionalità seguenti per gestire gli ordini di vendita di Walmart Marketplace:

* **Gestione delle inserzioni**-Collega facilmente le inserzioni dei prodotti confrontando i prodotti del catalogo [!DNL Commerce] con le [!DNL Walmart Marketplace] inserzioni esistenti.

* **Inventory management**-Gli elementi nell&#39;account del venditore del marketplace del commerciante vengono sincronizzati e aggiornati automaticamente da [!DNL Commerce] per garantire livelli di inventario accurati.

* **Aggiornamenti dei prezzi**—Mantenere prezzi accurati per le inserzioni sul marketplace con la sincronizzazione automatica dei prezzi. Quando un prezzo cambia in Adobe Commerce, le modifiche si riflettono sul marketplace.

* **Gestione ordini**: quando vengono creati nuovi ordini nel marketplace, [!DNL Channel Manager] sincronizza gli ordini con Adobe Commerce e invia le conferme degli ordini al marketplace. Questa conferma garantisce che l&#39;inventario sia prenotato per ogni ordine. L&#39;ultimo passaggio consiste nel creare gli ordini corrispondenti nel sistema Order Management [!DNL Commerce] per l&#39;elaborazione.

* **Gestione spedizione**: quando gli ordini vengono contrassegnati come spediti in Adobe Commerce, l&#39;aggiornamento della spedizione viene inviato a [!DNL Walmart Marketplace]. Questa notifica garantisce che i venditori soddisfino i requisiti SLA e che i clienti ricevano le notifiche di aggiornamento della spedizione per gli ordini correnti.

* **Annullamenti** - Quando gli ordini vengono annullati in Adobe Commerce, [!DNL Channel Manager] invia informazioni aggiornate sull&#39;ordine al marketplace per replicare l&#39;azione per l&#39;ordine del marketplace corrispondente. Al termine dell&#39;annullamento dell&#39;ordine, gli aggiornamenti della quantità di magazzino [!DNL Commerce] per riflettere gli articoli restituiti e gli aggiornamenti del magazzino vengono sincronizzati automaticamente con [!DNL Walmart Marketplace].

* **Restituzioni e rimborsi** - Quando Walmart Marketplace richiede una restituzione per gli articoli ordinati tramite il canale di vendita Adobe Commerce o di Magento Open Source, [!DNL Channel Manager] invia le informazioni della richiesta di restituzione allo store del canale di vendita Commerce per replicare la richiesta di restituzione. Quindi, il rimborso può essere elaborato utilizzando il [!DNL Commerce] [flusso di lavoro di rimborso](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow), metodo offline. Al termine del rimborso, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart in modo che lo stato di restituzione nell&#39;account del venditore del marketplace possa essere aggiornato per riflettere il rimborso.

## Latenza prevista per [!DNL Channel Manager] operazioni

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e un archivio [!DNL Walmart Marketplace] collegato richiedono un certo tempo per essere completati. Esaminare il tempo di elaborazione previsto per le operazioni [!DNL Channel Manager] per pianificare il funzionamento delle operazioni del canale di vendita.

**Latenza stimata per [!DNL Channel Manager] operazioni**

| **Operazione** | **Descrizione** | **Ritardo previsto** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a [!DNL Channel Manager] | Selezionare i prodotti dal catalogo prodotti [!DNL Commerce] e importarli in [!DNL Channel Manager]. | **Fino a cinque minuti**-Se selezioni molti prodotti, ad esempio un intero catalogo prodotti, il processo di importazione richiede più tempo. |
| Corrispondenza prodotti su [!DNL Walmart Marketplace] | Selezionare gli elenchi di prodotti in [!DNL Channel Manager] e inviarli a Walmart per la corrispondenza. | **Fino a 30 minuti**-Se selezioni molti prodotti, il processo di abbinamento richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti inventario | Quando la quantità di magazzino cambia in Commerce, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando il prezzo di un prodotto cambia, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con Walmart. | **Fino a cinque minuti** |
| Ordina sincronizzazioni da Walmart a [!DNL Commerce] | Il cliente ordina un prodotto [!DNL Commerce] su Walmart Marketplace. Walmart invia l&#39;ordine a [!DNL Channel Manager]. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in Order Management [!DNL Commerce] | [!DNL Channel Manager] crea l&#39;ordine [!DNL Commerce] dall&#39;ordine Walmart e aggiorna il dashboard dell&#39;ordine in modo da includere il numero di ordine [!DNL Commerce]. | **Fino a cinque minuti** |
| Aggiornamento dello stato della spedizione in [!DNL Commerce] Order Management | Quando un ordine viene spedito da Commerce, [!DNL Channel Manager] aggiorna lo stato di spedizione nel dashboard degli ordini e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa ricevere una notifica. | **Fino a cinque minuti** |
| Aggiornamento dell’annullamento di un ordine in Commerce Order Management | Quando un ordine viene annullato da Commerce, [!DNL Channel Manager] aggiorna lo stato dell&#39;ordine nel dashboard degli ordini e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa ricevere una notifica. Al termine dell&#39;annullamento dell&#39;ordine, la quantità di magazzino [!DNL Commerce] viene aggiornata per riflettere gli articoli restituiti. Quindi, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. | **Fino a cinque minuti** |


