---
title: Mappare gli attributi del catalogo
description: Mappa gli attributi per la corrispondenza [DNL! Prodotti Commerce a quelli esistenti [!DNL Walmart Marketplace] elenchi e sincronizzazione dei dati tra [!DNL Channel Manager] e [!DNL Walmart].
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: f1c37111df2f566b9673946bb9b2b282506f990c
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Mappare gli attributi del catalogo

Prima di pubblicare gli elenchi da [!DNL Commerce] a [!DNL Walmart Marketplace], devi mappare almeno un identificatore univoco dal tuo [!DNL Commerce] catalogo con l&#39;identificatore corrispondente da Walmart.
Questo passaggio deve corrispondere a [!DNL Commerce] prodotti a quelli esistenti [!DNL Walmart] elenchi e sincronizzazione dei dati dei prodotti tra [!DNL Commerce] e [!DNL Walmart].

Per la corrispondenza dei prodotti, la [!DNL Commerce] il prodotto deve avere almeno un attributo di prodotto che corrisponda a uno dei seguenti ID prodotto (ID prodotto) richiesti da [!DNL Walmart].

**Obbligatorio [!DNL Walmart] ID prodotto**

| **Tipo accettato** | **Nome** | **Finalità** | **Cifre accettabili** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Articolo commerciale globale | Scopo generale, utilizzato in tutto il mondo | 14 cifre |
| ISBN | Numero del registro standard internazionale | Libri elettronici, coperture e libri cartacei | 10 o 13 cifre |
| ISSN | Numero di serie standard internazionale | Numero di serie a 8 cifre utilizzato per identificare riviste, riviste, giornali e periodici di tutti i tipi consegnati su tutti i supporti-stampa ed elettronici | 8 cifre |
| UPC | Codice prodotto universale | Codice di tracciamento per la vendita al dettaglio standard | 12 cifre |

Se il catalogo non ha un attributo corrispondente, [aggiungere o convertire un attributo di catalogo esistente](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Mappare identificatori univoci

1. Sulla [!UICONTROL Listings] pagina per l&#39;archivio canali di vendita, seleziona **[!UICONTROL Settings]**.

   - Trova il [!DNL Walmart Marketplace] attributo da mappare.

   - Seleziona l’attributo corrispondente dal [!DNL Commerce] memorizzare il catalogo.

      L’esempio seguente mappa il [!UICONTROL Walmart Marketplace UPC] attributo all&#39;attributo UPC nel catalogo dei prodotti.
   ![Mappatura attributi per i criteri di corrispondenza dei prodotti](assets/products-map-attributes-for-match.png)
   - Facoltativamente, puoi mappare più attributi per aumentare le corrispondenze. Se mappi più attributi, selezionane uno come **Identificatore principale**. Questo

   - Seleziona **[!UICONTROL Save]**.


## Aggiorna la configurazione degli attributi mappati

Modifica l’identificatore di prodotto Commerce per i prodotti corrispondenti aggiornando le impostazioni di attributi mappate.

Ad esempio, invece di abbinare i prodotti in base al codice dell’attributo del prodotto Commerce UPC, puoi eseguire la corrispondenza in base allo SKU. Oppure, mappa attributi aggiuntivi per migliorare la corrispondenza.

1. Da **[!UICONTROL Listings]**, seleziona **[!UICONTROL Settings]**.

1. Nel modulo dell&#39;attributo Mappa , modifica la configurazione dell&#39;attributo mappato in base alle esigenze.
