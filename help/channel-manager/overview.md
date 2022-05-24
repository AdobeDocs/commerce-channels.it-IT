---
title: Informazioni [!DNL Channel Manager]
description: Scopri come installare e utilizzare [!DNL Channel Manager] per integrare Adobe Commerce e i negozi di Magento Open Source con i mercati di terze parti e creare un canale di vendita per gestire gli elenchi di Marketplace, i prezzi, l’inventario e le vendite direttamente dal tuo amministratore Commerce.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 9ccd205ccd4f4b3f4e6b9fed2c4d16893f4b0da8
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# Informazioni [!DNL Channel Manager]

[!DNL Channel Manager] consente di aumentare le vendite e raggiungere nuovi clienti integrando il catalogo dei prodotti Adobe Commerce o Magenti Open Source con [!DNL Walmart US Marketplace].

![[!DNL Channel Manager] vista amministratore dell&#39;estensione](assets/channel-manager-home.png)

Channel Manager supporta Adobe Commerce o i venditori di Magenti Open Source che desiderano vendere su Walmart Marketplace.

Dopo l’installazione e la configurazione [!DNL Channel Manager], [!DNL Commerce] L’amministratore è esteso per poter gestire [!DNL Walmart Marketplace] operazioni di vendita direttamente dal tuo ambiente Commerce.

* **Gestione dell&#39;elenco**- Pubblicare facilmente gli elenchi dei prodotti in base ai prodotti corrispondenti dal catalogo Commerce agli elenchi esistenti di Walmart Marketplace.

* **Inventory management**-Gli articoli nel conto del venditore del marketplace del commerciante vengono automaticamente sincronizzati e aggiornati da Commerce per garantire livelli di inventario precisi.

* **Aggiornamenti dei prezzi**-Mantenere prezzi precisi per le inserzioni di marketplace con sincronizzazione automatica dei prezzi. Quando un prezzo cambia in Adobe Commerce, le modifiche si riflettono sul mercato entro 10 minuti.

* **Gestione degli ordini**- Quando vengono creati nuovi ordini in un marketplace, Channel Manager sincronizza gli ordini con Adobe Commerce e invia conferme di ordine al marketplace per garantire che l’inventario sia riservato per ogni ordine.

* **Gestione della spedizione**- Quando gli ordini sono contrassegnati come spediti in Adobe Commerce, l&#39;aggiornamento della spedizione viene inviato al [!DNL Walmart Marketplace]. Questa notifica assicura che i venditori soddisfino i loro requisiti SLA e che i clienti ricevano notifiche di aggiornamento della spedizione per i loro ordini correnti.

* **Cancellazioni**- Quando gli ordini vengono annullati in Adobe Commerce, Channel Manager invia informazioni aggiornate sull’ordine al marketplace per replicare l’azione per l’ordine di marketplace corrispondente.

## Latenza prevista per le operazioni di Channel Manager

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e collegati [!DNL Walmart Marketplace] archiviare richiede un po&#39; di tempo per completare. Esamina il tempo di elaborazione previsto per [!DNL Channel Manager] operazioni che consentono di pianificare il funzionamento dei canali di vendita.

**Latenza stimata per le operazioni di Channel Manager**

| **Funzionamento** | **Descrizione** | **Ritardo previsto** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a Channel Manager | Seleziona i prodotti dal catalogo di prodotti Commerce e importali in Channel Manager. | **Fino a cinque minuti**- Se selezioni molti prodotti, ad esempio un intero catalogo di prodotti, il processo di importazione richiede più tempo. |
| Confronta prodotti su Walmart Marketplace | Seleziona gli elenchi dei prodotti in Channel Manager e inviali a Walmart per la corrispondenza. | **Fino a 30 minuti**- Se selezioni molti prodotti, il processo di corrispondenza richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti dell&#39;inventario | Quando la quantità di inventario cambia in Commerce, [!DNL Channel Manager] sincronizza l&#39;aggiornamento a Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando il prezzo di un prodotto cambia, Channel Manager sincronizza l&#39;aggiornamento a Walmart. | **Fino a cinque minuti** |
| Ordinare sincronizzazioni da Walmart a Commerce | Il cliente ordina un prodotto Commerce su Walmart Marketplace. Walmart invia l&#39;ordine a Channel Manager. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in Commerce Order Management | Channel Manager crea l’ordine Commerce dall’ordine Walmart e aggiorna il dashboard dell’ordine in modo da includere il numero dell’ordine Commerce. | **Fino a cinque minuti** |

