---
title: Impostazioni ordine Amazon
description: Utilizza le impostazioni ordine per determinare il modo in cui gli ordini Amazon vengono importati ed elaborati nel tuo store Commerce.
feature: Sales Channels, Orders, Inventory, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: a93ba31a95f32cc6ea285aed2399255021985693
workflow-type: tm+mt
source-wordcount: '1388'
ht-degree: 0%

---

# Impostazioni ordine Amazon

Le impostazioni dell&#39;ordine definiscono se e come gli ordini Amazon vengono importati ed elaborati in [!DNL Commerce] e sono accessibili nel [dashboard dello store](./amazon-store-dashboard.md).

Le impostazioni di importazione degli ordini sono impostate su `Enabled` per impostazione predefinita, il che significa che gli ordini Amazon vengono visualizzati nel dashboard dello store e creano gli ordini [!DNL Commerce] corrispondenti. Gli ordini importati possono essere gestiti nel flusso di lavoro [!DNL Commerce] [Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).

>[!NOTE]
>
>Indipendentemente dalle impostazioni dell’ordine, gli ordini Amazon esistenti prima dell’integrazione nello store non vengono importati.

Al termine dell&#39;[integrazione store](./store-integration.md), puoi modificare le impostazioni dell&#39;ordine. Se si impostano le impostazioni dell&#39;ordine su `Disabled`, gli ordini Amazon vengono visualizzati nel dashboard dello store ma devono essere gestiti nell&#39;account [!DNL Amazon Seller Central].

Quando un ordine viene creato su Amazon, non viene importato immediatamente in [!DNL Commerce]. Amazon assegna uno stato `Pending` agli ordini appena creati. Dopo che Amazon ha verificato l&#39;ordine e il metodo di pagamento, lo stato dell&#39;ordine viene modificato in `Unshipped`. Questa modifica dello stato attiva l&#39;importazione dell&#39;ordine e [!DNL Commerce] crea un ordine corrispondente.

Gli ordini importati da Amazon possono essere gestiti nel [!DNL Commerce] [flusso di lavoro ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). Vedi anche [Gestione ordini](./managing-orders.md).

## Configura impostazioni ordine {#configure-order-settings}

1. Fare clic su **[!UICONTROL Order Settings]** nel dashboard dell&#39;archivio.

1. Per **[!UICONTROL Import Amazon Orders]** (obbligatorio), scegliere un&#39;opzione:

   - `Disabled` - Scegliere se non si desidera creare gli ordini corrispondenti in [!DNL Commerce] quando vengono ricevuti nuovi ordini da Amazon. Quando vengono selezionati, tutti gli altri campi di questa pagina vengono disabilitati.

   - `Enabled` - (Predefinito) Scegliere quando si desidera creare [!DNL Commerce] ordini corrispondenti quando si ricevono nuovi ordini da Amazon. [!DNL Commerce] ordini creati in base allo stato e ai livelli di scorte di Amazon.

     >[!NOTE]
     >
     >L&#39;importazione degli ordini Amazon deve essere impostata su `Enabled` per gestire gli ordini Amazon nel flusso di lavoro [!DNL Commerce] [ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). Se è impostato su `Disabled`, gli ordini Amazon non hanno un numero di ordine [!DNL Commerce] corrispondente e non possono essere gestiti in [!DNL Commerce]. Gestisci questi ordini nel tuo account [!DNL Amazon Seller Central].

