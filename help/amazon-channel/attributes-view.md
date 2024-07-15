---
title: Attributi per le inserzioni Amazon
description: Il Sales Channel Amazon fornisce la scheda [!UICONTROL Attributes] per monitorare l'elenco degli attributi di Amazon e Commerce e il modo in cui vengono mappati per la corrispondenza dei prodotti.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Attributi per le inserzioni Amazon

La visualizzazione _[!UICONTROL Attributes]_mostra l&#39;elenco degli attributi di Amazon e [!DNL Commerce]. L’elenco indica anche gli attributi mappati per la corrispondenza del prodotto. Per ulteriori informazioni, vedere [Gestione attributi](./managing-attributes.md).

![Visualizzazione attributi](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

Dalla vista _[!UICONTROL Attributes]_, controlla le impostazioni degli attributi nella tabella e [crea o modifica](./creating-attributes.md) un attributo.

## Visualizzare l&#39;elenco degli attributi

1. Nella barra laterale _Admin_, passa a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e controlla l&#39;elenco degli attributi.

1. Crea o modifica un attributo, in base alle esigenze:

   - Per [creare](./creating-attributes.md#create-an-attribute) e definire valori attributo corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Create]**.

   - Per disattivare o [modificare le impostazioni](./creating-attributes.md#edit-an-attribute) o i valori degli attributi corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Edit]**.

     La modifica di un attributo include la modifica del mapping di attributi per la corrispondenza di prodotti.

| Campo | Descrizione |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | Il paese per l&#39;attività di vendita definito nel paese **[!DNL Amazon Marketplace]** durante [l&#39;integrazione dello store](./store-integration.md). |
| [!UICONTROL ID] | Valore di attributo generico generato da [!DNL Commerce] al momento della creazione dell&#39;attributo. |
| [!UICONTROL Amazon Attribute Name] | Nome dell’attributo importato da Amazon. |
| [!UICONTROL Product Catalog Attribute Code] | Se mappato, l&#39;attributo [!DNL Commerce] assegnato a mappare a _[!UICONTROL Amazon Attribute Name]_per i prodotti catalogo ed elenco corrispondenti. |
| [!UICONTROL Overwrite Magento Values] | Se l&#39;attributo è impostato su `Overwrite Existing Magento Values` nelle impostazioni attributo, la tabella mostra `Enabled`. Se l&#39;opzione è abilitata, significa che quando Amazon riceve informazioni aggiornate sul prodotto per l&#39;attributo, le nuove informazioni aggiornano (sovrascrivono) le informazioni corrispondenti per il prodotto nel catalogo [!DNL Commerce]. Può inoltre influire sui prodotti elencati negli store [!DNL Commerce]. |
| Stato | Indica se i valori degli attributi sono stati importati in [!DNL Commerce] e mappati a un attributo [!DNL Commerce]. Opzioni: `Enabled` / `Disabled` |
| Azione | Indica le opzioni dell&#39;attività disponibili per l&#39;attributo. Opzioni: `Create` / `Edit` |
