---
title: Inventario e aggiornamenti dei prezzi
description: '''[!DNL Channel Manager] sincronizza l’inventario e gli aggiornamenti dei prezzi tra Commerce Store e [!DNL Walmart Marketplace] per gestire le operazioni dei canali di vendita dal tuo amministratore Commerce'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 71ad5e3bc9ff6b909943a161472e4db7d375683f
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Aggiornare inventario e prezzi

[!DNL Channel Manager] tiene traccia dell’inventario e dei prezzi dei prodotti [!DNL Commerce] catalogo del prodotto e sincronizza gli aggiornamenti al canale di vendita collegato e [!DNL Walmart Marketplace]. La sincronizzazione assicura che gli elenchi dei prodotti riflettano la quantità e il prezzo correnti delle scorte.

## Aggiornamenti dell&#39;inventario

Quando i livelli di inventario dei prodotti cambiano [!DNL Commerce], [!DNL Channel Manager] sincronizza gli aggiornamenti al canale di vendita e al [!DNL Walmart Marketplace]. Gli aggiornamenti di inventario possono richiedere fino a 10 minuti per la sincronizzazione tra il canale di vendita e il [!DNL Walmart marketplace].

* **Aggiornamenti della quantità di magazzino nel catalogo prodotti**—Quando [!DNL Commerce] variazioni della quantità delle scorte a causa di [modifiche alla quantità di scorte manuali](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), rimborsi o annullamenti, [!DNL Channel Manager] sincronizza la modifica ai canali collegati e [!DNL Walmart Marketplace].

* **Ridurre la quantità di magazzino per riflettere [!DNL Walmart Marketplace] ordini**—Dopo un [!DNL Walmart Marketplace] ordina sincronizzazioni in [!DNL Channel Manager], [!DNL Channel Manager] invia l&#39;aggiornamento a [!DNL Commerce] sistema d&#39;ordine. [!DNL Commerce] adegua le quantità delle scorte in base all&#39;ordine. Quindi, la quantità aggiornata viene sincronizzata in [!DNL Walmart Marketplace]. Fino al completamento delle operazioni di sincronizzazione, è possibile che negli elenchi dei canali di vendita siano presenti quantità diverse e [!DNL Walmart].

>[!IMPORTANT]
>
>Dopo un [!DNL Walmart Marketplace] ordina sincronizzazioni in [!DNL Channel Manager], le quantità di inventario e le informazioni sugli ordini vengono aggiornate solo per i rimborsi e le cancellazioni iniziati a partire da [!DNL Commerce]. Se un ordine è rimborsato o annullato dal [!DNL Walmart marketplace], elabora la modifica da [!DNL Commerce] per garantire l&#39;accuratezza [!DNL Commerce] quantità di magazzino e informazioni sull&#39;ordine.

## Aggiornamenti dei prezzi

Quando il prezzo del prodotto cambia in [!DNL Commerce], [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. La visualizzazione del cambiamento di prezzo nel [!DNL Walmart Marketplace] elenco.

### Gestione dei prezzi per un prodotto pubblicato

1. Da [!UICONTROL Admin], seleziona **[!UICONTROL Catalog > Products]**.
1. Nella griglia del prodotto, individua il prodotto da aggiornare e seleziona **[!UICONTROL Edit]**.
1. Rivedi e aggiorna il prezzo in base alle esigenze.
1. **[!UICONTROL Save]** il cambiamento.

Per informazioni sulla gestione della configurazione del prezzo del prodotto in [!DNL Commerce], vedi [Gestire i prezzi](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
