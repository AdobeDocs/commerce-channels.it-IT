---
title: '[!DNL Channel Manager] Note sulla versione'
description: Informazioni aggiornate sulla versione di  [!DNL Channel Manager]  da Adobe Commerce.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Note sulla versione [!DNL Channel Manager]

Queste note sulla versione descrivono la versione iniziale di [!DNL Channel Manager] e includono:

![Nuove](../assets/new.svg) nuove funzionalità
![Problema risolto](../assets/fix.svg) correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti

Per informazioni sulle pianificazioni e sul supporto, consulta le [prossime versioni](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html).

Consulta [Disponibilità del prodotto](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) per sapere quali versioni di Adobe Commerce supportano questa estensione.

## v2.1.0

*3 ottobre 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![New](../assets/new.svg) Channel Manager è ora compatibile con [Adobe Commerce versione 2.4.7 beta](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html).

## v2.0.0

*20 marzo 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![New](../assets/new.svg)<!--CHAN-5893--> Channel Manager è ora compatibile con Adobe Commerce versione 2.4.6.

## v1.1.0

*23 novembre 2022*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg)<!--CHAN-5204--> **Restituzioni e rimborsi** - È ora possibile elaborare la procedura di restituzione e rimborso di Walmart Marketplace per gli ordini spediti tramite un archivio Adobe Commerce e Magento Open Source Channel Manager. Le informazioni e gli aggiornamenti su restituzioni e rimborsi vengono sincronizzati tra Walmart e Adobe Commerce in modo che i dati correnti siano disponibili sia nella vetrina [!DNL Commerce] che in [!DNL Walmart Marketplace]. Vedi [Ordini di reso e rimborso](return-refund-orders.md).

![Corretto](../assets/fix.svg)<!--CHAN-5661--> è stato corretto l&#39;errore `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` che si verificava durante la risincronizzazione dei dati degli ordini di Channel Manager tramite il comando `bin/magento saas:resync --feed orders`. L&#39;errore è stato risolto aggiornando le dipendenze del pacchetto Channel Manager per il modulo Sales Data Exporter, rinominato da `magento/module-sales-data-exporter` a `magento/module-sales-orders-data-exporter`.

## v1.0.0

*14 gennaio 2022*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) rilascio iniziale di Channel Manager per la disponibilità generale

