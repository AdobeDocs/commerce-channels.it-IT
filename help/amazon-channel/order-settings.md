---
title: Impostazioni ordine
description: Utilizza le impostazioni ordine per determinare il modo in cui gli ordini Amazon vengono importati ed elaborati nel tuo archivio Commerce.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Impostazioni ordine

Le impostazioni dell’ordine definiscono se e come gli ordini di Amazon vengono importati ed elaborati in [!DNL Commerce] e sono accessibili sul [dashboard store](./amazon-store-dashboard.md).

Le impostazioni di importazione dell&#39;ordine sono impostate su `Enabled` per impostazione predefinita, ciò significa che gli ordini di Amazon vengono visualizzati nel dashboard del negozio e creano [!DNL Commerce] ordini. Gli ordini importati possono essere gestiti in [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} flusso di lavoro.

>[!NOTE]
>
>Indipendentemente dalle impostazioni dell’ordine, gli ordini Amazon esistenti prima dell’integrazione nello store non vengono importati.

Dopo [integrazione store](./store-integration.md) è completato, puoi modificare le impostazioni dell’ordine. Se si impostano le impostazioni dell&#39;ordine su `Disabled`, gli ordini Amazon vengono visualizzati nel dashboard del negozio ma devono essere gestiti nel [!DNL Amazon Seller Central] account.

Quando un ordine viene creato su Amazon, non viene importato immediatamente in [!DNL Commerce]. Amazon assegna un `Pending` stato degli ordini appena creati. Dopo la verifica dell&#39;ordine e del metodo di pagamento da parte di Amazon, lo stato dell&#39;ordine viene modificato in `Unshipped`. Questa modifica di stato attiva l’importazione dell’ordine e [!DNL Commerce] crea un ordine corrispondente.

Gli ordini importati da Amazon possono essere gestiti nel [!DNL Commerce] [flusso di lavoro ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}. Vedi anche [Gestisci ordini](./managing-orders.md).

## Configura impostazioni ordine {#configure-order-settings}

1. Clic **[!UICONTROL Order Settings]** nel dashboard del negozio.

1. Per **[!UICONTROL Import Amazon Orders]** (obbligatorio), scegli un’opzione:

   - `Disabled` - Scegliere se non si desidera creare gli ordini corrispondenti in [!DNL Commerce] quando si ricevono nuovi ordini da Amazon. Quando vengono selezionati, tutti gli altri campi di questa pagina vengono disabilitati.

   - `Enabled` - (Predefinito) Scegli quando vuoi creare il corrispondente [!DNL Commerce] ordini quando vengono ricevuti nuovi ordini da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato e alle scorte di Amazon.

      >[!NOTE]
      >
      >Gli ordini di importazione Amazon devono essere impostati su `Enabled` per gestire gli ordini di Amazon in [!DNL Commerce] [ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} flusso di lavoro. Se impostato su `Disabled`, gli ordini Amazon non hanno un corrispondente [!DNL Commerce] numero di ordine e non può essere gestito in [!DNL Commerce]. Puoi gestire questi ordini nel tuo [!DNL Amazon Seller Central] account.

1. Per **[!UICONTROL Import Amazon Orders Into Magento Store]**, scegli quale [!DNL Commerce] memorizza gli ordini Amazon a cui sono associati quando l’ordine corrispondente viene creato in [!DNL Commerce].

   L&#39;impostazione predefinita è la visualizzazione Store del sito Web selezionato quando [ha aggiunto Amazon store](./store-integration.md). Se desideri modificare questa impostazione, l’elenco delle opzioni dipende dal [!DNL Commerce] archivi configurati nella configurazione. Consulta [Negozi](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target="_blank"}.

1. Per **[!UICONTROL Customer Creation]**, scegli un’opzione:

   - `No Customer Creation (guest)` - (Impostazione predefinita) Scegli se non desideri creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall’ordine di Amazon. Quando viene scelto, [!DNL Commerce] elabora un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest in [!DNL Commerce].

   - `Build New Customer Account` - Scegli quando creare un nuovo account cliente in [!DNL Commerce] utilizzando i dati cliente importati con l’ordine Amazon. Questa opzione consente di creare il database dei clienti a partire dagli ordini Amazon.

