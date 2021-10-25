---
title: Regole di elenco
description: Le regole di elenco consentono di determinare i prodotti del catalogo Commerce pubblicati come elenchi di Amazon Marketplace.
redirect_from: /sales-channels/asc/ob-listing-rules.html/sales-channels/asc/ob-listing-preview.html/sales-channels/asc/listing-rule-preview.html
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Regole di elenco

Puoi accedere alle regole di elenco per l’archivio nel [dashboard store](./amazon-store-dashboard.md).

Le regole di elenco definiscono le regole per determinare quali prodotti il canale di vendita Amazon pubblica in Amazon. Queste regole forniscono molte opzioni per creare regole semplici e complesse per includere o escludere i prodotti come elenchi. Ciascuna regola consiste in condizioni che stabiliscono i requisiti per l’idoneità all’elenco dei prodotti.

Le regole dell&#39;elenco vengono continuamente sincronizzate con le [!DNL Commerce] catalogo. Quando si aggiunge un nuovo [!DNL Commerce] i prodotti che soddisfano i requisiti di idoneità stabiliti dalle regole dell’elenco vengono elaborati automaticamente per l’inserimento nell’elenco in Amazon.

- Se desideri che tutti i tuoi prodotti siano pubblicati in un elenco Amazon, non definire alcuna condizione per le regole di elenco.

