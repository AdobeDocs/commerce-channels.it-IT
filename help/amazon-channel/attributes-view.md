---
title: Attributi
description: Amazon Sales Channel fornisce [!UICONTROL Attributes] per monitorare l’elenco degli attributi Amazon e Commerce e come vengono mappati per la corrispondenza dei prodotti.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Attributi

La _[!UICONTROL Attributes]_visualizza l’elenco di Amazon e [!DNL Commerce] attributi. L’elenco indica anche gli attributi mappati per la corrispondenza del prodotto. Per ulteriori informazioni, consulta [Gestisci attributi](./managing-attributes.md).

![Visualizzazione Attributi](assets/amazon-attributes-view.png)

Da _[!UICONTROL Attributes]_visualizza e rivedi le impostazioni degli attributi nella tabella e [creare o modificare](./creating-attributes.md) un attributo.

## Visualizza l’elenco degli attributi

1. Sulla _Amministratore_ barra laterale, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo Amazon e controlla l’elenco degli attributi.

1. Crea o modifica un attributo in base alle esigenze:

   - A [creare](./creating-attributes.md#create-an-attribute) e definire i valori degli attributi corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Create]**.

   - Per disattivare o [modificare le impostazioni](./creating-attributes.md#edit-an-attribute) Per i valori degli attributi corrispondenti, fare clic su **[!UICONTROL Edit]**.

      La modifica di un attributo include la modifica della mappatura degli attributi per la corrispondenza del prodotto.

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Country] | Il paese per l&#39;attività di vendita definito in  **[!DNL Amazon Marketplace]Paese** durante [integrazione store](./store-integration.md). |
| [!UICONTROL ID] | Valore dell&#39;attributo generico generato da [!DNL Commerce] quando viene creato l&#39;attributo. |
| [!UICONTROL Amazon Attribute Name] | Nome dell’attributo importato da Amazon. |
| [!UICONTROL Product Catalog Attribute Code] | Se mappata, la [!DNL Commerce] attributo assegnato alla mappatura _[!UICONTROL Amazon Attribute Name]_per i prodotti catalogo ed elenco corrispondenti. |
| [!UICONTROL Overwrite Magento Values] | Se l&#39;attributo è impostato su `Overwrite Existing Magento Values` in Impostazioni attributo, la tabella mostra `Enabled`. Attivato significa che quando le informazioni di prodotto aggiornate per l’attributo vengono ricevute da Amazon, le nuove informazioni aggiornano (sovrascrivono) le informazioni corrispondenti per il prodotto nel [!DNL Commerce] catalogo. Può anche influenzare i prodotti elencati nel [!DNL Commerce] negozi. |
| Stato | Indica se i valori dell&#39;attributo sono stati importati in [!DNL Commerce] e mappato su un [!DNL Commerce] attributo. Opzioni: `Enabled` / `Disabled` |
| Azione | Indica le opzioni dell&#39;attività disponibili per l&#39;attributo. Opzioni: `Create` / `Edit` |
