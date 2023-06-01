---
title: '''[!DNL Walmart] Requisiti"'
description: '''Verifica di disporre dei [!DNL Walmart Marketplace]informazioni e risorse da integrare con Channel Manager."'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# [!DNL Walmart] Requisiti

[!DNL Channel Manager] richiede le risorse e le informazioni seguenti per configurare un [!DNL Commerce] canale di vendita per [!DNL Walmart Marketplace.]

* A [!DNL Walmart] Account del venditore

* Una chiave API a cui collegare Adobe Commerce o Magenti Open Source [!DNL Walmart Marketplace]

   Il [!DNL Walmart Marketplace] Chiave API per abilitare l’integrazione tra [!DNL Channel Manager] ad Adobe [!DNL Commerce] o Magenti Open Source e il Walmart Marketplace. Imposta la chiave API in Seller Central prima di avviare il processo di onboarding di Channel Manager.

## Configurare un [!DNL Walmart Seller] account

Vai a [!DNL Walmart Seller Center] per configurare [Account del venditore Walmart](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## Genera un [!DNL Walmart Marketplace] Chiave API di produzione

1. Vai a [!DNL Walmart Marketplace] per generare un [chiave API di produzione del provider di soluzioni, ad Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Crea la chiave e configura le autorizzazioni:

   * Seleziona Adobe come provider di soluzioni.

   * Impostare le autorizzazioni come illustrato nella tabella seguente. Per ulteriori informazioni, consulta [Credenziali API](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) nel _Aiuto per i venditori di Walmart Marketplace_.

   **Adobe di configurazione della chiave API per Walmart**

   | **Autorizzazione** | **Impostazione** |
   |----------------|-------------|
   | Contenuto | Accesso completo |
   | Ottieni feed | Solo visualizzazione |
   | Inventario | Accesso completo |
   | Elementi | Accesso completo |
   | Tempo di ritardo | Accesso completo |
   | Ordine | Accesso completo |
   | Prezzo | Accesso completo |
   | Rapporti | Solo visualizzazione |
   | Restituisce | Accesso completo |
   | Regole | Accesso completo |
   | Spedizione | Accesso completo |

## [!DNL Walmart Marketplace] Stato store

Quando colleghi i prodotti al marketplace, la disponibilità dell’inserzione dipende dallo stato del [!DNL Walmart Marketplace] archivi:

* Per i negozi live, le offerte dei tuoi prodotti sono elencate e disponibili per la vendita al termine dell&#39;operazione di partita.

* Per i negozi che non sono live, le offerte di prodotti sono in staging e non visibili ai clienti. Quando [!DNL Walmart Marketplace] il negozio diventa live, le inserzioni in staging vengono inviate automaticamente al live store.

![[!DNL Walmart Seller Central] prodotti in staging](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>Dopo [!DNL Channel Manager] è installato e configurato, tutti gli aggiornamenti di inventario, prezzo e ordine vengono sincronizzati automaticamente. Non connettere [!DNL Channel Manager] in un negozio online di Walmart Marketplace fino a quando non vengono disattivate tutte le altre integrazioni che aggiornano i dati di prodotto e ordine. Se hai configurato altre integrazioni, verifica che la quantità e i prezzi dell’articolo in [!DNL Commerce] corrisponde alle quantità in [!DNL Walmart Marketplace] prima di collegarsi a un negozio live.

