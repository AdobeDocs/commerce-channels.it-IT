---
title: Azioni di elenco dei prodotti
description: Utilizza le impostazioni Azioni elenco prodotti per definire in che modo il catalogo Commerce interagisce con Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html: 
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 568
ht-degree: 0%

---

# Azioni nell’elenco dei prodotti

Le impostazioni delle azioni per l’elenco dei prodotti fanno parte delle impostazioni dell’elenco degli store. Le impostazioni dell&#39;elenco sono accessibili dal [dashboard del negozio](./amazon-store-dashboard.md).

Queste impostazioni definiscono il modo in cui il catalogo interagisce con Amazon. Queste impostazioni:

- Indica se i prodotti di catalogo [!DNL Commerce] che soddisfano i requisiti di idoneità di Amazon vengono inviati automaticamente al tuo account [!DNL Amazon Seller Central] per creare elenchi.

- Imposta il tempo di gestione predefinito per un ordine. Questo valore definisce il numero di giorni necessari per elaborare e spedire un ordine. Ad esempio, se qualcuno seleziona la spedizione di 2 giorni, il tempo di transito della spedizione non inizia fino al completamento dell&#39;elaborazione e i pacchetti vengono consegnati a un vettore. Il tempo totale di consegna è (tempo di movimentazione + tempo di transito + eventuali ferie).

## Configurare le impostazioni

1. Fai clic su **[!UICONTROL Listing Settings]** nel dashboard dello store.

1. Espandi la sezione _[!UICONTROL Product Listing Actions]_.

1. Per **[!UICONTROL Automatic List Action]** (obbligatorio), scegli un’opzione:

   - `Automatically List Eligible Products` - (Impostazione predefinita) Scegli quando i prodotti  [!DNL Commerce] del catalogo (che soddisfano i requisiti di idoneità di Amazon) verranno pubblicati automaticamente in Amazon e creeranno inserzioni Amazon.

   - `Do Not Automatically List Eligible Products` - Scegli quando selezionare manualmente i prodotti di  [!DNL Commerce] catalogo idonei e creare elenchi Amazon. Quando viene scelto, i prodotti del catalogo che soddisfano i criteri per l’inserimento nell’elenco e contengono tutte le informazioni richieste vengono visualizzati nella scheda [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale in Amazon.

1. Per **[!UICONTROL Default Handling Time]** (obbligatorio), immettere il numero di giorni necessari per il lead time prima della spedizione.

   Il valore predefinito è `2` giorni.

   >[!NOTE]
   >
   >Questo valore predefinito del tempo di gestione è valido solo per gli annunci Amazon creati tramite il canale di vendita Amazon. Gli elenchi Amazon creati nel tuo account [!DNL Amazon Seller Central] utilizzano il tempo di gestione predefinito impostato in Amazon.

1. Al termine, fai clic su **[!UICONTROL Save listing settings]**.

![Azioni nell’elenco dei prodotti](assets/amazon-product-listing-actions.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Automatic List Action] | Opzioni:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Consigliato) Scegli quando i prodotti  [!DNL Commerce] del catalogo (che soddisfano i requisiti di idoneità per Amazon) verranno pubblicati automaticamente in Amazon e creeranno annunci Amazon. Quando viene selezionata questa opzione, la scheda [_[!UICONTROL Ready to List]_](./ready-to-list.md) non viene visualizzata. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Scegli quando selezionare manualmente i prodotti di  [!DNL Commerce] catalogo idonei e creare elenchi Amazon. Quando viene scelto, i prodotti del catalogo che soddisfano i criteri per l’inserimento nell’elenco e contengono tutte le informazioni richieste vengono visualizzati nella scheda [_[!UICONTROL Ready to List]_](./ready-to-list.md) per la pubblicazione manuale.</li></ul> |
| [!UICONTROL Default Handling Time] | Il valore numerico che rappresenta il numero di giorni, in generale, necessari per elaborare e spedire gli ordini. Il valore predefinito è `2`. Questo valore viene utilizzato per gli elenchi Amazon creati in [!DNL Commerce] e pubblicati in Amazon. Questa impostazione non influisce sul tempo di gestione predefinito per gli elenchi di Amazon prima dell’integrazione con [!DNL Commerce].<br><br>Il valore definito nel canale di vendita Amazon non sostituisce il tempo di gestione predefinito definito in un elenco Amazon esistente. Quando un elemento **[!UICONTROL Handling Time Override]** viene abilitato e quindi rimosso, il tempo di gestione di un ordine ritorna al valore qui definito.<br><br>Se disponi di prodotti con tempi di gestione diversi, puoi creare un’sostituzione del tempo di gestione a livello di prodotto specifico. Puoi gestire le sostituzioni dei tempi nella scheda [_[!UICONTROL Overrides]_](./overrides.md) , per garantire la flessibilità necessaria per gestire l’implementazione del prodotto. Se non è presente alcuna sostituzione del tempo di gestione in [!DNL Commerce] per un prodotto, l’impostazione predefinita del tempo di gestione è il valore definito nell’elenco di Amazon.<br><br>Il tempo di gestione è un attributo regionale. Quando il valore viene modificato per un elenco, la modifica interessa tutti gli elenchi che condividono il valore [!DNL Amazon Seller SKU] in tutti gli archivi Amazon esistenti per la stessa area (definita in [integrazione store](./store-integration.md)). Tuttavia, la modifica del valore di un [!DNL Amazon Seller SKU] condiviso nell&#39;area Nord America non influisce sugli stessi prodotti elencati in un negozio con un&#39;area definita diversa. L&#39;archivio per l&#39;area con la data di creazione più vecchia controlla la priorità per le impostazioni dell&#39;ora di gestione predefinita. |

**Accesso rapido**  -  [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
