---
title: Creare e assegnare prodotti
description: Amazon Sales Channel fornisce la scheda [!UICONTROL New Third Party] per aiutare a creare e assegnare prodotti di catalogo Commerce corrispondenti agli elenchi di Amazon.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Creare e assegnare prodotti

Quando visualizzi la scheda _[!UICONTROL New Third Party]_, puoi associare i prodotti del catalogo [!DNL Commerce] a un elenco Amazon esistente. Ci sono due opzioni per questa corrispondenza. È possibile assegnare un elenco a un prodotto catalogo esistente oppure utilizzare le informazioni dell’elenco per creare prodotti catalogo. Queste opzioni sono utili quando gli elenchi Amazon non corrispondono automaticamente al catalogo [!DNL Commerce].

La corrispondenza (o l&#39;assegnazione) dei prodotti alle inserzioni Amazon è necessaria per utilizzare l&#39;intero set di funzioni del canale di vendita Amazon.

Quando crei un prodotto catalogo da un elenco Amazon:

- La **ASIN** diventa la SKU [!DNL Commerce]
- Il **nome dell&#39;elenco dei prodotti** diventa il nome dell&#39;elenco dei cataloghi
- Le **Prezzo** e **Quantità** vengono importate dall&#39;elenco Amazon

Le altre impostazioni necessarie sono determinate dalle [!DNL Commerce] impostazioni di prodotto selezionate durante la creazione.

Una volta create e confrontate, le inserzioni vengono rimosse dalla scheda _[!UICONTROL New Third Party]_e visualizzate nella scheda_[!UICONTROL Active]_.

## Assegnare un singolo prodotto catalogo a un elenco Amazon

1. Visualizza gli elenchi dei prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Trova l&#39;elenco da assegnare, fai clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e fai clic su **[!UICONTROL Assign Catalog Product]**.

   Questa azione apre la pagina _[!UICONTROL Assign Magento Catalog Product]_.

1. Cerca o filtra l&#39;elenco utilizzando i [controlli dell&#39;area di lavoro](./workspace-controls.md) e individua il prodotto di catalogo appropriato da associare all&#39;elenco.

1. Quando il prodotto corretto viene visualizzato nell’elenco, fare clic su **[!UICONTROL Assign Catalog Product]** nella colonna _[!UICONTROL Action]_.

Il prodotto e l’elenco ora corrispondono. Il canale di vendita Amazon può ora condividere con Amazon i dati relativi a prodotti ed elenchi e gestire la tua inserzione e le relative informazioni, tra cui prezzo di listino, prezzo di spedizione, scorte/quantità, informazioni e stato dell&#39;ordine e altro ancora.

## Creare un singolo prodotto di catalogo utilizzando le informazioni di elenco di Amazon

1. Visualizza gli elenchi dei prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Trova l&#39;elenco da creare nel catalogo [!DNL Commerce], fai clic su **[!UICONTROL Select]** nella colonna _[!UICONTROL Action]_e fai clic su **[!UICONTROL Create New Catalog Product]**.

   Questa azione apre la pagina _[!UICONTROL Create Magento Catalog Product]_.

1. Completa le impostazioni del catalogo per il prodotto.

   - Imposta l&#39;opzione **[!UICONTROL Enable Product(s)]** su `Yes` o `No` (obbligatorio).

      |Sì|Scegliere di rendere il prodotto idoneo per le vendite di vetrina [!DNL Commerce].|
|No|Scegliere di rendere il prodotto inidoneo per le vendite di vetrina [!DNL Commerce].|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fai clic sulla freccia rivolta verso il basso e seleziona una casella di controllo. Al termine, fai clic su **[!UICONTROL Done]** .

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) per il quale deve essere associato il prodotto.

      Le opzioni in questo elenco dipendono dalle impostazioni [!DNL Commerce] [Store configuration](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dai [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} configurati.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (predefinito)|Il prodotto non è incluso negli elenchi della vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.|
|**[!UICONTROL Catalog]**|Il prodotto viene visualizzato negli elenchi dei cataloghi.|
|**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.|
|**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dalle [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;} configurate.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

Il prodotto catalogo viene creato nel catalogo [!DNL Commerce] e assegnato all’elenco Amazon da cui è stato creato. Con l’elenco ora corrispondente a un elenco Amazon esistente, l’elenco viene rimosso dalla scheda _[!UICONTROL New Third Party]_e viene visualizzato nella scheda_[!UICONTROL Active]_ .

## Creare più prodotti di catalogo utilizzando le relative informazioni di elenco Amazon

1. Visualizza gli elenchi dei prodotti nella scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) .

1. Selezionare gli elenchi per i quali creare prodotti catalogo.

   È possibile selezionare singole caselle di controllo nella colonna a sinistra oppure fare clic sulla freccia rivolta verso il basso nella colonna in alto a sinistra e scegliere **[!UICONTROL Select All]** o **[!UICONTROL Select All on this Page]**.

