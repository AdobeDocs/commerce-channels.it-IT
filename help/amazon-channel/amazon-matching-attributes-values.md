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

Quando mappi gli attributi di Amazon su [!DNL Commerce] attributes, Amazon sales channel traccia e fornisce un elenco filtrabile di tutti i valori Amazon. Utilizzare questa pagina per verificare i valori per i collegamenti [!DNL Commerce] gli attributi vengono sincronizzati correttamente tra [!DNL Commerce] e Amazon. Puoi rivedere i valori sincronizzati per l’attributo Amazon collegato o non collegato a un [!DNL Commerce] attributo. Per creare o modificare gli attributi di Amazon, vedi [Creazione e modifica degli attributi](./creating-attributes.md).

La _Valore Amazon_ varia a seconda del tipo di attributo e dell’attributo Amazon visualizzato. Ad esempio, un valore Amazon elencato per `Label` è un valore di testo mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato.

## Visualizza i valori degli attributi

1. Sulla _[!UICONTROL Admin]_barra laterale, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Fai clic su **[!UICONTROL Attributes]** nel menu a sinistra, individua un attributo di Amazon e fai clic su **[!UICONTROL Create]** o **[!UICONTROL Edit]** in _[!UICONTROL Action]_colonna.

1. Fai clic sul pulsante **[!UICONTROL Matching Attribute Values]** scheda .

   Elenco con un [!DNL Commerce] i prodotti di catalogo mostrano un valore collegato nel _SKU prodotto Magento_ colonna. Facendo clic su un collegamento si apre la pagina corrispondente dei dettagli del prodotto del catalogo. Le modifiche apportate agli attributi di Amazon nella pagina dei dettagli del prodotto non vengono sincronizzate nuovamente sul canale di vendita Amazon.

>[!TIP]
>Per modificare o assegnare la mappatura di un elenco a un prodotto catalogo, vedi [Aggiorna informazioni richieste](./amazon-manually-update-incomplete-listing.md).

![Visualizza valori attributo](assets/amazon-managing-attribute-values.png)

| Campo | Descrizione |
|--- |--- |
| [!UICONTROL Region] | L&#39;area per l&#39;attività di vendita definita in **[!DNL Amazon Marketplace]Paese** durante l&#39;integrazione dello store. |
| [!UICONTROL Magento Product SKU] | Indica la [!DNL Commerce] prodotti sincronizzati con Amazon store. Il valore è un ID prodotto assegnato da [!DNL Commerce] e collegati a un prodotto nel catalogo. Per aprire il prodotto in [!DNL Commerce], fai clic sul collegamento. |
| [!UICONTROL ASIN] | Indica il numero di identificazione standard Amazon (ASIN) a 10 caratteri dell’identificatore univoco alfanumerico assegnato al prodotto da Amazon per l’identificazione del prodotto. |
| [!UICONTROL Amazon Value] | Indica il valore dell&#39;attributo selezionato. Il valore di Amazon varia a seconda del tipo di attributo e dell’attributo di Amazon visualizzato. Ad esempio, un valore Amazon elencato per `Label` è un valore di testo mentre `AmazonListPrice` sarebbe un importo numerico. Lo stato indica se il valore Amazon è stato importato. |
| [!UICONTROL Status] | Indica se i valori dell&#39;attributo sono stati importati in [!DNL Commerce] e collegati a un [!DNL Commerce] attributo. Opzioni: `Not Imported` / `Imported` |
