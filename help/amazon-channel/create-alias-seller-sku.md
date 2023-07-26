---
title: Crea un alias SKU del venditore Amazon
description: Puoi utilizzare lo SKU Alias Amazon Seller per creare inserzioni Amazon con più impostazioni internazionali dai prodotti del catalogo Commerce.
feature: Sales Channels, Products
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Crea un alias SKU del venditore Amazon

Un [!DNL Alias Amazon Seller SKU] viene utilizzato per creare un’inserzione di Amazon dallo stesso prodotto nel tuo [!DNL Commerce] catalogo. Se sei un venditore Amazon esperto, potresti avere familiarità con [SKU globale di Amazon](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"} e SKU specifiche per il marketplace per l&#39;inventario e la spedizione. Seguendo principi simili per il canale di vendita Amazon, lo SKU del venditore Amazon controlla le informazioni sull’elenco dei prodotti a livello multiregionale e il [!DNL Alias Amazon Seller SKU] può essere utilizzato per controllare le informazioni dell’elenco di prodotti a un livello specifico dell’area geografica.

Questa funzione può essere utilizzata per eseguire due funzioni:

- Creare un [!DNL Alias Amazon Seller SKU] per uno dei [!DNL Commerce] catalogare i prodotti per controllare le informazioni di elenco specifiche per l&#39;area.

  **Esempio**: sei un venditore sia negli Stati Uniti che in Canada. Ricorda che a ciascuno dei tuoi negozi dei canali di vendita Amazon può essere assegnata una sola area Amazon durante la configurazione. Pertanto, disponi di un negozio del canale di vendita Amazon con una regione statunitense definita e di un altro negozio con una regione canadese definita. Entrambi i negozi condividono [!DNL Commerce] catalogo per elencare informazioni in entrambe le aree geografiche, inclusi gli attributi di prodotto Amazon Seller SKU e ASIN. Pertanto, le inserzioni per il prodotto del catalogo saranno le stesse in entrambi i punti vendita, condividendo i prezzi, le scorte/quantità e altri attributi di prodotto. Ma, il tuo stock per il tuo negozio Canada navi da una posizione Canada, e il tuo negozio Stati Uniti navi da una posizione Stati Uniti. Pertanto, è necessario controllare la quantità dell&#39;inserzione separatamente per ogni negozio. Per eseguire questo tipo di controllo specifico per l’area geografica, puoi creare uno SKU del venditore Amazon di alias.

  In sostanza, puoi creare uno SKU del venditore Amazon di alias collegato allo stesso prodotto di catalogo e utilizzabile per ripubblicare la stessa inserzione in quell’area geografica.

- Creare un [!DNL Alias Amazon Seller SKU] e corrisponde a uno dei [!DNL Commerce] cataloga i prodotti in due inserzioni Amazon.

  **Esempio**: hai un prodotto catalogo che corrisponde a un’inserzione Amazon. Poiché Amazon ha spesso più inserzioni che rappresentano lo stesso prodotto, puoi scoprire un’altra inserzione Amazon per lo stesso prodotto, ma Amazon ha assegnato un codice ASIN diverso. Per aumentare la visibilità dei prodotti da includere, vuoi far corrispondere il prodotto del catalogo con i diversi valori ASIN e creare inserzioni per entrambi i valori ASIN. A questo scopo, puoi creare uno SKU del venditore Amazon per gli alias.

  In sostanza, puoi creare un’ [!DNL Alias Amazon Seller SKU] che può essere utilizzato per associare un singolo prodotto di catalogo a una seconda inserzione Amazon e per creare un’inserzione per il codice ASIN appena corrispondente. In questo caso, avrai a disposizione due inserzioni Amazon per lo stesso prodotto catalogo.

  Dopo aver creato uno SKU di Amazon Seller per alias, puoi utilizzare le impostazioni, le regole e le sostituzioni dell&#39;inserzione per controllare le informazioni dell&#39;inserzione per l&#39;area. Gli attributi del prodotto che possono essere definiti per area per un elenco includono quantità/scorte, metodo di evasione, condizione, idoneità del prodotto e tempo di gestione.

## Utilizzato per uno scopo specifico dell’area geografica {#region-specific}

Visualizza l’inserzione su _[!UICONTROL Product Listings]_page (_[!UICONTROL Inactive]_, _Attivo_, _Non ammissibile_, o _Terminato_ ).

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create Alias Seller SKU]**.

