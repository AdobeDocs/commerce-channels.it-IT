---
title: Informazioni su Amazon e sul catalogo Commerce
description: Il canale di vendita Amazon importa gli elenchi Amazon nel backend Commerce e sincronizza continuamente con i prodotti e le vendite.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Informazioni su Amazon e il catalogo [!DNL Commerce]

Il back-end Commerce o Magento Open Source di Adobe include un catalogo con tutti i prodotti e le impostazioni e informazioni associate (immagini, opzioni, prezzi e altro) e configurazioni di ordine e spedizione. Il tuo account [!DNL Amazon Seller Central] dispone anche di un catalogo e di configurazioni di ordine, che tengono rigorosamente traccia delle tue vendite attraverso il [!DNL Amazon Marketplace].

Per gestire e rivedere meglio il catalogo dei prodotti e le vendite in un&#39;unica posizione, il canale di vendita Amazon importa gli elenchi Amazon nel tuo [!DNL Commerce] backend, si sincronizza continuamente con i prodotti e le vendite, segnala problemi e tendenze. Supporta le integrazioni con più account [!DNL Amazon Seller Central], tracciando tutti i dati tramite la singola interfaccia per più vetrine.

## Attributi del prodotto

Adobe Commerce e Magento Open Source gestiscono le sincronizzazioni dei cataloghi con l&#39;uso di [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} per definire le impostazioni dei prodotti e i dati. Amazon utilizza anche gli attributi da mappare tramite onboarding. Durante le [attività pre-installazione](./amazon-pre-setup-tasks.md) per il canale di vendita Amazon, definisci gli attributi aggiuntivi di Amazon (se necessario) per garantire la corretta mappatura dei prodotti durante l&#39;importazione degli elenchi Amazon nel catalogo [!DNL Commerce]. Questi attributi includono UPC, EAN, ISBN e ASIN ([!DNL Amazon Standard Identification Number]). Attraverso l’onboarding, i prodotti vengono sincronizzati tra i cataloghi Amazon e [!DNL Commerce] utilizzando i tuoi attributi. La corretta mappatura dei prodotti [!DNL Commerce] e Amazon assicura una sincronizzazione continua delle informazioni sui prodotti, degli ordini e dell’inventario.

Se questi attributi non sono stati creati o configurati per il catalogo, è necessario aggiungere un [!DNL Commerce] [attributo di prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} e valori ai prodotti prima dell&#39;onboarding. Quando un attributo Amazon viene importato, può essere utilizzato per ricerca, navigazione, regole di prezzo e molto altro. Per ulteriori informazioni su questi attributi, consulta [Amazon: Cosa sono gli UPC, gli EAN, gli ISBN e gli ASIN?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

Dopo l’onboarding, puoi gestire e aggiornare gli attributi del prodotto e le mappature Amazon in qualsiasi momento.

## Elenco prodotti

Un elenco Amazon è una pagina di prodotto per ogni prodotto venduto tramite [!DNL Amazon Marketplace], che mostra descrizioni del prodotto, prezzi, immagini e altro ancora mappato attraverso gli attributi. Durante l’onboarding, puoi configurare la pubblicazione automatica dei prodotti [!DNL Commerce] negli elenchi di Amazon. Puoi anche importare gli elenchi Amazon esistenti mappandoli ai prodotti [!DNL Commerce].

Dopo aver creato un elenco di prodotti [!DNL Commerce], questi vengono inviati ad Amazon per l’approvazione. La maggior parte degli elenchi di successo sono approvati in poche ore. Se l’inserzione è approvata, viene visualizzata in [!DNL Amazon Marketplace] per gli ordini immediati dei clienti. L&#39;estensione [!DNL Amazon Sales Channel] fornisce un set di schede per rivedere gli elenchi di Amazon. A seconda del problema o dei dati richiesti, è necessario esaminare l&#39;account [!DNL Amazon Seller Central] per informazioni specifiche su questi elenchi.

- [Attivo](./active-listings.md): Elenca gli elenchi di prodotti approvati disponibili nel marketplace.

- [Pronto per l’elenco](./ready-to-list.md): Elenca i prodotti che soddisfano i requisiti delle regole e sono pronti per la pubblicazione in Amazon.

- [Inattivo](./inactive-listings.md): Elenca i prodotti che non sono disponibili sul mercato a causa di un blocco per un motivo specifico (come il problema del branding), chiusi e che richiedono la relisting e così via.

- [Non ammissibile](./ineligible-listings.md): A causa delle regole di quotazione, elenca i prodotti che non possono essere elencati attivamente sul mercato (ad esempio le date di  `0` quantità o di vendita).

- [Incompleto](./incomplete-listings.md): Elenca i prodotti che non contengono le informazioni richieste. Aggiorna i dati del prodotto per un&#39;altra revisione.

- [Terminato](./ended-listings.md): Elenca gli elenchi di prodotti idonei all’elenco ma rimossi manualmente da Amazon. È possibile inserire in un elenco dei prodotti.

## Sincronizzazione dei dati

Adobe Commerce e Magenti Open Source comunicano i dati di prodotto e ordine tra il tuo account [!DNL Amazon Seller Central] e il back-end [!DNL Commerce]. Gli aggiornamenti continui forniscono un&#39;unica fonte attraverso [!DNL Commerce] per gestire e mantenere gli inventari, soddisfare gli ordini, tenere traccia delle vendite e ridurre i costi di carico e la duplicazione del lavoro. Il reporting acquisisce i dati più recenti per tenere traccia delle tendenze e risolvere i problemi di comunicazione rilevati tra i due sistemi.

Tutta la sincronizzazione è gestita da un [lavoro cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, impostato per l&#39;aggiornamento ogni cinque minuti nel [Attività pre-installazione](./amazon-pre-setup-tasks.md).
