---
title: Configurare le impostazioni dei canali
description: Configura le impostazioni di Channel Manager e del canale di vendita per l'autenticazione, mappa gli attributi del catalogo e i vettori di spedizione necessari per coordinare le operazioni di vendita tra [!DNL Commerce] e [!DNL Walmart Marketplace].
source-git-commit: 5c478813af442a4e54cb5c64045698f04d710c9a
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Configurare le impostazioni del canale di vendita

Le impostazioni del canale di vendita consentono la comunicazione e la sincronizzazione dei dati tra [!DNL Commerce] e [!DNL Walmart Marketplace] in modo da gestire [!DNL Walmart Marketplace] operazioni di vendita da [!DNL Commerce] Amministratore:

In [!DNL Channel Manager], è possibile configurare alcune impostazioni dei canali di vendita durante il processo di onboarding. Dopo l’onboarding, puoi visualizzare e gestire la configurazione del canale dal *[!UICONTROL Channel Settings]* pagina.

- **[Mappa identificatori univoci](map-catalog-attributes.md)**-Prima di collegare gli elenchi da [!DNL Commerce] a [!DNL Walmart Marketplace], mappare almeno un identificatore univoco dal [!DNL Commerce] catalogo all&#39;identificatore corrispondente da [!DNL Walmart]. Questo passaggio deve corrispondere a [!DNL Commerce] prodotti a quelli esistenti [!DNL Walmart] elenchi e sincronizzazione dei dati dei prodotti tra [!DNL Commerce] e [!DNL Walmart].

- **[Mappa vettori di spedizione](map-shipping-carriers.md)**-Prima di elaborare [!DNL Walmart Marketplace] ordini da [!DNL Commerce], assicurati di mappare i vettori di spedizione dal tuo [!DNL Commerce] istanza ai corrispondenti vettori [!DNL Walmart Marketplace].

- **Credenziali API di Walmart**-Durante il [!DNL Channel Manager] il processo di onboarding, [Credenziali API di Walmart](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) dal [!DNL Walmart Marketplace Seller] account per la connessione [!DNL Commerce] a [!DNL Walmart Marketplace] per la comunicazione e la sincronizzazione dei dati. Se necessario, puoi [aggiorna queste credenziali](manage-wmt-connection.md) dal _[!UICONTROL Channel Settings]_pagina.
