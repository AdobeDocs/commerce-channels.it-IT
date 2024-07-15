---
title: Visualizzare i dettagli dell’inserzione di Amazon
description: Per comprendere le metriche della concorrenza sulle inserzioni Amazon e sulle singole modifiche SKU/prodotto, visita la pagina Dettagli sull’elenco dei prodotti.
feature: Sales Channels, Products, Merchandising
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Visualizzare i dettagli dell’inserzione di Amazon

La pagina _[!UICONTROL Product Listing Details]_contiene informazioni aggiuntive sugli elenchi di prodotti attivi, incluso il registro attività elenco, che mostra le modifiche su un singolo SKU/prodotto. Queste informazioni possono aiutarti a comprendere le metriche della concorrenza sui tuoi prodotti e sulle singole modifiche SKU/prodotto. Ulteriori informazioni su questa pagina includono:

- **[!UICONTROL Listing Details]** - Dettagli prodotto tra cui il nome e lo SKU del venditore Amazon
- **[!UICONTROL Listing Activity Log]** - Record cronologico di tutte le modifiche che si sono verificate per questa inserzione, ad esempio variazioni di prezzo e di quantità/scorte. Non sono necessarie ulteriori azioni. Questo registro viene fornito per la revisione al fine di comprendere la cronologia delle modifiche.
- **[!UICONTROL Buy Box Competitor Pricing]** - Dati per lo stato [[!DNL Buy Box]](./buy-box-competitor-pricing.md) di Amazon e i prezzi dei concorrenti
- **[!UICONTROL Lowest Competitor Pricing]** - Informazioni sui prezzi e sul feedback del concorrente Amazon più basso

Le home page del canale di vendita Amazon condividono alcuni [controlli dell&#39;area di lavoro](./workspace-controls.md) comuni che consentono di personalizzare i dati visualizzati.

## Dettagli inserzione

Le informazioni visualizzate sul prodotto includono:

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![Dettagli dell&#39;inserzione](assets/amazon-product-listing-details.png){width="600" zoomable="yes"}

## Registro attività elenco {#listing-activity-log}

Mostra tutte le attività recenti per l’elenco di Amazon. Le informazioni visualizzate includono:

- Amazon Seller SKU (SKU del venditore): identifica l’unità di gestione delle scorte (SKU) definita per l’inserzione.
- ASIN: identifica l’identificatore del prodotto Amazon a 10 cifre.
- Azione di inserzione: identifica il tipo di azione che si è verificata per l’inserzione.
- Commenti: fornisce ulteriori dettagli relativi al tipo di azione di inserimento nell’elenco che si è verificata.
- Data di esecuzione: identifica la data e l&#39;ora in cui si è verificata l&#39;azione.

![Dettagli elenco prodotti - Registro attività elenco](assets/amazon-listing-activity-log.png){width="600" zoomable="yes"}
__

## Prezzo Buy Box concorrente {#buy-box-competitor-pricing}

In questa scheda vengono visualizzate informazioni sul commerciante Amazon che detiene la posizione [[!DNL Buy Box]](./buy-box-competitor-pricing.md) per l&#39;inserzione. Queste informazioni possono essere utilizzate per comprendere il posizionamento dei prezzi dei tuoi concorrenti su Amazon. Le informazioni visualizzate includono:

- ASIN: identificatore del prodotto Amazon a 10 cifre.
- Venditore: identifica se sei il venditore [!DNL Buy Box]. Opzioni Sì / No.
- Condizione: identifica la condizione definita per l’elenco.
- Prezzo d&#39;inserzione: identifica il prezzo a cui è stata pubblicata l&#39;inserzione.
- Prezzo di spedizione: identifica il prezzo di spedizione aggiunto all&#39;inserzione.
- Landed Price (Prezzo di arrivo): identifica il prezzo di listino più il prezzo di spedizione per l&#39;inserzione.
- Ultimo aggiornamento: identifica la data e l’ora in cui le informazioni sui prezzi sono state aggiornate da Amazon.

![Dettagli dell&#39;elenco prodotti: prezzo Buy Box concorrente](assets/amazon-listing-details-buy-box-2.png){width="600" zoomable="yes"}

## Prezzi del concorrente più basso {#lowest-competitor-pricing}

In questa scheda vengono visualizzate informazioni sui concorrenti di Amazon per la stessa inserzione. Queste informazioni possono essere utilizzate per comprendere il posizionamento del prezzo e i [prezzi del concorrente più basso](./lowest-competitor-pricing.md). Le informazioni visualizzate includono:

- ASIN: identificatore del prodotto Amazon a 10 cifre.
- Condizione: identifica la condizione definita per l’elenco.
- Canale evasione: identifica il responsabile dell&#39;evasione. Opzioni: esercente/Amazon.
- Prezzo d&#39;inserzione: identifica il prezzo a cui è stata pubblicata l&#39;inserzione.
- Prezzo di spedizione: identifica il prezzo di spedizione aggiunto all&#39;inserzione.
- Landed Price (Prezzo di arrivo): identifica il prezzo di listino più il prezzo di spedizione per l&#39;inserzione.
- Punteggio di feedback: identifica il punteggio di feedback di Amazon per l’esercente al prezzo più basso.
- Conteggio feedback: identifica il conteggio dei feedback di Amazon per il commerciante al prezzo più basso.
- Ultimo aggiornamento: identifica la data e l’ora in cui le informazioni sui prezzi sono state aggiornate da Amazon.

![Dettagli dell&#39;elenco prodotti - prezzo concorrente più basso](assets/amazon-listing-details-lowest-comp.png){width="600" zoomable="yes"}
