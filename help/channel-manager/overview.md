---
title: Informazioni [!DNL Channel Manager]
description: Scopri come installare e utilizzare [!DNL Channel Manager] per integrare Adobe Commerce e i negozi di Magento Open Source con i marketplace di terze parti e creare un canale di vendita per gestire gli elenchi di marketplace, i prezzi, le scorte e le vendite in modo semplice dall’amministratore Commerce.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 7412a3d5b78e206521a048fb56edacd8f11ddb58
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Panoramica

Channel Manager per Adobe Commerce e Magenti Open Source offre uno spazio di lavoro utile nell&#39;amministratore per gestire le vendite di canali su mercati di terze parti come Walmart, Amazon ed eBay. Aumenta le vendite ed espandi verso nuovi mercati, gestendo al contempo le operazioni dei canali di vendita direttamente dal tuo amministratore Commerce.

![[!DNL Channel Manager] vista amministratore dell&#39;estensione](assets/channel-manager-admin-entry-page.png)

## Panoramica sulla versione beta

La versione beta di Channel Manager supporta Adobe Commerce o i venditori di Magenti Open Source che desiderano offrire prodotti su Walmart Marketplace.

Questa versione supporta le seguenti funzionalità per gestire le operazioni sui canali di vendita:

* Stabilire una connessione API tra Adobe Commerce o Magenti Open Source e Walmart Marketplace

* Pubblicare prodotti da Channel Manager a Walmart utilizzando la corrispondenza dei prodotti

* Visualizza lo stato dell’elenco dei prodotti in Channel Manager, ad esempio *disegno*, *elaborazione*, *corrispondente*, *errore*.

* Sincronizza le quantità di scorte dei prodotti abbinati da Commerce a Walmart

* Sincronizza i prezzi dei cataloghi per i prodotti abbinati da Commerce a Walmart

* Ricevi ordini da Walmart Marketplace e visualizzali in [!DNL Commerce] quadro comandi

### Latenza prevista per le operazioni di Channel Manager

I processi di sincronizzazione dei dati tra [!DNL Channel Manager] e collegati [!DNL Walmart Marketplace] archiviare richiede un po&#39; di tempo per completare. Esamina il tempo di elaborazione previsto per [!DNL Channel Manager] operazioni che consentono di pianificare il funzionamento dei canali di vendita.

**Latenza stimata per le operazioni di Channel Manager**

| **Funzionamento** | **Descrizione** | **Ritardo previsto** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| Aggiungi prodotti a Channel Manager | Seleziona i prodotti dal catalogo di prodotti Commerce e importali in Channel Manager. | **Fino a 5 minuti**- Se selezioni molti prodotti, ad esempio un intero catalogo di prodotti, il processo di importazione richiede più tempo. |
| Confronta prodotti su Walmart Marketplace | Seleziona gli elenchi dei prodotti in Channel Manager e inviali a Walmart per la corrispondenza. | **Fino a 30 minuti**- Se selezioni molti prodotti, il processo di corrispondenza richiede più tempo a seconda della quantità selezionata. |
| Aggiornamenti dell&#39;inventario | Quando la quantità di inventario cambia in Commerce. Channel Manager sincronizza l&#39;aggiornamento a Walmart. | **Fino a 10 minuti** |
| Aggiornamenti dei prezzi | Quando il prezzo di un prodotto cambia, Channel Manager sincronizza l&#39;aggiornamento a Walmart. | **Fino a 5 minuti** |
| Ordinare sincronizzazioni da Walmart a Commerce | Il cliente ordina un prodotto Commerce su Walmart Marketplace. Walmart invia l&#39;ordine a Channel Manager. L’ordine viene visualizzato nel dashboard dell’ordine. | **Fino a 30 minuti** |
| Ordine creato in Commerce Order Management | Channel Manager crea l’ordine Commerce dall’ordine Walmart e aggiorna il dashboard dell’ordine in modo da includere il numero dell’ordine Commerce. | **Fino a 5 minuti** |

## Prerequisiti per Walmart

Per integrare Commerce con Walmart Marketplace, è necessario disporre delle seguenti informazioni da parte di Walmart:

* Approvazione per vendere su Walmart e le credenziali per accedere all&#39;account registrato Marketplace Seller

* Una chiave API per collegare Adobe Commerce o Magento Open Source a Walmart Marketplace

   La chiave API Walmart Marketplace consente l&#39;integrazione tra Channel Manager per Adobe Commerce o Magenti Open Source e Walmart Marketplace. Imposta la chiave API in Seller Central prima di avviare il processo di onboarding di Channel Manager.

### Configurare un account venditore di Marketplace

1. [Invia la tua richiesta di vendita Walmart](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
2. Dopo aver ottenuto l&#39;approvazione da Walmart, [configurare il tuo account di Venditore Walmart](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Genera una chiave API di Marketplace Walmart

1. Vai a Walmart Marketplace per generare un [ad Adobe la chiave API di produzione del provider di soluzioni](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. Crea la chiave e configura le autorizzazioni:

   * Seleziona Adobe come provider della soluzione.

   * Imposta le autorizzazioni come mostrato nella tabella seguente. Per maggiori dettagli, vedi [Credenziali API](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) in *Aiuto per i venditori di Marketplace Walmart*.

&#x200B;|    **Adobe di configurazione della chiave API per Walmart**
&#x200B;| **Autorizzazione** | **Impostazione** | |—|—| | Contenuto | Accesso completo | | Ottieni feed | Solo visualizzazione | | Inventario | Accesso completo | | Articoli | Accesso completo | | Tempo di ritardo | Accesso completo | | Ordine | Accesso completo | | Prezzo | Accesso completo | | Rapporti | Solo visualizzazione | | Resi | Accesso completo | | Regole | Accesso completo | | Spedizione | Accesso completo |

## Stato del Negozio Marketplace di Walmart

Quando pubblichi i prodotti su Walmart Marketplace, la disponibilità dell&#39;elenco dipende dallo stato dei tuoi negozi Walmart Marketplace:

* Per i negozi live, le offerte dei prodotti sono elencate e disponibili per la vendita al termine dell&#39;operazione di abbinamento.

* Per i negozi che non sono in diretta, le offerte di prodotto sono organizzate e non sono visibili ai clienti. Non appena il negozio è in diretta, le inserzioni in serie vengono inviate automaticamente al negozio live.


![[!DNL Walmart Seller Central] prodotti a cascata](assets/walmart-seller-central-staged.png)
