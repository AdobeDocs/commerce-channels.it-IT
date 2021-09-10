---
title: Portata del prezzo
description: Utilizza l’ambito di determinazione dei prezzi Commerce per gestire i prezzi in base a più siti web o globalmente.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Scopo del prezzo

[!DNL Commerce] fornisce la configurazione dell&#39;ambito [ ](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price)tariffario{:target=&quot;_blank&quot;} da impostare su  `Global` o  `Website`. Se il prezzo è impostato su `Global`, esiste un&#39;unica fonte di prezzo per tutti i siti web. Se il prezzo è impostato su `Website`, i siti web possono variare il prezzo e hanno anche un valore predefinito di fallback. Consulta [Prezzo catalogo](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} nella guida utente di Commerce di base.

Se cambi l’ambito del prezzo del catalogo da `Global` a `Website`, anche tutti gli attributi del tipo di prezzo vengono modificati in `Website`. Vedere [Aggiunta di siti Web](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){:target=&quot;_blank&quot;}.

Quando si sceglie il prezzo di un sito web, ci sono due fonti di prezzo:

- Prezzo del sito web
- Il prezzo predefinito (calo)

Per l&#39;integrazione dei canali di vendita Amazon, in base alle [regole di elenco](./listing-rules.md), puoi mappare i prodotti da più siti web in un singolo [!DNL Amazon Marketplace] Paese (definito durante [l&#39;integrazione degli archivi](./store-integration.md)). Tuttavia, questa mappatura introduce il problema del prezzo da pubblicare se il prodotto esiste su più siti web con prezzi diversi.
