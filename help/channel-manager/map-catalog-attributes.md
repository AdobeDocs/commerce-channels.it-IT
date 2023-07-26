---
title: Mappa attributi catalogo
description: '''Mappa attributi per corrispondenza [DNL! Prodotti Commerce] a esistenti [!DNL Walmart Marketplace] elenchi e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart]."'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Mappa attributi catalogo

Prima di connettere le inserzioni da [!DNL Commerce] a [!DNL Walmart Marketplace], devi mappare almeno un identificatore univoco dal tuo [!DNL Commerce] all&#39;identificatore corrispondente di Walmart.

Questo passaggio è necessario per la corrispondenza [!DNL Commerce] prodotti a esistenti [!DNL Walmart] e per sincronizzare i dati di prodotto tra [!DNL Commerce] e [!DNL Walmart]. Il [!DNL Commerce] il prodotto deve avere almeno un attributo di prodotto che corrisponda a uno dei seguenti identificatori di prodotto (ID prodotto) richiesti da [!DNL Walmart].

**Obbligatorio [!DNL Walmart] ID prodotto**

| **Tipo accettato** | **Nome** | **Finalità** | **Cifre accettabili** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Articolo commerciale globale | Uso generale, utilizzato in tutto il mondo | 14 cifre |
| ISBN | Numero internazionale standard del libro | Cartaceo, copertina rigida e libri elettronici | 10 o 13 cifre |
| ISSN | Numero di serie standard internazionale | Numero di serie a 8 cifre utilizzato per identificare riviste, giornali, quotidiani e periodici di ogni tipo consegnati su tutti i supporti cartacei ed elettronici | 8 cifre |
| UPC | Codice prodotto universale | Codice di tracciamento standard per la vendita al dettaglio | 12 cifre |

Se il catalogo non ha un attributo corrispondente, [aggiungere o convertire un attributo di catalogo esistente](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

## Mappare identificatori univoci

1. Dalla sezione **[!UICONTROL Listings]** o **[!UICONTROL Orders]** pagina per il negozio del canale di vendita, seleziona **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, seleziona **[!UICONTROL Map Attributes]**.

   - Trova il [!DNL Walmart Marketplace] attributo da mappare.

   - Seleziona l’attributo corrispondente da [!DNL Commerce] catalogo del negozio.

     L&#39;esempio seguente mappa [!UICONTROL Walmart Marketplace UPC] all’attributo UPC nel catalogo dei prodotti.

     ![Mappa gli attributi per i criteri di corrispondenza prodotto](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - Seleziona **[!UICONTROL Save]**.
