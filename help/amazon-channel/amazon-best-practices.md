---
title: Best practice e limitazioni per  [!DNL Amazon sales channel]
description: Rivedi le best practice e le limitazioni nell’utilizzo del canale di vendita Amazon per Adobe Commerce e Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Best practice e limitazioni per [!DNL Amazon sales channel]

Le best practice includono:

- Il canale di vendita Amazon può influenzare le tue inserzioni Amazon aumentando o diminuendo i prezzi, sincronizzando le informazioni sui prodotti (comprese le azioni disponibili) e aggiungendo, aggiornando ed eliminando le inserzioni. Rivedi le inserzioni in base allo stato durante la configurazione e regola le impostazioni ([impostazioni inserzioni](./listing-settings.md), [regole inserzioni](./listing-rules.md), [regole prezzi](./pricing-products.md), [sostituzioni](./overrides.md) e così via) prima di completare la configurazione dello store. Se necessario, queste impostazioni possono anche essere modificate dopo la configurazione.

- Il canale di vendita Amazon può impostare le regole di prezzo per adeguare automaticamente il prezzo dell&#39;inserzione. Le protezioni automatizzate per la determinazione dei prezzi includono le caratteristiche [prezzo base](./floor-price.md) e [prezzo limite opzionale](./optional-ceiling-price.md) di [regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md). L&#39;uso di queste protezioni aiuta a garantire che i prezzi delle inserzioni non scendano sotto il tuo costo o al di sopra di un prezzo definito.

- La sincronizzazione dei dati tra il canale di vendita Amazon e Amazon è controllata dalle impostazioni [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). La limitazione incorporata tra [!DNL Commerce] e Amazon contribuisce a garantire una trasmissione dei dati fluida ed efficiente, ma durante i periodi di traffico di eCommerce elevato (come il Black Friday), l&#39;aggiornamento dei sistemi Amazon potrebbe richiedere più tempo del solito. Imposta l&#39;esecuzione del cron [!DNL Commerce] una volta ogni cinque minuti.

- Il canale di vendita Amazon importa le informazioni sull’ordine Amazon. Per gestire gli ordini Amazon nel canale di vendita Amazon, è necessario assicurarsi che le [impostazioni ordine](./order-settings.md) siano definite per importare e creare un ordine [!DNL Commerce] corrispondente per ogni ordine Amazon. Se non è definita, puoi visualizzare solo le informazioni sull’ordine di Amazon. Tutte le imposte per le vendite tramite Amazon vengono ancora gestite e rimesse tramite l&#39;account [!DNL Amazon Seller Central]. In alcuni stati, Amazon è tenuta a riscuotere e rimettere automaticamente le imposte. Per altri stati, i venditori hanno la possibilità di calcolare le imposte manualmente o automaticamente. Vedi [Amazon: Criteri fiscali](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. Potrebbe essere necessario accedere all&#39;account [!DNL Amazon Seller Central] per visualizzare la documentazione sulla politica fiscale di Amazon.

- Per le aree geografiche del Regno Unito, è consigliabile iscriversi al [Servizio di calcolo IVA di Amazon](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} prima dell&#39;onboarding del canale di vendita Amazon.

  >[!NOTE]
  >
  >Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

Le limitazioni includono:

- I tipi di prodotti raggruppati, gift card e bundle che fanno parte del catalogo [!DNL Commerce] non sono supportati dal canale di vendita Amazon per l&#39;inserimento in Amazon.

- Il canale di vendita Amazon non può creare un’inserzione per un prodotto che non ha un’inserzione Amazon esistente o precedente. Se un prodotto non esiste in [!DNL Amazon Seller Central] con un ASIN, è necessario aggiungerlo in [!DNL Amazon Seller Central] in modo che Amazon possa assegnare al prodotto un ASIN. Dopo aver aggiunto un prodotto in Amazon e aver creato un’inserzione, questa può essere associata al catalogo nel canale di vendita Amazon e sincronizzata.
