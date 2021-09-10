---
title: Visualizza dettagli elenco
description: Per comprendere le metriche sulla concorrenza negli elenchi di Amazon e sulle singole modifiche SKU/prodotto, consulta la pagina Dettagli elenco prodotti .
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Visualizza dettagli elenco

La pagina _[!UICONTROL Product Listing Details]_mostra informazioni aggiuntive sugli elenchi di prodotti attivi, incluso il registro delle attività di elenco che mostra le modifiche su un singolo SKU/Prodotto. Queste informazioni possono essere utili per comprendere le metriche della concorrenza sui prodotti e sulle modifiche di singoli SKU/prodotti. Ulteriori informazioni su questa pagina includono:

- **[!UICONTROL Listing Details]** - Dettagli del prodotto, tra cui Nome e SKU del venditore Amazon
- **[!UICONTROL Listing Activity Log]** - Registrazione cronologica di tutte le modifiche apportate alla quotazione, ad esempio le variazioni di prezzo e di quantità/scorte. Non sono necessarie ulteriori azioni. Questo registro è fornito per la revisione per comprendere la cronologia delle modifiche.
- **[!UICONTROL Buy Box Competitor Pricing]** - Dati sullo  [[!DNL Buy Box]](./buy-box-competitor-pricing.md) stato di Amazon e sui prezzi dei concorrenti
- **[!UICONTROL Lowest Competitor Pricing]** - Informazioni sui prezzi e sul feedback del concorrente Amazon più basso

Le home page del canale di vendita Amazon condividono alcuni controlli comuni [workspace](./workspace-controls.md) che consentono di personalizzare i dati visualizzati.

## Dettagli dell&#39;elenco

Le informazioni sul prodotto visualizzate includono:

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![Dettagli dell&#39;elenco](assets/amazon-product-listing-details.png)

## Elenco del registro delle attività {#listing-activity-log}

Mostra tutte le attività recenti per l’elenco Amazon. Le informazioni visualizzate comprendono:

- SKU del venditore Amazon: Identifica la SKU (Stock Keeping Unit) definita per la quotazione.
- ASIN: Identifica l’identificatore di prodotto Amazon a 10 cifre.
- Azione di elenco: Identifica il tipo di azione che si è verificata per l’elenco.
- Commenti: Fornisce ulteriori dettagli relativi al tipo di azione di elenco che si è verificata.
- Eseguito In: Identifica la data e l’ora in cui si è verificata l’azione.

![Dettagli dell’elenco dei prodotti - Elencare il registro delle attività](assets/amazon-listing-activity-log.png)
__

## Prezzi concorrenza Buy Box {#buy-box-competitor-pricing}

In questa scheda vengono visualizzate informazioni sul commerciante Amazon che detiene la posizione [[!DNL Buy Box]](./buy-box-competitor-pricing.md) per l’elenco. Queste informazioni possono essere utilizzate per comprendere il posizionamento dei prezzi dei tuoi concorrenti su Amazon. Le informazioni visualizzate comprendono:

- ASIN: Identificatore del prodotto Amazon a 10 cifre.
- Il venditore: Identifica se sei il venditore [!DNL Buy Box]. Opzioni Sì / No
- Condizione: Identifica la condizione definita per l’elenco.
- Prezzo di listino: Identifica il prezzo di pubblicazione dell&#39;inserzione.
- Prezzo di spedizione: Identifica il prezzo di spedizione aggiunto all&#39;elenco.
- Prezzo di atterraggio: Identifica il prezzo di listino più il prezzo di spedizione per l&#39;inserzione.
- Ultimo aggiornamento: Identifica la data e l’ora in cui le informazioni sui prezzi sono state aggiornate da Amazon.

![Dettagli dell’elenco dei prodotti: Prezzo concorrente Buy Box](assets/amazon-listing-details-buy-box-2.png)

## Prezzi più bassi per i concorrenti {#lowest-competitor-pricing}

In questa scheda vengono visualizzate informazioni sui concorrenti Amazon per lo stesso elenco. Queste informazioni possono essere utilizzate per comprendere il posizionamento del prezzo e il [prezzo più basso per la concorrenza](./lowest-competitor-pricing.md). Le informazioni visualizzate comprendono:

- ASIN: Identificatore del prodotto Amazon a 10 cifre.
- Condizione: Identifica la condizione definita per l’elenco.
- Canale di evasione: Identifica il responsabile dell&#39;adempimento. Opzioni: Merchant/Amazon.
- Prezzo di listino: Identifica il prezzo di pubblicazione dell&#39;inserzione.
- Prezzo di spedizione: Identifica il prezzo di spedizione aggiunto all&#39;elenco.
- Prezzo di atterraggio: Identifica il prezzo di listino più il prezzo di spedizione per l&#39;inserzione.
- Valutazione feedback: Identifica il rating di feedback Amazon per il commerciante al prezzo più basso.
- Conteggio feedback: Identifica il conteggio dei feedback di Amazon per il commerciante al prezzo più basso.
- Ultimo aggiornamento: Identifica la data e l’ora in cui le informazioni sui prezzi sono state aggiornate da Amazon.

![Dettagli dell&#39;elenco dei prodotti - prezzi più bassi per i concorrenti](assets/amazon-listing-details-lowest-comp.png)
