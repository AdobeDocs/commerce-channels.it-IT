---
title: Canale di vendita Amazon - Ambito del prezzo
description: Utilizza l’ambito di determinazione prezzi di Commerce per gestire i prezzi in base a più siti web o a livello globale.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Limite di prezzo

[!DNL Commerce] fornisce la configurazione per l&#39;ambito [determinazione prezzi](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) da impostare su `Global` o `Website`. Se il prezzo è impostato su `Global`, è disponibile un&#39;unica origine prezzo per tutti i siti Web. Se il prezzo è impostato su `Website`, i siti Web possono variare i prezzi e avere anche un valore di prezzo predefinito di fallback (vedi [Ambito prezzo](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Se si modifica l&#39;ambito del prezzo del catalogo da `Global` a `Website`, anche tutti gli attributi del tipo di prezzo verranno modificati in `Website`. Vedere [Aggiunta di siti Web](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Quando si sceglie il prezzo di un sito Web, sono disponibili due origini di prezzo:

- Prezzo del sito web
- Prezzo predefinito (di riserva)

Per l&#39;integrazione del canale di vendita Amazon, in base alle [regole di inserzione](./listing-rules.md), è possibile mappare prodotti da più siti Web in un unico paese [!DNL Amazon Marketplace] (definito durante l&#39;[integrazione store](./store-integration.md)). Tuttavia, questa mappatura introduce la questione di quale prezzo dovrebbe essere pubblicato se il prodotto esiste su più siti web con prezzi diversi.
