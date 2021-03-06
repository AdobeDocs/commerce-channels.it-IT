---
title: Registri e rapporti sull’archivio
description: Utilizza i registri e i rapporti dell’archivio per vedere cosa succede nell’Adobe Commerce o nel tuo archivio Magenti Open Source e negli elenchi di Amazon Marketplace.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Registri e archiviare i rapporti

L’estensione del canale di vendita Amazon include alcuni registri e rapporti sugli archivi importanti che ti consentono di visualizzare le modifiche che interessano gli elenchi e gli ordini di Amazon. Puoi utilizzare questi rapporti per vedere cosa succede nel tuo negozio e per comprendere vari stati di inserimento nell’elenco.

Non sono disponibili azioni per i registri o i rapporti dell’archivio, in quanto si tratta di funzioni di sola revisione.

È possibile accedere ai seguenti registri dal [dashboard store](./amazon-store-dashboard.md).

- La [Registro delle modifiche dell&#39;elenco](./listing-changes-log.md) mostra le modifiche che si sono verificate nel tuo account Amazon Seller come riflesso delle impostazioni del tuo canale di vendita Amazon.

- La [Registro errori di comunicazione](./communication-errors-log.md) mostra eventuali errori di comunicazione segnalati con Amazon.

È possibile accedere ai seguenti rapporti specifici per archivio dal [dashboard store](./amazon-store-dashboard.md).

- La [Analisi dei prezzi competitiva](./competitive-price-analysis.md) il rapporto mostra che il tuo Amazon _prezzo franco_ (prezzo di listino più prezzo di spedizione) in relazione [Buy Box](./buy-box-competitor-pricing.md) prezzo e [concorrente più basso](./lowest-competitor-pricing.md) prezzo.

- La [Miglioramenti all’elenco](./listing-improvements.md) il rapporto mostra tutti i miglioramenti suggeriti nell’elenco forniti da Amazon per lo store selezionato.

>[!TIP]
>
>È inoltre possibile controllare il file di registro per ulteriori informazioni quando è necessaria una risoluzione dei problemi. Vedi [impostazioni dell&#39;amministratore del canale di vendita](./sales-channel-settings.md). La registrazione della sincronizzazione dei canali di vendita Amazon viene scritta nel `{Commerce Root}/var/log/channel_amazon.log` e può essere visualizzato in [modalità sviluppatore](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}.
