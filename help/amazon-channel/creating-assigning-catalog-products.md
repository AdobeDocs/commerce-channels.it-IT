---
title: Creazione e assegnazione di prodotti per il canale di vendita Amazon
description: Il Sales Channel Amazon fornisce la scheda [!UICONTROL New Third Party] per facilitare la creazione e l'assegnazione di prodotti del catalogo Commerce corrispondenti agli elenchi Amazon.
feature: Sales Channels, Products, Configuration
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Creare e assegnare prodotti

Quando visualizzi la scheda _[!UICONTROL New Third Party]_, puoi far corrispondere i prodotti del catalogo [!DNL Commerce] con un&#39;inserzione Amazon esistente. Sono disponibili due opzioni per questa corrispondenza. È possibile assegnare un&#39;inserzione a un prodotto di catalogo esistente oppure utilizzare le informazioni dell&#39;inserzione per creare prodotti di catalogo. Queste opzioni sono utili quando le inserzioni Amazon non corrispondono automaticamente al catalogo [!DNL Commerce].

Per utilizzare tutte le funzioni del canale di vendita Amazon è necessario far corrispondere (o assegnare) i prodotti alle inserzioni Amazon.

Quando crei un prodotto catalogo da un’inserzione Amazon:

- Il **ASIN** diventa lo SKU [!DNL Commerce]
- Il **nome elenco prodotti** diventa il nome elenco catalogo
- Il **prezzo** e la **quantità** sono importati dall&#39;elenco di Amazon

Le altre impostazioni necessarie sono determinate dalle impostazioni di prodotto [!DNL Commerce] selezionate durante la creazione.

Quando vengono create e associate, le inserzioni vengono rimosse dalla scheda _[!UICONTROL New Third Party]_e vengono visualizzate nella scheda_[!UICONTROL Active]_.

## Assegnare un singolo prodotto catalogo a un’inserzione Amazon

1. Visualizza gli elenchi di prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Trovare l&#39;inserzione che si desidera assegnare nell&#39;elenco, fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e quindi su **[!UICONTROL Assign Catalog Product]**.

   Questa azione apre la pagina _[!UICONTROL Assign Magento Catalog Product]_.

1. Cercare o filtrare l&#39;elenco utilizzando i [controlli area di lavoro](./workspace-controls.md) e individuare il prodotto catalogo appropriato per la corrispondenza con l&#39;elenco.

1. Quando il prodotto corretto viene visualizzato nell&#39;elenco, fare clic su **[!UICONTROL Assign Catalog Product]** nella colonna _[!UICONTROL Action]_.

Il prodotto e l’inserzione ora corrispondono. Il canale di vendita Amazon ora può condividere i dati dei prodotti e delle inserzioni con Amazon e gestire le tue inserzioni e le relative informazioni, inclusi il prezzo di vendita, il prezzo di spedizione, le scorte/quantità, le informazioni e lo stato degli ordini e altro ancora.

## Creare un singolo prodotto di catalogo utilizzando le informazioni dell’elenco di Amazon

1. Visualizza gli elenchi di prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Trovare l&#39;inserzione che si desidera creare nel catalogo [!DNL Commerce], fare clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e quindi su **[!UICONTROL Create New Catalog Product]**.

   Questa azione apre la pagina _[!UICONTROL Create Magento Catalog Product]_.

1. Completa le impostazioni del catalogo per il prodotto.

   - Imposta **[!UICONTROL Enable Product(s)]** su `Yes` o `No` (obbligatorio).

     |Sì|Scegliere di rendere il prodotto idoneo per le vendite [!DNL Commerce] in vetrina.|
