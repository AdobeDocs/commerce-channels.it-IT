---
title: '"[!DNL Walmart] Requisiti"'
description: '"Verifica di disporre del[!DNL Walmart Marketplace]informazioni e risorse da integrare con Channel Manager."'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 07e1faf90676b404e3f5ee28ddc13d81ea82a5a5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Walmart] requisiti

[!DNL Channel Manager] richiede le risorse e le informazioni seguenti per configurare un [!DNL Commerce] canale di vendita per [!DNL Walmart Marketplace.]

* Autorizzazione a vendere [!DNL Walmart] e le credenziali per accedere all&#39;account del venditore di Marketplace registrato

* Una chiave API per collegare Adobe Commerce o Magento Open Source a [!DNL Walmart Marketplace]

   La [!DNL Walmart Marketplace] La chiave API consente l’integrazione tra [!DNL Channel Manager] per Adobe Commerce o Magenti Open Source e il Marketplace Walmart. Imposta la chiave API in Seller Central prima di avviare il processo di onboarding di Channel Manager.

## Imposta un [!DNL Walmart Seller] account

1. [Invia la tua richiesta di vendita Walmart](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. Dopo aver ottenuto l&#39;approvazione da [!DNL Walmart], [configurare il tuo account di Venditore Walmart](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Genera un [!DNL Walmart Marketplace] Chiave API di produzione

1. Vai a [!DNL Walmart Marketplace] per generare un [ad Adobe la chiave API di produzione del provider di soluzioni](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

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

## [!DNL Walmart Marketplace] Stato del negozio

Quando colleghi i prodotti al marketplace, la disponibilità dell&#39;elenco dipende dallo stato del tuo [!DNL Walmart Marketplace] negozi:

* Per gli archivi live, le offerte dei prodotti sono elencate e disponibili per la vendita al termine dell’operazione di abbinamento.

* Per i negozi che non sono in diretta, le offerte di prodotto sono organizzate e non sono visibili ai clienti. Quando il [!DNL Walmart Marketplace] il negozio va in diretta, le inserzioni in serie vengono inviate automaticamente al negozio live.

![[!DNL Walmart Seller Central] prodotti a cascata](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>Dopo [!DNL Channel Manager] è installato e configurato, tutti gli aggiornamenti di inventario, prezzo, ordine vengono sincronizzati automaticamente. Non collegare Channel Manager a un negozio Walmart Marketplace live finché non avrai disabilitato altre integrazioni che aggiornano i dati di prodotto e ordine e sei pronto per la sincronizzazione degli aggiornamenti Commerce con [!DNL Walmart Marketplace].

