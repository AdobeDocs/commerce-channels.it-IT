---
title: Portata del prezzo
description: Utilizza l’ambito di determinazione dei prezzi Commerce per gestire i prezzi in base a più siti web o globalmente.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Scopo del prezzo

[!DNL Commerce] fornisce la configurazione per [ambito tariffario](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} da impostare su `Global` o `Website`. Se il prezzo è impostato su `Global`, esiste un&#39;unica fonte di prezzo per tutti i siti web. Se il prezzo è impostato su `Website`, i siti web possono variare i prezzi e hanno anche un valore predefinito di fallback. Vedi [Prezzo catalogo](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} nella guida utente di Commerce di base.

Se cambi l&#39;ambito del prezzo del catalogo da `Global` a `Website`, anche tutti gli attributi del tipo di prezzo vengono modificati in `Website`. Vedi [Aggiunta di siti Web](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target=&quot;_blank&quot;}.

Quando si sceglie il prezzo di un sito web, ci sono due fonti di prezzo:

- Prezzo del sito web
- Il prezzo predefinito (calo)

Per l’integrazione dei canali di vendita Amazon, in base al [regole di elenco](./listing-rules.md), puoi mappare i prodotti da più siti web in un unico [!DNL Amazon Marketplace] Paese (definito durante [integrazione store](./store-integration.md)). Tuttavia, questa mappatura introduce il problema del prezzo da pubblicare se il prodotto esiste su più siti web con prezzi diversi.
