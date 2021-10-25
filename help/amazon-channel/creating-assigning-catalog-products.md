---
title: Creare e assegnare prodotti
description: Amazon Sales Channel fornisce [!UICONTROL New Third Party] per creare e assegnare prodotti catalogo Commerce corrispondenti agli elenchi di Amazon.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Creare e assegnare prodotti

Durante la visualizzazione _[!UICONTROL New Third Party]_è possibile [!DNL Commerce] catalogare i prodotti in un elenco Amazon esistente. Ci sono due opzioni per questa corrispondenza. È possibile assegnare un elenco a un prodotto catalogo esistente oppure utilizzare le informazioni dell’elenco per creare prodotti catalogo. Queste opzioni sono utili quando le inserzioni Amazon non corrispondono automaticamente alle [!DNL Commerce] catalogo.

La corrispondenza (o l&#39;assegnazione) dei prodotti alle inserzioni Amazon è necessaria per utilizzare l&#39;intero set di funzioni del canale di vendita Amazon.

Quando crei un prodotto catalogo da un elenco Amazon:

- La **ASINO** diventa [!DNL Commerce] SKU
- La **Nome elenco prodotti** diventa Nome elenco catalogo
- La **Prezzo** e **Quantità** sono importati dall’elenco Amazon

Il resto delle impostazioni necessarie è determinato dalla [!DNL Commerce] impostazioni di prodotto selezionate durante la creazione.

Quando vengono creati e confrontati, gli elenchi vengono rimossi dal _[!UICONTROL New Third Party]_e vengono visualizzati nella scheda_[!UICONTROL Active]_ scheda .

## Assegnare un singolo prodotto catalogo a un elenco Amazon

1. Visualizza gli elenchi dei prodotti in [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda .

1. Trova l&#39;inserzione che desideri assegnare nell&#39;elenco, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_e fai clic su **[!UICONTROL Assign Catalog Product]**.

   Questa azione apre la _[!UICONTROL Assign Magento Catalog Product]_pagina.

1. Cerca o filtra l’elenco utilizzando [controlli dell&#39;area di lavoro](./workspace-controls.md) e individua il prodotto di catalogo appropriato da associare all’elenco.

1. Quando il prodotto corretto viene visualizzato nell’elenco, fai clic su **[!UICONTROL Assign Catalog Product]** in _[!UICONTROL Action]_colonna.

Il prodotto e l’elenco ora corrispondono. Il canale di vendita Amazon può ora condividere con Amazon i dati relativi a prodotti ed elenchi e gestire la tua inserzione e le relative informazioni, tra cui prezzo di listino, prezzo di spedizione, scorte/quantità, informazioni e stato dell&#39;ordine e altro ancora.

## Creare un singolo prodotto di catalogo utilizzando le informazioni di elenco di Amazon

1. Visualizza gli elenchi dei prodotti in [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda .

1. Trova l&#39;inserzione che desideri creare nel tuo [!DNL Commerce] catalogo, fai clic su **[!UICONTROL Select]** in _[!UICONTROL Action]_e fai clic su **[!UICONTROL Create New Catalog Product]**.

   Questa azione apre la _[!UICONTROL Create Magento Catalog Product]_pagina.

1. Completa le impostazioni del catalogo per il prodotto.

   - Imposta **[!UICONTROL Enable Product(s)]** passa a `Yes` o `No` (obbligatorio).

      |Sì|Scegliere di rendere il prodotto idoneo per la [!DNL Commerce] vendite nei negozi.| |No|Scegliere di rendere il prodotto inidoneo per il [!DNL Commerce] vendite di magazzino.|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fai clic sulla freccia rivolta verso il basso e seleziona una casella di controllo. Fai clic su **[!UICONTROL Done]** una volta finito.

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) per il quale il prodotto deve essere associato.

      Le opzioni di questo elenco dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Impostazioni {target=&quot;_blank&quot;}.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni di questo elenco dipendono dal [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} configurato.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (Impostazione predefinita)|Il prodotto non è incluso negli elenchi della vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.| |**[!UICONTROL Catalog]**|Il prodotto viene visualizzato negli elenchi del catalogo.| |**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.| |**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo e disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dal [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;} configurato.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

Il prodotto catalogo viene creato nel [!DNL Commerce] catalogo e assegnato all’elenco Amazon da cui è stato creato. Con l’elenco ora corrispondente a un elenco Amazon esistente, l’elenco viene rimosso dalla _[!UICONTROL New Third Party]_e vengono visualizzati nella_[!UICONTROL Active]_ scheda .

## Creare più prodotti di catalogo utilizzando le relative informazioni di elenco Amazon

1. Visualizza gli elenchi dei prodotti in [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) scheda .

1. Selezionare gli elenchi per i quali creare prodotti catalogo.

   È possibile selezionare singole caselle di controllo nella colonna a sinistra oppure fare clic sulla freccia rivolta verso il basso nella colonna in alto a sinistra e scegliere **[!UICONTROL Select All]** o **[!UICONTROL Select All on this Page]**.

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create New Catalog Product(s)]**.

1. Per accettare il messaggio di conferma e aprire la _[!UICONTROL Create Magento Catalog Product]_pagina, fai clic su **[!UICONTROL OK]**.

1. Completa le impostazioni del catalogo per i prodotti.

   >[!NOTE]
   >Quando si creano prodotti di catalogo per più elenchi selezionati, le impostazioni di prodotto inserite vengono applicate a tutti gli elenchi.

   - Imposta **[!UICONTROL Enable Product(s)]** passa a `Yes` o `No` (obbligatorio).

      |Sì|Scegliere di rendere il prodotto idoneo per la [!DNL Commerce] vendite nei negozi.| |No|Scegliere di rendere il prodotto inidoneo per il [!DNL Commerce] vendite di magazzino.|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fai clic sulla freccia rivolta verso il basso e seleziona una casella di controllo. Fai clic su **Fine** una volta finito.

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) per il quale il prodotto deve essere associato.

      Le opzioni di questo elenco dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Impostazioni {target=&quot;_blank&quot;}.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni di questo elenco dipendono dal [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} configurato.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (Impostazione predefinita)|Il prodotto non è incluso negli elenchi della vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.| |**[!UICONTROL Catalog]**|Il prodotto viene visualizzato negli elenchi del catalogo.| |**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.| |**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo e disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dal [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;} configurato.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

I prodotti del catalogo vengono creati nel [!DNL Commerce] catalogo e assegnato all’elenco Amazon da cui è stato creato. Con le voci ora corrispondenti al rispettivo elenco Amazon, le inserzioni vengono rimosse dalla sezione [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) e vengono visualizzati nella [_[!UICONTROL Active]_](./active-listings.md) scheda .

![Crea prodotto catalogo Commerce](assets/amazon-magento-catalog-product.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Obbligatorio) Se abilitato, il prodotto è visibile nel [!DNL Commerce] vetrina. Se disabilitato, il prodotto non viene visualizzato nel tuo [!DNL Commerce] vetrina. |
| [!UICONTROL Categories] | Per immettere il nome della categoria del nuovo prodotto o selezionare una categoria, fai clic sulla freccia rivolta verso il basso per visualizzare le opzioni disponibili. Le opzioni dipendono dal [categorie](https://docs.magento.com/user-guide/catalog/category-create.html)Configurazione di {target=&quot;_blank&quot;}. |
| [!UICONTROL Website Ids] | (Obbligatorio) Scegli il sito web (vetrina) per il quale il prodotto da associare. Le opzioni dipendono dal [!DNL Commerce] [configurazione archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Impostazioni {target=&quot;_blank&quot;} |
| ID set di attributi | Scegli un set di attributi. Le opzioni dipendono dalla configurazione [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Visibility] | Opzioni:<ul><li>**[!UICONTROL Not Visible Individually]** - Il prodotto non è visibile nel [!DNL Commerce] vetrina (più comune per i prodotti varianti).</li><li>**[!UICONTROL Catalog]** - Consente l’accesso al prodotto tramite la categoria a cui è associato all’interno del sito web.</li><li>**Ricerca** - Consente di trovare il prodotto solo tramite lo strumento di ricerca.</li><li>**[!UICONTROL Catalog and Search]** - Consente l&#39;accesso ai prodotti tramite la struttura della categoria e lo strumento di ricerca.</li></ul> |
| [!UICONTROL Assign Tax Class] | Assegnare una classe di imposta al nuovo prodotto. Le opzioni dipendono dalla configurazione [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;}. |
