---
title: Canale di vendita Amazon - [!UICONTROL Listing Rules]
description: Le regole di utilizzo determinano i prodotti del catalogo Commerce pubblicati come inserzioni Amazon Marketplace.
feature: Sales Channels, Products
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# [!UICONTROL Listing Rules]

È possibile accedere alle regole di elenco per l&#39;archivio nel [dashboard archivio](./amazon-store-dashboard.md).

Le regole di elenco definiscono le regole per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici o complesse da includere o escludere prodotti come inserzioni. Ogni regola è costituita da condizioni che impostano i requisiti per l’idoneità all’elenco dei prodotti.

Le regole di inserzione vengono continuamente sincronizzate con il catalogo [!DNL Commerce]. Quando si aggiungono nuovi prodotti [!DNL Commerce] che soddisfano i requisiti di idoneità impostati dalle regole di inserzione, i prodotti vengono elaborati automaticamente per l&#39;inserimento in Amazon.

- Se desideri che tutti i prodotti vengano pubblicati in un’inserzione Amazon, non definire alcuna condizione per le regole dell’inserzione.

- Se desideri limitare quali dei tuoi prodotti catalogo vengono pubblicati in Amazon, definisci le condizioni della regola dell’inserzione. La definizione delle condizioni per le regole di inserzione di Amazon segue la stessa logica e la stessa procedura della definizione delle condizioni per le [regole di prezzo del carrello](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

- Se le regole di inserzione escludono un prodotto, lo stato di idoneità per quel prodotto cambia in `Ineligible`. I prodotti non ammissibili non vengono pubblicati in Amazon.

- Se un prodotto non idoneo è già presente nell&#39;elenco di Amazon e si abbina l&#39;elenco di Amazon al prodotto di catalogo [!DNL Commerce], la quantità dell&#39;elenco di Amazon viene modificata in `0` per impedire le vendite del prodotto. Le inserzioni Amazon possono essere [rimosse manualmente](./end-listings-manually.md).

Le modifiche alla quantità e allo stato di idoneità influiscono su tutte le inserzioni che condividono lo SKU del venditore Amazon nei marketplace esistenti per i negozi che vendono nella stessa area (come definito in _[!UICONTROL Amazon Marketplace Country]_durante l&#39;[integrazione dello store](./store-integration.md)). Tuttavia, una modifica a un [!DNL Amazon Seller SKU] condiviso in una regione non influisce sulle inserzioni Amazon del prodotto in un altro paese.

![Regole di elenco](assets/ob-listing-rules.png){width="600" zoomable="yes"}

## Configurare le impostazioni delle regole di elenco

1. Fare clic su **[!UICONTROL Listing Rules]** nel dashboard dell&#39;archivio.

1. Definisci le condizioni desiderate per l’idoneità dei prodotti a essere elencati in Amazon.

Vedi [Esempio: definire una condizione](./ob-define-condition-example.md).

| Campo | Descrizione |
|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Websites] | Le opzioni disponibili dipendono dai [siti Web](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) configurati nella configurazione di [!DNL Commerce]. Seleziona il sito web per i prodotti idonei elencati su Amazon. È possibile selezionare un solo sito web, in quanto ogni sito web richiede un negozio Amazon univoco creato nel canale di vendita Amazon. |
| [!UICONTROL Conditions] | Utilizzato per definire gli attributi [!DNL Commerce] per l&#39;idoneità del prodotto nell&#39;area geografica Amazon. Vedi [Esempio: definire una condizione](./ob-define-condition-example.md). |

## Area di lavoro Condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

- Non aggiungere condizioni se tutti i prodotti all’interno dei siti web selezionati sono idonei.
- Esiste un set complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che stai tentando di elencare e a quanto potrebbero essere occupati i sistemi di Amazon (ad esempio il Black Friday), potrebbe volerci del tempo perché i tuoi elementi vengano elencati su Amazon.

Per ulteriori informazioni sulle condizioni, vedere [Descrivere le condizioni](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html).

## Anteprima regola elenco

Quando modifichi le definizioni delle condizioni per le regole di inserzione, puoi fare clic su **[!UICONTROL Preview Changes]** per applicare le modifiche alle regole e visualizzare l&#39;impatto delle inserzioni. Verifica le inserzioni in questa funzione di anteprima prima di salvare le modifiche apportate alla regola per le inserzioni.

Le tue inserzioni in Amazon vengono confrontate con le tue regole e condizioni definite. È quindi possibile esaminare:

- Quali prodotti passano a uno stato non idoneo in base all&#39;account [!DNL Amazon Seller Central] corrente
- Quali prodotti tornano allo stato idoneo da uno stato non idoneo
- Quali sono i nuovi prodotti Amazon e quali sono aggiunti all&#39;inserzione Amazon dai tuoi [!DNL Commerce] prodotti idonei?

Anteprima inserzione ti consente di visualizzare in anteprima le tue inserzioni potenziali in Amazon e di apportare le modifiche necessarie alle regole di inserzione.

Le tue inserzioni potenziali in Amazon vengono inserite nella pagina _[!UICONTROL Listing Preview]_in una delle tre schede seguenti:

- **[!UICONTROL Ineligible Listings]** - I prodotti elencati non sono idonei per l&#39;inserzione in Amazon in base alle regole e alle condizioni correnti.

  I prodotti non ammissibili non vengono pubblicati in Amazon. Se un prodotto non idoneo è già presente nell&#39;elenco di Amazon e si abbina l&#39;elenco di Amazon al prodotto di catalogo [!DNL Commerce], la quantità dell&#39;elenco di Amazon viene modificata in `0` per impedire le vendite del prodotto. Per rimuovere manualmente un&#39;inserzione, vedi [Terminazione di un&#39;inserzione Amazon](./end-listings-manually.md). I prodotti che non sono idonei in base ai requisiti Amazon non sono elencati qui. Questi prodotti sono elencati nella [scheda Inserzioni inattive](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - I prodotti elencati sono idonei per l&#39;inserzione in Amazon in base alle regole e alle condizioni correnti e sono idonei anche in base ai requisiti Amazon. Questo elenco include le tue inserzioni Amazon esistenti che importano (se hai **Importa inserzioni di terze parti** impostato su `Import Listing` nelle [Impostazioni inserzioni](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - I prodotti elencati includono i prodotti del catalogo [!DNL Commerce] che sono appena idonei per l&#39;inserzione in Amazon in base alle regole e alle condizioni correnti e creano e pubblicano nuove inserzioni in Amazon.

### Visualizza l&#39;anteprima dell&#39;inserzione

1. Fare clic su **[!UICONTROL Listing Rules]** nel dashboard dell&#39;archivio.

1. Visualizza o aggiungi le [regole di inserzione](./listing-rules.md).

1. Modifica le [condizioni delle regole di elenco](./ob-define-condition-example.md).

1. Fare clic su **[!UICONTROL Preview Changes]**.

1. Rivedi e conferma le inserzioni nelle schede _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ e _[!UICONTROL New Listings]_.

1. Se le tue inserzioni corrispondono alle tue aspettative, fai clic su **[!UICONTROL Save and close]**.

   Se le tue inserzioni non vengono visualizzate come previsto, fai clic su **[!UICONTROL Back]** e modifica le regole e le condizioni fino a quando le inserzioni non corrispondono alle tue aspettative.

![Anteprima regola elenco](assets/amazon-listing-rule-preview.png){width="600" zoomable="yes"}

### Elenco dei record di anteprima

| Campo | Descrizione |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product ID] | Numero sequenziale univoco assegnato a un prodotto catalogo [!DNL Commerce] quando viene aggiunto. |
| [!UICONTROL Thumbnail] | Mostra una miniatura dell&#39;immagine principale del prodotto. |
| [!UICONTROL Name] | Il nome del prodotto, gestito nella [!DNL Commerce] [griglia prodotti](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html). |
| [!UICONTROL Type] | Tipo di prodotto, gestito nella griglia prodotti [!DNL Commerce]. |
| [!UICONTROL Attribute Set] | Nome del set di attributi utilizzato come modello per il prodotto, gestito nella griglia prodotti [!DNL Commerce]. |
| [!UICONTROL SKU] | L&#39;unità di gestione scorte univoca assegnata al prodotto, gestita nella griglia prodotti [!DNL Commerce]. |
| [!UICONTROL Visibility] | Indica dove è visibile il prodotto, gestito nella griglia prodotti [!DNL Commerce]. Opzioni:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Stato | Indica lo stato del prodotto, gestito nella griglia prodotti [!DNL Commerce]. Opzioni: `Enabled` / `Disabled` |

![Anteprima dell&#39;elenco del flusso di lavoro](assets/listing-preview-flowchart.png){width="500" zoomable="yes"}
