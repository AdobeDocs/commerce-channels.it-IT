---
title: Canale di vendita Amazon - [!UICONTROL Listing Rules]
description: Le regole di utilizzo degli elenchi determinano i prodotti del catalogo Commerce pubblicati come inserzioni di Amazon Marketplace.
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---

# [!UICONTROL Listing Rules]

Puoi accedere alle regole di inserzione per archiviare in [dashboard store](./amazon-store-dashboard.md).

Le regole di elenco definiscono le regole per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici o complesse da includere o escludere prodotti come inserzioni. Ogni regola è costituita da condizioni che impostano i requisiti per l’idoneità all’elenco dei prodotti.

Le regole di inserzione vengono continuamente sincronizzate con [!DNL Commerce] catalogo. Quando aggiungi nuovo [!DNL Commerce] prodotti che soddisfano i requisiti di idoneità impostati dalle regole di inserzione, i prodotti vengono elaborati automaticamente per l’inserzione su Amazon.

- Se desideri che tutti i prodotti vengano pubblicati in un’inserzione Amazon, non definire alcuna condizione per le regole dell’inserzione.

- Se desideri limitare quali dei tuoi prodotti catalogo vengono pubblicati in Amazon, definisci le condizioni della regola dell’inserzione. La definizione delle condizioni per le regole di inserzione di Amazon segue la stessa logica e la stessa procedura della definizione delle condizioni per [Regole prezzo carrello](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

- Se le regole di inserzione escludono un prodotto, lo stato di idoneità per quel prodotto cambia in `Ineligible`. I prodotti non ammissibili non vengono pubblicati in Amazon.

- Se un prodotto non idoneo è già presente nell’elenco di Amazon e l’inserzione di Amazon corrisponde a [!DNL Commerce] prodotto del catalogo, la quantità per l’elenco Amazon diventa `0` per impedire la vendita del prodotto. Le inserzioni Amazon possono essere [rimosso manualmente](./end-listings-manually.md).

Le modifiche alla quantità e allo stato di idoneità influiscono su tutte le inserzioni che condividono lo SKU del venditore Amazon nei mercati esistenti per i negozi che vendono nella stessa area (come definito in _[!UICONTROL Amazon Marketplace Country]_durante [integrazione store](./store-integration.md)). Tuttavia, una modifica a un [!DNL Amazon Seller SKU] in un’area geografica non influisce sulle inserzioni Amazon del prodotto in un altro paese.

![Regole di inserzione](assets/ob-listing-rules.png){width="600" zoomable="yes"}

## Configurare le impostazioni delle regole di elenco

1. Clic **[!UICONTROL Listing Rules]** nel dashboard del negozio.

1. Definisci le condizioni desiderate per l’idoneità dei prodotti a essere elencati in Amazon.

Consulta [Esempio: definire una condizione](./ob-define-condition-example.md).

| Campo | Descrizione |
|---|---|
| [!UICONTROL Websites] | Le opzioni disponibili dipendono dal [siti web](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) che hai configurato nel tuo [!DNL Commerce] configurazione. Seleziona il sito web per i prodotti idonei elencati su Amazon. È possibile selezionare un solo sito web, in quanto ogni sito web richiede un negozio Amazon univoco creato nel canale di vendita Amazon. |
| [!UICONTROL Conditions] | Utilizzato per definire [!DNL Commerce] attributi per l’idoneità del prodotto nell’area geografica Amazon. Consulta [Esempio: definire una condizione](./ob-define-condition-example.md). |

## Area di lavoro Condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

- Non aggiungere condizioni se tutti i prodotti all’interno dei siti web selezionati sono idonei.
- Esiste un set complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che stai tentando di elencare e a quanto potrebbero essere occupati i sistemi di Amazon (ad esempio il Black Friday), potrebbe volerci del tempo perché i tuoi elementi vengano elencati su Amazon.

Per ulteriori informazioni sulle condizioni, consulta [Descrivi le condizioni](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

## Anteprima regola elenco

Quando modifichi le definizioni delle condizioni per le regole di inserzione, puoi fare clic su **[!UICONTROL Preview Changes]** per applicare le modifiche alle regole e visualizzare l&#39;impatto delle inserzioni. Verifica le inserzioni in questa funzione di anteprima prima di salvare le modifiche apportate alla regola per le inserzioni.

Le tue inserzioni in Amazon vengono confrontate con le tue regole e condizioni definite. È quindi possibile esaminare:

- Quali prodotti passano a uno stato non idoneo in base al [!DNL Amazon Seller Central] account
- Quali prodotti tornano allo stato idoneo da uno stato non idoneo
- Quali sono i nuovi prodotti Amazon e quali sono stati aggiunti all’inserzione su Amazon dal tuo sito idoneo [!DNL Commerce] products

Anteprima inserzione ti consente di visualizzare in anteprima le tue inserzioni potenziali in Amazon e di apportare le modifiche necessarie alle regole di inserzione.

Le tue inserzioni potenziali su Amazon si popolano su _[!UICONTROL Listing Preview]_pagina in una delle tre schede seguenti:

- **[!UICONTROL Ineligible Listings]** - I prodotti elencati non sono idonei per l’inserzione in Amazon in base alle regole e condizioni correnti.

   I prodotti non ammissibili non vengono pubblicati in Amazon. Se un prodotto non idoneo è già presente nell’elenco di Amazon e l’inserzione di Amazon corrisponde a [!DNL Commerce] prodotto del catalogo, la quantità per l’elenco Amazon diventa `0` per impedire la vendita del prodotto. Per rimuovere manualmente un’inserzione, consulta [Chiusura di un’inserzione di Amazon](./end-listings-manually.md). I prodotti che non sono idonei in base ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella [Scheda per le inserzioni inattive](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - I prodotti elencati sono idonei per l’inserzione in Amazon in base alle regole e condizioni correnti dell’inserzione e sono inoltre idonei in base ai requisiti Amazon. Questo elenco include le tue inserzioni esistenti di Amazon che importano (se hai **Importa elenchi di terze parti** imposta su `Import Listing` in [Impostazioni elenco](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - I prodotti elencati includono [!DNL Commerce] cataloga i prodotti che sono appena idonei per l’inserzione in Amazon in base alle regole e condizioni correnti e crea e pubblica nuove inserzioni in Amazon.

### Visualizza l&#39;anteprima dell&#39;inserzione

1. Clic **[!UICONTROL Listing Rules]** nel dashboard del negozio.

1. Visualizza o aggiungi [regole di inserzione](./listing-rules.md).

1. Modificare il [Condizioni delle regole di elenco](./ob-define-condition-example.md).

1. Clic **[!UICONTROL Preview Changes]**.

1. Controlla e conferma le inserzioni nella sezione _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_, e _[!UICONTROL New Listings]_schede.

1. Se le tue inserzioni corrispondono alle tue aspettative, fai clic su **[!UICONTROL Save and close]**.

   Se le tue inserzioni non vengono visualizzate come previsto, fai clic su **[!UICONTROL Back]** e modifica le regole e le condizioni fino a quando le inserzioni non corrispondono alle tue aspettative.

![Anteprima regola elenco](assets/amazon-listing-rule-preview.png){width="600" zoomable="yes"}

### Elenco dei record di anteprima

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Product ID] | Numero sequenziale univoco assegnato a un [!DNL Commerce] al momento dell’aggiunta del prodotto al catalogo. |
| [!UICONTROL Thumbnail] | Mostra una miniatura dell&#39;immagine principale del prodotto. |
| [!UICONTROL Name] | Il nome del prodotto, gestito nel [!DNL Commerce] [griglia prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html). |
| [!UICONTROL Type] | Il tipo di prodotto, gestito in [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL Attribute Set] | Nome del set di attributi utilizzato come modello per il prodotto, gestito in [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL SKU] | L&#39;unità di stoccaggio univoca assegnata al prodotto, gestita nel [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL Visibility] | Indica dove è visibile il prodotto, gestito nel [!DNL Commerce] griglia dei prodotti. Opzioni:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Stato | Indica lo stato del prodotto, gestito nel [!DNL Commerce] griglia dei prodotti. Opzioni: `Enabled` / `Disabled` |

![Flusso di lavoro di anteprima elenco](assets/listing-preview-flowchart.png){width="500" zoomable="yes"}
