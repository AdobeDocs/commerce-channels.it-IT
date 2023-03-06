---
title: Creare e assegnare prodotti
description: Il Sales Channel Amazon fornisce [!UICONTROL New Third Party] per creare e assegnare i prodotti del catalogo Commerce corrispondenti alle inserzioni di Amazon.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# Creare e assegnare prodotti

Durante la visualizzazione _[!UICONTROL New Third Party]_, è possibile impostare una corrispondenza con [!DNL Commerce] catalogare i prodotti in un elenco Amazon esistente. Sono disponibili due opzioni per questa corrispondenza. È possibile assegnare un&#39;inserzione a un prodotto di catalogo esistente oppure utilizzare le informazioni dell&#39;inserzione per creare prodotti di catalogo. Queste opzioni sono utili quando le inserzioni di Amazon non corrispondono automaticamente al tuo [!DNL Commerce] catalogo.

Per utilizzare tutte le funzioni del canale di vendita Amazon è necessario far corrispondere (o assegnare) i prodotti alle inserzioni Amazon.

Quando crei un prodotto catalogo da un’inserzione Amazon:

- Il **ASIN** diventa [!DNL Commerce] SKU
- Il **Nome elenco prodotti** diventa il nome dell’inserzione nel catalogo
- Il **Prezzo** e **Quantità** vengono importati dall’elenco di Amazon

Le altre impostazioni necessarie vengono determinate dal [!DNL Commerce] impostazioni del prodotto selezionate durante la creazione.

Quando vengono create e associate, le inserzioni vengono rimosse dal _[!UICONTROL New Third Party]_e vengono visualizzati sul_[!UICONTROL Active]_ scheda.

## Assegnare un singolo prodotto catalogo a un’inserzione Amazon

1. Visualizza le tue inserzioni di prodotti su [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda.

1. Individua l’inserzione da assegnare nell’elenco, fai clic su **[!UICONTROL Select]** nel _[!UICONTROL Action]_e fai clic su **[!UICONTROL Assign Catalog Product]**.

   Questa azione apre il _[!UICONTROL Assign Magento Catalog Product]_pagina.

1. Cercare o filtrare l&#39;elenco utilizzando [controlli workspace](./workspace-controls.md) e individua il prodotto di catalogo appropriato da abbinare all’inserzione.

1. Quando il prodotto corretto viene visualizzato nell’elenco, fai clic su **[!UICONTROL Assign Catalog Product]** nel _[!UICONTROL Action]_colonna.

Il prodotto e l’inserzione ora corrispondono. Il canale di vendita Amazon ora può condividere i dati dei prodotti e delle inserzioni con Amazon e gestire le tue inserzioni e le relative informazioni, inclusi il prezzo di vendita, il prezzo di spedizione, le scorte/quantità, le informazioni e lo stato degli ordini e altro ancora.

## Creare un singolo prodotto di catalogo utilizzando le informazioni dell’elenco di Amazon

1. Visualizza le tue inserzioni di prodotti su [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda.

1. Trova l’inserzione che desideri creare nella tua [!DNL Commerce] catalogo, fai clic su **[!UICONTROL Select]** nel _[!UICONTROL Action]_e fai clic su **[!UICONTROL Create New Catalog Product]**.

   Questa azione apre il _[!UICONTROL Create Magento Catalog Product]_pagina.

1. Completa le impostazioni del catalogo per il prodotto.

   - Imposta **[!UICONTROL Enable Product(s)]** passa a `Yes` o `No` (obbligatorio).

      |Sì|Scegliere se rendere il prodotto idoneo per il proprio [!DNL Commerce] vendite in vetrina.| |No|Scegli di rendere il prodotto non idoneo per il tuo [!DNL Commerce] vendite vetrina.|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fare clic sulla freccia rivolta verso il basso e selezionare una casella di controllo della categoria. Clic **[!UICONTROL Done]** al termine.

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) a cui associare il prodotto.

      Le opzioni in questo elenco dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} impostazioni.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dal [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} hai configurato.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (impostazione predefinita)|Il prodotto non è incluso nelle inserzioni in vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.| |**[!UICONTROL Catalog]**|Il prodotto viene visualizzato nelle inserzioni del catalogo.| |**[!UICONTROL Search]**|Il prodotto è disponibile per operazioni di ricerca.| |**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dal [classi fiscali](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} hai configurato.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