1. Per **[!UICONTROL Order Number Source]**, scegli un’opzione:

   - `Build Using Magento Order Number` - (Impostazione predefinita) Scegli quando vuoi creare un [!DNL Commerce] numero di ordine per l’ordine Amazon corrispondente utilizzando [!DNL Commerce] ID ordine assegnato in modo incrementale.

   - `Build Using Amazon Order Number` - Scegli quando creare il [!DNL Commerce] numero di ordine utilizzando il corrispondente numero di ordine assegnato da Amazon.
   >[!NOTE]
   >
   >Dopo l’importazione di un ordine, il numero dell’ordine di Amazon viene visualizzato nel _[!UICONTROL Recent Orders]_nel dashboard del negozio. Il [!DNL Commerce] numero ordine viene visualizzato quando si visualizzano i dettagli dell&#39;ordine in [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} Workspace.

1. Per **[!UICONTROL Order Status]** (obbligatorio), scegli un’opzione:

   - `Default Order Status` - (Impostazione predefinita) Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon lo stato predefinito definito per i nuovi ordini. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato personalizzato per i nuovi ordini) è `Pending`. Consulta [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

   - `Custom Order Status` - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito.

   - `Processing Order Status` - Attivato quando **[!UICONTROL Order Status]** è impostato su `Custom Order Status`. Scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon. Le opzioni in questo campo si basano sulle opzioni di stato predefinite in [!DNL Commerce]. Consulta [Stato ordine](https://docs.magento.com/user-guide/sales/order-status.html). Puoi anche creare uno stato dell’ordine personalizzato da visualizzare qui per la selezione. Per creare uno stato dell’ordine personalizzato, consulta [Stato ordine personalizzato](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}.

1. Al termine, fai clic su **[!UICONTROL Save order settings]**.

![Impostazioni ordine](assets/amazon-order-settings.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Amazon Orders] | Opzioni:<ul><li>**[!UICONTROL Disabled]** - Scegliere se non si desidera creare gli ordini corrispondenti in [!DNL Commerce] quando si ricevono nuovi ordini da Amazon. Quando vengono selezionati, tutti gli altri campi di questa pagina vengono disabilitati.</li><li>**[!UICONTROL Enabled]** - (Predefinito) Scegli quando vuoi creare il corrispondente [!DNL Commerce] ordini quando vengono ricevuti nuovi ordini da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato e alle scorte di Amazon.</li></ul><br><br>`Enabled` deve essere scelto per gestire gli ordini di Amazon in [!DNL Commerce]. Quando `Disabled` viene selezionato, gli ordini Amazon vengono visualizzati nel dashboard del negozio, ma devono essere gestiti nel tuo [!DNL Amazon Seller Central] account. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Scegli quale [!DNL Commerce] archiviare gli ordini Amazon a cui sono associati quando vengono creati in [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workspace. This setting defaults to the Store View for the [!DNL Commerce] website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target="_blank"}. |
| [!UICONTROL Customer Creation] | Opzioni:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Impostazione predefinita) Scegli se non desideri creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall’ordine di Amazon. Quando viene selezionata, questa opzione comunica [!DNL Commerce] per elaborare un ordine Amazon importato nello stesso modo in cui elabora un pagamento come ospite.</li><li>**[!UICONTROL Build New Customer Account]** - Scegliere quando si desidera creare un nuovo account cliente nel [!DNL Commerce] database del cliente che utilizza i dati del cliente importati con l’ordine Amazon. Questa opzione consente di creare [!DNL Commerce] database dei clienti basato sugli ordini di Amazon.</li></ul> |
| Origine numero ordine | Opzioni:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Impostazione predefinita) Scegli quando vuoi creare un [!DNL Commerce] numero di ordine per l’ordine Amazon corrispondente utilizzando [!DNL Commerce] ID ordine assegnato in modo incrementale. </li><li>**Genera con numero ordine Amazon** - Scegli quando creare il [!DNL Commerce] numero di ordine utilizzando il corrispondente numero di ordine assegnato da Amazon.</li></ul> |
| Ordini in sospeso | Opzioni:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Scegliere quando non si desidera [!DNL Commerce] quantità di scorte interessate dagli ordini Amazon. Scegli se utilizzare Amazon per il processo di evasione (FBA). Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata non influisce sulla [!DNL Commerce] quantità di magazzino.</li><li>**[!UICONTROL Reserve Quantity]** - Scegli quando desideri che la quantità dell&#39;ordine nell&#39;ordine Amazon sia &quot;prenotata&quot; nel tuo [!DNL Commerce] quantità di magazzino. Una volta scelto e ricevi un ordine Amazon, la quantità ordinata verrà &quot;prenotata&quot; nel tuo [!DNL Commerce] quantità di scorte per evitare [!DNL Commerce] azioni derivanti da &quot;vendita eccessiva&quot;. La quantità &quot;prenotata&quot; non è disponibile per l&#39;acquisto tramite [!DNL Commerce] vetrina.</li></ul> |
| [!UICONTROL Order Status] | Opzioni:<ul><li>**[!UICONTROL Default Order Status]** - (Impostazione predefinita) Scegliere quando si desidera assegnare lo stato predefinito dell&#39;ordine ai nuovi ordini importati da Amazon. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato personalizzato per i nuovi ordini) è `Pending`. Consulta [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito. Quando viene scelto, **[!UICONTROL Processing Order Status]** consente di scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon.</li></ul> |
| [!UICONTROL Processing Orders Status] | Attivato quando _[!UICONTROL Order Status]_è impostato su `Custom Order Status`. Scegliere lo stato dell&#39;ordine da assegnare ai nuovi ordini. Le opzioni in questo campo dipendono dalle opzioni di stato predefinite in [!DNL Commerce]. Consulta [Stato ordine](https://docs.magento.com/user-guide/sales/order-status.html){target="_blank"}. You can also create a custom order status to show here. To create a custom order status, see [Custom Order Status](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}. |

