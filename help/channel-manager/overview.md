---
title: '"Informazioni su [!DNL Channel Manager]"'
description: '"Scopri come installare e utilizzare [!DNL Channel Manager] per integrare Adobe Commerce e i negozi di Magento Open Source con i mercati di terze parti e creare un canale di vendita per gestire gli elenchi di Marketplace, i prezzi, l’inventario e le vendite direttamente dal tuo amministratore Commerce."'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 690eeb5d03b23cac11f3c14b04601c514c76e0bd
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---


# Informazioni [!DNL Channel Manager]

[!DNL Channel Manager] aiuta i commercianti ad aumentare le vendite, raggiungere nuovi clienti, semplificare le operazioni di vendita e risparmiare tempo integrando un catalogo di prodotti Adobe Commerce o Magento Open Source con [!DNL Walmart Marketplace].

![[!DNL Channel Manager] vista amministratore dell&#39;estensione](assets/channel-manager-home.png)

[!DNL Channel Manager] supporta Adobe Commerce o i commercianti di Magenti Open Source che desiderano vendere su [!DNL Walmart Marketplace] estendendo [!DNL Commerce] Amministrazione con funzionalità di gestione [!DNL Walmart Marketplace] vendita, inventario e prezzi dei prodotti direttamente dall&#39;ambiente Commerce.

L’amministratore esteso ottimizza le operazioni perché i commercianti possono utilizzare gli stessi flussi di lavoro e gli stessi processi per gestire le vendite sia da Commerce storefronts che da Walmart Marketplace.

Dopo l’installazione e la configurazione [!DNL Channel Manager], puoi utilizzare le seguenti funzionalità per gestire gli ordini di vendita di Walmart Marketplace:

* **Gestione dell&#39;elenco**- Facile connessione degli elenchi dei prodotti mediante l&#39;abbinamento dei prodotti [!DNL Commerce] catalogo a esistente [!DNL Walmart Marketplace] elenchi.

* **Inventory management**-Gli articoli nel conto del venditore del marketplace del commerciante vengono automaticamente sincronizzati e aggiornati da Commerce per garantire livelli di inventario precisi.

* **Aggiornamenti dei prezzi**-Mantenere prezzi precisi per le inserzioni di marketplace con sincronizzazione automatica dei prezzi. Quando un prezzo cambia in Adobe Commerce, le modifiche si riflettono sul mercato.

* **Gestione degli ordini**- Quando vengono creati nuovi ordini in un mercato, [!DNL Channel Manager] sincronizza gli ordini con Adobe Commerce, invia conferme d’ordine al marketplace per garantire che l’inventario sia riservato per ogni ordine e crea un ordine corrispondente nel sistema Commerce Order Management per l’elaborazione.

* **Gestione della spedizione**- Quando gli ordini sono contrassegnati come spediti in Adobe Commerce, l&#39;aggiornamento della spedizione viene inviato al [!DNL Walmart Marketplace]. Questa notifica assicura che i venditori soddisfino i loro requisiti SLA e che i clienti ricevano notifiche di aggiornamento della spedizione per i loro ordini correnti.

* **Cancellazioni**-Quando gli ordini vengono annullati in Adobe Commerce, [!DNL Channel Manager] invia informazioni aggiornate sull’ordine al marketplace per replicare l’azione per l’ordine di marketplace corrispondente.  Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] gli aggiornamenti della quantità delle scorte per riflettere gli articoli restituiti e gli aggiornamenti delle scorte sono sincronizzati automaticamente in [!DNL Walmart Marketplace].

## Latenza prevista per [!DNL Channel Manager] operazioni

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e collegati [!DNL Walmart Marketplace] archiviare richiede un po&#39; di tempo per completare. Esamina il tempo di elaborazione previsto per [!DNL Channel Manager] operazioni che consentono di pianificare il funzionamento dei canali di vendita.

**Latenza stimata per [!DNL Channel Manager] operazioni**

| **Funzionamento** | **Descrizione** | **Ritardo previsto** |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a [!DNL Channel Manager] | Seleziona i prodotti dal catalogo di prodotti Commerce e importali in [!DNL Channel Manager]. | **Fino a cinque minuti**- Se selezioni molti prodotti, ad esempio un intero catalogo di prodotti, il processo di importazione richiede più tempo. |
| Confronta prodotti su [!DNL Walmart Marketplace] | Seleziona gli elenchi dei prodotti in [!DNL Channel Manager] e inviare a Walmart per la corrispondenza. | **Fino a 30 minuti**- Se selezioni molti prodotti, il processo di corrispondenza richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti dell&#39;inventario | Quando la quantità di inventario cambia in Commerce, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando cambia il prezzo di un prodotto, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart. | **Fino a cinque minuti** |
| Ordinare sincronizzazioni da Walmart a Commerce | Il cliente ordina un prodotto Commerce su Walmart Marketplace. Walmart invia l&#39;ordine a [!DNL Channel Manager]. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in Commerce Order Management | [!DNL Channel Manager] crea l’ordine Commerce dall’ordine Walmart e aggiorna il dashboard dell’ordine in modo da includere il numero dell’ordine Commerce. | **Fino a cinque minuti** |
| Aggiornamento dello stato della spedizione in Gestione ordini di Commerce | Quando un ordine viene spedito da Commerce, [!DNL Channel Manager] aggiorna lo stato di spedizione nel dashboard dell&#39;ordine e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa essere informato. | **Fino a cinque minuti** |
| Aggiornamento dell&#39;annullamento dell&#39;ordine in Gestione ordini di Commerce | Quando un ordine viene annullato da Commerce, [!DNL Channel Manager] aggiorna lo stato dell&#39;ordine nel dashboard dell&#39;ordine e invia l&#39;aggiornamento a Walmart marketplace in modo che il cliente possa ricevere notifiche. Al termine dell&#39;annullamento dell&#39;ordine, il [!DNL Commerce] la quantità di magazzino viene aggiornata per riflettere gli articoli restituiti. Allora, [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. | **Fino a cinque minuti** |