1. In _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Create New Catalog Product(s)]**.

1. Per accettare il messaggio di conferma e aprire la pagina _[!UICONTROL Create Magento Catalog Product]_, fai clic su **[!UICONTROL OK]**.

1. Completa le impostazioni del catalogo per i prodotti.

   >[!NOTE]
   >Quando si creano prodotti di catalogo per più elenchi selezionati, le impostazioni di prodotto inserite vengono applicate a tutti gli elenchi.

   - Imposta l&#39;opzione **[!UICONTROL Enable Product(s)]** su `Yes` o `No` (obbligatorio).

      |Sì|Scegliere di rendere il prodotto idoneo per le vendite di vetrina [!DNL Commerce].|
|No|Scegliere di rendere il prodotto inidoneo per le vendite di vetrina [!DNL Commerce].|

   - Per **[!UICONTROL Categories]**, assegna una categoria per il prodotto (facoltativo).

      Per selezionare la categoria del prodotto, fai clic sulla freccia rivolta verso il basso e seleziona una casella di controllo. Al termine, fai clic su **Fine**.

   - Per **[!UICONTROL Website Ids]**, scegli il sito web (vetrina) per il quale deve essere associato il prodotto.

      Le opzioni in questo elenco dipendono dalle impostazioni [!DNL Commerce] [Store configuration](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}.

   - Per **[!UICONTROL Attribute Set Id]** (obbligatorio), scegli un’opzione.

      `Default` è la selezione predefinita. Le opzioni in questo elenco dipendono dai [!DNL Commerce] [set di attributi](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;} configurati.

   - Per **[!UICONTROL Visibility]**, scegli un’opzione per il nuovo prodotto.

      |**[!UICONTROL Not Visible Individually]** (predefinito)|Il prodotto non è incluso negli elenchi della vetrina, anche se potrebbe essere disponibile come variante di un altro prodotto.|
|**[!UICONTROL Catalog]**|Il prodotto viene visualizzato negli elenchi dei cataloghi.|
|**[!UICONTROL Search]**|Il prodotto è disponibile per le operazioni di ricerca.|
|**[!UICONTROL Catalog and Search]**|Il prodotto è incluso negli elenchi di catalogo ed è disponibile per le operazioni di ricerca.|

   - Per **[!UICONTROL Assign Tax Class]**, scegli un’opzione per il prodotto.

      Le opzioni visualizzate in questo elenco dipendono dalle [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;} configurate.

   - Al termine, fai clic su **[!UICONTROL Create Catalog Products]**.

I prodotti del catalogo vengono creati nel catalogo [!DNL Commerce] e assegnati all’elenco Amazon da cui sono stati creati. Ora che gli elenchi corrispondono al rispettivo elenco Amazon, gli elenchi vengono rimossi dalla scheda [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) e vengono visualizzati nella scheda [_[!UICONTROL Active]_](./active-listings.md) .

![Crea prodotto catalogo Commerce](assets/amazon-magento-catalog-product.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Obbligatorio) Se abilitato, il prodotto è visibile nella vetrina [!DNL Commerce] . Se disabilitata, il prodotto non viene visualizzato nella vetrina [!DNL Commerce]. |
| [!UICONTROL Categories] | Per immettere il nome della categoria del nuovo prodotto o selezionare una categoria, fai clic sulla freccia rivolta verso il basso per visualizzare le opzioni disponibili. Le opzioni dipendono dalla configurazione [categories](https://docs.magento.com/user-guide/catalog/category-create.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Website Ids] | (Obbligatorio) Scegli il sito web (vetrina) per il quale il prodotto da associare. Le opzioni dipendono dalle impostazioni di [!DNL Commerce] [configurazione dell&#39;archivio](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} |
| ID set di attributi | Scegli un set di attributi. Le opzioni dipendono dai set di attributi [!DNL Commerce] [configurati](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Visibility] | Opzioni:<ul><li>**[!UICONTROL Not Visible Individually]** - Il prodotto non è visibile nella  [!DNL Commerce] vetrina (più comune per i prodotti varianti).</li><li>**[!UICONTROL Catalog]** - Consente l’accesso al prodotto tramite la categoria a cui è associato all’interno del sito web.</li><li>**Ricerca**  - Consente di trovare il prodotto solo tramite lo strumento di ricerca.</li><li>**[!UICONTROL Catalog and Search]** - Consente l&#39;accesso ai prodotti tramite la struttura della categoria e lo strumento di ricerca.</li></ul> |
| [!UICONTROL Assign Tax Class] | Assegnare una classe di imposta al nuovo prodotto. Le opzioni dipendono dalle [classi di imposta](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;} configurate. |
