---
title: '''[!DNL Channel Manager] Note sulla versione"'
description: Informazioni aggiornate sulla versione di [!DNL Channel Manager] da Adobe Commerce.
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 9cc1b79089771ef9a58d22379197b210d31e1670
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# [!DNL Channel Manager] Note sulla versione

Queste note sulla versione descrivono la versione iniziale di [!DNL Channel Manager] e comprendono:

![Nuovo](../assets/new.svg) Nuove funzioni
![Problema risolto](../assets/fix.svg) Correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti


## v1.1.0

![Nuovo](../assets/new.svg)<!--CHAN-5204--> **Restituzioni**- È ora possibile elaborare il processo di restituzione e rimborso di Walmart Marketplace per gli ordini spediti attraverso un negozio Adobe Commerce e Magenti Open Source Channel Manager. Informazioni e aggiornamenti su restituzioni e rimborsi sono sincronizzati tra Walmart e Adobe Commerce in modo che i dati correnti siano disponibili in entrambi i [!DNL Commerce] vetrina e [!DNL Walmart Marketplace]. Vedi [Ordini di restituzione](return-refund-orders.md).

![Fisso](../assets/fix.svg)<!--CHAN-5661--> È stato corretto il `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` errore che si è verificato durante la risincronizzazione dei dati degli ordini di Channel Manager utilizzando `bin/magento saas:resync --feed orders` comando. L&#39;errore è stato risolto aggiornando le dipendenze del pacchetto Channel Manager per il modulo Esportatore dati di vendita, che è stato rinominato da `magento/module-sales-data-exporter` a `magento/module-sales-orders-data-exporter`.

## v1.0.0

Versione iniziale, compatibile con le seguenti versioni Commerce:

* Open Source (CE): 2.4.x
* Adobe Commerce (EE): 2.4.x
* Adobe Commerce for Cloud (ECE): 2.4.x
* Stabilità: Stabile
