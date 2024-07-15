---
title: Mappa attributi catalogo
description: 'Mappa attributi per corrispondenza [DNL! Commerce] prodotti alle  [!DNL Walmart Marketplace] inserzioni esistenti e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart].'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Mappa attributi catalogo

Prima di connettere le inserzioni da [!DNL Commerce] a [!DNL Walmart Marketplace], è necessario mappare almeno un identificatore univoco del catalogo [!DNL Commerce] all&#39;identificatore corrispondente di Walmart.

Questo passaggio è necessario per far corrispondere [!DNL Commerce] prodotti con [!DNL Walmart] inserzioni esistenti e per sincronizzare i dati dei prodotti tra [!DNL Commerce] e [!DNL Walmart]. Il prodotto [!DNL Commerce] deve avere almeno un attributo di prodotto che corrisponda a uno dei seguenti identificatori di prodotto (ID prodotto) richiesti da [!DNL Walmart].

**Richiesti [!DNL Walmart] ID prodotto**

| **Tipo accettato** | **Nome** | **Scopo** | **Cifre Accettabili** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Articolo commerciale globale | Uso generale, utilizzato in tutto il mondo | 14 cifre |
| ISBN | Numero internazionale standard del libro | Cartaceo, copertina rigida e libri elettronici | 10 o 13 cifre |
| ISSN | Numero di serie standard internazionale | Numero di serie a 8 cifre utilizzato per identificare riviste, giornali, quotidiani e periodici di ogni tipo consegnati su tutti i supporti cartacei ed elettronici | 8 cifre |
| UPC | Codice prodotto universale | Codice di tracciamento standard per la vendita al dettaglio | 12 cifre |

Se il catalogo non ha un attributo corrispondente, [aggiungi o converti un attributo di catalogo esistente](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

## Mappare identificatori univoci

1. Dalla pagina **[!UICONTROL Listings]** o **[!UICONTROL Orders]** per lo store dei canali di vendita, selezionare **[!UICONTROL Channel Settings]**.

1. In **[!UICONTROL Channel Settings]**, selezionare **[!UICONTROL Map Attributes]**.

   - Trovare l&#39;attributo [!DNL Walmart Marketplace] da mappare.

   - Selezionare l&#39;attributo corrispondente dal catalogo dell&#39;archivio [!DNL Commerce].

     Nell&#39;esempio seguente l&#39;attributo [!UICONTROL Walmart Marketplace UPC] viene mappato sull&#39;attributo UPC nel catalogo prodotti.

     ![Mappa gli attributi per i criteri di corrispondenza prodotto](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - Selezionare **[!UICONTROL Save]**.
