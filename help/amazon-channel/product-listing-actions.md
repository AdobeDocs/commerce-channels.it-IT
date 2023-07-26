---
title: Canale di vendita Amazon - Azioni dell’elenco prodotti
description: Utilizza le impostazioni Azioni elenco prodotti per definire il modo in cui il catalogo Commerce interagisce con Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Azioni per l’elenco dei prodotti

Le impostazioni delle azioni dell’elenco dei prodotti fanno parte delle impostazioni dell’elenco dei punti vendita. Le impostazioni dell&#39;inserzione sono accessibili da [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni definiscono come il catalogo interagisce con Amazon. Queste impostazioni:

- Indica se [!DNL Commerce] i prodotti del catalogo che soddisfano i requisiti di idoneità di Amazon vengono inviati automaticamente al [!DNL Amazon Seller Central] per creare inserzioni.

- Impostare il tempo di gestione predefinito per un ordine. Questo valore definisce il numero di giorni necessari per elaborare e spedire un ordine. Ad esempio, se qualcuno seleziona una spedizione di 2 giorni, il tempo di transito della spedizione non inizia fino al completamento dell’elaborazione e i pacchetti vengono consegnati a un vettore. Il tempo totale di consegna è (tempo di imballaggio + tempo di transito + eventuali festività).

## Configurare le impostazioni

1. Clic **[!UICONTROL Listing Settings]** nel dashboard del negozio.

1. Espandi _[!UICONTROL Product Listing Actions]_sezione.

1. Per **[!UICONTROL Automatic List Action]** (obbligatorio), scegli un’opzione:

   - `Automatically List Eligible Products` - (Impostazione predefinita) Scegli quando desideri [!DNL Commerce] catalogare i prodotti (che soddisfano i requisiti di idoneità di Amazon) per pubblicarli automaticamente in Amazon e creare inserzioni Amazon.

   - `Do Not Automatically List Eligible Products` - Scegli quando desideri selezionare manualmente le [!DNL Commerce] catalogare i prodotti e creare inserzioni Amazon. Quando vengono scelti, i prodotti del catalogo che soddisfano i criteri di inserzione e contengono tutte le informazioni richieste vengono visualizzati sul [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale in Amazon.

1. Per **[!UICONTROL Default Handling Time]** (obbligatorio), inserire il numero di giorni necessari per il lead time prima della spedizione.

   Il valore predefinito è `2` giorni.

   >[!NOTE]
   >
   >Questo valore predefinito è valido solo per le inserzioni Amazon create tramite il canale di vendita Amazon. Tutte le inserzioni Amazon create nel tuo [!DNL Amazon Seller Central] utilizza il tempo di gestione predefinito impostato in Amazon.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Azioni per l’elenco dei prodotti](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | Opzioni:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Consigliato) Scegli quando vuoi il tuo [!DNL Commerce] catalogare i prodotti (che soddisfano i requisiti di idoneità di Amazon) per pubblicarli automaticamente in Amazon e creare inserzioni Amazon. Quando viene scelto, il [_[!UICONTROL Ready to List]_](./ready-to-list.md) non viene visualizzata. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Scegli quando desideri selezionare manualmente gli idonei [!DNL Commerce] catalogare i prodotti e creare inserzioni Amazon. Quando vengono scelti, i prodotti del catalogo che soddisfano i criteri di inserzione e contengono tutte le informazioni richieste vengono visualizzati sul [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale.</li></ul> |
| [!UICONTROL Default Handling Time] | Il valore numerico che rappresenta il numero di giorni, in generale, necessari per elaborare e spedire gli ordini. Il valore predefinito è `2`. Questo valore viene utilizzato per le inserzioni Amazon create in [!DNL Commerce] e pubblicati in Amazon. Il tempo di gestione predefinito per le inserzioni Amazon prima dell’integrazione con [!DNL Commerce] non sono interessati da questa impostazione.<br><br>Il valore definito nel canale di vendita Amazon non sostituisce il tempo di imballaggio predefinito definito in un’inserzione Amazon esistente. Quando un **[!UICONTROL Handling Time Override]** è attivato e quindi rimosso, il Tempo di gestione di un ordine ritorna al valore qui definito.<br><br>Se i prodotti hanno tempi di gestione diversi, puoi creare una sostituzione dei tempi di gestione a livello di prodotto specifico. Puoi gestire le sostituzioni dei tempi di gestione in [_[!UICONTROL Overrides]_](./overrides.md) offre la flessibilità necessaria per gestire l’adempimento del prodotto. Se non è presente alcuna sostituzione del tempo di gestione in [!DNL Commerce] per un prodotto, il valore predefinito del tempo di gestione è il valore definito nell’elenco di Amazon.<br><br>Il tempo di gestione è un attributo regionale. Quando si modifica il valore di un&#39;inserzione, la modifica ha effetto su tutte le inserzioni che condividono [!DNL Amazon Seller SKU] in tutti gli store Amazon esistenti per la stessa area (definita in [integrazione store](./store-integration.md)). Tuttavia, la modifica del valore di una [!DNL Amazon Seller SKU] nell’area Nord America non influisce sugli stessi prodotti elencati in un negozio con un’area definita diversa. L’archivio dell’area con la data di creazione più vecchia controlla la priorità per le impostazioni di Ora di gestione predefinita. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
