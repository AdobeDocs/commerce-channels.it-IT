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

Quando mappi gli attributi Amazon a [!DNL Commerce] attributi, canale di vendita Amazon tiene traccia e fornisce un elenco filtrabile di tutti i valori Amazon. Utilizzare questa pagina per verificare i valori per il collegamento [!DNL Commerce] attributi sincronizzati correttamente tra [!DNL Commerce] e Amazon. Puoi rivedere i valori sincronizzati per l&#39;attributo Amazon collegato o non collegato a un [!DNL Commerce] attributo. Per creare o modificare gli attributi di Amazon, consulta [Creazione e modifica di attributi](./creating-attributes.md).

Il _Valore Amazon_ varia a seconda del tipo di attributo e dell’attributo Amazon visualizzati. Ad esempio, un valore Amazon elencato per `Label` sarebbe un valore di testo mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato.

## Visualizzare i valori degli attributi

1. Il giorno _[!UICONTROL Admin]_barra laterale, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Clic **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e fai clic su **[!UICONTROL Create]** o **[!UICONTROL Edit]** nel _[!UICONTROL Action]_colonna.

1. Fai clic su **[!UICONTROL Matching Attribute Values]** scheda.

   Le inserzioni che hanno un corrispondente [!DNL Commerce] il prodotto di catalogo mostra un valore collegato nel _[!UICONTROL Magento Product SKU]_colonna. Facendo clic su un collegamento si apre la pagina dei dettagli del prodotto di catalogo corrispondente. Le modifiche apportate agli attributi di Amazon nella pagina dei dettagli del prodotto non vengono sincronizzate con il canale di vendita di Amazon.

>[!TIP]
>Per modificare o assegnare il mapping per un&#39;inserzione a un prodotto catalogo, vedere [Aggiorna informazioni richieste](./amazon-manually-update-incomplete-listing.md).

![Visualizza valori attributo](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Campo | Descrizione |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | Area per l&#39;attività di vendita definita in **[!DNL Amazon Marketplace]Paese** durante l’integrazione del punto vendita. |
| [!UICONTROL Magento Product SKU] | Indica il [!DNL Commerce] prodotti sincronizzati con Amazon store. Il valore è un ID prodotto assegnato da [!DNL Commerce] e collegati a un prodotto nel catalogo. Per aprire il prodotto in [!DNL Commerce], fai clic sul collegamento. |
| [!UICONTROL ASIN] | Indica l&#39;identificatore univoco alfanumerico ASIN (Amazon Standard Identification Number) di 10 caratteri assegnato al prodotto da Amazon per l&#39;identificazione del prodotto. |
| [!UICONTROL Amazon Value] | Indica il valore dell&#39;attributo selezionato. Il valore Amazon varia a seconda del tipo di attributo e dell’attributo Amazon visualizzati. Ad esempio, un valore Amazon elencato per `Label` sarebbe un valore di testo mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato. |
| [!UICONTROL Status] | Indica se i valori degli attributi sono stati importati in [!DNL Commerce] e collegato a un [!DNL Commerce] attributo. Opzioni: `Not Imported` / `Imported` |
