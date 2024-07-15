---
title: Aggiornamenti di magazzino e prezzo
description: '[!DNL Channel Manager] sincronizza gli aggiornamenti di inventario e prezzo tra lo  [!DNL Commerce] store e [!DNL Walmart Marketplace] in modo da poter gestire le operazioni del canale di vendita da [!DNL Commerce] Amministratore'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Aggiorna scorte e prezzi

[!DNL Channel Manager] tiene traccia dell&#39;inventario e dei prezzi dei prodotti nel catalogo prodotti [!DNL Commerce] e sincronizza gli aggiornamenti al canale di vendita connesso e a [!DNL Walmart Marketplace]. L&#39;operazione di sincronizzazione garantisce che gli elenchi dei prodotti riflettano la quantità di scorte e i prezzi correnti.


>[!IMPORTANT]
>
>Dopo l&#39;installazione e la configurazione di [!DNL Channel Manager], tutti gli aggiornamenti di inventario, prezzo e ordine vengono sincronizzati automaticamente. Se vendi già su Walmart Marketplace, assicurati di disabilitare qualsiasi altra integrazione che aggiorni i dati del prodotto e dell’ordine. Verificare quindi che i livelli delle scorte e i prezzi nella vetrina [!DNL Commerce] siano accurati e corrispondano ai dati in [!DNL Walmart Marketplace] prima di connettere [!DNL Channel Manager] all&#39;archivio di Live Marketplace.


## Aggiornamenti inventario

Quando i livelli di inventario dei prodotti cambiano in [!DNL Commerce], [!DNL Channel Manager] sincronizza gli aggiornamenti in [!DNL Walmart Marketplace]. La sincronizzazione degli aggiornamenti dell&#39;inventario tra il canale di vendita e [!DNL Walmart marketplace] può richiedere fino a 10 minuti.

* **Aggiornamenti alla quantità di scorte nel catalogo prodotti** - Quando [!DNL Commerce] la quantità di scorte cambia a causa di [modifiche manuali della quantità di scorte](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), rimborsi o annullamenti, [!DNL Channel Manager] sincronizza la modifica nei canali collegati e [!DNL Walmart Marketplace].

* **Riduci la quantità di scorte per riflettere [!DNL Walmart Marketplace] ordini**. Dopo la sincronizzazione di un ordine [!DNL Walmart Marketplace] in [!DNL Channel Manager], [!DNL Channel Manager] invia l&#39;aggiornamento al sistema di ordini [!DNL Commerce]. [!DNL Commerce] regola le quantità di scorte in base all&#39;ordine. La quantità aggiornata viene quindi sincronizzata in [!DNL Walmart Marketplace]. Fino al completamento delle operazioni di sincronizzazione, è possibile che vengano visualizzate quantità diverse nelle inserzioni del canale di vendita e [!DNL Walmart].

>[!IMPORTANT]
>
>Dopo la sincronizzazione di un ordine [!DNL Walmart Marketplace] in [!DNL Channel Manager], le quantità di magazzino e le informazioni sull&#39;ordine vengono aggiornate solo per i rimborsi e gli annullamenti avviati a partire da [!DNL Commerce]. Se un ordine viene rimborsato o annullato da [!DNL Walmart marketplace], elaborare la modifica da [!DNL Commerce] per garantire la precisione di [!DNL Commerce] quantità di magazzino e informazioni sull&#39;ordine.

## Aggiornamenti dei prezzi

Quando il prezzo del prodotto cambia in [!DNL Commerce], [!DNL Channel Manager] sincronizza l&#39;aggiornamento in [!DNL Walmart Marketplace]. La visualizzazione della modifica del prezzo nell&#39;inserzione [!DNL Walmart Marketplace] può richiedere fino a cinque minuti.

### Gestire i prezzi di un prodotto connesso

1. Da [!UICONTROL Admin], selezionare **[!UICONTROL Catalog > Products]**.
1. Nella griglia del prodotto, individuare il prodotto da aggiornare e selezionare **[!UICONTROL Edit]**.
1. Rivedi e aggiorna il prezzo in base alle esigenze.
1. **[!UICONTROL Save]** la modifica.

Per informazioni sulla gestione della configurazione del prezzo del prodotto in [!DNL Commerce], vedere [Gestione prezzi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