- Se desideri limitare i prodotti del catalogo pubblicati in Amazon, definisci le condizioni della regola di elenco. La definizione delle condizioni per le regole di elenco di Amazon segue la stessa logica e la stessa procedura utilizzata per definire le condizioni per [Regole del prezzo del carrello](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

- Se le regole di elenco escludono un prodotto, lo stato di idoneità del prodotto cambia in `Ineligible`. I prodotti non consentiti non vengono pubblicati in Amazon.

- Se un prodotto non idoneo è già elencato in Amazon e l’elenco Amazon corrisponde al tuo [!DNL Commerce] prodotto catalogo, la quantità per l’elenco di Amazon cambia in `0` per impedire la vendita del prodotto. Gli elenchi di Amazon possono essere [rimosso manualmente](./end-listings-manually.md).

Le modifiche alla quantità e allo stato di idoneità influiscono su tutte le inserzioni che condividono lo SKU del venditore Amazon nei mercati esistenti per i negozi che vendono nella stessa regione (come definito in _[!UICONTROL Amazon Marketplace Country]_durante [integrazione store](./store-integration.md)). Tuttavia, è stata apportata una modifica a un [!DNL Amazon Seller SKU] in una regione non influisce sugli elenchi Amazon del prodotto in un paese diverso.

![Regole di elenco](assets/ob-listing-rules.png)

## Configurare le impostazioni delle regole di elenco

1. Fai clic su **[!UICONTROL Listing Rules]** sul dashboard dello store.

1. Definisci le condizioni desiderate per l’idoneità dei prodotti da elencare in Amazon.

Vedi [Esempio: Definire una condizione](./ob-define-condition-example.md).

| Campo | Descrizione |
|---|---|
| [!UICONTROL Websites] | Le opzioni disponibili dipendono dal [siti web](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} configurato nel tuo [!DNL Commerce] configurazione. Seleziona il sito web per i prodotti idonei elencati in Amazon. È possibile selezionare un solo sito web, in quanto ogni sito web richiede un negozio Amazon univoco creato nel canale di vendita Amazon. |
| [!UICONTROL Conditions] | Utilizzato per definire le [!DNL Commerce] attributi per l’idoneità dei prodotti nell’area Amazon. Vedi [Esempio: Definire una condizione](./ob-define-condition-example.md). |

## Area di lavoro delle condizioni

È possibile fare clic su qualsiasi area delle condizioni in grassetto per visualizzare le varie opzioni.

- Non aggiungere condizioni se tutti i prodotti all’interno dei siti web selezionati sono idonei.
- Esiste un insieme complesso di processi back-end per comunicare direttamente con i sistemi Amazon. In base al numero di elementi che si sta tentando di elencare e al livello di disponibilità dei sistemi Amazon (ad esempio il Black Friday), potrebbe essere necessario del tempo per elencare gli elementi in Amazon.

Per ulteriori informazioni sulle condizioni, vedi [Descrizione delle condizioni](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

## Anteprima regola di elenco

Quando modifichi le definizioni delle condizioni per le regole di elenco, puoi fare clic su **[!UICONTROL Preview Changes]** per applicare le regole cambia e visualizzare l’impatto degli elenchi. Verifica gli elenchi in questa funzione di anteprima dell&#39;elenco prima di salvare le modifiche alla regola dell&#39;elenco.

Gli elenchi Amazon vengono confrontati con le tue regole e condizioni definite. Puoi quindi rivedere:

- Quali prodotti vengono spostati in uno stato non idoneo in base al tuo attuale [!DNL Amazon Seller Central] account
- Quali prodotti vengono trasferiti da uno stato non idoneo a quello idoneo?
- Quali prodotti sono Nuovi elenchi Amazon e sono stati aggiunti alla tua inserzione Amazon dal tuo idoneo [!DNL Commerce] products

Anteprima nell’elenco ti consente di visualizzare in anteprima i tuoi potenziali elenchi Amazon e di apportare le modifiche necessarie alle regole per gli elenchi.

Gli elenchi Amazon potenziali si popolano sul _[!UICONTROL Listing Preview]_in una delle tre schede:

- **[!UICONTROL Ineligible Listings]** - I prodotti elencati non sono idonei per l’inserimento nell’elenco Amazon in base alle regole e alle condizioni dell’elenco corrente.

   I prodotti non consentiti non vengono pubblicati in Amazon. Se un prodotto non idoneo è già elencato in Amazon e l’elenco Amazon corrisponde al tuo [!DNL Commerce] prodotto catalogo, la quantità per l’elenco di Amazon cambia in `0` per impedire la vendita del prodotto. Per rimuovere manualmente un elenco, vedi [Terminazione di un elenco Amazon](./end-listings-manually.md). I prodotti non idonei ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella [Scheda Inserzioni inattive](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - I prodotti elencati possono essere inseriti nell’elenco di Amazon in base alle regole e alle condizioni dell’elenco corrente e possono essere inclusi anche nei requisiti Amazon. Questo elenco include gli elenchi Amazon esistenti che importano (se sono disponibili **Importa elenchi di terze parti** impostato su `Import Listing` in [Impostazioni elenco](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - I prodotti elencati includono [!DNL Commerce] i prodotti di catalogo che sono appena idonei per l’inserimento nell’elenco di Amazon in base alle regole e alle condizioni dell’elenco corrente e creano e pubblicano nuovi elenchi di Amazon.

### Visualizza anteprima dell&#39;inserzione

1. Fai clic su **[!UICONTROL Listing Rules]** sul dashboard dello store.

1. Visualizza o aggiungi il tuo [regole di elenco](./listing-rules.md).

1. Modifica il [Condizioni della regola di elenco](./ob-define-condition-example.md).

1. Fai clic su **[!UICONTROL Preview Changes]**.

1. Rivedi e conferma le tue inserzioni nel _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ e _[!UICONTROL New Listings]_schede.

1. Se le inserzioni corrispondono alle aspettative, fai clic su **[!UICONTROL Save and close]**.

   Se le inserzioni non vengono visualizzate come previsto, fare clic su **[!UICONTROL Back]** e modifica le regole e le condizioni finché le inserzioni non corrispondono alle tue aspettative.

![Anteprima regola di elenco](assets/amazon-listing-rule-preview.png)

### Elencare record di anteprima

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Product ID] | Il numero univoco sequenziale assegnato a un [!DNL Commerce] prodotto catalogo quando viene aggiunto. |
| [!UICONTROL Thumbnail] | Mostra una miniatura dell’immagine del prodotto principale. |
| [!UICONTROL Name] | Nome del prodotto, gestito nella [!DNL Commerce] [griglia prodotti](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Type] | Il tipo di prodotto, gestito nella [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL Attribute Set] | Il nome del set di attributi utilizzato come modello per il prodotto, gestito nel [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL SKU] | Unità di conservazione delle scorte univoca assegnata al prodotto, gestita nel [!DNL Commerce] griglia dei prodotti. |
| [!UICONTROL Visibility] | Indica dove il prodotto è visibile, gestito nella [!DNL Commerce] griglia dei prodotti. Opzioni:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Stato | Indica lo stato del prodotto, gestito nel [!DNL Commerce] griglia dei prodotti. Opzioni: `Enabled` / `Disabled` |

![Elenco del flusso di lavoro di anteprima](assets/listing-preview-flowchart.png)
