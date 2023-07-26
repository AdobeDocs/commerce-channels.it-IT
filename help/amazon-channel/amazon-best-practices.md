---
title: Best practice e limitazioni per [!DNL Amazon sales channel]
description: Rivedi le best practice e le limitazioni nell’utilizzo del canale di vendita Amazon per Adobe Commerce e Magenti Open Source.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Best practice e limitazioni per [!DNL Amazon sales channel]

Le best practice includono:

- Il canale di vendita Amazon può influenzare le tue inserzioni Amazon aumentando o diminuendo i prezzi, sincronizzando le informazioni sui prodotti (comprese le azioni disponibili) e aggiungendo, aggiornando ed eliminando le inserzioni. Controlla le tue inserzioni in base allo stato durante la configurazione e regola le impostazioni ([impostazioni elenco](./listing-settings.md), [regole di inserzione](./listing-rules.md), [regole di determinazione prezzi](./pricing-products.md), [sostituzioni](./overrides.md)e così via) prima di completare la configurazione del negozio. Se necessario, queste impostazioni possono anche essere modificate dopo la configurazione.

- Il canale di vendita Amazon può impostare le regole di prezzo per adeguare automaticamente il prezzo dell&#39;inserzione. Le misure di protezione automatizzate dei prezzi includono [prezzo base](./floor-price.md) e [prezzo massimo opzionale](./optional-ceiling-price.md) caratteristiche di [Regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md). L&#39;uso di queste protezioni aiuta a garantire che i prezzi delle inserzioni non scendano sotto il tuo costo o al di sopra di un prezzo definito.

- La sincronizzazione dei dati tra il canale di vendita di Amazon e Amazon è controllata dal tuo [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) impostazioni. Limitazione incorporata tra [!DNL Commerce] e Amazon contribuisce a garantire una trasmissione dei dati fluida ed efficiente, ma durante periodi di traffico e-commerce elevati (come il Black Friday), l’aggiornamento dei sistemi Amazon potrebbe richiedere più tempo del solito. Imposta il [!DNL Commerce] cron da eseguire una volta ogni cinque minuti.

- Il canale di vendita Amazon importa le informazioni sull’ordine Amazon. Per gestire gli ordini Amazon nel canale di vendita Amazon, assicurati che il tuo [impostazioni ordine](./order-settings.md) sono definiti per importare e creare un [!DNL Commerce] per ogni ordine di Amazon. Se non è definita, puoi visualizzare solo le informazioni sull’ordine di Amazon. Tutte le imposte per le vendite tramite Amazon vengono ancora gestite e rimesse tramite [!DNL Amazon Seller Central] account. In alcuni stati, Amazon è tenuta a riscuotere e rimettere automaticamente le imposte. Per altri stati, i venditori hanno la possibilità di calcolare le imposte manualmente o automaticamente. Consulta [Amazon: Politiche fiscali](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. Potrebbe essere necessario accedere al [!DNL Amazon Seller Central] per visualizzare la documentazione sulle politiche fiscali di Amazon.

- Per le regioni del Regno Unito, è consigliabile iscriversi al programma [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} prima dell’onboarding di Amazon sales channel.

  >[!NOTE]
  >
  >Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

Le limitazioni includono:

- Bundle, gift card e tipi di prodotto raggruppati che fanno parte del tuo [!DNL Commerce] il catalogo non è supportato dal canale di vendita Amazon per l’inserimento in Amazon.

- Il canale di vendita Amazon non può creare un’inserzione per un prodotto che non ha un’inserzione Amazon esistente o precedente. Se un prodotto non esiste in [!DNL Amazon Seller Central] con un codice ASIN, deve essere aggiunto in [!DNL Amazon Seller Central] in modo che Amazon possa assegnare al prodotto un codice ASIN. Dopo aver aggiunto un prodotto in Amazon e aver creato un’inserzione, questa può essere associata al catalogo nel canale di vendita Amazon e sincronizzata.
