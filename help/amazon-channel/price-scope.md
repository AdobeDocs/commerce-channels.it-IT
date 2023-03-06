---
title: Limite prezzo
description: Utilizza l’ambito di determinazione prezzi di Commerce per gestire i prezzi in base a più siti web o a livello globale.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Limite prezzo

[!DNL Commerce] fornisce la configurazione per [ambito di determinazione prezzi](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} nella guida utente di base di Commerce.

Se modifichi l’ambito del prezzo del catalogo da `Global` a `Website`, anche tutti gli attributi del tipo di prezzo cambiano in `Website`. Consulta [Aggiunta di siti Web](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}.

Quando si sceglie il prezzo di un sito Web, sono disponibili due origini di prezzo:

- Prezzo del sito web
- Prezzo predefinito (di riserva)

Per l’integrazione del canale di vendita Amazon, in base al [regole di inserzione](./listing-rules.md), è possibile mappare prodotti da più siti web in un unico [!DNL Amazon Marketplace] Paese (definito durante [integrazione store](./store-integration.md)). Tuttavia, questa mappatura introduce la questione di quale prezzo dovrebbe essere pubblicato se il prodotto esiste su più siti web con prezzi diversi.
