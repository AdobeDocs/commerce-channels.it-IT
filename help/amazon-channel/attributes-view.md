---
title: Attributi
description: Amazon Sales Channel fornisce la scheda [!UICONTROL Attributes] per monitorare l’elenco degli attributi Amazon e Commerce e come vengono mappati per la corrispondenza dei prodotti.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Attributi

La vista _[!UICONTROL Attributes]_mostra l’elenco degli attributi Amazon e [!DNL Commerce] . L’elenco indica anche gli attributi mappati per la corrispondenza del prodotto. Per ulteriori informazioni, consulta [Gestione attributi](./managing-attributes.md).

![Visualizzazione Attributi](assets/amazon-attributes-view.png)

Dalla visualizzazione _[!UICONTROL Attributes]_, controlla le impostazioni dell’attributo nella tabella e [crea o modifica](./creating-attributes.md) un attributo.

## Visualizza l’elenco degli attributi

1. Nella barra laterale _Amministratore_, vai a **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e controlla l’elenco degli attributi.

1. Crea o modifica un attributo in base alle esigenze:

   - Per [creare](./creating-attributes.md#create-an-attribute) e definire i valori degli attributi corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Create]**.

   - Per disattivare o [modificare le impostazioni](./creating-attributes.md#edit-an-attribute) o i valori degli attributi corrispondenti per l&#39;attributo, fare clic su **[!UICONTROL Edit]**.

      La modifica di un attributo include la modifica della mappatura degli attributi per la corrispondenza del prodotto.

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Country] | Il paese per l&#39;attività di vendita definita in **[!DNL Amazon Marketplace]Paese** durante [l&#39;integrazione del negozio](./store-integration.md). |
| [!UICONTROL ID] | Valore dell&#39;attributo generico generato da [!DNL Commerce] al momento della creazione dell&#39;attributo. |
| [!UICONTROL Amazon Attribute Name] | Nome dell’attributo importato da Amazon. |
| [!UICONTROL Product Catalog Attribute Code] | Se mappato, l&#39;attributo [!DNL Commerce] assegnato alla mappatura su _[!UICONTROL Amazon Attribute Name]_per i prodotti di catalogo ed elenco corrispondenti. |
| [!UICONTROL Overwrite Magento Values] | Se l&#39;attributo è impostato su `Overwrite Existing Magento Values` in Impostazioni attributo, la tabella mostra `Enabled`. Attivato significa che quando le informazioni di prodotto aggiornate per l’attributo vengono ricevute da Amazon, le nuove informazioni aggiornano (sovrascrivono) le informazioni corrispondenti per il prodotto nel catalogo [!DNL Commerce]. Può anche influenzare i prodotti elencati nei tuoi [!DNL Commerce] negozi. |
| Stato | Indica se i valori dell&#39;attributo sono stati importati in [!DNL Commerce] e mappati su un attributo [!DNL Commerce]. Opzioni: `Enabled` / `Disabled` |
| Azione | Indica le opzioni dell&#39;attività disponibili per l&#39;attributo. Opzioni: `Create` / `Edit` |
