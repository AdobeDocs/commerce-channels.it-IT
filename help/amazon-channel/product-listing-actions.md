---
title: Azioni di elenco dei prodotti
description: Utilizza le impostazioni Azioni elenco prodotti per definire in che modo il catalogo Commerce interagisce con Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Azioni nell’elenco dei prodotti

Le impostazioni delle azioni per l’elenco dei prodotti fanno parte delle impostazioni dell’elenco degli store. Le impostazioni dell’elenco sono accessibili dal [dashboard store](./amazon-store-dashboard.md).

Queste impostazioni definiscono il modo in cui il catalogo interagisce con Amazon. Queste impostazioni:

- Indica se il [!DNL Commerce] i prodotti di catalogo che soddisfano i requisiti di idoneità di Amazon vengono inviati automaticamente al tuo [!DNL Amazon Seller Central] per creare elenchi.

- Imposta il tempo di gestione predefinito per un ordine. Questo valore definisce il numero di giorni necessari per elaborare e spedire un ordine. Ad esempio, se qualcuno seleziona la spedizione di 2 giorni, il tempo di transito della spedizione non inizia fino al completamento dell&#39;elaborazione e i pacchetti vengono consegnati a un vettore. Il tempo totale di consegna è (tempo di movimentazione + tempo di transito + eventuali ferie).

## Configurare le impostazioni

1. Fai clic su **[!UICONTROL Listing Settings]** sul dashboard dello store.

1. Espandi la _[!UICONTROL Product Listing Actions]_sezione .

1. Per **[!UICONTROL Automatic List Action]** (obbligatorio), scegli un’opzione:

   - `Automatically List Eligible Products` - (Predefinito) Scegli quando desideri [!DNL Commerce] prodotti di catalogo (che soddisfano i requisiti di idoneità di Amazon) per pubblicare automaticamente in Amazon e creare annunci Amazon.

   - `Do Not Automatically List Eligible Products` - Scegli quando selezionare manualmente il tuo idoneo [!DNL Commerce] catalogare prodotti e creare elenchi Amazon. Quando scelto, i prodotti del catalogo che soddisfano i criteri di inserimento nell’elenco e contengono tutte le informazioni richieste vengono visualizzati nella [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale in Amazon.

1. Per **[!UICONTROL Default Handling Time]** (obbligatorio), specificare il numero di giorni necessari per il lead time prima della spedizione.

   Il valore predefinito è `2` giorni.

   >[!NOTE]
   >
   >Questo valore predefinito del tempo di gestione è valido solo per gli annunci Amazon creati tramite il canale di vendita Amazon. Qualsiasi elenco Amazon creato nel tuo [!DNL Amazon Seller Central] l&#39;account utilizza il tempo di gestione predefinito impostato in Amazon.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Azioni nell’elenco dei prodotti](assets/amazon-product-listing-actions.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Automatic List Action] | Opzioni:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (consigliato) Scegli quando desideri [!DNL Commerce] prodotti di catalogo (che soddisfano i requisiti di idoneità di Amazon) per pubblicare automaticamente in Amazon e creare annunci Amazon. Quando viene scelto, il [_[!UICONTROL Ready to List]_](./ready-to-list.md) la scheda non viene visualizzata. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Scegli quando selezionare manualmente i prodotti idonei [!DNL Commerce] catalogare prodotti e creare inserzioni Amazon. Quando scelto, i prodotti del catalogo che soddisfano i criteri di inserimento nell’elenco e contengono tutte le informazioni richieste vengono visualizzati nella [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale.</li></ul> |
| [!UICONTROL Default Handling Time] | Il valore numerico che rappresenta il numero di giorni, in generale, necessari per elaborare e spedire gli ordini. Il valore predefinito è `2`. Questo valore viene utilizzato per gli elenchi Amazon creati in [!DNL Commerce] e pubblicati in Amazon. Il tempo di gestione predefinito per gli elenchi di Amazon prima dell’integrazione con [!DNL Commerce] non sono interessati da questa impostazione.<br><br>Il valore definito nel canale di vendita Amazon non sostituisce il tempo di gestione predefinito definito in un elenco Amazon esistente. Quando un **[!UICONTROL Handling Time Override]** viene attivato e quindi rimosso. Il tempo di gestione di un ordine ritorna al valore qui definito.<br><br>Se disponi di prodotti con tempi di gestione diversi, puoi creare un’sostituzione del tempo di gestione a livello di prodotto specifico. Puoi gestire le sostituzioni dei tempi di gestione nel [_[!UICONTROL Overrides]_](./overrides.md) scheda , che offre la flessibilità necessaria per gestire l&#39;implementazione del prodotto. Se non è presente alcuna sostituzione del tempo di gestione in [!DNL Commerce] per un prodotto, il valore predefinito del tempo di gestione è il valore definito nell’elenco di Amazon.<br><br>Il tempo di gestione è un attributo regionale. Quando il valore viene modificato per un elenco, la modifica interessa tutti gli elenchi che condividono il [!DNL Amazon Seller SKU] in tutti gli archivi Amazon esistenti per la stessa area (definito in [integrazione store](./store-integration.md)). Tuttavia, la modifica del valore di una condivisione [!DNL Amazon Seller SKU] nell’area Nord America non influisce sugli stessi prodotti elencati in un negozio con un’area definita diversa. L&#39;archivio per l&#39;area con la data di creazione più vecchia controlla la priorità per le impostazioni dell&#39;ora di gestione predefinita. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
