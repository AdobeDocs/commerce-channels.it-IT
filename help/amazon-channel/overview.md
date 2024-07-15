---
title: "Introduzione a  [!DNL Amazon Sales Channel]"
description: "[!DNL Amazon Sales Channel] consente ai commercianti di vendere senza problemi i prodotti in  [!DNL Amazon Marketplace]."
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Introduzione a [!DNL Amazon Sales Channel]

In qualità di commerciante Adobe Commerce o di Magento Open Source, puoi utilizzare l&#39;estensione [!DNL Amazon Sales Channel] per integrare i tuoi negozi con la destinazione globale più grande del mondo per gli acquisti su Internet. Questa estensione consente alle vendite Amazon connettendo [!DNL Commerce] con il tuo account [!DNL Amazon Seller Central] e fornendo sia l&#39;automazione che la sincronizzazione dei dati di catalogo e ordine. Gestisci completamente tutte le inserzioni Amazon, implementa regole di prezzo semplici o intelligenti e gestisci gli ordini e le scorte tramite un unico dashboard [!DNL Commerce].

Dopo [l&#39;onboarding](./amazon-onboarding-home.md), [!DNL Commerce] diventa un &quot;centro di comando centrale&quot; per la gestione e il controllo delle inserzioni, degli ordini e dell&#39;inventario di Amazon e dei prezzi del tuo archivio Amazon. L&#39;[integrazione store](./store-integration.md) collega l&#39;istanza [!DNL Commerce] e Amazon per sincronizzare i dati tra entrambe le piattaforme. Il canale di vendita Amazon consente di:

- [Onboarding](./amazon-onboarding-home.md) e integrazione di uno o più account [!DNL Amazon Seller Central] con Adobe Commerce o Magento Open Source.

- Importa e sincronizza gli elenchi Amazon esistenti e abbina i prodotti nel tuo catalogo [!DNL Commerce], creando un catalogo di prodotti centralizzato.

- Crea e gestisci le inserzioni Amazon per i prodotti nel tuo catalogo [!DNL Commerce].

- Visualizza ed evade gli ordini (di spedizione) in [!DNL Commerce] e Amazon, sincronizzando le informazioni sullo stato degli ordini, sul pagamento e sul rimborso.

- Visualizza i registri per analisi ed errori per [prezzi competitivi](./competitive-price-analysis.md), [modifiche alle inserzioni](./listing-changes-log.md) e [problemi di comunicazione](./communication-errors-log.md).

Accedi ai tuoi negozi Amazon per visualizzare e gestire tutte queste funzioni, informazioni sull&#39;account, inserzioni, ordini e altro ancora sul canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## Promozioni e prezzi

Con l&#39;estensione [!DNL Amazon Sales Channel], è possibile:

- Sincronizzare i prezzi dell&#39;inserzione Amazon con il prezzo di catalogo [!DNL Commerce] (o un attributo di prezzo alternativo).

- Abilita [prezzi barrato](./listing-price.md#configure-listing-price-settings) MSRP nelle tue inserzioni Amazon per aumentare la proposta di valore per il cliente.

- Abilita e gestisci il [prezzo minimo annunciato (MAP)](./listing-price.md#configure-listing-price-settings) nelle tue inserzioni Amazon.

- Configura ulteriori [IVA](./listing-price.md#configure-listing-price-settings) nel prezzo Amazon.

- Imposta un valore personalizzato per la &quot;quantità disponibile&quot; nelle [impostazioni per le scorte/quantità](./stock-quantity.md#configure-stock--quantity-settings) da mostrare con le inserzioni Amazon per aumentare l&#39;urgenza dell&#39;acquirente.

## Regole di determinazione prezzi

Con l&#39;estensione [!DNL Amazon Sales Channel], è possibile:

- Crea [regole di prezzo](./pricing-products.md) impilabili, flessibili e complesse per gestire i prezzi Amazon per le vendite quotidiane o le promozioni stagionali.

- Crea i prezzi [floor](./floor-price.md) e [ceiling](./optional-ceiling-price.md) per proteggere i prezzi più bassi e più alti.

- Crea e gestisci [regole di rideterminazione prezzi intelligenti](./intelligent-repricing-rules.md) che adeguano automaticamente i prezzi dei tuoi prodotti rispetto agli altri concorrenti di Amazon ([concorrente più basso](./lowest-competitor-pricing.md) e [Buy Box](./buy-box-competitor-pricing.md) prezzo).

## Gestione feed catalogo

Con l&#39;estensione [!DNL Amazon Sales Channel], è possibile:

- Importa le inserzioni (prodotti) Amazon esistenti e abbina i prodotti esistenti o crea prodotti nel catalogo [!DNL Commerce].

- Publish i tuoi prodotti [!DNL Commerce] in Amazon per creare inserzioni Amazon.

- Crea [sostituzioni](./creating-editing-overrides.md) per impostare un singolo prezzo, il tempo di imballaggio, la condizione e il messaggio relativo alle note del venditore.

- Importa e mappa gli [attributi](./attributes-view.md) del prodotto dalle tue inserzioni Amazon in modo che corrispondano automaticamente ai prodotti nel catalogo [!DNL Commerce].

- Imposta più parametri di ricerca per far corrispondere le inserzioni Amazon al tuo catalogo [!DNL Commerce].

- Definisci le [regole di inserzione](./listing-rules.md) per determinare quali dei tuoi prodotti [!DNL Commerce] possono essere inseriti in Amazon.

- Imposta un [tempo di gestione](./product-listing-actions.md) predefinito per le nuove inserzioni Amazon.

- Abbina le condizioni dell&#39;elenco in base a un attributo [!DNL Commerce].

- Aggiungi note del venditore per ogni tipo di condizione (facoltativo).

- Implementa le soglie di quantità durante l&#39;importazione di inserzioni Amazon nel catalogo [!DNL Commerce].

- Visualizza i [miglioramenti consigliati all&#39;elenco](./listing-improvements.md).

## Gestione degli ordini e servizio clienti

Con l&#39;estensione [!DNL Amazon Sales Channel], è possibile:

- Supporto ed elaborazione degli ordini in Amazon e [!DNL Commerce].

- [Importa](./order-settings.md#configure-order-settings) i tuoi ordini Amazon in [!DNL Commerce] o lasciali in Amazon.

- Definisci quali store del tuo sito Web [!DNL Commerce] associare agli ordini di Amazon per l&#39;importazione e la gestione degli ordini.

- Visualizza, annulla e spedisci ordini da [!DNL Commerce] e/o Amazon a seconda delle [impostazioni di evasione](./fulfilled-by.md).

- Mappare lo stato dell&#39;ordine Amazon allo stato personalizzato entro [!DNL Commerce] (facoltativo).

- Visualizza e gestisci gli errori degli ordini per risolvere i problemi e connettersi con i clienti.

- Invia i dati di tracciamento degli ordini al tuo account [!DNL Amazon Seller Central].

- [Annulla ordini](./cancel-unshipped-order.md) e seleziona una risposta del motivo.

- Visualizza le informazioni sull&#39;[ordine recente](./amazon-store-dashboard.md) per gli ordini Amazon.

## Generazione rapporti

Con l&#39;estensione [!DNL Amazon Sales Channel], puoi rivedere le informazioni del rapporto su:

- Elenchi per stato di attivi, inattivi, idonei e incompleti.

- Ordini in attesa di spedizione.

- Ordini più recenti.

- Amazon [registro delle modifiche alle inserzioni](./listing-changes-log.md) per esaminare le modifiche ai feed di prodotti/inserzioni (come prezzo e quantità).

- Dati sui prezzi del concorrente per il prodotto [Buy Box](./buy-box-competitor-pricing.md).

- Prodotto [Dati relativi ai prezzi più bassi per i concorrenti](./lowest-competitor-pricing.md).

## Supporto per le vendite globali

Con l&#39;estensione [!DNL Amazon Sales Channel], è possibile:

- Gestisci più aree geografiche (paesi) di [!DNL Amazon Marketplace].

- Supporta più valute utilizzando lo strumento di configurazione della valuta [Commerce](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html).

- Gestire le spedizioni dalle sedi dei prodotti e dai centri di evasione Amazon.

## Gestione clienti

Crea il tuo database clienti di [!DNL Commerce] [importando i dati dei clienti](./order-settings.md#configure-order-settings) associati ai tuoi ordini Amazon. Aumenta il tuo potenziale di marketing attraverso questo elenco esteso di clienti attraverso le tue [!DNL Amazon Marketplace] inserzioni e [!DNL Commerce] vetrina.


Iniziare è facile. Un breve processo di onboarding ti guida nella creazione di un account [!DNL Amazon Seller Central] e nell&#39;integrazione con il tuo store dei canali di vendita Amazon e il tuo catalogo [!DNL Commerce] per gestire le inserzioni, gli ordini, l&#39;inventario e l&#39;evasione di Amazon. Una dashboard centrale mostra gli aggiornamenti di stato per tutte le integrazioni dei punti vendita del canale di vendita Amazon e le inserzioni Amazon. Raggiungi nuovi clienti nel [!DNL Amazon Marketplace] globale con processi semplificati e automatizzati, il tutto a un costo minimo o nullo rispetto alla configurazione di un nuovo sistema.

Dopo aver integrato l&#39;account [!DNL Amazon Seller Central], l&#39;estensione [!DNL Amazon Sales Channel] consente di gestire gli account e sincronizzare i dati tra [!DNL Commerce] e Amazon. Consente di creare inserzioni, gestire promozioni, impostare i prezzi e gestire l&#39;inventario e l&#39;evasione direttamente tramite l&#39;amministratore [!DNL Commerce]. Queste opzioni includono regole di determinazione dei prezzi che monitorano i prezzi di Amazon per lo stesso articolo e adeguano automaticamente i prezzi per renderli più competitivi.

