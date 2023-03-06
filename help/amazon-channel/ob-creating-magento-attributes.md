---
title: Crea [!DNL Commerce] Attributi per Amazon
description: Prima di completare il processo di onboarding del canale di vendita Amazon, assicurati di disporre dei [!UICONTROL Commerce] attributi del prodotto.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Crea [!DNL Commerce] Attributi per Amazon

Prima di effettuare l’onboarding [!DNL Amazon Seller Central] account, è consigliabile aggiungere [!DNL Commerce] [attributi prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"} per mappare gli elenchi di prodotti. Dopo aver completato l’onboarding, puoi gestire gli attributi del prodotto tramite [Attributi](./managing-attributes.md) scheda di [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina.

Queste istruzioni spiegano in dettaglio come creare [!DNL Commerce] attributi per Amazon ASIN e Amazon Condition. Si consiglia di creare attributi aggiuntivi, tra cui Amazon EAN, Amazon ISBN e Amazon UPC. Puoi anche creare un attributo Prezzo di Amazon se desideri utilizzare il prezzo di Amazon come origine del prezzo per le regole di determinazione prezzi. Questi attributi vengono utilizzati per configurare le impostazioni relative alle inserzioni e ai prezzi durante l’onboarding. Utilizza questi attributi anche per creare inserzioni in Amazon e per aggiornare e sincronizzare [!DNL Commerce] con le tue inserzioni Amazon.

Le impostazioni di Ricerca nel catalogo consentono di impostare i parametri di ricerca corrispondenti che consentono di eseguire il mapping degli idonei [!DNL Commerce] prodotti con inserzioni Amazon. Una volta eseguito il mapping, Amazon attiva le azioni relative alla determinazione dei prezzi, alla quantità, alle sostituzioni e alla sincronizzazione di ordini e prodotti.

La definizione di questi valori aumenta il rischio di corrispondenze esatte, riducendo al minimo la necessità di abbinare manualmente gli elenchi di prodotti in un secondo momento. Aggiunta di attributi come parte dell’onboarding [attività di preconfigurazione](./amazon-pre-setup-tasks.md), il canale di vendita Amazon ha un potenziale più elevato per abbinare automaticamente i prodotti durante l’onboarding e sincronizzare i dati dei prodotti tra Amazon e [!DNL Commerce] dopo l’onboarding.

Se crei solo l’attributo ASIN di Amazon (senza aggiungere valori ASIN per prodotto), il tuo [!DNL Commerce] I prodotti potrebbero non corrispondere automaticamente alle inserzioni Amazon. Puoi abbinare manualmente i tuoi prodotti tramite _Recensione store_. Tuttavia, la corrispondenza manuale non crea gli elementi di dati necessari per condividere e sincronizzare i dati di prodotto.

>[!IMPORTANT]
>
>Se aggiorni un codice ASIN, UPC o un altro elemento dati per un prodotto con corrispondenza manuale, devi aggiornare i dati in entrambe le posizioni: [!DNL Commerce] e l’inserzione nel tuo catalogo [!DNL Amazon Seller Central] account.

## Creare l’attributo di prodotto Amazon ASIN

1. Accedi al tuo [!DNL Commerce] Amministratore

1. Clic **[!UICONTROL Stores]** nel menu a sinistra.

1. In _[!UICONTROL Attributes]_, fare clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà degli attributi, fai clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon ASIN` (il nome dell&#39;attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegli `Text Field`.

1. Per **[!UICONTROL Values Required]**, scegli `No`.

   Anche se è richiesto un codice ASIN di Amazon per elencare un prodotto su Amazon, alcuni dei prodotti del catalogo potrebbero non essere elencati su Amazon.

1. Espandi _[!UICONTROL Advanced Attribute Properties]_e impostare le opzioni:

   - Per **[!UICONTROL Attribute Code]**, immetti `amazon_asin`.

   - Per **[!UICONTROL Scope]**, scegli `Global`.

   - Per **[!UICONTROL Unique Value]**, scegli `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegli `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegli `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegli `Yes`.

1. Clic **[!UICONTROL Save Attribute]**.

![Attributo Amazon ASIN](assets/creating-asin-attribute.png)

## Creare l’attributo di prodotto Condizione di Amazon

1. Accedi al tuo [!DNL Commerce] Amministratore

1. Clic **[!UICONTROL Stores]** nel menu a sinistra.

1. In _[!UICONTROL Attributes]_, fare clic su **[!UICONTROL Product]**.

1. Per aprire le proprietà dell’attributo, fai clic su **[!UICONTROL Add New Attribute]**.

1. Per **[!UICONTROL Default Label]**, immetti `Amazon Condition` (il nome dell&#39;attributo).

1. Per **[!UICONTROL Catalog Input Type for Store Owner]**, scegli `Dropdown`.

   Il _[!UICONTROL Manage Options (Values of your Attribute)]_viene visualizzata la sezione.

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

1. Clic **[!UICONTROL Add Option]**.

1. Seleziona la **[!UICONTROL Is Default]** per la condizione che desideri sia la selezione predefinita.

1. In _[!UICONTROL Admin]_, immetti il testo per l’etichetta della condizione che stai aggiungendo, ad esempio `New`, `Used`, e `Used-Like New`)

1. Clic **[!UICONTROL Add Option]** per aggiungere altre opzioni, in base alle esigenze.

1. Espandi _[!UICONTROL Advanced Attribute Properties]_e impostare le opzioni.

   - Per **[!UICONTROL Attribute Code]**, immetti `amazon_condition`.

   - Per **[!UICONTROL Scope]**, scegli `Global`.

   - Per **[!UICONTROL Unique Value]**, scegli `No`.

   - Per **[!UICONTROL Input Validation for Store Owner]**, scegli `None`.

   - Per **[!UICONTROL Add to Column Options]**, scegli `Yes`.

   - Per **[!UICONTROL Use in Filter Options]**, scegli `Yes`.

1. Clic **[!UICONTROL Save Attribute]**.

![Attributo condizione Amazon](assets/creating-amazon-condition-attribute.png)

![Icona Successivo](assets/btn-next.png) [**Continua ad aggiungere o verificare la chiave API**](./amazon-verify-api-key.md)
