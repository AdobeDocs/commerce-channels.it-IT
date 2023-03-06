---
title: Informazioni su Amazon e sul catalogo Commerce
description: Il canale di vendita Amazon importa le inserzioni Amazon nel backend Commerce e si sincronizza continuamente con i prodotti e le vendite.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# AMAZON e [!DNL Commerce] Catalogo

Il tuo backend Adobe Commerce o Magento Open Source include un catalogo con tutti i prodotti e le relative impostazioni e informazioni (immagini, opzioni, prezzi e altro) e configurazioni di ordine e spedizione. Il tuo [!DNL Amazon Seller Central] l&#39;account dispone anche di un catalogo e configurazioni degli ordini, tenendo traccia rigorosamente delle vendite attraverso [!DNL Amazon Marketplace].

Per gestire e rivedere meglio il catalogo dei prodotti e le vendite attraverso un&#39;unica posizione, il canale di vendita Amazon importa le tue inserzioni Amazon nel tuo [!DNL Commerce] back-end, si sincronizza continuamente con prodotti e vendite e segnala problemi e tendenze. Supporta le integrazioni con più [!DNL Amazon Seller Central] account, tenendo traccia di tutti i dati tramite l&#39;unica interfaccia per più storefront.

## Attributi del prodotto

Adobe Commerce e il Magento Open Source gestiscono le sincronizzazioni dei cataloghi con l’utilizzo dei prodotti [attributi](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} per definire le impostazioni e i dati del prodotto. Amazon utilizza anche attributi da mappare tramite l’onboarding. Durante [attività di preconfigurazione](./amazon-pre-setup-tasks.md) per il canale di vendita Amazon, puoi definire attributi Amazon aggiuntivi (se necessario) per garantire le mappature corrette dei prodotti durante l’importazione delle inserzioni Amazon nel tuo [!DNL Commerce] catalogo. Questi attributi includono UPC, EAN, ISBN e ASIN ([!DNL Amazon Standard Identification Number]). Grazie all’onboarding, i prodotti si sincronizzano tra Amazon e [!DNL Commerce] cataloghi utilizzando gli attributi. Mappatura corretta del [!DNL Commerce] I prodotti Amazon garantiscono una sincronizzazione continua di informazioni sui prodotti, ordini e inventario.

Se non hai creato o configurato questi attributi per il catalogo, devi aggiungere una [!DNL Commerce] [attributo prodotto](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} and values to your products before onboarding. When an Amazon attribute is imported, it can be used for search, navigation, price rules, and much more. See [What Do ASIN, UPC, EAN, ISBN, SKU and Other Barcodes Mean?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

Dopo l’onboarding, puoi gestire e aggiornare gli attributi del prodotto e le mappature di Amazon in qualsiasi momento.

## Elenco prodotti

Un&#39;inserzione di Amazon è una pagina di prodotto per ogni prodotto che vendi tramite [!DNL Amazon Marketplace], che mostra descrizioni di prodotto, prezzi, immagini e altro ancora mappati tramite attributi. Durante l’onboarding, puoi configurare [!DNL Commerce] I prodotti possono essere pubblicati automaticamente nelle inserzioni di Amazon. Puoi anche importare le tue inserzioni esistenti di Amazon mappandole sul tuo [!DNL Commerce] prodotti.

Dopo aver creato un&#39;inserzione [!DNL Commerce] prodotti, vengono inviati ad Amazon per l&#39;approvazione. La maggior parte delle inserzioni scadute viene approvata entro poche ore. Se l&#39;inserzione viene approvata, viene visualizzata nella [!DNL Amazon Marketplace] per gli ordini immediati dei clienti. Il [!DNL Amazon Sales Channel] L&#39;estensione fornisce un set di schede per esaminare le inserzioni di Amazon. A seconda del problema o dei dati richiesti, è necessario rivedere [!DNL Amazon Seller Central] account per dettagli specifici su queste inserzioni.

- [Attivo](./active-listings.md): elenca gli elenchi di prodotti approvati disponibili sul marketplace.

- [Pronto per l&#39;elenco](./ready-to-list.md): elenca i prodotti che soddisfano i requisiti delle regole di elenco e che sono pronti per la pubblicazione in Amazon.

- [Inattivo](./inactive-listings.md): elenca i prodotti che non sono disponibili sul marketplace perché sono bloccati per un motivo specifico (ad esempio un problema di branding), sono chiusi e richiedono la reinserimento nell’elenco e così via.

- [Non ammissibile](./ineligible-listings.md): a causa delle regole di inserzione, elenca i prodotti che non possono essere attivamente elencati sul marketplace (ad esempio `0` quantità o date di vendita).

- [Incompleto](./incomplete-listings.md): elenca i prodotti per i quali mancano le informazioni richieste. Aggiorna i dati del prodotto per un’altra revisione.

- [Terminato](./ended-listings.md): elenca gli elenchi di prodotti idonei per l’inserimento nell’elenco ma rimossi manualmente da Amazon. Puoi rimettere in vendita questi prodotti.

## Sincronizzazione dei dati

Adobe Commerce e il Magento Open Source comunicano i dati di prodotti e ordini tra [!DNL Amazon Seller Central] account e [!DNL Commerce] backend. Gli aggiornamenti continui forniscono un’unica origine tramite [!DNL Commerce] gestire e gestire le scorte, evadere gli ordini, tenere traccia delle vendite e ridurre i costi comuni e la duplicazione del lavoro. Il reporting acquisisce i dati più recenti per monitorare le tendenze e risolvere i problemi di comunicazione rilevati tra i due sistemi.

Tutta la sincronizzazione è gestita da un [lavoro cron](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}, impostato per l&#39;aggiornamento ogni cinque minuti [Attività di pre-configurazione](./amazon-pre-setup-tasks.md).
