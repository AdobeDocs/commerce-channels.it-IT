---
title: Registra e archivia i rapporti per le inserzioni Amazon
description: Utilizza i registri e i rapporti dell’archivio per vedere cosa sta succedendo nel tuo archivio Adobe Commerce o Magento Open Source e nelle tue inserzioni Amazon Marketplace.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Registra e archivia i rapporti per le inserzioni Amazon

L’estensione del canale di vendita Amazon include alcuni registri e rapporti sui negozi importanti che ti consentono di visualizzare le modifiche che interessano le inserzioni e gli ordini Amazon. Puoi utilizzare questi rapporti per vedere cosa sta succedendo nel tuo store e per comprendere i vari stati delle inserzioni.

Non sono disponibili azioni per i registri o i rapporti store, in quanto sono funzioni di sola revisione.

I seguenti registri sono accessibili da [dashboard store](./amazon-store-dashboard.md).

- Il [Registro delle modifiche alle inserzioni](./listing-changes-log.md) mostra le modifiche apportate al tuo account Amazon Seller come riflesso delle impostazioni del tuo canale di vendita Amazon.

- Il [Registro errori di comunicazione](./communication-errors-log.md) mostra eventuali errori di comunicazione segnalati con Amazon.

È possibile accedere ai seguenti rapporti specifici dello store da [dashboard store](./amazon-store-dashboard.md).

- Il [Analisi dei prezzi competitivi](./competitive-price-analysis.md) mostra che il tuo Amazon _prezzo allo sbarco_ (prezzo di listino più prezzo di spedizione) in relazione al [Buy Box](./buy-box-competitor-pricing.md) prezzo e [concorrente più basso](./lowest-competitor-pricing.md) prezzo.

- Il [Miglioramenti alle inserzioni](./listing-improvements.md) Il rapporto mostra tutti i miglioramenti suggeriti per l’inserzione forniti da Amazon per lo store selezionato.

>[!TIP]
>
>È inoltre possibile controllare il file di registro per ulteriori informazioni quando è necessaria la risoluzione dei problemi. Consulta [Impostazioni amministrazione canale di vendita](./sales-channel-settings.md). La registrazione di sincronizzazione del canale di vendita Amazon viene scritta in `{Commerce Root}/var/log/channel_amazon.log` e possono essere visualizzati in [modalità sviluppatore](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes).
