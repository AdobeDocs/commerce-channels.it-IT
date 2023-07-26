---
title: Attributi per le inserzioni Amazon
description: Il Sales Channel Amazon fornisce [!UICONTROL Attributes] per monitorare l’elenco degli attributi di Amazon e Commerce e come vengono mappati per la corrispondenza dei prodotti.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Attributi per le inserzioni Amazon

Il _[!UICONTROL Attributes]_visualizza il tuo elenco di Amazon e [!DNL Commerce] attributi. L’elenco indica anche gli attributi mappati per la corrispondenza del prodotto. Per ulteriori informazioni, consulta [Gestisci attributi](./managing-attributes.md).

![Visualizzazione Attributi](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Dalla sezione _[!UICONTROL Attributes]_visualizzare, controllare le impostazioni degli attributi nella tabella e [creare o modificare](./creating-attributes.md) un attributo.

## Visualizzare l&#39;elenco degli attributi

1. Il giorno _Amministratore_ barra laterale, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Clic **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e controlla l’elenco degli attributi.

1. Crea o modifica un attributo, in base alle esigenze:

   - A [creare](./creating-attributes.md#create-an-attribute) e definire i valori degli attributi corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Create]**.

   - Per disattivare o [modificare le impostazioni](./creating-attributes.md#edit-an-attribute) o Corrispondenza valori attributo per l&#39;attributo, fare clic su **[!UICONTROL Edit]**.

     La modifica di un attributo include la modifica del mapping di attributi per la corrispondenza di prodotti.

| Campo | Descrizione |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Il paese per l&#39;attività di vendita definito in  **[!DNL Amazon Marketplace]Paese** durante [integrazione store](./store-integration.md). |
| [!UICONTROL ID] | Valore attributo generico generato da [!DNL Commerce] quando viene creato l’attributo. |
| [!UICONTROL Amazon Attribute Name] | Nome dell’attributo importato da Amazon. |
| [!UICONTROL Product Catalog Attribute Code] | Se mappato, il [!DNL Commerce] attributo assegnato per la mappatura a _[!UICONTROL Amazon Attribute Name]_per trovare i prodotti del catalogo e dell&#39;elenco corrispondenti. |
| [!UICONTROL Overwrite Magento Values] | Se l’attributo è impostato su `Overwrite Existing Magento Values` nella tabella Impostazioni attributo è riportata `Enabled`. Abilitato significa che quando vengono ricevute da Amazon informazioni di prodotto aggiornate per l’attributo, le nuove informazioni aggiornano (sovrascrivono) le informazioni corrispondenti per il prodotto nel [!DNL Commerce] catalogo. Può anche interessare i prodotti elencati nel [!DNL Commerce] negozi. |
| Stato | Indica se i valori degli attributi sono stati importati in [!DNL Commerce] e mappato a una [!DNL Commerce] attributo. Opzioni: `Enabled` / `Disabled` |
| Azione | Indica le opzioni dell&#39;attività disponibili per l&#39;attributo. Opzioni: `Create` / `Edit` |