1. Per **[!UICONTROL Import Amazon Orders Into Magento Store]**, scegliere a quale archivio [!DNL Commerce] sono associati gli ordini Amazon quando l&#39;ordine corrispondente viene creato in [!DNL Commerce].

   Per impostazione predefinita, questa impostazione corrisponde alla vista Store del sito Web selezionato quando [hai aggiunto l&#39;Amazon Store](./store-integration.md). Se si desidera modificare questa impostazione, l&#39;elenco delle opzioni dipende dagli archivi [!DNL Commerce] impostati nella configurazione. Vedi [Archivi](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html).

1. Per **[!UICONTROL Customer Creation]**, scegliere un&#39;opzione:

   - `No Customer Creation (guest)` - (Predefinito) Scegliere se non si desidera creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall&#39;ordine Amazon. Quando viene scelto, [!DNL Commerce] elabora un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest in [!DNL Commerce].

   - `Build New Customer Account` - Scegliere quando si desidera creare un nuovo account cliente in [!DNL Commerce] utilizzando i dati cliente importati con l&#39;ordine Amazon. Questa opzione consente di creare il database dei clienti a partire dagli ordini Amazon.

1. Per **[!UICONTROL Order Number Source]**, scegliere un&#39;opzione:

   - `Build Using Magento Order Number` - (Predefinito) Scegliere quando si desidera creare un numero di ordine [!DNL Commerce] univoco per l&#39;ordine Amazon corrispondente utilizzando l&#39;ID di ordine [!DNL Commerce] assegnato in modo incrementale.

   - `Build Using Amazon Order Number` - Scegliere quando creare il numero di ordine [!DNL Commerce] utilizzando il corrispondente numero di ordine assegnato da Amazon.

   >[!NOTE]
   >
   >Dopo l&#39;importazione di un ordine, il numero dell&#39;ordine Amazon viene visualizzato nell&#39;elenco _[!UICONTROL Recent Orders]_nel dashboard dello store. Il numero di ordine [!DNL Commerce] viene visualizzato quando si visualizzano i dettagli dell&#39;ordine nell&#39;area di lavoro [!DNL Commerce] [Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).

1. Per **[!UICONTROL Order Status]** (obbligatorio), scegliere un&#39;opzione:

   - `Default Order Status` - (Predefinito) Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon lo stato predefinito definito per i nuovi ordini. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato personalizzato per i nuovi ordini) è `Pending`. Vedi [Elaborazione degli ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

   - `Custom Order Status` - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito.

   - `Processing Order Status` - Abilitato quando **[!UICONTROL Order Status]** è impostato su `Custom Order Status`. Scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon. Le opzioni in questo campo si basano sulle opzioni di stato predefinite in [!DNL Commerce]. Consulta [Stato ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Puoi anche creare uno stato dell’ordine personalizzato da visualizzare qui per la selezione. Per creare uno stato ordine personalizzato, vedere [Stato ordine personalizzato](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status).

1. Al termine, fare clic su **[!UICONTROL Save order settings]**.

![Impostazioni ordine](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | Opzioni:<ul><li>**[!UICONTROL Disabled]** - Scegliere se non si desidera creare gli ordini corrispondenti in [!DNL Commerce] quando vengono ricevuti nuovi ordini da Amazon. Quando vengono selezionati, tutti gli altri campi di questa pagina vengono disabilitati.</li><li>**[!UICONTROL Enabled]** - (Predefinito) Scegliere quando si desidera creare [!DNL Commerce] ordini corrispondenti quando si ricevono nuovi ordini da Amazon. [!DNL Commerce] ordini creati in base allo stato e ai livelli di scorte di Amazon.</li></ul><br><br>`Enabled` deve essere scelto per gestire gli ordini Amazon in [!DNL Commerce]. Quando si sceglie `Disabled`, gli ordini Amazon vengono visualizzati nel dashboard dello store, ma gli ordini devono essere gestiti nell&#39;account [!DNL Amazon Seller Central]. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | Scegli a quali [!DNL Commerce] archivi sono associati gli ordini Amazon quando vengono creati nell&#39;area di lavoro [!DNL Commerce] [Ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html). L&#39;impostazione predefinita è la Visualizzazione archivio per il sito Web [!DNL Commerce] selezionato quando [hai aggiunto l&#39;archivio Amazon](./store-integration.md). Se si desidera modificare questa impostazione, l&#39;elenco delle opzioni dipende dagli archivi [!DNL Commerce] impostati nella configurazione. Vedi [Archivi](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html). |
| [!UICONTROL Customer Creation] | Opzioni:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (Predefinito) Scegliere se non si desidera creare un account cliente in [!DNL Commerce] utilizzando i dati cliente importati dall&#39;ordine Amazon. Se selezionata, questa opzione indica a [!DNL Commerce] di elaborare un ordine Amazon importato nello stesso modo in cui elabora un pagamento guest.</li><li>**[!UICONTROL Build New Customer Account]** - Scegliere quando si desidera creare un nuovo account cliente nel database clienti [!DNL Commerce] utilizzando i dati cliente importati con l&#39;ordine Amazon. Questa opzione consente di creare il database clienti [!DNL Commerce] dagli ordini Amazon.</li></ul> |
| Numero ordine Source | Opzioni:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (Predefinito) Scegliere quando si desidera creare un numero di ordine [!DNL Commerce] univoco per l&#39;ordine Amazon corrispondente utilizzando l&#39;ID di ordine [!DNL Commerce] assegnato in modo incrementale. </li><li>**Genera con numero ordine Amazon** - Scegli quando creare il numero ordine [!DNL Commerce] utilizzando il numero ordine assegnato da Amazon corrispondente.</li></ul> |
| Ordini in sospeso | Opzioni:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Scegli quando non vuoi che la quantità di azioni di [!DNL Commerce] sia influenzata dagli ordini Amazon. Scegli se utilizzare Amazon per il processo di evasione (FBA). Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata non influisce sulla quantità di scorte [!DNL Commerce].</li><li>**[!UICONTROL Reserve Quantity]** - Scegli quando vuoi che la quantità dell&#39;ordine nell&#39;ordine Amazon sia &quot;prenotata&quot; nella quantità di azioni [!DNL Commerce]. Quando viene scelto e si riceve un ordine Amazon, la quantità ordinata verrà &quot;prenotata&quot; nella quantità di scorte [!DNL Commerce] per evitare che le scorte di [!DNL Commerce] vengano &quot;vendute in eccesso&quot;. La quantità &quot;prenotata&quot; non è disponibile per l&#39;acquisto tramite la vetrina [!DNL Commerce].</li></ul> |
| [!UICONTROL Order Status] | Opzioni:<ul><li>**[!UICONTROL Default Order Status]** - (Predefinito) Scegliere quando si desidera assegnare ai nuovi ordini importati da Amazon lo stato predefinito per i nuovi ordini. Lo stato predefinito per i nuovi ordini (a meno che non sia stato creato uno stato personalizzato per i nuovi ordini) è `Pending`. Vedi [Elaborazione degli ordini](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).</li><li>**[!UICONTROL Custom Order Status]** - Scegliere quando si desidera assegnare agli ordini appena creati importati da Amazon uno stato diverso da quello predefinito. Se selezionato, **[!UICONTROL Processing Order Status]** consente di scegliere lo stato da utilizzare per gli ordini appena creati importati da Amazon.</li></ul> |
| [!UICONTROL Processing Orders Status] | Abilitato quando _[!UICONTROL Order Status]_è impostato su `Custom Order Status`. Scegliere lo stato dell&#39;ordine da assegnare ai nuovi ordini. Le opzioni in questo campo dipendono dalle opzioni di stato predefinite in [!DNL Commerce]. Consulta [Stato ordine](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html). Puoi anche creare uno stato personalizzato dell’ordine da visualizzare qui. Per creare uno stato ordine personalizzato, vedere [Stato ordine personalizzato] |

## [!DNL Commerce] creazione ordine

[!DNL Commerce] ordini creati per gli ordini Amazon in base alle seguenti condizioni di stato e di magazzino.

### Creazione di ordini con Inventory management

>[!NOTE]
>
>Supportato solo nelle integrazioni Adobe Commerce e Magento Open Source 2.3.x.

| Canale di evasione | Stato inventario [!DNL Commerce] | Stato ordine Amazon | Impostazione [!UICONTROL Create Magento Order] | Inventario riservato |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
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
>Se un ordine Amazon viene importato con lo stato `Partially Shipped` o `Shipped`, la prenotazione inventario creata si riferisce a tutti gli articoli dell&#39;ordine. Il canale di vendita Amazon non compensa gli articoli precedentemente spediti.
>
>Se un ordine è evaso da Amazon (FBA) ma un articolo è nello stato `out of stock`, [!DNL Commerce] non è in grado di creare un ordine corrispondente. Si tratta di una limitazione delle integrazioni Inventory management.
