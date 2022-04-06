---
title: Inventario e aggiornamenti dei prezzi
description: '''[!DNL Channel Manager] sincronizza l’inventario e gli aggiornamenti dei prezzi tra Commerce Store e [!DNL Walmart Marketplace] per gestire le operazioni dei canali di vendita dal tuo amministratore Commerce'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a1944052f02968c36495275cd5ddfb2ca43ce967
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Inventario e aggiornamenti dei prezzi

[!DNL Channel Manager] tiene traccia dell&#39;inventario e del prezzo dei prodotti nel negozio di canale. Quando l&#39;inventario o il prezzo cambiano, gli aggiornamenti si sincronizzano con [!DNL Channel Manager] e [!DNL Walmart Marketplace] per riflettere la quantità corrente di scorte e la determinazione dei prezzi negli elenchi dei prodotti.

## Aggiornamenti dell&#39;inventario

Quando i livelli di inventario cambiano, Channel Manager sincronizza gli aggiornamenti tra Commerce e Walmart Marketplace per garantire che Channel Manager e Walmart Marketplace abbiano la quantità di stock corretta.

La sincronizzazione degli aggiornamenti di inventario tra Channel Manager e marketplace può richiedere fino a 10 minuti.

* **Aggiornamenti della quantità di magazzino nel catalogo prodotti**-Quando la quantità di magazzino Commerce cambia a causa di [modifiche alla quantità di scorte manuali](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), rimborsi o annullamenti, Channel Manager sincronizza la modifica ai canali collegati e [!DNL Walmart Marketplace].

* **Ridurre la quantità di azioni per riflettere gli ordini di Walmart Marketplace**- Dopo che un ordine di Marketplace Walmart si sincronizza con Channel Manager, Channel Manager invia l&#39;aggiornamento al sistema di ordini Commerce. Il commercio adegua le quantità delle scorte in base all&#39;ordine. Quindi, la quantità aggiornata viene sincronizzata con Walmart Marketplace. Fino al completamento delle operazioni di sincronizzazione, potrebbero verificarsi differenze di quantità tra Channel Manager e Marketplace.

>[!IMPORTANT]
>
> Dopo che un ordine Walmart Marketplace viene sincronizzato con Channel Manager, le quantità di inventario e le informazioni sull&#39;ordine vengono aggiornate solo per i rimborsi e le cancellazioni iniziati da Commerce. Se un ordine viene rimborsato o annullato da Walmart Marketplace, elabora la modifica da Commerce per garantire l&#39;accuratezza delle quantità di inventario e delle informazioni sull&#39;ordine di Commerce.

## Aggiornamenti dei prezzi

Quando il prezzo del prodotto cambia in Commerce, Channel Manager sincronizza l’aggiornamento dal [!DNL Commerce] catalogo di prodotti in [!DNL Walmart Marketplace]. Il mercato può richiedere fino a cinque minuti per visualizzare le modifiche del prezzo.

### Gestione dei prezzi per un prodotto pubblicato

1. Da [!UICONTROL Admin], seleziona **[!UICONTROL Catalog > Products]**.
1. Nella griglia del prodotto, individua il prodotto da aggiornare e seleziona **[!UICONTROL Edit]**.
1. Rivedi e aggiorna il prezzo in base alle esigenze.
1. **[!UICONTROL Save]** il cambiamento.

Per informazioni dettagliate sulla gestione della configurazione del prezzo del prodotto in Commerce, consulta [Gestire i prezzi](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
