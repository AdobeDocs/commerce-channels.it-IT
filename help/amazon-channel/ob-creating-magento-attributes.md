---
title: Creare attributi Commerce per Amazon
description: Prima di completare il processo di onboarding del canale di vendita Amazon, assicurati di disporre degli attributi di prodotto [!UICONTROL Commerce] necessari.
role: Admin
feature: Sales Channels, Products, Configuration
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Creare attributi Commerce per Amazon

Prima di effettuare l&#39;onboarding degli account [!DNL Amazon Seller Central], è consigliabile aggiungere [!DNL Commerce] [attributi di prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) per mappare gli elenchi di prodotti. Dopo aver completato l&#39;onboarding, puoi gestire gli attributi del prodotto tramite la scheda [Attributi](./managing-attributes.md) della [home del canale di vendita Amazon](./amazon-sales-channel-home.md).

Queste istruzioni spiegano come creare gli attributi [!DNL Commerce] per Amazon ASIN e Amazon Condition. Si consiglia di creare attributi aggiuntivi, tra cui Amazon EAN, Amazon ISBN e Amazon UPC. Puoi anche creare un attributo Prezzo di Amazon se desideri utilizzare il prezzo di Amazon come origine del prezzo per le regole di determinazione prezzi. Questi attributi vengono utilizzati per configurare le impostazioni relative alle inserzioni e ai prezzi durante l’onboarding. Utilizza questi attributi anche per creare inserzioni Amazon e per aggiornare e sincronizzare il catalogo [!DNL Commerce] con le tue inserzioni Amazon.

Le impostazioni di Ricerca nel catalogo consentono di impostare i parametri di ricerca corrispondenti che consentono di mappare i prodotti [!DNL Commerce] idonei con le inserzioni Amazon. Una volta eseguito il mapping, Amazon attiva le azioni relative alla determinazione dei prezzi, alla quantità, alle sostituzioni e alla sincronizzazione di ordini e prodotti.

La definizione di questi valori aumenta il rischio di corrispondenze esatte, riducendo al minimo la necessità di abbinare manualmente gli elenchi di prodotti in un secondo momento. Aggiungendo gli attributi come parte delle [attività di configurazione preliminari all&#39;onboarding](./amazon-pre-setup-tasks.md), il canale di vendita Amazon ha un potenziale maggiore per abbinare automaticamente i prodotti durante l&#39;onboarding e sincronizzare i dati dei prodotti tra Amazon e [!DNL Commerce] dopo l&#39;onboarding.

Se crei solo l&#39;attributo Amazon ASIN (senza aggiungere valori ASIN per prodotto), i prodotti [!DNL Commerce] potrebbero non corrispondere automaticamente alle inserzioni Amazon. Puoi abbinare manualmente i tuoi prodotti tramite _Store Review_. Tuttavia, la corrispondenza manuale non crea gli elementi di dati necessari per condividere e sincronizzare i dati di prodotto.

>[!IMPORTANT]
>
>Se si aggiorna un codice ASIN, UPC o un altro elemento dati per un prodotto con corrispondenza manuale, è necessario aggiornare i dati in entrambe le posizioni: il catalogo [!DNL Commerce] e l&#39;inserzione nell&#39;account [!DNL Amazon Seller Central].

## Creare l’attributo di prodotto Amazon ASIN

1. Accedi all&#39;amministratore [!DNL Commerce].

1. Fare clic su **[!UICONTROL Stores]** nel menu a sinistra.

1. Nella sezione _[!UICONTROL Attributes]_, fare clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà degli attributi, fare clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon ASIN` (il nome dell&#39;attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegliere `Text Field`.

1. Per **[!UICONTROL Values Required]**, scegliere `No`.

   Anche se è richiesto un codice ASIN di Amazon per elencare un prodotto su Amazon, alcuni dei prodotti del catalogo potrebbero non essere elencati su Amazon.

1. Espandere la sezione _[!UICONTROL Advanced Attribute Properties]_e impostare le opzioni:

   - Per **[!UICONTROL Attribute Code]**, immettere `amazon_asin`.

   - Per **[!UICONTROL Scope]**, scegliere `Global`.

   - Per **[!UICONTROL Unique Value]**, scegliere `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegliere `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegliere `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegliere `Yes`.

1. Fare clic su **[!UICONTROL Save Attribute]**.

![Attributo Amazon ASIN](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Creare l’attributo di prodotto Condizione di Amazon

1. Accedi all&#39;amministratore [!DNL Commerce].

1. Fare clic su **[!UICONTROL Stores]** nel menu a sinistra.

1. Nella sezione _[!UICONTROL Attributes]_, fare clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà dell&#39;attributo, fare clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon Condition` (il nome dell&#39;attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegliere `Dropdown`.

   Viene visualizzata la sezione _[!UICONTROL Manage Options (Values of your Attribute)]_.

1. Per **[!UICONTROL Values Required]**, scegliere `No`.

1. Per **[!UICONTROL Manage Options (Values for your Attribute)]**, aggiungi tutte le opzioni di condizione.

   Le condizioni standard di Amazon includono:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Fare clic su **[!UICONTROL Add Option]**.

1. Selezionare l&#39;opzione **[!UICONTROL Is Default]** per la condizione che si desidera sia la selezione predefinita.

1. Nella colonna _[!UICONTROL Admin]_immettere il testo per l&#39;etichetta della condizione che si sta aggiungendo (ad esempio `New`, `Used` e `Used-Like New`)

1. Fare clic su **[!UICONTROL Add Option]** per aggiungere altre opzioni, in base alle esigenze.

1. Espandere la sezione _[!UICONTROL Advanced Attribute Properties]_e impostare le opzioni.

   - Per **[!UICONTROL Attribute Code]**, immettere `amazon_condition`.

   - Per **[!UICONTROL Scope]**, scegliere `Global`.

   - Per **[!UICONTROL Unique Value]**, scegliere `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegliere `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegliere `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegliere `Yes`.

1. Fare clic su **[!UICONTROL Save Attribute]**.

![Attributo condizione Amazon](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![Icona successiva](assets/btn-next.png) [**Continua ad aggiungere o verificare la chiave API**](./amazon-verify-api-key.md)
