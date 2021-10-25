---
title: Best practice e limitazioni per il canale di vendita Amazon
description: Controlla le best practice e le limitazioni quando utilizzi il canale di vendita Amazon per Adobe Commerce e il Magento Open Source.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Best practice e limitazioni per il canale di vendita Amazon

Le best practice includono:

- Il canale di vendita Amazon può influenzare le tue inserzioni Amazon aumentando o diminuendo i prezzi, sincronizzando le informazioni sui prodotti (incluse le azioni disponibili) e aggiungendo, aggiornando e terminando (eliminando) le inserzioni. Rivedi gli elenchi in base allo stato durante la configurazione e regola le impostazioni ([elenco delle impostazioni](./listing-settings.md), [regole di elenco](./listing-rules.md), [regole di determinazione dei prezzi](./pricing-products.md), [sostituzioni](./overrides.md)e così via) prima di completare la configurazione dello store. Queste impostazioni possono essere modificate anche dopo la configurazione, a seconda delle necessità.

- Il canale di vendita Amazon può impostare le regole di prezzo per regolare automaticamente il prezzo dell&#39;annuncio. Le garanzie dei prezzi automatizzati includono: [prezzo base](./floor-price.md) e [prezzo massimo facoltativo](./optional-ceiling-price.md) caratteristiche [Regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md). L&#39;uso di queste garanzie aiuta a garantire che i prezzi di inserzione non vadano al di sotto del costo o al di sopra di un prezzo definito.

- La sincronizzazione dei dati tra il canale di vendita Amazon e Amazon è controllata dal tuo [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html)Impostazioni {target=&quot;_blank&quot;}. Limitazione integrata tra [!DNL Commerce] e Amazon contribuisce a garantire una trasmissione dei dati fluida ed efficiente, ma durante gli elevati tempi di traffico e-commerce (come il Black Friday), l’aggiornamento dei sistemi Amazon potrebbe richiedere più tempo del solito. Imposta le [!DNL Commerce] cron da correre una volta ogni cinque minuti.

- Il canale di vendita Amazon importa le informazioni sull&#39;ordine Amazon. Per gestire gli ordini Amazon nel canale di vendita Amazon, devi assicurarti che [impostazioni ordine](./order-settings.md) sono definiti per importare e creare un [!DNL Commerce] per ogni ordine Amazon. Se non è definito, puoi visualizzare solo le informazioni sull’ordine di Amazon. Tutte le imposte per le vendite tramite Amazon sono ancora gestite e rimesse tramite il tuo [!DNL Amazon Seller Central] conto. In alcuni stati, Amazon è tenuto a riscuotere e sgravare automaticamente le imposte. Per gli altri stati, i venditori hanno la possibilità di calcolare le imposte manualmente o automaticamente. Vedi [Amazon: Politiche fiscali](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}. Potrebbe essere necessario accedere al [!DNL Amazon Seller Central] per visualizzare la documentazione relativa ai criteri fiscali di Amazon.

- Per le regioni del Regno Unito è consigliabile iscriversi al programma [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;} prima dell&#39;onboarding del canale di vendita Amazon.


   >[!NOTE]
   >
   >Potrebbero essere necessari 10-14 giorni perché Amazon verifichi e attivi il tuo account Servizio di calcolo dell&#39;IVA.

Le limitazioni includono:

- Bundle, carta regalo e tipi di prodotti raggruppati che fanno parte del tuo [!DNL Commerce] Il catalogo non è supportato dal canale di vendita Amazon per l’inserimento nell’elenco di Amazon.

- Il canale di vendita Amazon non può creare un elenco per un prodotto che non ha un elenco Amazon esistente o precedente. Se un prodotto non esiste in [!DNL Amazon Seller Central] con un ASIN, deve essere aggiunto in [!DNL Amazon Seller Central] in modo che Amazon possa assegnare al prodotto un valore ASIN. Dopo aver aggiunto un prodotto in Amazon e aver creato un elenco, quest’ultimo può essere abbinato al catalogo nel canale di vendita Amazon e sincronizzato.
