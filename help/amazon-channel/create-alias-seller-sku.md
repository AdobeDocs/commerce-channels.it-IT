---
title: Creare una SKU del venditore di alias Amazon
description: Puoi utilizzare lo SKU del venditore di alias Amazon per creare elenchi Amazon multiregionali dai tuoi prodotti di catalogo Commerce.
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Creare una SKU del venditore di alias Amazon

Un [!DNL Alias Amazon Seller SKU] viene utilizzato per creare un elenco Amazon dallo stesso prodotto nel tuo [!DNL Commerce] catalogo. Se sei un venditore esperto di Amazon, potresti avere familiarità con il [SKU globale di Amazon](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target=&quot;_blank&quot;} e SKU specifico per Marketplace per inventario e spedizione. Seguendo principi simili per il canale di vendita Amazon, lo SKU del venditore di Amazon controlla le informazioni sull’elenco dei prodotti a livello multi-regionale e il [!DNL Alias Amazon Seller SKU] può essere utilizzato per controllare le informazioni sull’elenco dei prodotti a un livello specifico per l’area.

Questa funzione può essere utilizzata per eseguire due funzioni:

- Crea un [!DNL Alias Amazon Seller SKU] per uno dei [!DNL Commerce] catalogare i prodotti per controllare le informazioni di elenco specifiche per regione.

   **Esempio**: Sei un venditore sia negli Stati Uniti che in Canada. Ricorda che a ciascuno dei tuoi rivenditori di canali di vendita Amazon può essere assegnata una sola area geografica Amazon durante la configurazione. Quindi, hai un negozio di canali di vendita Amazon con una regione definita degli Stati Uniti e un altro negozio con una regione definita del Canada. Entrambi i negozi condividono la tua [!DNL Commerce] catalogo per l’inserimento di informazioni in entrambe le aree, inclusi gli attributi di prodotto SKU (Stock Keeping Unit) e ASIN di Amazon. Quindi, le inserzioni per il prodotto di catalogo sarebbero le stesse in entrambi i negozi, condividendo prezzi, stock/quantità e altri attributi di prodotto. Ma, le vostre scorte per il vostro Canada immagazzinano le navi da una posizione Canada, e il vostro negozio Stati Uniti spediscono da una posizione degli Stati Uniti. Pertanto, è necessario controllare la quantità di inserzione separatamente per ogni negozio. Per eseguire questo tipo di controllo specifico per l&#39;area geografica, è possibile creare uno SKU del venditore di Alias Amazon.

   In sostanza, puoi creare uno SKU Venditore alias Amazon collegato allo stesso prodotto catalogo e può essere utilizzato per ripubblicare lo stesso elenco in tale area.

- Crea un [!DNL Alias Amazon Seller SKU] e fai corrispondere uno dei tuoi [!DNL Commerce] catalogare i prodotti in due elenchi Amazon.

   **Esempio**: Hai un prodotto catalogo che corrisponde a un elenco Amazon. Poiché Amazon dispone spesso di più elenchi che rappresentano lo stesso prodotto, puoi scoprire un altro elenco Amazon per lo stesso prodotto, ma Amazon ha assegnato un diverso ASIN all’elenco. Per aumentare la visibilità del prodotto da includere, è necessario associare il prodotto catalogo ai diversi valori ASIN e creare elenchi per entrambi i valori ASIN. A questo scopo, puoi creare uno SKU del venditore di alias Amazon.

   In sostanza, puoi creare un [!DNL Alias Amazon Seller SKU] che può essere utilizzato per associare un singolo prodotto di catalogo a un secondo elenco Amazon e per creare un elenco per il nuovo ASIN corrispondente. In questo scenario, si potrebbero avere due elenchi Amazon per lo stesso prodotto catalogo.

   Dopo aver creato uno SKU del venditore di Alias Amazon, puoi utilizzare le impostazioni, le regole e le sostituzioni dell&#39;inserzione per controllare le informazioni dell&#39;inserzione per la regione. Gli attributi di prodotto che possono essere definiti per regione per un elenco includono quantità/scorte, metodo di evasione, condizione, idoneità del prodotto e tempo di gestione.

