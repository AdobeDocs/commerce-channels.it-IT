---
title: Impostazioni ordine
description: Utilizza le impostazioni Ordine per determinare in che modo gli ordini Amazon vengono importati ed elaborati nel tuo negozio Commerce.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Impostazioni ordine

Le impostazioni dell’ordine definiscono se e come gli ordini di Amazon vengono importati ed elaborati in [!DNL Commerce] e sono accessibili sul [dashboard store](./amazon-store-dashboard.md).

Le impostazioni di importazione dell’ordine sono impostate su `Enabled` per impostazione predefinita, gli ordini Amazon vengono visualizzati sul dashboard dello store e creati corrispondenti [!DNL Commerce] ordini. Gli ordini importati possono essere gestiti nel [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html)Flusso di lavoro {target=&quot;_blank&quot;}.

>[!NOTE]
>
>Indipendentemente dalle impostazioni dell’ordine, gli ordini Amazon esistenti prima dell’integrazione dell’archivio non vengono importati.

Dopo [integrazione store](./store-integration.md) è completo, è possibile modificare le impostazioni dell&#39;ordine. Se imposti le impostazioni dell&#39;ordine su `Disabled`, gli ordini di Amazon vengono visualizzati sul dashboard dello store ma devono essere gestiti nel [!DNL Amazon Seller Central] conto.

Quando un ordine viene creato su Amazon, non viene importato immediatamente in [!DNL Commerce]. Amazon assegna un `Pending` stato degli ordini appena creati. Dopo che Amazon verifica il metodo dell&#39;ordine e del pagamento, lo stato dell&#39;ordine viene modificato in `Unshipped`. Questa modifica dello stato attiva l’importazione dell’ordine e [!DNL Commerce] crea un ordine corrispondente.

Gli ordini importati da Amazon possono essere gestiti nel [!DNL Commerce] [flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}. Vedi anche [Gestisci ordini](./managing-orders.md).

## Configurare le impostazioni dell’ordine {#configure-order-settings}

1. Fai clic su **[!UICONTROL Order Settings]** sul dashboard dello store.