Il prodotto del catalogo viene creato nel [!DNL Commerce] e assegnati all’inserzione Amazon da cui è stata creata. Ora che l’elenco corrisponde a un elenco Amazon esistente, l’elenco viene rimosso da _[!UICONTROL New Third Party]_e vengono visualizzati nel_[!UICONTROL Active]_ scheda.

## Creare più prodotti catalogo utilizzando le informazioni dell’elenco Amazon

1. Visualizza le tue inserzioni di prodotti su [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda.

1. Seleziona le inserzioni per le quali creare prodotti catalogo.

   È possibile selezionare singole caselle di controllo nella colonna a sinistra oppure fare clic sulla freccia rivolta verso il basso nella colonna in alto a sinistra e scegliere **[!UICONTROL Select All]** o **[!UICONTROL Select All on this Page]**.

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create New Catalog Product(s)]**.

1. Per accettare il messaggio di conferma e aprire _[!UICONTROL Create Magento Catalog Product]_pagina, fai clic su **[!UICONTROL OK]**.

1. Completa le impostazioni del catalogo per i prodotti.

   >[!NOTE]
   >Quando si creano prodotti catalogo per più inserzioni selezionate, le impostazioni dei prodotti inserite vengono applicate a tutte le inserzioni.

   - Imposta **[!UICONTROL Enable Product(s)]** passa a `Yes` o `No` (obbligatorio).

      |Sì|Scegliere se rendere il prodotto idoneo per il proprio [!DNL Commerce] vendite in vetrina.| |No|Scegli di rendere il prodotto non idoneo per il tuo [!DNL Commerce] vendite vetrina.|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fare clic sulla freccia rivolta verso il basso e selezionare una casella di controllo della categoria. Clic **Fine** al termine.

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) a cui associare il prodotto.

      Le opzioni in questo elenco dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} impostazioni.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dal [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} hai configurato.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (impostazione predefinita)|Il prodotto non è incluso nelle inserzioni in vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.| |**[!UICONTROL Catalog]**|Il prodotto viene visualizzato nelle inserzioni del catalogo.| |**[!UICONTROL Search]**|Il prodotto è disponibile per operazioni di ricerca.| |**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dal [classi fiscali](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} hai configurato.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

I prodotti del catalogo vengono creati nel [!DNL Commerce] e assegnati all’inserzione Amazon da cui è stata creata. Con le inserzioni ora associate alla loro rispettiva inserzione Amazon, le inserzioni vengono rimosse dal [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) e vengono visualizzati nel [_[!UICONTROL Active]_](./active-listings.md) scheda.

![Crea prodotto catalogo Commerce](assets/amazon-magento-catalog-product.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Obbligatorio) Se abilitata, il prodotto è visibile nel [!DNL Commerce] vetrina. Se è disabilitato, il prodotto non viene visualizzato nel [!DNL Commerce] vetrina. |
| [!UICONTROL Categories] | È possibile immettere il nome della categoria per il nuovo prodotto o selezionare una categoria facendo clic sulla freccia rivolta verso il basso per visualizzare le opzioni. Le opzioni dipendono dal [categorie](https://docs.magento.com/user-guide/catalog/category-create.html){target="_blank"} configurazione. |
| [!UICONTROL Website Ids] | (Obbligatorio) Scegli il sito web (vetrina) a cui associare il prodotto. Le opzioni dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} impostazioni |
| ID set di attributi | Scegliere una serie di attributi. Le opzioni dipendono dalla configurazione [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"}. |
| [!UICONTROL Visibility] | Opzioni:<ul><li>**[!UICONTROL Not Visible Individually]** - Il prodotto non è visibile nel [!DNL Commerce] vetrina (più comune per i prodotti varianti).</li><li>**[!UICONTROL Catalog]** - Consente di accedere al prodotto tramite la categoria a cui è associato all&#39;interno del sito Web.</li><li>**Ricerca** - Permette di trovare il prodotto solo tramite lo strumento di ricerca.</li><li>**[!UICONTROL Catalog and Search]** - Consente di accedere ai prodotti tramite la struttura delle categorie e lo strumento di ricerca.</li></ul> |
| [!UICONTROL Assign Tax Class] | Assegnare una classe di imposta al nuovo prodotto. Le opzioni dipendono dalla configurazione [classi fiscali](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"}. |
