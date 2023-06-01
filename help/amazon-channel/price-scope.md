---
title: Canale di vendita Amazon - Ambito del prezzo
description: Utilizza l’ambito di determinazione prezzi di Commerce per gestire i prezzi in base a più siti web o a livello globale.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Limite di prezzo

[!DNL Commerce] fornisce la configurazione per [ambito di determinazione prezzi](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) da impostare su `Global` o `Website`. Se la determinazione prezzi è impostata su `Global`, esiste un’unica fonte di prezzo per tutti i siti web. Se la determinazione prezzi è impostata su `Website`, i tuoi siti web possono variare i prezzi e avere anche un valore di prezzo predefinito di fallback (vedi [Limite di prezzo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Se modifichi l’ambito del prezzo del catalogo da `Global` a `Website`, anche tutti gli attributi del tipo di prezzo cambiano in `Website`. Consulta [Aggiunta di siti Web](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Quando si sceglie il prezzo di un sito Web, sono disponibili due origini di prezzo:

- Prezzo del sito web
- Prezzo predefinito (di riserva)

Per l’integrazione del canale di vendita Amazon, in base al [regole di inserzione](./listing-rules.md), è possibile mappare prodotti da più siti web in un unico [!DNL Amazon Marketplace] Paese (definito durante [integrazione store](./store-integration.md)). Tuttavia, questa mappatura introduce la questione di quale prezzo dovrebbe essere pubblicato se il prodotto esiste su più siti web con prezzi diversi.