1. Per **[!UICONTROL Import Amazon Orders]** (obbligatorio), scegli un’opzione:

   - `Disabled` - Scegliere quando non si desidera creare ordini corrispondenti in [!DNL Commerce] quando vengono ricevuti nuovi ordini da Amazon. Se selezionato, tutti gli altri campi della pagina vengono disabilitati.

   - `Enabled` - (Predefinito) Scegli quando vuoi creare il corrispondente [!DNL Commerce] ordini quando nuovi ordini vengono ricevuti da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato di Amazon e ai livelli di stock.

      >[!NOTE]
      >
      >Importa ordini Amazon deve essere impostato su `Enabled` per gestire gli ordini Amazon in [!DNL Commerce] [ordini](https://docs.magento.com/user-guide/sales/orders.html)Flusso di lavoro {target=&quot;_blank&quot;}. Quando è impostato su `Disabled`, gli ordini Amazon non hanno un [!DNL Commerce] numero d&#39;ordine e non può essere gestito in [!DNL Commerce]. Gestisci questi ordini nel tuo [!DNL Amazon Seller Central] conto.

1. Per **[!UICONTROL Import Amazon Orders Into Magento Store]**, scegli quale [!DNL Commerce] archivia gli ordini di Amazon a cui sono associati quando viene creato l’ordine corrispondente in [!DNL Commerce].

   Per impostazione predefinita, questa impostazione consente di visualizzare il sito Web selezionato come Store View quando [aggiunto l’archivio Amazon](./store-integration.md). Se desideri modificare questa impostazione, l’elenco delle opzioni dipende dalla [!DNL Commerce] archivi configurati nella configurazione. Vedi [Negozi](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target=&quot;_blank&quot;}.

1. Per **[!UICONTROL Customer Creation]**, scegli un’opzione:

   - `No Customer Creation (guest)` - (Impostazione predefinita) Scegli se non desideri creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall’ordine Amazon. Se scelto, [!DNL Commerce] elabora un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest [!DNL Commerce].

   - `Build New Customer Account` - Scegli quando creare un nuovo account cliente in [!DNL Commerce] utilizzando i dati cliente importati con l’ordine Amazon. Questa opzione consente di creare il database dei clienti dagli ordini di Amazon.

1. Per **[!UICONTROL Order Number Source]**, scegli un’opzione:

   - `Build Using Magento Order Number` - (Predefinito) Scegli quando vuoi creare un&#39;unica [!DNL Commerce] numero dell&#39;ordine per l&#39;ordine Amazon corrispondente utilizzando [!DNL Commerce] ID ordine assegnato in modo incrementale.

   - `Build Using Amazon Order Number` - Scegli quando desideri creare il [!DNL Commerce] numero di ordine utilizzando il numero di ordine assegnato da Amazon corrispondente.
   >[!NOTE]
   >
   >Dopo l’importazione di un ordine, il numero dell’ordine Amazon viene visualizzato nella _[!UICONTROL Recent Orders]_nel dashboard dello store. La [!DNL Commerce] il numero dell&#39;ordine viene visualizzato quando si visualizzano i dettagli dell&#39;ordine nel [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html)Area di lavoro {target=&quot;_blank&quot;}.

1. Per **[!UICONTROL Order Status]** (obbligatorio), scegli un’opzione:

   - `Default Order Status` - (Impostazione predefinita) Scegli quando vuoi assegnare ai nuovi ordini importati da Amazon lo stato predefinito dell’ordine definito per i nuovi ordini. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato di ordine personalizzato per i nuovi ordini) è `Pending`. Vedi [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

   - `Custom Order Status` - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito.

   - `Processing Order Status` - Abilitato quando **[!UICONTROL Order Status]** è impostato su `Custom Order Status`. Scegli lo stato da utilizzare per gli ordini appena creati importati da Amazon. Le opzioni in questo campo si basano sulle opzioni di stato predefinite in [!DNL Commerce]. Vedi [Stato dell&#39;ordine](https://docs.magento.com/user-guide/sales/order-status.html). Puoi anche creare uno stato di ordine personalizzato da visualizzare qui per la selezione. Per creare uno stato di ordine personalizzato, consulta [Stato ordine personalizzato](https://docs.magento.com/user-guide/sales/order-status-custom.html){target=&quot;_blank&quot;}.

1. Al termine, fai clic su **[!UICONTROL Save order settings]**.

![Impostazioni ordine](assets/amazon-order-settings.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Amazon Orders] | Opzioni:<ul><li>**[!UICONTROL Disabled]** - Scegliere quando non si desidera creare ordini corrispondenti in [!DNL Commerce] quando vengono ricevuti nuovi ordini da Amazon. Se selezionato, tutti gli altri campi della pagina vengono disabilitati.</li><li>**[!UICONTROL Enabled]** - (Predefinito) Scegli quando vuoi creare il corrispondente [!DNL Commerce] ordini quando nuovi ordini vengono ricevuti da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato di Amazon e ai livelli di stock.</li></ul><br><br>`Enabled` deve essere scelto per gestire gli ordini Amazon in [!DNL Commerce]. Quando `Disabled` viene selezionato, gli ordini Amazon vengono visualizzati sul dashboard dello store, ma gli ordini devono essere gestiti nel [!DNL Amazon Seller Central] conto. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Scegli quale [!DNL Commerce] archivia gli ordini Amazon a cui sono associati quando vengono creati nel [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html)Area di lavoro {target=&quot;_blank&quot;}. Per impostazione predefinita, questa impostazione utilizza la Vista store per [!DNL Commerce] sito web selezionato quando [aggiunto l’archivio Amazon](./store-integration.md). Se desideri modificare questa impostazione, l’elenco delle opzioni dipende dalla [!DNL Commerce] archivi configurati nella configurazione. Vedi [Negozi](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Opzioni:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Impostazione predefinita) Scegli se non desideri creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall’ordine Amazon. Quando scelto, questa opzione comunica [!DNL Commerce] per elaborare un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest.</li><li>**[!UICONTROL Build New Customer Account]** - Scegli quando creare un nuovo account cliente nel tuo [!DNL Commerce] database del cliente utilizzando i dati del cliente importati con l&#39;ordine Amazon. Questa opzione aiuta a creare [!DNL Commerce] database dei clienti dai tuoi ordini Amazon.</li></ul> |
| Origine numero ordine | Opzioni:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Predefinito) Scegli quando vuoi creare un&#39;unica [!DNL Commerce] numero dell&#39;ordine per l&#39;ordine Amazon corrispondente utilizzando [!DNL Commerce] ID ordine assegnato in modo incrementale. </li><li>**Genera con il numero di ordine di Amazon** - Scegli quando desideri creare il [!DNL Commerce] numero di ordine utilizzando il numero di ordine assegnato da Amazon corrispondente.</li></ul> |
| Ordini in sospeso | Opzioni:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Scegli quando non vuoi il tuo [!DNL Commerce] quantità di magazzino interessata dagli ordini Amazon. Scegli se utilizzi Amazon per il processo di evasione (FBA, Compliance Process). Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata non influisce sul [!DNL Commerce] quantità delle scorte.</li><li>**[!UICONTROL Reserve Quantity]** - Scegli quando vuoi che la quantità dell&#39;ordine nell&#39;ordine Amazon sia &quot;riservata&quot; nel tuo [!DNL Commerce] quantità delle scorte. Quando scelto e ricevete un ordine Amazon, la quantità ordinata &quot;riserva&quot; nel vostro [!DNL Commerce] quantità di scorte per evitare il vostro [!DNL Commerce] azioni da &quot;over selling&quot;. La quantità &quot;riservata&quot; non è disponibile per l&#39;acquisto tramite il tuo [!DNL Commerce] vetrina.</li></ul> |
| [!UICONTROL Order Status] | Opzioni:<ul><li>**[!UICONTROL Default Order Status]** - (Impostazione predefinita) Scegli quando vuoi assegnare lo stato predefinito dell’ordine ai nuovi ordini importati da Amazon. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato di ordine personalizzato per i nuovi ordini) è `Pending`. Vedi [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito. Se scelto, **[!UICONTROL Processing Order Status]** consente di scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon.</li></ul> |
| [!UICONTROL Processing Orders Status] | Abilitato quando _[!UICONTROL Order Status]_è impostato su `Custom Order Status`. Scegliere lo stato dell&#39;ordine da assegnare ai nuovi ordini. Le opzioni in questo campo dipendono dalle opzioni di stato predefinite in [!DNL Commerce]. Vedi [Stato dell&#39;ordine](https://docs.magento.com/user-guide/sales/order-status.html){target=&quot;_blank&quot;}. Puoi anche creare uno stato di ordine personalizzato da visualizzare qui. Per creare uno stato di ordine personalizzato, consulta [Stato ordine personalizzato](https://docs.magento.com/user-guide/sales/order-status-custom.html){target=&quot;_blank&quot;}. |

## [!DNL Commerce] creazione di ordini

[!DNL Commerce] gli ordini vengono creati per gli ordini Amazon in base alle seguenti condizioni di stato e di inventario.

### Creazione di ordini con Gestione scorte

>[!NOTE]
>
>Supportato solo nelle integrazioni Adobe Commerce e Magenti Open Source 2.3.x .

| Canale di evasione | [!DNL Commerce] Stato inventario | Stato dell’ordine di Amazon | [!UICONTROL Create Magento Order] Impostazione | Inventario riservato |
|---|---|---|---|---|
| FBA | In magazzino<br>Non disponibile<br>Non gestire | In sospeso | No | No |
| FBA | In magazzino<br>Non disponibile<br>Non gestire | PendingAvailability | No | No |
| FBA | In magazzino<br>Non disponibile<br>Non gestire | Annullato | No | No |
| FBA | In magazzino<br>Non disponibile<br>Non gestire | Errore | No | No |
| FBA | In magazzino<br>Non disponibile<br>Non gestire | Non spedito | No | No |
| FBA | In magazzino<br>Non disponibile<br>Non gestire | ParzialmenteSpedito | No | No |
| FBA | In magazzino<br>Non gestire | Spedito | Sì | No |
| FBA | Non disponibile | Spedito | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | In sospeso | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | PendingAvailability | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | Annullato | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | Errore | No | No |
| FBM | In magazzino<br>Non gestire | Non spedito | Sì | Sì |
| FBM | Non disponibile | Non spedito | No | No |
| FBM | In magazzino<br>Non gestire | ParzialmenteSpedito | Sì | Sì |
| FBM | Non disponibile | ParzialmenteSpedito | No | No |
| FBM | In magazzino<br>Non gestire | Spedito | Sì | Sì |
| FBM | Non disponibile | Spedito | No | No |

>[!NOTE]
>Se un ordine Amazon viene importato in un `Partially Shipped` o `Shipped` stato, la prenotazione di magazzino creata è per tutti gli articoli nell&#39;ordine. Il canale di vendita Amazon non compensa gli articoli che sono stati precedentemente spediti.
>
>Se un ordine viene evaso da Amazon (FBA) ma un articolo è in `out of stock` status, [!DNL Commerce] non è in grado di creare un ordine corrispondente. Si tratta di una limitazione delle integrazioni di Inventory Management.