## [!DNL Commerce] creazione ordine

[!DNL Commerce] gli ordini vengono creati per gli ordini di Amazon in base ai seguenti stati e condizioni di magazzino.

### Creazione di ordini con Inventory management

>[!NOTE]
>
>Supportato solo nelle integrazioni Adobe Commerce e Magenti Open Source 2.3.x.

| Canale di evasione | [!DNL Commerce] Stato inventario | Stato ordine Amazon | [!UICONTROL Create Magento Order] Impostazione | Inventario riservato |
|---|---|---|---|---|
| FBA | In magazzino<br>Esaurito<br>Non gestire | In sospeso | No | No |
| FBA | In magazzino<br>Esaurito<br>Non gestire | PendingAvailability | No | No |
| FBA | In magazzino<br>Esaurito<br>Non gestire | Annullato | No | No |
| FBA | In magazzino<br>Esaurito<br>Non gestire | Errore | No | No |
| FBA | In magazzino<br>Esaurito<br>Non gestire | Non spedito | No | No |
| FBA | In magazzino<br>Esaurito<br>Non gestire | PartiallyShipped | No | No |
| FBA | In magazzino<br>Non gestire | Spedito | Sì | No |
| FBA | Esaurito | Spedito | No | No |
| FBM | In magazzino<br>Esaurito<br>Non gestire | In sospeso | No | No |
| FBM | In magazzino<br>Esaurito<br>Non gestire | PendingAvailability | No | No |
| FBM | In magazzino<br>Esaurito<br>Non gestire | Annullato | No | No |
| FBM | In magazzino<br>Esaurito<br>Non gestire | Errore | No | No |
| FBM | In magazzino<br>Non gestire | Non spedito | Sì | Sì |
| FBM | Esaurito | Non spedito | No | No |
| FBM | In magazzino<br>Non gestire | PartiallyShipped | Sì | Sì |
| FBM | Esaurito | PartiallyShipped | No | No |
| FBM | In magazzino<br>Non gestire | Spedito | Sì | Sì |
| FBM | Esaurito | Spedito | No | No |

>[!NOTE]
>Se un ordine Amazon viene importato in un `Partially Shipped` o `Shipped` stato, la prenotazione del magazzino creata si riferisce a tutti gli articoli nell’ordine. Il canale di vendita Amazon non compensa gli articoli precedentemente spediti.
>
>Se un ordine è evaso da Amazon (FBA) ma è presente un articolo `out of stock` stato, [!DNL Commerce] non è in grado di creare un ordine corrispondente. Si tratta di una limitazione delle integrazioni Inventory management.
