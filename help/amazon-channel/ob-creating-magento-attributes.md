---
title: Creare attributi [!DNL Commerce] per Amazon
description: Prima di completare il processo di onboarding dei canali di vendita Amazon, assicurati di disporre degli attributi di prodotto [!UICONTROL Commerce] necessari.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Creare attributi [!DNL Commerce] per Amazon

Prima di eseguire l&#39;onboarding degli account [!DNL Amazon Seller Central], è consigliabile aggiungere [!DNL Commerce] [attributi di prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){:target=&quot;_blank&quot;} per mappare gli elenchi di prodotti. Dopo aver completato l’onboarding, puoi gestire gli attributi del prodotto tramite la scheda [Attributi](./managing-attributes.md) della pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md).

Queste istruzioni spiegano come creare gli attributi [!DNL Commerce] per Amazon ASIN e Amazon Condition. Si consiglia di creare attributi aggiuntivi tra cui Amazon EAN, Amazon ISBN e Amazon UPC. Puoi anche creare un attributo del prezzo di Amazon se desideri utilizzare il prezzo di listino di Amazon come origine del prezzo per le regole di prezzo. Questi attributi vengono utilizzati per configurare le impostazioni di quotazione e di quotazione durante l’onboarding. Utilizza anche questi attributi durante la creazione di elenchi Amazon e durante l’aggiornamento e la sincronizzazione del catalogo [!DNL Commerce] con gli elenchi Amazon.

Le impostazioni di Ricerca nel catalogo consentono di impostare i parametri di ricerca corrispondenti che consentono di mappare i prodotti [!DNL Commerce] idonei con gli elenchi di Amazon. Quando viene mappata, Amazon attiva azioni relative a prezzi, quantità, sostituzioni e sincronizzazione di ordini e prodotti.

La definizione di questi valori aumenta il potenziale di corrispondenze esatte, riducendo al minimo la necessità di abbinare manualmente gli elenchi di prodotti in un secondo momento. Aggiungendo gli attributi come parte delle attività di onboarding [pre-configurazione](./amazon-pre-setup-tasks.md), il canale di vendita Amazon ha un potenziale più elevato per la corrispondenza automatica dei prodotti durante l&#39;onboarding e la sincronizzazione dei dati di prodotto tra Amazon e [!DNL Commerce] dopo l&#39;onboarding.

Se crei solo l’attributo Amazon ASIN (senza aggiungere valori ASIN per prodotto), i prodotti [!DNL Commerce] potrebbero non corrispondere automaticamente agli elenchi Amazon. Puoi abbinare manualmente i tuoi prodotti tramite _Store Review_. Tuttavia, la corrispondenza manuale non crea gli elementi dati necessari per condividere e sincronizzare i dati del prodotto.

>[!IMPORTANT]
>
>Se aggiorni un elemento dati ASIN, UPC o di altro tipo per un prodotto corrispondente manualmente, devi aggiornare i dati in entrambe le posizioni: il catalogo [!DNL Commerce] e l&#39;elenco nel tuo account [!DNL Amazon Seller Central].

## Creare l’attributo di prodotto Amazon ASIN

1. Accedi al tuo amministratore [!DNL Commerce].

1. Fai clic su **[!UICONTROL Stores]** nel menu a sinistra.

1. Nella sezione _[!UICONTROL Attributes]_, fai clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà degli attributi, fai clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon ASIN` (il nome dell’attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegli `Text Field`.

1. Per **[!UICONTROL Values Required]**, scegli `No`.

   Sebbene sia necessario un Amazon ASIN per elencare un prodotto su Amazon, alcuni dei prodotti di catalogo potrebbero non essere elencati su Amazon.

1. Espandi la sezione _[!UICONTROL Advanced Attribute Properties]_e imposta le opzioni:

   - Per **[!UICONTROL Attribute Code]**, immetti `amazon_asin`.

   - Per **[!UICONTROL Scope]**, scegli `Global`.

   - Per **[!UICONTROL Unique Value]**, scegli `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegli `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegli `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegli `Yes`.

1. Fare clic su **[!UICONTROL Save Attribute]**.

![Attributo Amazon ASIN](assets/creating-asin-attribute.png)

## Creare l’attributo di prodotto Amazon Condition

1. Accedi al tuo amministratore [!DNL Commerce].

1. Fai clic su **[!UICONTROL Stores]** nel menu a sinistra.

1. Nella sezione _[!UICONTROL Attributes]_, fai clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà dell&#39;attributo, fai clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon Condition` (il nome dell’attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegli `Dropdown`.

   Viene visualizzata la sezione _[!UICONTROL Manage Options (Values of your Attribute)]_.

1. Per **[!UICONTROL Values Required]**, scegli `No`.

1. Per **[!UICONTROL Manage Options (Values for your Attribute)]**, aggiungi ciascuna delle opzioni di condizione.

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

1. Selezionare l’opzione **[!UICONTROL Is Default]** per la condizione che si desidera impostare come selezione predefinita.

1. Nella colonna _[!UICONTROL Admin]_, immetti il testo per l’etichetta della condizione che stai aggiungendo (ad esempio `New`, `Used` e `Used-Like New`)

1. Fai clic su **[!UICONTROL Add Option]** per aggiungere altre opzioni, in base alle esigenze.

1. Espandi la sezione _[!UICONTROL Advanced Attribute Properties]_e imposta le opzioni.

   - Per **[!UICONTROL Attribute Code]**, immetti `amazon_condition`.

   - Per **[!UICONTROL Scope]**, scegli `Global`.

   - Per **[!UICONTROL Unique Value]**, scegli `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegli `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegli `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegli `Yes`.

1. Fare clic su **[!UICONTROL Save Attribute]**.

![Attributo condizione Amazon](assets/creating-amazon-condition-attribute.png)

![Icona ](assets/btn-next.png) [**SuccessivaContinua ad aggiungere o verificare la chiave API**](./amazon-verify-api-key.md)
