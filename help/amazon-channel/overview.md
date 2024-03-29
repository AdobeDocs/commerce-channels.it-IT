---
title: "Introduzione a [!DNL Amazon Sales Channel]"
description: "[!DNL Amazon Sales Channel] consente ai commercianti di vendere direttamente i prodotti nel [!DNL Amazon Marketplace]."
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# Introduzione a [!DNL Amazon Sales Channel]

In qualità di venditore Adobe Commerce o di Magento Open Source, puoi utilizzare [!DNL Amazon Sales Channel] estensione per integrare i tuoi negozi con la più grande destinazione globale del mondo per gli acquisti su internet. Questa estensione abilita le vendite di Amazon tramite la connessione [!DNL Commerce] con il [!DNL Amazon Seller Central] e fornendo sia l&#39;automazione che la sincronizzazione dei dati di catalogo e ordine. Gestisci completamente tutte le inserzioni Amazon, implementa regole di prezzo semplici o intelligenti e gestisci gli ordini e l&#39;inventario tramite un unico [!DNL Commerce] dashboard.

Dopo [onboarding](./amazon-onboarding-home.md), [!DNL Commerce] diventa un &quot;centro di comando centrale&quot; per la gestione e il controllo delle inserzioni, degli ordini e dell&#39;inventario di Amazon e dei prezzi del tuo Amazon Store. [Integrazione store](./store-integration.md) connette il tuo [!DNL Commerce] e Amazon per sincronizzare i dati tra entrambe le piattaforme. Il canale di vendita Amazon consente di:

- [Onboarding](./amazon-onboarding-home.md) e integrarne uno o più [!DNL Amazon Seller Central] account con Adobe Commerce o Magento Open Source.

- Importa e sincronizza le inserzioni esistenti di Amazon e abbina i tuoi prodotti con quelli del tuo [!DNL Commerce] , creando un catalogo di prodotti centralizzato.

- Crea e gestisci gli elenchi di Amazon per i prodotti nel tuo [!DNL Commerce] catalogo.

- Visualizza ed evade ordini (spedizione) in [!DNL Commerce] e Amazon, sincronizzando le informazioni sullo stato degli ordini, sui pagamenti e sui rimborsi.

- Visualizza registri per analisi ed errori per [prezzi competitivi](./competitive-price-analysis.md), [modifiche elenco](./listing-changes-log.md), e [problemi di comunicazione](./communication-errors-log.md).

Accedi ai tuoi negozi Amazon per visualizzare e gestire tutte queste funzioni, informazioni sull’account, inserzioni, ordini e altro ancora sul canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## Promozioni e prezzi

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi:

- Sincronizza i prezzi delle inserzioni Amazon con [!DNL Commerce] prezzo di catalogo (o attributo di prezzo alternativo).

