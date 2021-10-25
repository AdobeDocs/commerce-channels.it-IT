---
title: Informazioni su Amazon e sul catalogo Commerce
description: Il canale di vendita Amazon importa gli elenchi Amazon nel backend Commerce e sincronizza continuamente con i prodotti e le vendite.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Informazioni su Amazon e [!DNL Commerce] catalogo

Il backend Adobe Commerce o Magento Open Source include un catalogo con tutti i prodotti e le impostazioni e informazioni associate (immagini, opzioni, prezzi e altro ancora) e le configurazioni di ordine e spedizione. Le [!DNL Amazon Seller Central] l&#39;account dispone anche di un catalogo e configurazioni di ordine, tenendo rigorosamente traccia delle vendite attraverso [!DNL Amazon Marketplace].

Per gestire e rivedere meglio il catalogo dei prodotti e le vendite tramite un&#39;unica posizione, il canale di vendita Amazon importa i tuoi annunci Amazon nel tuo [!DNL Commerce] back-end, sincronizza continuamente con prodotti e vendite e segnala problemi e tendenze. Supporta le integrazioni con più [!DNL Amazon Seller Central] account, tracciamento di tutti i dati tramite l&#39;interfaccia singola per più vetrine.

## Attributi del prodotto

Adobe Commerce e Magenti Open Source gestiscono le sincronizzazioni dei cataloghi con l&#39;uso del prodotto [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} per definire le impostazioni del prodotto e i dati. Amazon utilizza anche gli attributi da mappare tramite onboarding. Periodo [attività pre-installazione](./amazon-pre-setup-tasks.md) per il canale di vendita Amazon, definisci gli attributi aggiuntivi di Amazon (se necessario) per garantire la corretta mappatura del prodotto durante l’importazione degli elenchi Amazon nel [!DNL Commerce] catalogo. Questi attributi includono UPC, EAN, ISBN e ASIN ([!DNL Amazon Standard Identification Number]). Attraverso l’onboarding, la sincronizzazione dei prodotti tra Amazon e [!DNL Commerce] cataloghi utilizzando gli attributi. Mappatura corretta della [!DNL Commerce] e i prodotti Amazon garantiscono una sincronizzazione continua delle informazioni sui prodotti, degli ordini e delle scorte.

Se questi attributi non sono stati creati o configurati per il catalogo, è necessario aggiungere un [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} e i valori ai prodotti prima dell&#39;onboarding. Quando un attributo Amazon viene importato, può essere utilizzato per ricerca, navigazione, regole di prezzo e molto altro. Per ulteriori informazioni su questi attributi, consulta [Amazon: Cosa sono gli UPC, gli EAN, gli ISBN e gli ASIN?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

Dopo l’onboarding, puoi gestire e aggiornare gli attributi del prodotto e le mappature Amazon in qualsiasi momento.

## Elenco prodotti

Un elenco Amazon è una pagina di prodotto per ogni prodotto venduto tramite [!DNL Amazon Marketplace], visualizzazione di descrizioni del prodotto, prezzi, immagini e altro ancora mappati tramite attributi. Durante l’onboarding, puoi configurare le [!DNL Commerce] i prodotti possono essere pubblicati automaticamente negli elenchi di Amazon. Puoi anche importare gli elenchi Amazon esistenti mappandoli al tuo [!DNL Commerce] prodotti.

Quando hai creato un elenco [!DNL Commerce] i prodotti vengono inviati ad Amazon per l’approvazione. La maggior parte degli elenchi di successo sono approvati in poche ore. Se l&#39;inserzione è approvata, viene visualizzata nella [!DNL Amazon Marketplace] per ordini immediati da parte dei clienti. La [!DNL Amazon Sales Channel] L&#39;estensione fornisce un set di schede per esaminare gli elenchi di Amazon. A seconda del problema o dei dati richiesti, devi rivedere il tuo [!DNL Amazon Seller Central] tenere conto dei dettagli specifici relativi a tali elenchi.

- [Attivo](./active-listings.md): Elenca gli elenchi di prodotti approvati disponibili nel marketplace.

- [Pronto per l&#39;elenco](./ready-to-list.md): Elenca i prodotti che soddisfano i requisiti delle regole e sono pronti per la pubblicazione in Amazon.

- [Inattivo](./inactive-listings.md): Elenca i prodotti che non sono disponibili sul mercato a causa di un blocco per un motivo specifico (come il problema del branding), chiusi e che richiedono la relisting e così via.

- [Non applicabile](./ineligible-listings.md): A causa delle regole di inserimento nell’elenco, elenca i prodotti che non possono essere elencati attivamente sul mercato (ad esempio `0` quantità o date di vendita).

- [Incompleto](./incomplete-listings.md): Elenca i prodotti che non contengono le informazioni richieste. Aggiorna i dati del prodotto per un&#39;altra revisione.

- [Terminato](./ended-listings.md): Elenca gli elenchi di prodotti idonei all’elenco ma rimossi manualmente da Amazon. È possibile inserire in un elenco dei prodotti.

## Sincronizzazione dei dati

Adobe Commerce e Magenti Open Source comunicano i dati relativi a prodotti e ordini tra le [!DNL Amazon Seller Central] e [!DNL Commerce] backend. Gli aggiornamenti continui forniscono una singola fonte attraverso [!DNL Commerce] per gestire e mantenere gli inventari, soddisfare gli ordini, tenere traccia delle vendite e ridurre i costi di carico e la duplicazione del lavoro. Il reporting acquisisce i dati più recenti per tenere traccia delle tendenze e risolvere i problemi di comunicazione rilevati tra i due sistemi.

Tutta la sincronizzazione è gestita da un [cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, impostare l&#39;aggiornamento ogni cinque minuti nel [Attività pre-installazione](./amazon-pre-setup-tasks.md).
