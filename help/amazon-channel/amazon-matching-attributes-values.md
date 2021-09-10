---
title: Visualizzare la mappatura degli attributi di Amazon
description: Verifica i valori degli attributi Commerce collegati per la corretta sincronizzazione tra Commerce e Amazon.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Visualizzare la mappatura degli attributi Amazon

Quando mappi gli attributi Amazon agli attributi [!DNL Commerce], il canale di vendita Amazon tiene traccia e fornisce un elenco filtrabile di tutti i valori Amazon. Usa questa pagina per verificare la corretta sincronizzazione dei valori per gli attributi collegati [!DNL Commerce] tra [!DNL Commerce] e Amazon. Puoi rivedere i valori sincronizzati per gli attributi Amazon collegati o non collegati a un attributo [!DNL Commerce] . Per creare o modificare gli attributi di Amazon, consulta [Creazione e modifica di attributi](./creating-attributes.md).

Il _valore Amazon_ varia a seconda del tipo di attributo e dell&#39;attributo Amazon visualizzato. Ad esempio, un valore Amazon elencato per `Label` è un valore di testo, mentre `AmazonListPrice` è un valore numerico. Lo stato indica se il valore Amazon è stato importato.

## Visualizza i valori degli attributi

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e fai clic su **[!UICONTROL Create]** o **[!UICONTROL Edit]** nella colonna _[!UICONTROL Action]_.

1. Fai clic sulla scheda **[!UICONTROL Matching Attribute Values]** .

   Gli elenchi con un prodotto di catalogo [!DNL Commerce] corrispondente mostrano un valore collegato nella colonna _SKU del prodotto di Magento_. Facendo clic su un collegamento si apre la pagina corrispondente dei dettagli del prodotto del catalogo. Le modifiche apportate agli attributi di Amazon nella pagina dei dettagli del prodotto non vengono sincronizzate nuovamente sul canale di vendita Amazon.

>[!TIP]
>Per modificare o assegnare la mappatura di un elenco a un prodotto di catalogo, consulta [Aggiornare le informazioni richieste](./amazon-manually-update-incomplete-listing.md).

![Visualizza valori attributo](assets/amazon-managing-attribute-values.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Region] | L&#39;area per l&#39;attività di vendita definita in **[!DNL Amazon Marketplace]Paese** durante l&#39;integrazione dello store. |
| [!UICONTROL Magento Product SKU] | Indica i prodotti [!DNL Commerce] sincronizzati con l&#39;archivio Amazon. Il valore è un ID prodotto assegnato da [!DNL Commerce] e collegato a un prodotto nel catalogo. Per aprire il prodotto in [!DNL Commerce], fai clic sul collegamento . |
| [!UICONTROL ASIN] | Indica il numero di identificazione standard Amazon (ASIN) a 10 caratteri dell’identificatore univoco alfanumerico assegnato al prodotto da Amazon per l’identificazione del prodotto. |
| [!UICONTROL Amazon Value] | Indica il valore dell&#39;attributo selezionato. Il valore di Amazon varia a seconda del tipo di attributo e dell’attributo di Amazon visualizzato. Ad esempio, un valore Amazon elencato per `Label` è un valore di testo, mentre `AmazonListPrice` è un valore numerico. Lo stato indica se il valore Amazon è stato importato. |
| [!UICONTROL Status] | Indica se i valori dell&#39;attributo sono stati importati in [!DNL Commerce] e collegati a un attributo [!DNL Commerce] . Opzioni: `Not Imported` / `Imported` |
