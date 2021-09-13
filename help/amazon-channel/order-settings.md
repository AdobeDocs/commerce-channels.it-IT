---
title: Impostazioni ordine
description: Utilizza le impostazioni Ordine per determinare in che modo gli ordini Amazon vengono importati ed elaborati nel tuo negozio Commerce.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Impostazioni ordine

Le impostazioni dell&#39;ordine definiscono se e come gli ordini di Amazon vengono importati ed elaborati in [!DNL Commerce] e possono essere aperti sul [dashboard dell&#39;archivio](./amazon-store-dashboard.md).

Le impostazioni di importazione dell’ordine sono impostate su `Enabled` per impostazione predefinita, il che significa che gli ordini Amazon vengono visualizzati sul dashboard dello store e creano gli ordini [!DNL Commerce] corrispondenti. Gli ordini importati possono essere gestiti nel flusso di lavoro [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.

>[!NOTE]
>
>Indipendentemente dalle impostazioni dell’ordine, gli ordini Amazon esistenti prima dell’integrazione dell’archivio non vengono importati.

Al termine dell&#39; [integrazione dell&#39;archivio](./store-integration.md), puoi modificare le impostazioni dell&#39;ordine. Se imposti le impostazioni dell&#39;ordine su `Disabled`, gli ordini Amazon vengono visualizzati sul dashboard dello store ma devono essere gestiti nel tuo account [!DNL Amazon Seller Central].

Quando un ordine viene creato su Amazon, non viene importato immediatamente in [!DNL Commerce]. Amazon assegna uno stato `Pending` ai nuovi ordini creati. Dopo che Amazon verifica il metodo dell&#39;ordine e del pagamento, lo stato dell&#39;ordine viene modificato in `Unshipped`. Questa modifica dello stato attiva l’importazione dell’ordine e [!DNL Commerce] crea un ordine corrispondente.

Gli ordini importati da Amazon possono essere gestiti nel flusso di lavoro [!DNL Commerce] [ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}. Vedere anche [Gestire gli ordini](./managing-orders.md).

## Configurare le impostazioni dell’ordine {#configure-order-settings}

1. Fai clic su **[!UICONTROL Order Settings]** nel dashboard dello store.

1. Per **[!UICONTROL Import Amazon Orders]** (obbligatorio), scegli un’opzione:

   - `Disabled` - Scegli quando non vuoi creare ordini corrispondenti in  [!DNL Commerce] quando nuovi ordini vengono ricevuti da Amazon. Se selezionato, tutti gli altri campi della pagina vengono disabilitati.

   - `Enabled` - (Impostazione predefinita) Scegli quando vuoi creare  [!DNL Commerce] gli ordini corrispondenti quando nuovi ordini vengono ricevuti da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato di Amazon e ai livelli di stock.

      >[!NOTE]
      >
      >Importa ordini Amazon deve essere impostato su `Enabled` per gestire gli ordini Amazon nel flusso di lavoro [!DNL Commerce] [ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}. Se impostato su `Disabled`, gli ordini Amazon non hanno un numero d&#39;ordine [!DNL Commerce] corrispondente e non possono essere gestiti in [!DNL Commerce]. Puoi gestire questi ordini nel tuo account [!DNL Amazon Seller Central] .

1. Per **[!UICONTROL Import Amazon Orders Into Magento Store]**, scegli a quale [!DNL Commerce] archivio sono associati gli ordini Amazon quando viene creato l’ordine corrispondente in [!DNL Commerce].

   Per impostazione predefinita, questa impostazione consente di visualizzare il sito Web selezionato quando [è stato aggiunto l&#39;archivio Amazon](./store-integration.md). Per modificare questa impostazione, l’elenco delle opzioni dipende dagli archivi [!DNL Commerce] configurati nella configurazione. Vedere [Negozi](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){:target=&quot;_blank&quot;}.

1. Per **[!UICONTROL Customer Creation]**, scegli un’opzione:

   - `No Customer Creation (guest)` - (Impostazione predefinita) Scegli quando non vuoi creare un account cliente  [!DNL Commerce] utilizzando i dati del cliente importati dall&#39;ordine Amazon. Quando scelto, [!DNL Commerce] elabora un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest in [!DNL Commerce].

   - `Build New Customer Account` - Scegli quando creare un nuovo account cliente  [!DNL Commerce] utilizzando i dati cliente importati con l’ordine Amazon. Questa opzione consente di creare il database dei clienti dagli ordini di Amazon.

1. Per **[!UICONTROL Order Number Source]**, scegli un’opzione:

   - `Build Using Magento Order Number` - (Impostazione predefinita) Scegli quando creare un numero di  [!DNL Commerce] ordine univoco per l’ordine Amazon corrispondente utilizzando l’ID ordine assegnato  [!DNL Commerce] incrementalmente.

   - `Build Using Amazon Order Number` - Scegli quando creare il numero di  [!DNL Commerce] ordine utilizzando il numero di ordine assegnato da Amazon corrispondente.
   >[!NOTE]
   >
   >Dopo l’importazione di un ordine, il numero dell’ordine Amazon viene visualizzato nell’elenco _[!UICONTROL Recent Orders]_nel dashboard store. Il numero dell&#39;ordine [!DNL Commerce] viene visualizzato quando si visualizzano i dettagli dell&#39;ordine nell&#39;area di lavoro [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.

1. Per **[!UICONTROL Order Status]** (obbligatorio), scegli un’opzione:

   - `Default Order Status` - (Impostazione predefinita) Scegli quando vuoi assegnare ai nuovi ordini importati da Amazon lo stato predefinito dell’ordine definito per i nuovi ordini. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato di ordine personalizzato per i nuovi ordini) è `Pending`. Vedere [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html){:target=&quot;_blank&quot;}.

   - `Custom Order Status` - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito.

   - `Processing Order Status` - Abilitato quando  **[!UICONTROL Order Status]** è impostato su  `Custom Order Status`. Scegli lo stato da utilizzare per gli ordini appena creati importati da Amazon. Le opzioni in questo campo si basano sulle opzioni di stato predefinite in [!DNL Commerce]. Vedere [Stato ordine](https://docs.magento.com/user-guide/sales/order-status.html). Puoi anche creare uno stato di ordine personalizzato da visualizzare qui per la selezione. Per creare uno stato di ordine personalizzato, consulta [Stato ordine personalizzato](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}.

1. Al termine, fai clic su **[!UICONTROL Save order settings]**.

![Impostazioni ordine](assets/amazon-order-settings.png)

| Campo | Descrizione |
|---|---|
| [!UICONTROL Import Amazon Orders] | Opzioni:<ul><li>**[!UICONTROL Disabled]** - Scegli quando non vuoi creare ordini corrispondenti in  [!DNL Commerce] quando nuovi ordini vengono ricevuti da Amazon. Se selezionato, tutti gli altri campi della pagina vengono disabilitati.</li><li>**[!UICONTROL Enabled]** - (Impostazione predefinita) Scegli quando vuoi creare  [!DNL Commerce] gli ordini corrispondenti quando nuovi ordini vengono ricevuti da Amazon. [!DNL Commerce] gli ordini vengono creati in base allo stato di Amazon e ai livelli di stock.</li></ul><br><br>`Enabled` deve essere scelto per gestire gli ordini Amazon in  [!DNL Commerce]. Quando si seleziona `Disabled`, gli ordini Amazon vengono visualizzati sul dashboard dello store, ma devono essere gestiti nel tuo account [!DNL Amazon Seller Central]. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Scegli a quali [!DNL Commerce] archiviare gli ordini Amazon sono associati quando vengono creati nell&#39;area di lavoro [!DNL Commerce] [Ordini](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}. Per impostazione predefinita, questa impostazione consente di visualizzare il sito Web [!DNL Commerce] selezionato quando [è stato aggiunto l&#39;archivio Amazon](./store-integration.md). Per modificare questa impostazione, l’elenco delle opzioni dipende dagli archivi [!DNL Commerce] configurati nella configurazione. Vedere [Negozi](https://docs.magento.com/user-guide/stores/stores-all-stores.html){:target=&quot;_blank&quot;}. |
| [!UICONTROL Customer Creation] | Opzioni:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Impostazione predefinita) Scegli quando non vuoi creare un account cliente  [!DNL Commerce] utilizzando i dati del cliente importati dall&#39;ordine Amazon. Quando è selezionata, questa opzione comunica a [!DNL Commerce] di elaborare un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest.</li><li>**[!UICONTROL Build New Customer Account]** - Scegli quando creare un nuovo account cliente nel database del  [!DNL Commerce] cliente utilizzando i dati del cliente importati con l&#39;ordine Amazon. Questa opzione consente di creare il database dei clienti [!DNL Commerce] dagli ordini Amazon.</li></ul> |
| Origine numero ordine | Opzioni:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Impostazione predefinita) Scegli quando creare un numero di  [!DNL Commerce] ordine univoco per l’ordine Amazon corrispondente utilizzando l’ID ordine assegnato  [!DNL Commerce] incrementalmente. </li><li>**Crea con numero d&#39;ordine Amazon** : scegli quando vuoi creare il numero d&#39; [!DNL Commerce] ordine utilizzando il corrispondente numero d&#39;ordine assegnato da Amazon.</li></ul> |
| Ordini in sospeso | Opzioni:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Scegliere se non si desidera che la quantità  [!DNL Commerce] delle scorte sia influenzata dagli ordini Amazon. Scegli se utilizzi Amazon per il processo di evasione (FBA, Compliance Process). Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata non influisce sulla quantità di [!DNL Commerce] stock.</li><li>**[!UICONTROL Reserve Quantity]** - Scegliere quando si desidera che la quantità dell&#39;ordine nell&#39;ordine Amazon sia &quot;riservata&quot; nella quantità  [!DNL Commerce] di magazzino. Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata verrà &quot;riservata&quot; nella quantità di [!DNL Commerce] stock per evitare che le [!DNL Commerce] azioni vengano &quot;vendute in eccesso&quot;. La quantità &quot;riservata&quot; non è disponibile per l&#39;acquisto tramite la vetrina [!DNL Commerce].</li></ul> |
| [!UICONTROL Order Status] | Opzioni:<ul><li>**[!UICONTROL Default Order Status]** - (Impostazione predefinita) Scegli quando vuoi assegnare lo stato predefinito dell’ordine ai nuovi ordini importati da Amazon. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato di ordine personalizzato per i nuovi ordini) è `Pending`. Vedere [Ordini di elaborazione](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]**: scegli quando vuoi assegnare uno stato diverso da quello predefinito agli ordini appena creati importati da Amazon. Quando scelto, **[!UICONTROL Processing Order Status]** consente di scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon.</li></ul> |
| [!UICONTROL Processing Orders Status] | Abilitato quando _[!UICONTROL Order Status]_è impostato su `Custom Order Status`. Scegliere lo stato dell&#39;ordine da assegnare ai nuovi ordini. Le opzioni in questo campo dipendono dalle opzioni di stato predefinite in [!DNL Commerce]. Vedere [Stato ordine](https://docs.magento.com/user-guide/sales/order-status.html){:target=&quot;_blank&quot;}. Puoi anche creare uno stato di ordine personalizzato da visualizzare qui. Per creare uno stato di ordine personalizzato, consulta [Stato ordine personalizzato](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}. |

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
| FBA | In-stock<br>Non gestire | Spedito | Sì | No |
| FBA | Non disponibile | Spedito | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | In sospeso | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | PendingAvailability | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | Annullato | No | No |
| FBM | In magazzino<br>Non disponibile<br>Non gestire | Errore | No | No |
| FBM | In-stock<br>Non gestire | Non spedito | Sì | Sì |
| FBM | Non disponibile | Non spedito | No | No |
| FBM | In-stock<br>Non gestire | ParzialmenteSpedito | Sì | Sì |
| FBM | Non disponibile | ParzialmenteSpedito | No | No |
| FBM | In-stock<br>Non gestire | Spedito | Sì | Sì |
| FBM | Non disponibile | Spedito | No | No |

>[!NOTE]
>Se un ordine Amazon viene importato in uno stato `Partially Shipped` o `Shipped`, la prenotazione di inventario creata è per tutti gli articoli nell&#39;ordine. Il canale di vendita Amazon non compensa gli articoli che sono stati precedentemente spediti.
>
>Se un ordine viene evaso da Amazon (FBA) ma lo stato di un articolo è `out of stock`, [!DNL Commerce] non è in grado di creare un ordine corrispondente. Si tratta di una limitazione delle integrazioni di Inventory Management.