|No|Scegliere di rendere il prodotto non idoneo per le vendite in vetrina [!DNL Commerce].|

   - Per **[!UICONTROL Categories]**, assegnare una categoria per il prodotto (facoltativo).

     Per selezionare la categoria del prodotto, fare clic sulla freccia rivolta verso il basso e selezionare una casella di controllo della categoria. Al termine, fare clic su **[!UICONTROL Done]**.

   - Per **[!UICONTROL Website Ids]**, scegli il sito Web (vetrina) a cui associare il prodotto.

     Le opzioni in questo elenco dipendono dalle impostazioni della [!DNL Commerce] [configurazione archivio](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html).

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegliere un&#39;opzione.

     `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dai [!DNL Commerce] [set di attributi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) configurati.

   - Per **[!UICONTROL Visibility]**, scegli un&#39;opzione per il nuovo prodotto.

     |**[!UICONTROL Not Visible Individually]** (impostazione predefinita)|Il prodotto non è incluso nelle inserzioni in vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.|
|**[!UICONTROL Catalog]**|Il prodotto viene visualizzato nelle inserzioni del catalogo.|
|**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.|
|**[!UICONTROL Catalog and Search]**|Il prodotto è incluso nelle inserzioni del catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un&#39;opzione per il prodotto.

     Le opzioni visualizzate in questo elenco dipendono dalle [classi fiscali](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) configurate.

   - Al termine, fare clic su **[!UICONTROL Create Catalog Products]**.

Il prodotto del catalogo viene creato nel catalogo [!DNL Commerce] e assegnato all&#39;elenco Amazon da cui è stato creato. Quando l&#39;inserzione corrisponde a un&#39;inserzione Amazon esistente, viene rimossa dalla scheda _[!UICONTROL New Third Party]_e viene visualizzata nella scheda_[!UICONTROL Active]_.

## Creare più prodotti catalogo utilizzando le informazioni dell’elenco Amazon

1. Visualizza gli elenchi di prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md).

1. Seleziona le inserzioni per le quali creare prodotti catalogo.

   È possibile selezionare singole caselle di controllo nella colonna a sinistra oppure fare clic sulla freccia rivolta verso il basso nella colonna in alto a sinistra e scegliere **[!UICONTROL Select All]** o **[!UICONTROL Select All on this Page]**.

1. In _[!UICONTROL Actions]_, fare clic su **[!UICONTROL Create New Catalog Product(s)]**.

1. Per accettare il messaggio di conferma e aprire la pagina _[!UICONTROL Create Magento Catalog Product]_, scegliere **[!UICONTROL OK]**.

1. Completa le impostazioni del catalogo per i prodotti.

   >[!NOTE]
   >Quando si creano prodotti catalogo per più inserzioni selezionate, le impostazioni dei prodotti inserite vengono applicate a tutte le inserzioni.

   - Imposta **[!UICONTROL Enable Product(s)]** su `Yes` o `No` (obbligatorio).

     |Sì|Scegliere di rendere il prodotto idoneo per le vendite [!DNL Commerce] in vetrina.|
|No|Scegliere di rendere il prodotto non idoneo per le vendite in vetrina [!DNL Commerce].|

   - Per **[!UICONTROL Categories]**, assegnare una categoria per il prodotto (facoltativo).

     Per selezionare la categoria del prodotto, fare clic sulla freccia rivolta verso il basso e selezionare una casella di controllo della categoria. Al termine, fai clic su **Fine**.

   - Per **[!UICONTROL Website Ids]**, scegli il sito Web (vetrina) a cui associare il prodotto.

     Le opzioni in questo elenco dipendono dalle impostazioni della [!DNL Commerce] [configurazione archivio](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html).

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegliere un&#39;opzione.

     `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dai [!DNL Commerce] [set di attributi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) configurati.

   - Per **[!UICONTROL Visibility]**, scegli un&#39;opzione per il nuovo prodotto.

     |**[!UICONTROL Not Visible Individually]** (impostazione predefinita)|Il prodotto non è incluso nelle inserzioni in vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.|
|**[!UICONTROL Catalog]**|Il prodotto viene visualizzato nelle inserzioni del catalogo.|
|**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.|
|**[!UICONTROL Catalog and Search]**|Il prodotto è incluso nelle inserzioni del catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un&#39;opzione per il prodotto.

     Le opzioni visualizzate in questo elenco dipendono dalle [classi fiscali](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) configurate.

   - Al termine, fare clic su **[!UICONTROL Create Catalog Products]**.

I prodotti del catalogo vengono creati nel catalogo [!DNL Commerce] e assegnati all&#39;elenco Amazon da cui sono stati creati. Con le inserzioni ora associate alla rispettiva inserzione Amazon, le inserzioni vengono rimosse dalla scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) e vengono visualizzate nella scheda [_[!UICONTROL Active]_](./active-listings.md).

![Crea prodotto catalogo Commerce](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Product(s)] | (Obbligatorio) Se abilitato, il prodotto è visibile nella vetrina [!DNL Commerce]. Se disabilitato, il prodotto non viene visualizzato nella vetrina [!DNL Commerce]. |
| [!UICONTROL Categories] | È possibile immettere il nome della categoria per il nuovo prodotto o selezionare una categoria facendo clic sulla freccia rivolta verso il basso per visualizzare le opzioni. Le opzioni dipendono dalla configurazione di [categorie](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html). |
| [!UICONTROL Website Ids] | (Obbligatorio) Scegli il sito web (vetrina) a cui associare il prodotto. Le opzioni dipendono dalle impostazioni della [!DNL Commerce] [configurazione archivio](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) |
| ID set di attributi | Scegliere una serie di attributi. Le opzioni dipendono dai [!DNL Commerce] [set di attributi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) configurati. |
| [!UICONTROL Visibility] | Opzioni:<ul><li>**[!UICONTROL Not Visible Individually]** - Il prodotto non è visibile nella tua vetrina [!DNL Commerce] (più comune per i prodotti varianti).</li><li>**[!UICONTROL Catalog]** - Consente di accedere al prodotto tramite la categoria a cui è associato all&#39;interno del sito Web.</li><li>**Ricerca** - Consente di trovare il prodotto solo tramite lo strumento di ricerca.</li><li>**[!UICONTROL Catalog and Search]** - Consente l&#39;accesso ai prodotti tramite la struttura delle categorie e lo strumento di ricerca.</li></ul> |
| [!UICONTROL Assign Tax Class] | Assegnare una classe di imposta al nuovo prodotto. Le opzioni dipendono dalle [classi fiscali](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) configurate. |