- Abilita MSRP [prezzo barrato](./listing-price.md#configure-listing-price-settings) nelle inserzioni Amazon per aumentare la proposta di valore per il cliente.

- Attiva e gestisci [Prezzo minimo annunciato (MAP)](./listing-price.md#configure-listing-price-settings) nelle inserzioni di Amazon.

- Configurare ulteriori [Imposta IVA](./listing-price.md#configure-listing-price-settings) nel prezzo di Amazon.

- Imposta un valore personalizzato per &quot;quantità disponibile&quot; nel tuo [impostazioni scorte/quantità](./stock-quantity.md#configure-stock--quantity-settings) da mostrare con le tue inserzioni Amazon per aumentare l&#39;urgenza dell&#39;acquirente.

## Regole di determinazione prezzi

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi:

- Creare file impilabili, flessibili e complessi [regole di determinazione prezzi](./pricing-products.md) per gestire i prezzi di Amazon per le vendite giornaliere o le promozioni stagionali.

- Crea [piano](./floor-price.md) e [soffitto](./optional-ceiling-price.md) per proteggere i prezzi più bassi e più alti.

- Creare e gestire [regole di rideterminazione intelligente dei prezzi](./intelligent-repricing-rules.md) che adeguano automaticamente i prezzi dei prodotti rispetto ad altri concorrenti di Amazon ([concorrente più basso](./lowest-competitor-pricing.md) e [Buy Box](./buy-box-competitor-pricing.md) prezzo).

## Gestione feed catalogo

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi:

- Importa le inserzioni (prodotti) Amazon esistenti e abbina i prodotti esistenti o creali nel tuo [!DNL Commerce] catalogo.

- Pubblicare [!DNL Commerce] Amazon per creare inserzioni in Amazon.

- Crea [sostituzioni](./creating-editing-overrides.md) per impostare un singolo prezzo, il tempo di imballaggio, la condizione e il messaggio note del venditore.

- Importare e mappare il prodotto [attributi](./attributes-view.md) dalle tue inserzioni Amazon per abbinarle automaticamente ai prodotti presenti nel tuo [!DNL Commerce] catalogo.

- Imposta più parametri di ricerca per far corrispondere le inserzioni Amazon al tuo [!DNL Commerce] catalogo.

- Definisci [regole di inserzione](./listing-rules.md) per determinare quale [!DNL Commerce] I prodotti possono essere elencati in Amazon.

- Imposta un valore predefinito [tempo di imballaggio](./product-listing-actions.md) per le nuove inserzioni in Amazon.

- Abbina condizioni di elenco in base a una [!DNL Commerce] attributo.

- Aggiungi note del venditore per ogni tipo di condizione (facoltativo).

- Implementa le soglie di quantità quando importi le inserzioni Amazon nel tuo [!DNL Commerce] catalogo.

- Visualizza consigliato [miglioramenti alle inserzioni](./listing-improvements.md).

## Gestione degli ordini e servizio clienti

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi:

- Supporto ed elaborazione degli ordini in Amazon e [!DNL Commerce].

- [Importa](./order-settings.md#configure-order-settings) ordini Amazon in [!DNL Commerce] o lasciali in Amazon.

- Definisci quale [!DNL Commerce] store di siti Web da associare agli ordini di Amazon per l&#39;importazione e la gestione degli ordini.

- Visualizza, annulla e spedisci ordini da [!DNL Commerce] e/o Amazon a seconda del [impostazioni di esecuzione](./fulfilled-by.md).

- Mappa il tuo stato dell’ordine di Amazon sullo stato personalizzato in [!DNL Commerce] (facoltativo).

- Visualizza e gestisci gli errori degli ordini per risolvere i problemi e connettersi con i clienti.

- Invia i dati di tracciamento degli ordini al tuo [!DNL Amazon Seller Central] account.

- [Annulla ordini](./cancel-unshipped-order.md) e seleziona una risposta al motivo.

- Visualizza [ordine recente](./amazon-store-dashboard.md) informazioni per gli ordini Amazon.

## Generazione rapporti

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi rivedere le informazioni del rapporto relative a:

- Elenchi per stato di attivi, inattivi, idonei e incompleti.

- Ordini in attesa di spedizione.

- Ordini più recenti.

- Amazon [registro delle modifiche delle inserzioni](./listing-changes-log.md) per esaminare le modifiche apportate ai feed di prodotti/elenchi (ad esempio prezzo e quantità).

- Prodotto [Buy Box](./buy-box-competitor-pricing.md) Dati sui prezzi dei concorrenti.

- Prodotto [Prezzi più bassi per i concorrenti](./lowest-competitor-pricing.md) dati.

## Supporto per le vendite globali

Con il [!DNL Amazon Sales Channel] dell&#39;estensione, puoi:

- Gestire più [!DNL Amazon Marketplace] regioni (paesi).

- Supporto di più valute tramite [Strumento di configurazione della valuta Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html).

- Gestire le spedizioni dalle sedi dei prodotti e dai centri di evasione Amazon.

## Gestione clienti

Crea il tuo [!DNL Commerce] database clienti di [importazione dei dati dei clienti](./order-settings.md#configure-order-settings) associato agli ordini di Amazon. Espandi il tuo potenziale di marketing con questo elenco esteso di clienti attraverso [!DNL Amazon Marketplace] inserzioni e [!DNL Commerce] vetrina.


Iniziare è facile. Un breve processo di onboarding ti guida nella creazione di un [!DNL Amazon Seller Central] e l&#39;integrazione con il tuo Amazon sales channel store e il tuo [!DNL Commerce] catalogo per gestire le inserzioni, gli ordini, le scorte e l&#39;evasione di Amazon. Una dashboard centrale mostra gli aggiornamenti di stato per tutte le integrazioni dei punti vendita del canale di vendita Amazon e le inserzioni Amazon. Raggiungi nuovi clienti nel mondo [!DNL Amazon Marketplace] con processi semplificati e automatizzati, il tutto a un costo minimo o nullo rispetto alla creazione di un nuovo sistema.

Dopo aver integrato [!DNL Amazon Seller Central] account, il [!DNL Amazon Sales Channel] consente di gestire gli account e sincronizzare i dati tra [!DNL Commerce] e Amazon. Consente di creare inserzioni, gestire promozioni, impostare i prezzi e gestire l&#39;inventario e la consegna direttamente tramite [!DNL Commerce] Amministratore Queste opzioni includono regole di determinazione dei prezzi che monitorano i prezzi di Amazon per lo stesso articolo e adeguano automaticamente i prezzi per renderli più competitivi.

