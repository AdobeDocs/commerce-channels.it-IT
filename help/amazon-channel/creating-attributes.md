---
title: Creare e modificare gli attributi
description: Amazon Sales Channel fornisce la vista Attributi per aiutarti a esaminare gli attributi correnti di Amazon e gli attributi Commerce collegati.
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Creare e modificare gli attributi

Crea o aggiorna [!DNL Commerce] gli attributi vengono venduti tramite Amazon e aggiornati dagli store. Controlla gli attributi correnti di Amazon e collegati [!DNL Commerce] gli attributi attraverso [_[!UICONTROL Attributes]_visualizzare](./attributes-view.md) della home page del canale di vendita Amazon. La_[!UICONTROL Action]_ mostra le azioni disponibili per l’attributo. Puoi creare e mappare un nuovo [!DNL Commerce] per un attributo Amazon non collegato, oppure puoi modificare un attributo esistente [!DNL Commerce] e la relativa mappatura su un attributo Amazon.

Quando crei e aggiorni gli attributi, puoi verificare i valori degli attributi per [!DNL Commerce] e prodotti Amazon. Questi valori possono essere diversi se non si sincronizzano e si importano valori da Amazon. Per esaminare i valori di Amazon per questi attributi, vedi [Revisione della mappatura degli attributi di Amazon](./amazon-matching-attributes-values.md). Se desideri modificare tali valori, puoi [modificare o creare una mappatura](./amazon-manually-update-incomplete-listing.md) tra Amazon e [!DNL Commerce].

## Creare un attributo {#create-an-attribute}

Questi passaggi creano un [!DNL Commerce] Attribuiscilo e mappalo su un attributo Amazon. A seconda delle configurazioni, i valori possono iniziare la sincronizzazione tra i cataloghi.

1. Sulla _Amministratore_ barra laterale, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e fai clic su **[!UICONTROL Create Attribute]** in _[!UICONTROL Action]_colonna.

1. Per abilitare la sincronizzazione dei valori Amazon con i collegamenti [!DNL Commerce] attributo, set **[!UICONTROL Is Active]** a `Yes`.

   Quando è impostato su `Yes`, i valori vengono sincronizzati in base alla configurazione.

1. Scegli `Create New Magento Attribute` per **[!UICONTROL Select Magento Product Attribute]**.

   L&#39;attributo viene mappato sul **[!UICONTROL Amazon Attribute Name]**.

1. Inserisci un **[!UICONTROL Magento Product Attribute Name]**.

1. Inserisci un **[!UICONTROL Magento Product Attribute Code]**.

   Questo valore deve essere tutto minuscolo senza spazi.

1. Per **[!UICONTROL Attribute Set Ids]**, scegli un set di attributi da assegnare.

   In genere, gli attributi fanno parte di un set di attributi, ad esempio un set per i colori con attributi per blu, verde, giallo e rosso.

1. Per **[!UICONTROL Type]**, scegli il tipo di valore dell’attributo, ad esempio testo e numeri.

   Questa opzione influisce sul valore consentito per l&#39;attributo.

1. Per **[!UICONTROL Use for Promo Rule Conditions]**, impostato su `Yes` per consentire all’attributo di essere disponibile per un parametro nelle condizioni promozionali.

1. Per **[!UICONTROL Used in Search]**, impostato su `Yes` se l’attributo e il valore possono essere utilizzati nelle ricerche di prodotto.

1. Per **[!UICONTROL Comparable on Storefront]**, impostato su `Yes` se il valore dell’attributo può essere utilizzato nella funzionalità &quot;Confronta per&quot; di Amazon.

1. Scegli la [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} per l&#39;attributo, quindi seleziona una o più visualizzazioni store in cui importare i valori Amazon.

   Se l&#39;ambito è impostato su `Global`, _[!UICONTROL Store View]_non può essere modificato dopo la creazione dell&#39;attributo.

   Se scegli `All Store Views (Global)`, sincronizza e salva i valori in tutte le viste Amazon Store. È possibile sincronizzare i valori solo con viste store specifiche.

1. Al termine, fai clic su **[!UICONTROL Save Attribute Settings]**.

Dopo il salvataggio, puoi modificare l’attributo per rivedere le impostazioni e le impostazioni corrispondenti ad Amazon e [!DNL Commerce] valori dell&#39;attributo. Puoi anche indicare se i valori di Amazon devono essere sovrascritti [!DNL Commerce] valori.