1. Per **[!UICONTROL Assign New Seller SKU]**, inserisci un valore alfanumerico univoco.

   Questo valore deve essere univoco (non deve essere utilizzato per altri prodotti o alias nel catalogo).

1. Per **[!UICONTROL Assign New ASIN]**, non apportare alcuna modifica.

   Questo valore viene compilato automaticamente con il codice ASIN del prodotto corrispondente al prodotto del catalogo. La modifica di questo valore corrisponde al prodotto del catalogo in due elenchi Amazon basati sul codice ASIN.

1. Attiva/disattiva **[!UICONTROL Remove Existing Seller SKU]** in base alle esigenze.

   - `Yes` - Scegli di eliminare l’inserzione e di crearne una nuova utilizzando le nuove informazioni fornite.

   - `No` - Scegli di creare un&#39;inserzione e mantenere invariata la precedente.

1. Clic **[!UICONTROL Save Listing Update]**.

## Utilizzato per associare un singolo prodotto catalogo a due inserzioni Amazon

1. Visualizza l’inserzione su _[!UICONTROL Product Listings]_page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_, o _[!UICONTROL Ended]_schede).

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create Alias Seller SKU]**.

1. Per **[!UICONTROL Assign New Seller SKU]**, inserisci un valore alfanumerico univoco.

   Questo valore deve essere univoco (non deve essere utilizzato per altri prodotti o alias nel catalogo).

1. Per **[!UICONTROL Assign New ASIN]**, inserisci un valore alfanumerico univoco.

   Questo valore viene compilato automaticamente con il codice ASIN del prodotto corrispondente al prodotto del catalogo. La modifica di questo valore corrisponde al prodotto del catalogo in due elenchi Amazon basati sul codice ASIN.

1. Attiva/disattiva **[!UICONTROL Remove Existing Seller SKU]** in base alle esigenze.

   - `Yes` - Scegli di eliminare l’inserzione e di crearne una nuova utilizzando le nuove informazioni fornite.

   - `No` - Scegli di creare un&#39;altra inserzione e mantenere invariata la precedente.

1. Clic **[!UICONTROL Save Listing Update]**.

![crea un alias Amazon Seller SKU](assets/amazon-alias-sku-create.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Assign New Seller SKU] | Inserisci un nuovo valore alfanumerico univoco da collegare allo SKU originale del venditore di Amazon. Questo numero viene utilizzato solo dal canale di vendita Amazon per corrispondere al prodotto del catalogo. Puoi utilizzare qualsiasi valore SKU, ma il valore può essere utilizzato solo una volta nel catalogo. |
| [!UICONTROL Assign New ASIN] | Immettere il valore ASIN per l&#39;inserzione alla quale si desidera associare il prodotto del catalogo. Modifica questo campo solo quando si abbina un singolo prodotto catalogo all’ASIN per un’altra inserzione dello stesso prodotto. Questo valore deve corrispondere al codice ASIN assegnato da Amazon, altrimenti l’inserzione non verrà rifiutata da Amazon. |
| [!UICONTROL Remove Existing Seller SKU] | Opzioni:<ul><li>**[!UICONTROL Yes]** - Scegli di eliminare l’inserzione e di crearne una nuova utilizzando le nuove informazioni fornite. La nuova inserzione viene visualizzata nel _[!UICONTROL Active]_e la vecchia inserzione si sposta sul_ Terminato _scheda.</li><li>**[!UICONTROL No]** - Scegli di creare un&#39;altra inserzione e mantenere invariata la precedente. Entrambe le voci vengono visualizzate nella scheda Attivo dopo la creazione della nuova voce.</li></ul> |
