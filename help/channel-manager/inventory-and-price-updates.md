---
title: Aggiornamenti di magazzino e prezzo
description: '[!DNL Channel Manager] sincronizza gli aggiornamenti di inventario e prezzo tra [!DNL Commerce] memorizzare e [!DNL Walmart Marketplace] in modo da poter gestire le operazioni del canale di vendita da [!DNL Commerce] Amministratore'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Aggiorna scorte e prezzi

[!DNL Channel Manager] tiene traccia dell&#39;inventario e dei prezzi dei prodotti nel [!DNL Commerce] catalogo dei prodotti e sincronizza gli aggiornamenti al canale di vendita connesso e [!DNL Walmart Marketplace]. L&#39;operazione di sincronizzazione garantisce che gli elenchi dei prodotti riflettano la quantità di scorte e i prezzi correnti.


>[!IMPORTANT]
>
>Dopo [!DNL Channel Manager] è installato e configurato, tutti gli aggiornamenti di inventario, prezzo e ordine vengono sincronizzati automaticamente. Se vendi già su Walmart Marketplace, assicurati di disabilitare qualsiasi altra integrazione che aggiorni i dati del prodotto e dell’ordine. Quindi, verifica che i livelli delle scorte e i prezzi nell&#39; [!DNL Commerce] sono precise e corrispondono ai dati in [!DNL Walmart Marketplace] prima della connessione [!DNL Channel Manager] al negozio live marketplace.


## Aggiornamenti inventario

Quando i livelli di inventario dei prodotti cambiano in [!DNL Commerce], [!DNL Channel Manager] sincronizza gli aggiornamenti a [!DNL Walmart Marketplace]. La sincronizzazione degli aggiornamenti dell&#39;inventario tra il canale di vendita e il [!DNL Walmart marketplace].

* **Aggiornamenti alla quantità di scorte nel catalogo prodotti**- Quando [!DNL Commerce] variazioni quantità di magazzino a causa di [modifiche quantità scorte manuali](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), rimborsi o annullamenti, [!DNL Channel Manager] sincronizza la modifica ai canali collegati e [!DNL Walmart Marketplace].

* **Riduci quantità di magazzino per riflettere [!DNL Walmart Marketplace] ordini**- Dopo un [!DNL Walmart Marketplace] ordina sincronizzazioni a [!DNL Channel Manager], [!DNL Channel Manager] invia l&#39;aggiornamento al [!DNL Commerce] sistema di ordinazione. [!DNL Commerce] adegua le quantità delle scorte in base all&#39;ordine. Quindi, la quantità aggiornata viene sincronizzata in [!DNL Walmart Marketplace]. Fino al completamento delle operazioni di sincronizzazione, nelle inserzioni del canale di vendita potrebbero essere visibili quantità diverse e [!DNL Walmart].

>[!IMPORTANT]
>
>Dopo un [!DNL Walmart Marketplace] ordina sincronizzazioni a [!DNL Channel Manager], le quantità di magazzino e le informazioni sugli ordini vengono aggiornate solo per i rimborsi e gli annullamenti avviati dal [!DNL Commerce]. Se un ordine viene rimborsato o annullato dal [!DNL Walmart marketplace], elabora la modifica da [!DNL Commerce] per garantire l&#39;accuratezza [!DNL Commerce] le quantità di magazzino e le informazioni sugli ordini.

## Aggiornamenti dei prezzi

Quando il prezzo del prodotto cambia in [!DNL Commerce], [!DNL Channel Manager] sincronizza l&#39;aggiornamento con [!DNL Walmart Marketplace]. Possono essere necessari fino a cinque minuti perché la modifica del prezzo venga visualizzata nel [!DNL Walmart Marketplace] elenco.

### Gestire i prezzi di un prodotto connesso

1. Dalla sezione [!UICONTROL Admin], seleziona **[!UICONTROL Catalog > Products]**.
1. Nella griglia del prodotto, individua il prodotto da aggiornare e seleziona **[!UICONTROL Edit]**.
1. Rivedi e aggiorna il prezzo in base alle esigenze.
1. **[!UICONTROL Save]** il cambiamento.

Per assistenza nella gestione della configurazione del prezzo del prodotto in [!DNL Commerce], vedi [Gestisci prezzi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