![crea impostazioni attributo](assets/amazon-attribute-settings-create.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Is Active] | Indica se questo attributo è attivo e sincronizzato tra Amazon e [!DNL Commerce]. Imposta su `Yes` per garantire i valori degli attributi da Amazon e [!DNL Commerce] rimane sincronizzato per l&#39;attributo selezionato. |
| Seleziona attributo prodotto Magento | Indica l&#39;attributo selezionato da collegare al nome dell&#39;attributo Amazon elencato. Quando crei un attributo, scegli `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | Mostra il nome dell’attributo Amazon scelto. L&#39;attributo selezionato è collegato a questo attributo di Amazon. Non è possibile modificare questo valore tramite [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Indica il nome dell&#39;attributo o l&#39;etichetta. |
| [!UICONTROL Magento Product Attribute Code] | Indica il codice dell&#39;attributo, il tutto in caratteri minuscoli senza spazi. |
| [!UICONTROL Attribute Set Ids] | Indica il set di attributi a cui assegnare l&#39;attributo. Gli attributi tendono a far parte di un set di attributi, ad esempio un set per colori con attributi per blu, verde, giallo e rosso. |
| [!UICONTROL Type] | Indica il tipo di valore del valore dell&#39;attributo, ad esempio testo e numeri. La selezione influisce sul valore consentito per l&#39;attributo. |
| [!UICONTROL Use for Promo Rule Conditions] | Passa a `Yes` per consentire all’attributo di essere disponibile per un parametro nelle condizioni promozionali. |
| [!UICONTROL Used in Search] | Indica se l’attributo e il valore possono essere utilizzati nelle ricerche di prodotto. |
| [!UICONTROL Comparable on Storefront] | Indica se il valore dell&#39;attributo può essere utilizzato nella funzionalità &quot;Confronta per&quot; di Amazon. |
| [!UICONTROL Magento Product Attribute Scope] | Indica la [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} per l&#39;attributo. Opzioni: Visualizzazione globale/Store<br>Quando è impostato su `Global`, la visualizzazione archivio non può essere modificata dopo la creazione dell&#39;attributo. |
| [!UICONTROL Store Views (to import values into to)] | Viene visualizzato solo quando l&#39;ambito è impostato su `Store View`. Scegli la [vista store](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} a cui vengono sincronizzati i valori dell&#39;attributo Amazon. Scelta `All Store Views (Global)` aggiorna il valore in tutti [!DNL Commerce] memorizzare le visualizzazioni. |

## Modificare un attributo {#edit-an-attribute}

1. Sulla _Amministratore_ barra laterale, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e fai clic su **[!UICONTROL Edit]** in _[!UICONTROL Action]_colonna.

1. Per abilitare o disabilitare la sincronizzazione dei valori di Amazon ai [!DNL Commerce] attributo, set **È attivo** a `Yes` o `No`.

   Quando è impostato su `Yes`, i valori vengono sincronizzati in base alla configurazione.

1. Per **[!UICONTROL Select Magento Product Attribute]**, verifica o aggiorna l&#39;attributo da mappare al **[!UICONTROL Amazon Attribute Name]**.

1. Indica se desideri che il valore dell&#39;attributo Amazon in arrivo sovrascriva il valore dell&#39;attributo esistente.

   Ad esempio, potrebbe non essere utile sovrascrivere i prezzi di Amazon in [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Mantiene il valore, mantenendo valori diversi per il tuo [!DNL Commerce] e Amazon.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Sovrascrive il valore nel [!DNL Commerce] catalogo di prodotto con il valore Amazon in arrivo.

1. Se disponibile per la modifica, scegli uno o più **[!UICONTROL Store Views (to import Amazon values into)]**.

   Se l&#39;attributo è stato creato con un `Global` il campo di applicazione _Visualizzazione store_ non può essere modificato dopo la creazione dell&#39;attributo.

   Se scegli `All Store Views (Global)`, sincronizza e salva i valori in tutte le viste store. È possibile sincronizzare i valori solo con viste store specifiche.

1. Al termine, fai clic su **[!UICONTROL Save Attribute Settings]**.

![modificare le impostazioni degli attributi](assets/amazon-attribute-settings-edit.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Is Active] | Indica se questo attributo è attivo e sincronizzato tra Amazon e [!DNL Commerce]. Imposta su `Yes` per garantire i valori degli attributi da Amazon e [!DNL Commerce] rimane sincronizzato per l&#39;attributo selezionato. |
| [!UICONTROL Select Magento Product Attribute] | Indica il [!DNL Commerce] attributo da collegare al nome dell&#39;attributo Amazon elencato. Se si desidera modificare i collegamenti [!DNL Commerce] , scegli un attributo diverso dall’elenco a discesa. I valori si sincronizzano in base alle configurazioni. |
| [!UICONTROL Amazon Attribute Name] | Mostra il nome dell’attributo Amazon come definito in [!DNL Amazon Seller Central]. Il [!DNL Commerce] collegamenti di attributi a questo attributo Amazon. Non è possibile modificare questo valore tramite [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Indica se i valori degli attributi di Amazon sovrascrivono quelli esistenti [!DNL Commerce] valori, che interessano tutti i prodotti con questo [!DNL Commerce] attributo.<ul><li>**Non sovrascrivere i valori dei Magenti esistenti** - (Predefinito) Mantiene il [!DNL Commerce] valore, mantenendo valori diversi per [!DNL Commerce] e Amazon.</li><li>**Sovrascrivi valori di Magento esistenti** - Salva il valore di Amazon sul [!DNL Commerce] nel [!DNL Commerce] catalogo dei prodotti.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Non viene visualizzato durante la modifica di un attributo se l&#39;attributo è stato creato con `Global` ambito di applicazione. Indica la [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;} creato e impostato su `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Scegli la tua [!DNL Commerce] [vista store](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} a cui sincronizzare i valori degli attributi Amazon. Scelta `All Store Views (Global)` aggiorna il valore in tutte le viste store. |
