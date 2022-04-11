---
title: Configurare la corrispondenza dei prodotti
description: Mappare gli attributi per la corrispondenza dei prodotti Commerce agli elenchi esistenti di Walmart Marketplace
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Configurare la corrispondenza dei prodotti

Prima di pubblicare l’elenco su Walmart Marketplace, mappa almeno un identificatore univoco dagli attributi del catalogo dei prodotti a uno degli identificatori di prodotto Walmart Marketplace richiesti. Questo passaggio è necessario per abbinare i prodotti sul Marketplace Walmart.

Per la corrispondenza dei prodotti, il prodotto Commerce deve avere almeno uno dei seguenti ID prodotto (ID prodotto) negli attributi del catalogo.

**ID prodotti Walmart richiesti**

| **Tipo accettato** | **Nome** | **Finalità** | **Cifre accettabili** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Articolo commerciale globale | Scopo generale, utilizzato in tutto il mondo | 14 cifre |
| ISBN | Numero del registro standard internazionale | Libri elettronici, coperture e libri cartacei | 10 o 13 cifre |
| ISSN | Numero di serie standard internazionale | Numero di serie a 8 cifre utilizzato per identificare riviste, riviste, giornali e periodici di tutti i tipi consegnati su tutti i supporti-stampa ed elettronici | 8 cifre |
| ISBN | Numero del registro standard internazionale | Paperback, copertina rigida ed elettronica | 12 cifre |

Se nel catalogo è presente un tipo diverso di attributo ID prodotto, convertirlo in uno dei tipi richiesti. Quindi, mapparla all&#39;attributo Walmart Marketplace corrispondente nella configurazione Listing per l&#39;archivio Channel Manager.

## Configurare le impostazioni degli attributi di prodotto

1. Sulla [!UICONTROL Listings] per il canale di vendita collegato, selezionare uno o più prodotti in *Bozza* stato.

1. Seleziona **[!UICONTROL Settings]**.

   - Trova l&#39;attributo Marketplace Walmart da mappare.

   - Seleziona l&#39;attributo corrispondente dal catalogo store.

      L’esempio seguente mappa l’attributo UPC di Walmart Marketplace all’attributo UPC nel catalogo dei prodotti.
   ![Mappatura attributi per i criteri di corrispondenza dei prodotti](assets/products-map-attributes-for--match.png)

   - Seleziona **[!UICONTROL Save]**.


## Aggiorna la configurazione degli attributi mappati

Modifica l’identificatore di prodotto Commerce per i prodotti corrispondenti aggiornando le impostazioni di attributi mappate.

Ad esempio, invece di abbinare i prodotti in base al codice dell’attributo del prodotto Commerce UPC, puoi eseguire la corrispondenza in base allo SKU. Oppure, mappa attributi aggiuntivi per migliorare la corrispondenza.

1. Da **[!UICONTROL Listings]**, seleziona **[!UICONTROL Settings]**.

1. Nel modulo dell&#39;attributo Mappa , modifica la configurazione dell&#39;attributo mappato in base alle esigenze.