## Utilizzato per uno scopo specifico della regione {#region-specific}

Visualizza l&#39;elenco _[!UICONTROL Product Listings]_page (_[!UICONTROL Inactive]_, _Attivo_, _Non applicabile_ oppure _Terminato_ ).

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create Alias Seller SKU]**.

1. Per **[!UICONTROL Assign New Seller SKU]**, immetti un valore alfanumerico univoco.

   Questo valore deve essere univoco (non utilizzato per nessun altro prodotto o alias nel catalogo).

1. Per **[!UICONTROL Assign New ASIN]**, non apportare modifiche.

   Questo valore viene compilato automaticamente con l’ASIN del prodotto corrispondente al prodotto del catalogo. La modifica di questo valore corrisponde al prodotto di catalogo in due elenchi Amazon basati su ASIN.

1. Attiva/disattiva la **[!UICONTROL Remove Existing Seller SKU]** se necessario.

   - `Yes` - Scegliere di eliminare l&#39;elenco e creare un elenco utilizzando le nuove informazioni fornite.

   - `No` - Scegliere di creare un elenco e mantenere il vecchio elenco invariato.

1. Fai clic su **[!UICONTROL Save Listing Update]**.

## Utilizzato per associare un singolo prodotto di catalogo a due elenchi Amazon

1. Visualizza l&#39;elenco _[!UICONTROL Product Listings]_page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ oppure _[!UICONTROL Ended]_schede).

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create Alias Seller SKU]**.

1. Per **[!UICONTROL Assign New Seller SKU]**, immetti un valore alfanumerico univoco.

   Questo valore deve essere univoco (non utilizzato per nessun altro prodotto o alias nel catalogo).

1. Per **[!UICONTROL Assign New ASIN]**, immetti un valore alfanumerico univoco.

   Questo valore viene compilato automaticamente con l’ASIN del prodotto corrispondente al prodotto del catalogo. La modifica di questo valore corrisponde al prodotto di catalogo in due elenchi Amazon basati su ASIN.

1. Attiva/disattiva la **[!UICONTROL Remove Existing Seller SKU]** se necessario.

   - `Yes` - Scegliere di eliminare l&#39;elenco e creare un elenco utilizzando le nuove informazioni fornite.

   - `No` - Scegliere di creare un altro elenco e mantenere il vecchio elenco invariato.

1. Fai clic su **[!UICONTROL Save Listing Update]**.

![creare un codice SKU del venditore di alias Amazon](assets/amazon-alias-sku-create.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Assign New Seller SKU] | Immetti un nuovo valore alfanumerico univoco da collegare alla SKU originale del venditore Amazon. Questo numero viene utilizzato solo dal canale di vendita Amazon per abbinare al prodotto di catalogo. Puoi utilizzare qualsiasi valore SKU, ma il valore può essere utilizzato solo una volta nel catalogo. |
| [!UICONTROL Assign New ASIN] | Immettere il valore ASIN per l&#39;elenco a cui si desidera associare il prodotto catalogo. Modifica questo campo solo quando si abbina un singolo prodotto di catalogo all’ASIN per un altro elenco per lo stesso prodotto. Questo valore deve corrispondere all’ASIN assegnato da Amazon, altrimenti l’elenco non verrà rifiutato da Amazon. |
| [!UICONTROL Remove Existing Seller SKU] | Opzioni:<ul><li>**[!UICONTROL Yes]** - Scegliere di eliminare l&#39;elenco e creare un elenco utilizzando le nuove informazioni fornite. Il nuovo elenco viene visualizzato nel _[!UICONTROL Active]_e la vecchia inserzione si sposta_ Terminato _scheda .</li><li>**[!UICONTROL No]** - Scegliere di creare un altro elenco e mantenere il vecchio elenco invariato. Entrambi gli elenchi vengono visualizzati nella scheda Attivo dopo la creazione del nuovo elenco.</li></ul> |
