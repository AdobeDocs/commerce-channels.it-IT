---
title: Registra e archivia i rapporti per le inserzioni Amazon
description: Utilizza i registri e i rapporti dell’archivio per vedere cosa sta succedendo nel tuo archivio Adobe Commerce o Magento Open Source e nelle tue inserzioni Amazon Marketplace.
feature: Sales Channels, Logs
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Registra e archivia i rapporti per le inserzioni Amazon

L’estensione del canale di vendita Amazon include alcuni registri e rapporti sui negozi importanti che ti consentono di visualizzare le modifiche che interessano le inserzioni e gli ordini Amazon. Puoi utilizzare questi rapporti per vedere cosa sta succedendo nel tuo store e per comprendere i vari stati delle inserzioni.

Non sono disponibili azioni per i registri o i rapporti store, in quanto sono funzioni di sola revisione.

È possibile accedere ai seguenti registri dal [dashboard dello store](./amazon-store-dashboard.md).

- Il [registro delle modifiche alle inserzioni](./listing-changes-log.md) mostra le modifiche che si sono verificate nel tuo account Amazon Seller come riflesso delle impostazioni del tuo canale di vendita Amazon.

- Il [registro errori di comunicazione](./communication-errors-log.md) mostra eventuali errori di comunicazione segnalati con Amazon.

È possibile accedere ai seguenti report specifici dell&#39;archivio dal [dashboard dell&#39;archivio](./amazon-store-dashboard.md).

- Il rapporto dell&#39;[Analisi prezzi competitivi](./competitive-price-analysis.md) indica che il tuo Amazon _ha acquistato il prezzo_ (prezzo di listino più prezzo di spedizione) in relazione al prezzo [Buy Box](./buy-box-competitor-pricing.md) e al prezzo [del concorrente più basso](./lowest-competitor-pricing.md).

- Il report [Miglioramenti elenco](./listing-improvements.md) mostra tutti i miglioramenti suggeriti per l&#39;elenco forniti da Amazon per l&#39;archivio selezionato.

>[!TIP]
>
>È inoltre possibile controllare il file di registro per ulteriori informazioni quando è necessaria la risoluzione dei problemi. Consulta [Impostazioni amministratore canale vendite](./sales-channel-settings.md). La registrazione sincronizzazione canale di vendita Amazon è scritta nel file `{Commerce Root}/var/log/channel_amazon.log` e può essere visualizzata in [modalità sviluppatore](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes).
