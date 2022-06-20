---
title: Mappare gli attributi del catalogo
description: Mappa gli attributi per la corrispondenza [DNL! Prodotti Commerce a quelli esistenti [!DNL Walmart Marketplace] elenchi e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart].
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 97128dcf45d7672e958c771f88389aba40c6e39e
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Mappare gli attributi del catalogo

Prima di collegare gli elenchi da [!DNL Commerce] a [!DNL Walmart Marketplace], devi mappare almeno un identificatore univoco dal tuo [!DNL Commerce] catalogo con l&#39;identificatore corrispondente da Walmart.

Questo passaggio deve corrispondere a [!DNL Commerce] prodotti a quelli esistenti [!DNL Walmart] elenchi e sincronizzazione dei dati dei prodotti tra [!DNL Commerce] e [!DNL Walmart]. La [!DNL Commerce] il prodotto deve avere almeno un attributo di prodotto che corrisponda a uno dei seguenti ID prodotto (ID prodotto) richiesti da [!DNL Walmart].

**Obbligatorio [!DNL Walmart] ID prodotto**

| **Tipo accettato** | **Nome** | **Finalità** | **Cifre accettabili** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Articolo commerciale globale | Scopo generale, utilizzato in tutto il mondo | 14 cifre |
| ISBN | Numero del registro standard internazionale | Libri elettronici, coperture e libri cartacei | 10 o 13 cifre |
| ISSN | Numero di serie standard internazionale | Numero di serie a 8 cifre utilizzato per identificare riviste, riviste, giornali e periodici di tutti i tipi consegnati su tutti i supporti-stampa ed elettronici | 8 cifre |
| UPC | Codice prodotto universale | Codice di tracciamento per la vendita al dettaglio standard | 12 cifre |

Se il catalogo non ha un attributo corrispondente, [aggiungere o convertire un attributo di catalogo esistente](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Mappare identificatori univoci

1. Da **[!UICONTROL Listings]** o **[!UICONTROL Orders]** pagina per l&#39;archivio canali di vendita, seleziona **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, seleziona **[!UICONTROL Shipping Carriers]**.

   - Trova il [!DNL Walmart Marketplace] attributo da mappare.

   - Seleziona l’attributo corrispondente dal [!DNL Commerce] memorizzare il catalogo.

      L’esempio seguente mappa il [!UICONTROL Walmart Marketplace UPC] attributo all&#39;attributo UPC nel catalogo dei prodotti.
   ![Mappatura attributi per i criteri di corrispondenza dei prodotti](assets/products-map-attributes-for-match.png)

   - Seleziona **[!UICONTROL Save]**.


