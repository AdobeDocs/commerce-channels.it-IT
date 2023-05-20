---
title: '''[!DNL Channel Manager] Note sulla versione'
description: Informazioni aggiornate sulla versione di [!DNL Channel Manager] da Adobe Commerce.
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: d3acde7aa297ba33dffa7854aa7578985ad12c9b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# [!DNL Channel Manager] Note sulla versione

Queste note sulla versione descrivono la versione iniziale di [!DNL Channel Manager] e includono:

![Nuovo](../assets/new.svg) Nuove funzioni
![Problema risolto](../assets/fix.svg) Correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti


## v2.0.0

*20 marzo 2023*

[!BADGE Compatibilità]{type=Informative tooltip="Compatibilità"}

![Nuovo](../assets/new.svg)<!--CHAN-5893--> Channel Manager è ora compatibile con Adobe Commerce versione 2.4.6.

## v1.1.0

*23 novembre 2022*

[!BADGE Compatibilità]{type=Informative tooltip="Compatibilità"}

![Nuovo](../assets/new.svg)<!--CHAN-5204--> **Restituzioni e restituzioni**- È ora possibile elaborare la procedura di restituzione e rimborso di Walmart Marketplace per gli ordini spediti attraverso un negozio Adobe Commerce e Magenti Open Source Channel Manager. Le informazioni e gli aggiornamenti su restituzioni e rimborsi vengono sincronizzati tra Walmart e Adobe Commerce in modo che i dati correnti siano disponibili sia nel [!DNL Commerce] vetrina e [!DNL Walmart Marketplace]. Consulta [Ordini di reso e di rimborso](return-refund-orders.md).

![Fisso](../assets/fix.svg)<!--CHAN-5661--> È stato corretto il `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` errore che si è verificato durante la risincronizzazione dei dati degli ordini di Channel Manager utilizzando `bin/magento saas:resync --feed orders` comando. L’errore è stato risolto aggiornando le dipendenze del pacchetto Channel Manager per il modulo Sales Data Exporter, rinominato da `magento/module-sales-data-exporter` a `magento/module-sales-orders-data-exporter`.

## v1.0.0

*14 gennaio 2022*

[!BADGE Compatibilità]{type=Informative tooltip="Compatibilità"}

![Nuovo](../assets/new.svg) Versione iniziale di Channel Manager per la disponibilità generale

