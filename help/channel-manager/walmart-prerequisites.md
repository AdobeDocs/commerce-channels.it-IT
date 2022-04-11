---
title: Prerequisiti per Walmart
description: Verifica di disporre delle informazioni e delle risorse di Walmart Marketplace necessarie per l'integrazione con Channel Manager.
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Prerequisiti per Walmart

Channel Manager richiede le risorse e le informazioni seguenti per configurare un canale di vendita Commerce per Walmart Marketplace.

* Approvazione per vendere su Walmart e le credenziali per accedere all&#39;account registrato Marketplace Seller

* Una chiave API per collegare Adobe Commerce o Magento Open Source a Walmart Marketplace

   La chiave API Walmart Marketplace consente l&#39;integrazione tra Channel Manager per Adobe Commerce o Magenti Open Source e Walmart Marketplace. Imposta la chiave API in Seller Central prima di avviare il processo di onboarding di Channel Manager.

## Configurare un account venditore di Marketplace

1. [Invia la tua richiesta di vendita Walmart](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. Dopo aver ottenuto l&#39;approvazione da Walmart, [configurare il tuo account di Venditore Walmart](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Genera una chiave API di produzione di Marketplace Walmart

1. Vai a Walmart Marketplace per generare un [ad Adobe la chiave API di produzione del provider di soluzioni](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Crea la chiave e configura le autorizzazioni:

   * Seleziona Adobe come provider della soluzione.

   * Imposta le autorizzazioni come mostrato nella tabella seguente. Per maggiori dettagli, vedi [Credenziali API](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in _Aiuto per i venditori di Marketplace Walmart_.

   **Adobe di configurazione della chiave API per Walmart**

   | **Autorizzazione** | **Impostazione** |
   |----------------|-------------|
   | Contenuto | Accesso completo |
   | Ottieni feed | Solo visualizzazione |
   | Inventario | Accesso completo |
   | Elementi | Accesso completo |
   | Tempo ritardo | Accesso completo |
   | Ordine | Accesso completo |
   | Prezzo | Accesso completo |
   | Rapporti | Solo visualizzazione |
   | Restituisce | Accesso completo |
   | Regole | Accesso completo |
   | Spedizione | Accesso completo |

## Stato del Negozio Marketplace di Walmart

Quando pubblichi i prodotti su Walmart Marketplace, la disponibilità dell&#39;elenco dipende dallo stato dei tuoi negozi Walmart Marketplace:

* Per gli archivi live, le offerte dei prodotti sono elencate e disponibili per la vendita al termine dell’operazione di abbinamento.

* Per i negozi che non sono in diretta, le offerte di prodotto sono organizzate e non sono visibili ai clienti. Quando il negozio è in diretta, le inserzioni in serie vengono inviate automaticamente al Live Store.

![[!DNL Walmart Seller Central] prodotti a cascata](assets/walmart-seller-central-staged.png)
