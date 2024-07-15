---
title: Amazon e il catalogo Commerce
description: Il canale di vendita Amazon importa le inserzioni Amazon nel backend Commerce e si sincronizza continuamente con i prodotti e le vendite.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog Management
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Amazon e il catalogo [!DNL Commerce]

Il tuo backend Adobe Commerce o Magento Open Source include un catalogo con tutti i prodotti e le relative impostazioni e informazioni (immagini, opzioni, prezzi e altro) e configurazioni di ordine e spedizione. L&#39;account [!DNL Amazon Seller Central] dispone anche di un catalogo e di configurazioni degli ordini, tenendo traccia delle vendite attraverso [!DNL Amazon Marketplace].

Per gestire e rivedere meglio il catalogo dei prodotti e le vendite in un&#39;unica posizione, il canale di vendita Amazon importa le inserzioni Amazon nel backend di [!DNL Commerce], si sincronizza continuamente con i prodotti e le vendite e segnala problemi e tendenze. Supporta le integrazioni con più account [!DNL Amazon Seller Central], tenendo traccia di tutti i dati tramite la singola interfaccia per più storefront.

## Attributi del prodotto

Adobe Commerce e Magento Open Source gestiscono le sincronizzazioni del catalogo con l&#39;utilizzo degli [attributi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) del prodotto per definire le impostazioni e i dati del prodotto. Amazon utilizza anche attributi da mappare tramite l’onboarding. Durante le [attività di preconfigurazione](./amazon-pre-setup-tasks.md) per il canale di vendita Amazon, puoi definire attributi Amazon aggiuntivi (se necessario) per garantire le corrette mappature dei prodotti durante l&#39;importazione delle inserzioni Amazon nel catalogo [!DNL Commerce]. Questi attributi includono UPC, EAN, ISBN e ASIN ([!DNL Amazon Standard Identification Number]). Grazie all&#39;onboarding, i prodotti vengono sincronizzati tra i cataloghi Amazon e [!DNL Commerce] utilizzando i tuoi attributi. La mappatura corretta dei prodotti [!DNL Commerce] e Amazon garantisce una sincronizzazione continua di informazioni sui prodotti, ordini e inventario.

Se non hai creato o configurato questi attributi per il catalogo, devi aggiungere un [!DNL Commerce] [attributo di prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) e dei valori ai prodotti prima dell&#39;onboarding. Quando un attributo Amazon viene importato, può essere utilizzato per la ricerca, la navigazione, le regole di prezzo e molto altro. Vedi [Cosa significano ASIN, UPC, EAN, ISBN, SKU e altri codici a barre?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

Dopo l’onboarding, puoi gestire e aggiornare gli attributi del prodotto e le mappature di Amazon in qualsiasi momento.

## Elenco prodotti

Un&#39;inserzione di Amazon è una pagina di prodotto per ogni prodotto venduto tramite [!DNL Amazon Marketplace], con descrizioni di prodotto, prezzi, immagini e altro ancora mappati tramite attributi. Durante l&#39;onboarding, puoi configurare i prodotti [!DNL Commerce] che possono essere pubblicati automaticamente nelle inserzioni di Amazon. Puoi anche importare le tue inserzioni Amazon esistenti mappandole ai tuoi prodotti [!DNL Commerce].

Dopo aver creato un&#39;inserzione di [!DNL Commerce] prodotti, questi vengono inviati ad Amazon per l&#39;approvazione. La maggior parte delle inserzioni scadute viene approvata entro poche ore. Se l&#39;inserzione viene approvata, verrà visualizzata in [!DNL Amazon Marketplace] per gli ordini immediati dei clienti. L&#39;estensione [!DNL Amazon Sales Channel] fornisce un set di schede per esaminare le inserzioni Amazon. A seconda del problema o dei dati richiesti, è necessario controllare l&#39;account [!DNL Amazon Seller Central] per i dettagli specifici di queste inserzioni.

- [Attivo](./active-listings.md): elenca gli elenchi di prodotti approvati disponibili nel marketplace.

- [Pronto per l&#39;elenco](./ready-to-list.md): elenca i prodotti che soddisfano i requisiti delle regole dell&#39;elenco e che sono pronti per la pubblicazione in Amazon.

- [Inattivo](./inactive-listings.md): elenca i prodotti che non sono disponibili sul marketplace perché bloccati per un motivo specifico (ad esempio un problema di branding), chiusi e che richiedono la rimessa in vendita e così via.

- [Non idoneo](./ineligible-listings.md): a causa delle regole di inserzione, elenca i prodotti che non possono essere inseriti attivamente nel marketplace (ad esempio `0` quantità o date di vendita).

- [Incompleto](./incomplete-listings.md): elenca i prodotti per i quali mancano le informazioni richieste. Aggiorna i dati del prodotto per un’altra revisione.

- [Terminato](./ended-listings.md): elenca gli elenchi di prodotti idonei per l&#39;inserimento ma rimossi manualmente da Amazon. Puoi rimettere in vendita questi prodotti.

## Sincronizzazione dei dati

Adobe Commerce e Magento Open Source comunicano i dati di prodotti e ordini tra l&#39;account [!DNL Amazon Seller Central] e il backend [!DNL Commerce]. Gli aggiornamenti continui forniscono un&#39;unica origine tramite [!DNL Commerce] per gestire e gestire gli inventari, evadere gli ordini, tenere traccia delle vendite e ridurre i costi comuni e la duplicazione del lavoro. Il reporting acquisisce i dati più recenti per monitorare le tendenze e risolvere i problemi di comunicazione rilevati tra i due sistemi.

Tutta la sincronizzazione è gestita da un [processo cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html), impostato per l&#39;aggiornamento ogni cinque minuti nelle [attività precedenti all&#39;installazione](./amazon-pre-setup-tasks.md).
