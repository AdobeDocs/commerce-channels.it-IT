---
title: Creazione e modifica degli attributi per il canale di vendita Amazon
description: Il Sales Channel Amazon fornisce la vista Attributi per aiutarti a rivedere gli attributi Amazon correnti e gli attributi Commerce collegati.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# Creare e modificare gli attributi

Crea o aggiorna gli attributi [!DNL Commerce] mentre vendi tramite Amazon e aggiorna i tuoi negozi. Rivedi gli attributi Amazon correnti e gli attributi [!DNL Commerce] collegati tramite la [_[!UICONTROL Attributes]_visualizzazione](./attributes-view.md) della home page del canale di vendita Amazon. La colonna_[!UICONTROL Action]_ mostra le azioni disponibili per l&#39;attributo. È possibile creare e mappare un nuovo attributo [!DNL Commerce] per un attributo Amazon non collegato oppure modificare un attributo [!DNL Commerce] esistente e il relativo mapping a un attributo Amazon.

Durante la creazione e l&#39;aggiornamento degli attributi, è possibile verificare i valori degli attributi per [!DNL Commerce] e i prodotti Amazon. Questi valori possono essere diversi se non si sincronizzano e non si importano valori da Amazon. Per esaminare i valori Amazon per questi attributi, vedere [Analisi del mapping degli attributi Amazon](./amazon-matching-attributes-values.md). Se desideri modificare questi valori, puoi [modificare o creare una mappatura](./amazon-manually-update-incomplete-listing.md) tra Amazon e [!DNL Commerce].

## Creare un attributo {#create-an-attribute}

Questi passaggi creano un attributo [!DNL Commerce] e lo associano a un attributo Amazon. A seconda delle configurazioni, i valori possono iniziare la sincronizzazione tra i cataloghi.

1. Nella barra laterale _Admin_, passa a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fare clic su **[!UICONTROL Attributes]** nel menu a sinistra, individuare un attributo Amazon e fare clic su **[!UICONTROL Create Attribute]** nella colonna _[!UICONTROL Action]_.

1. Per abilitare la sincronizzazione dei valori Amazon con l&#39;attributo [!DNL Commerce] collegato, impostare **[!UICONTROL Is Active]** su `Yes`.

   Se è impostato su `Yes`, i valori vengono sincronizzati in base alla configurazione.

1. Scegli `Create New Magento Attribute` per **[!UICONTROL Select Magento Product Attribute]**.

   L&#39;attributo è mappato al scelto per **[!UICONTROL Amazon Attribute Name]**.

1. Immetti **[!UICONTROL Magento Product Attribute Name]**.

1. Immetti **[!UICONTROL Magento Product Attribute Code]**.

   Questo valore deve essere tutto minuscolo senza spazi.

1. Per **[!UICONTROL Attribute Set Ids]**, scegliere un set di attributi da assegnare.

   In genere, gli attributi fanno parte di un set di attributi, ad esempio un set per i colori con attributi blu, verde, giallo e rosso.

1. Per **[!UICONTROL Type]**, scegliere il tipo di valore dell&#39;attributo, ad esempio testo e numeri.

   Questa opzione influisce sul valore consentito per l’attributo.

1. Per **[!UICONTROL Use for Promo Rule Conditions]**, impostare su `Yes` per consentire la disponibilità dell&#39;attributo per un parametro nelle condizioni promozionali.

1. Per **[!UICONTROL Used in Search]**, impostare su `Yes` se l&#39;attributo e il valore possono essere utilizzati nelle ricerche di prodotti.

1. Per **[!UICONTROL Comparable on Storefront]**, impostare su `Yes` se il valore dell&#39;attributo può essere utilizzato nella funzionalità &quot;Compare By&quot; di Amazon.

1. Scegliere l&#39;[!DNL Commerce] [ambito](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) per l&#39;attributo, quindi selezionare una o più visualizzazioni archivio in cui importare i valori Amazon.

   Se l&#39;ambito è impostato su `Global`, non è possibile modificare _[!UICONTROL Store View]_dopo la creazione dell&#39;attributo.

   Se si sceglie `All Store Views (Global)`, i valori verranno sincronizzati e salvati in tutte le visualizzazioni dello store di Amazon. Puoi sincronizzare i valori solo con specifiche visualizzazioni archivio.

1. Al termine, fare clic su **[!UICONTROL Save Attribute Settings]**.

Dopo il salvataggio, è possibile modificare l&#39;attributo per esaminare le impostazioni e i valori Amazon e [!DNL Commerce] corrispondenti per l&#39;attributo. Puoi anche indicare se i valori di Amazon devono sovrascrivere [!DNL Commerce] valori.

