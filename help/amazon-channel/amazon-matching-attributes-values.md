---
title: Visualizza mappatura attributi di Amazon
description: Verifica i valori per gli attributi Commerce collegati per la corretta sincronizzazione tra Commerce e Amazon.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Visualizza mappatura attributi di Amazon

Quando mappi gli attributi Amazon agli attributi [!DNL Commerce], il canale di vendita Amazon tiene traccia e fornisce un elenco filtrabile di tutti i valori Amazon. Utilizzare questa pagina per verificare la corretta sincronizzazione dei valori degli attributi [!DNL Commerce] collegati tra [!DNL Commerce] e Amazon. È possibile rivedere i valori sincronizzati per l&#39;attributo Amazon collegato o non collegato a un attributo [!DNL Commerce]. Per creare o modificare gli attributi di Amazon, vedere [Creazione e modifica degli attributi](./creating-attributes.md).

Il valore _Amazon_ varia a seconda del tipo di attributo e dell&#39;attributo Amazon visualizzato. Ad esempio, un valore Amazon elencato per `Label` sarebbe un valore di testo, mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato.

## Visualizzare i valori degli attributi

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Fare clic su **[!UICONTROL Attributes]** nel menu a sinistra, individuare un attributo Amazon e fare clic su **[!UICONTROL Create]** o **[!UICONTROL Edit]** nella colonna _[!UICONTROL Action]_.

1. Fare clic sulla scheda **[!UICONTROL Matching Attribute Values]**.

   Le inserzioni con un prodotto catalogo [!DNL Commerce] corrispondente mostrano un valore collegato nella colonna _[!UICONTROL Magento Product SKU]_. Facendo clic su un collegamento si apre la pagina dei dettagli del prodotto di catalogo corrispondente. Le modifiche apportate agli attributi di Amazon nella pagina dei dettagli del prodotto non vengono sincronizzate con il canale di vendita di Amazon.

>[!TIP]
>Per modificare o assegnare il mapping per un&#39;inserzione a un prodotto del catalogo, vedere [Aggiorna informazioni richieste](./amazon-manually-update-incomplete-listing.md).

![Visualizza valori attributo](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | L&#39;area per l&#39;attività di vendita definita nel paese **[!DNL Amazon Marketplace]** durante l&#39;integrazione dello store. |
| [!UICONTROL Magento Product SKU] | Indica i prodotti [!DNL Commerce] sincronizzati con l&#39;archivio Amazon. Il valore è un ID prodotto assegnato da [!DNL Commerce] e collegato a un prodotto nel catalogo. Per aprire il prodotto in [!DNL Commerce], fare clic sul collegamento. |
| [!UICONTROL ASIN] | Indica l&#39;identificatore univoco alfanumerico ASIN (Amazon Standard Identification Number) di 10 caratteri assegnato al prodotto da Amazon per l&#39;identificazione del prodotto. |
| [!UICONTROL Amazon Value] | Indica il valore dell&#39;attributo selezionato. Il valore Amazon varia a seconda del tipo di attributo e dell’attributo Amazon visualizzati. Ad esempio, un valore Amazon elencato per `Label` sarebbe un valore di testo, mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato. |
| [!UICONTROL Status] | Indica se i valori dell&#39;attributo sono stati importati in [!DNL Commerce] e collegati a un attributo [!DNL Commerce]. Opzioni: `Not Imported` / `Imported` |
