---
title: '[!DNL Walmart] requisiti'
description: '''Verificare di disporre delle informazioni e delle risorse necessarie [!DNL Walmart Marketplace]per l''integrazione con Channel Manager.'''
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# [!DNL Walmart] requisiti

[!DNL Channel Manager] richiede le risorse e le informazioni seguenti per configurare un canale di vendita [!DNL Commerce] per [!DNL Walmart Marketplace.]

* Un account venditore [!DNL Walmart]

* Chiave API per connettere Adobe Commerce o Magento Open Source a [!DNL Walmart Marketplace]

  La chiave API [!DNL Walmart Marketplace] abilita l&#39;integrazione tra [!DNL Channel Manager], ad Adobe [!DNL Commerce] o Magento Open Source, e Walmart Marketplace. Imposta la chiave API in Seller Central prima di avviare il processo di onboarding di Channel Manager.

## Configura un account [!DNL Walmart Seller]

Vai a [!DNL Walmart Seller Center] per configurare il tuo [account venditore Walmart](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## Genera una chiave API di produzione [!DNL Walmart Marketplace]

1. Vai a [!DNL Walmart Marketplace] per generare una chiave API di produzione del provider di soluzioni [ad Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Crea la chiave e configura le autorizzazioni:

   * Seleziona Adobe come provider di soluzioni.

   * Impostare le autorizzazioni come illustrato nella tabella seguente. Per informazioni dettagliate, vedere [Credenziali API](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) nella _Guida del venditore di Walmart Marketplace_.

   **Adobe configurazione chiave API per Walmart**

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

## Stato dell&#39;archivio [!DNL Walmart Marketplace]

Quando si connettono i prodotti al marketplace, la disponibilità dell&#39;inserzione dipende dallo stato degli store [!DNL Walmart Marketplace]:

* Per i negozi live, le offerte dei tuoi prodotti sono elencate e disponibili per la vendita al termine dell&#39;operazione di partita.

* Per i negozi che non sono live, le offerte di prodotti sono in staging e non visibili ai clienti. Quando l&#39;archivio [!DNL Walmart Marketplace] diventa attivo, le inserzioni in attesa vengono inviate automaticamente all&#39;archivio attivo.

![[!DNL Walmart Seller Central] prodotti in staging](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>Dopo l&#39;installazione e la configurazione di [!DNL Channel Manager], tutti gli aggiornamenti di inventario, prezzo e ordine vengono sincronizzati automaticamente. Non connettere [!DNL Channel Manager] a un archivio di Walmart Marketplace attivo finché non sono state disabilitate altre integrazioni che aggiornano i dati di prodotto e ordine. Se sono state configurate altre integrazioni, verificare che la quantità dell&#39;articolo e i prezzi in [!DNL Commerce] corrispondano alle quantità in [!DNL Walmart Marketplace] prima di connettersi a un negozio live.