![crea impostazioni attributo](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Indica se l&#39;attributo è attivo e sincronizza attivamente tra Amazon e [!DNL Commerce]. Imposta su `Yes` per garantire che i valori degli attributi da Amazon e [!DNL Commerce] rimangano sincronizzati per l&#39;attributo selezionato. |
| Seleziona attributo prodotto Magento | Indica l’attributo selezionato che desideri collegare al Nome attributo di Amazon elencato. Durante la creazione di un attributo, scegliere `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | Mostra il nome dell’attributo Amazon scelto. L’attributo selezionato è collegato a questo attributo di Amazon. Impossibile modificare questo valore tramite [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | Indica il nome attributo o &quot;label&quot;. |
| [!UICONTROL Magento Product Attribute Code] | Indica il codice attributo, tutto in caratteri minuscoli senza spazi. |
| [!UICONTROL Attribute Set Ids] | Indica la serie di attributi a cui assegnare l&#39;attributo. Gli attributi tendono a far parte di un set di attributi, ad esempio un set per i colori con attributi per il blu, il verde, il giallo e il rosso. |
| [!UICONTROL Type] | Indica il tipo di valore del valore dell&#39;attributo, ad esempio testo e numeri. La selezione influisce sul valore consentito per l’attributo. |
| [!UICONTROL Use for Promo Rule Conditions] | Attiva `Yes` per consentire la disponibilità dell&#39;attributo per un parametro nelle condizioni promozionali. |
| [!UICONTROL Used in Search] | Indica se l’attributo e il valore possono essere utilizzati nelle ricerche di prodotti. |
| [!UICONTROL Comparable on Storefront] | Indica se il valore dell’attributo può essere utilizzato nella funzionalità &quot;Confronta per&quot; di Amazon. |
| [!UICONTROL Magento Product Attribute Scope] | Indica l&#39;[ambito](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) per l&#39;attributo. Opzioni: Global / Store View<br>Se è impostato su `Global`, non è possibile modificare la Store View dopo la creazione dell&#39;attributo. |
| [!UICONTROL Store Views (to import values into to)] | Viene visualizzato solo se l&#39;ambito è impostato su `Store View`. Scegliere la [visualizzazione archivio](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) in cui vengono sincronizzati i valori degli attributi Amazon. Se si sceglie `All Store Views (Global)`, il valore verrà aggiornato in tutte le [!DNL Commerce] visualizzazioni dello store. |

## Modificare un attributo {#edit-an-attribute}

1. Nella barra laterale _Admin_, passa a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fare clic su **[!UICONTROL Attributes]** nel menu a sinistra, individuare un attributo Amazon e fare clic su **[!UICONTROL Edit]** nella colonna _[!UICONTROL Action]_.

1. Per abilitare o disabilitare la sincronizzazione dei valori Amazon con l&#39;attributo [!DNL Commerce] collegato, impostare **Is Active** su `Yes` o `No`.

   Se è impostato su `Yes`, i valori vengono sincronizzati in base alla configurazione.

1. Per **[!UICONTROL Select Magento Product Attribute]**, verificare o aggiornare l&#39;attributo da mappare al **[!UICONTROL Amazon Attribute Name]** scelto.

1. Indica se desideri che il valore dell’attributo Amazon in entrata sovrascriva il valore dell’attributo esistente.

   Ad esempio, potrebbe non essere necessario sovrascrivere i prezzi da Amazon in [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - Mantiene il valore, mantenendo valori diversi per gli archivi [!DNL Commerce] e Amazon.

   - **[!UICONTROL Overwrite Existing Magento Values]** - Sovrascrive il valore nel catalogo prodotti [!DNL Commerce] con il valore Amazon in ingresso.

1. Se disponibile per la modifica, scegliere uno o più **[!UICONTROL Store Views (to import Amazon values into)]**.

   Se l&#39;attributo è stato creato con un ambito `Global`, la _Visualizzazione archivio_ non può essere modificata dopo la creazione dell&#39;attributo.

   Se si sceglie `All Store Views (Global)`, i valori verranno sincronizzati e salvati in tutte le visualizzazioni dello store. Puoi sincronizzare i valori solo con specifiche visualizzazioni archivio.

1. Al termine, fare clic su **[!UICONTROL Save Attribute Settings]**.

![modifica impostazioni attributo](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | Indica se l&#39;attributo è attivo e sincronizza attivamente tra Amazon e [!DNL Commerce]. Imposta su `Yes` per garantire che i valori degli attributi da Amazon e [!DNL Commerce] rimangano sincronizzati per l&#39;attributo selezionato. |
| [!UICONTROL Select Magento Product Attribute] | Indica l&#39;attributo [!DNL Commerce] selezionato che si desidera collegare al nome dell&#39;attributo Amazon elencato. Se si desidera modificare l&#39;attributo [!DNL Commerce] collegato, scegliere un attributo diverso dall&#39;elenco a discesa. I valori vengono sincronizzati in base alle configurazioni. |
| [!UICONTROL Amazon Attribute Name] | Mostra il nome dell&#39;attributo Amazon definito in [!DNL Amazon Seller Central]. L&#39;attributo [!DNL Commerce] selezionato è collegato a questo attributo di Amazon. Impossibile modificare questo valore tramite [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Indica se i valori dell&#39;attributo Amazon sovrascrivono i valori [!DNL Commerce] esistenti, influendo su tutti i prodotti con questo attributo [!DNL Commerce].<ul><li>**Non sovrascrivere i valori di Magento esistenti** - (impostazione predefinita) Mantiene il valore [!DNL Commerce], mantenendo valori diversi per gli archivi [!DNL Commerce] e Amazon.</li><li>**Sovrascrivi valori Magenti esistenti** - Salva il valore Amazon sul valore [!DNL Commerce] nel catalogo prodotti [!DNL Commerce].</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | Non viene visualizzato quando si modifica un attributo se l&#39;attributo è stato creato con l&#39;ambito `Global`. Indica che l&#39;[!DNL Commerce] [ambito](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) è stato creato e impostato su `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | Scegli la [!DNL Commerce] [vista archivio](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) in cui sincronizzare i valori degli attributi di Amazon. Se si sceglie `All Store Views (Global)`, il valore verrà aggiornato in tutte le visualizzazioni dello store. |
