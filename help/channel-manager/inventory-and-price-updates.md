---
title: Inventario e aggiornamenti dei prezzi
description: '"[!DNL Channel Manager] sincronizza l’inventario e gli aggiornamenti dei prezzi tra Commerce Store e [!DNL Walmart Marketplace] per gestire le operazioni dei canali di vendita dal tuo amministratore Commerce"'
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Inventario e aggiornamenti dei prezzi

Channel Manager tiene traccia dell&#39;inventario e dei prezzi dei prodotti pubblicati e sincronizza le modifiche apportate a Channel Manager e a Walmart Marketplace per riflettere la quantità di azioni e i prezzi correnti negli elenchi dei prodotti.**

## Aggiornamenti dell&#39;inventario

Quando i livelli di inventario cambiano, Channel Manager sincronizza gli aggiornamenti tra il catalogo di prodotti Commerce e il Marketplace Walmart in modo che sia Channel Manager che Walmart Marketplace visualizzino la quantità di azioni corrente.

La visualizzazione delle modifiche all’inventario in Channel Manager e Walmart Marketplace può richiedere fino a 5 minuti.

* **Aggiornamenti della quantità di magazzino nel catalogo prodotti**- Se la quantità di magazzino Commerce cambia per un prodotto venduto su Walmart a causa di un [modifica manuale della quantità delle scorte](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html) o un rimborso o un annullamento dell&#39;ordine, Channel Manager sincronizza il cambiamento con il canale di vendita collegato e il [!DNL Walmart Marketplace].

* **Ridurre la quantità di azioni per riflettere gli ordini di Walmart Marketplace**- Dopo che un ordine di Marketplace Walmart si sincronizza con Channel Manager, Channel Manager invia l&#39;aggiornamento al sistema di ordini Commerce. Il commercio adegua le quantità delle scorte in base all&#39;ordine. Quindi, la quantità aggiornata viene sincronizzata con Walmart Marketplace. potrebbero essere presenti alcune differenze nella quantità delle scorte mostrate in Channel Manager e Marketplace fino al completamento delle operazioni di sincronizzazione.

>[!IMPORTANT]
>
> Dopo che un ordine Walmart Marketplace si sincronizza con Channel Manager, le quantità di inventario e altre informazioni di elaborazione degli ordini vengono aggiornate solo per i rimborsi e le cancellazioni iniziati da Commerce. Se un ordine viene rimborsato o annullato da Walmart Marketplace, elabora la modifica da Commerce per assicurarsi che le quantità di inventario e le informazioni sull’ordine di Commerce siano accurate.

## Aggiornamenti dei prezzi

Quando il prezzo del prodotto cambia in Commerce, Channel Manager sincronizza l’aggiornamento dal catalogo prodotti Commerce a Walmart Marketplace. La visualizzazione delle modifiche di inventario può richiedere fino a 5 minuti.

### Gestione dei prezzi per un prodotto pubblicato

1. Da [!UICONTROL Admin], seleziona **[!UICONTROL Catalog > Products]**.
1. Nella griglia del prodotto, individua il prodotto da aggiornare e seleziona **[!UICONTROL Edit]**.
1. Rivedi e aggiorna il prezzo in base alle esigenze.
1. **[!UICONTROL Save]** il cambiamento.

Channel Manager sincronizza gli aggiornamenti dei prezzi al negozio di canale e [!DNL Walmart Marketplace]. Questa operazione può richiedere fino a 5 minuti.

Per informazioni dettagliate sulla gestione della configurazione del prezzo del prodotto in Commerce, consulta [Gestire i prezzi](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
