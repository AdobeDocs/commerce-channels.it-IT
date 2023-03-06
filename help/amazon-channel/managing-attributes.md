---
title: Gestisci attributi
description: Puoi gestire la mappatura degli attributi del prodotto Commerce agli attributi di Amazon per garantire informazioni accurate sui prodotti tra i sistemi.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Gestisci attributi

AMAZON e [!DNL Commerce] entrambi utilizzano un sistema di proprietà del prodotto, note come attributi, utilizzato per definire un prodotto. Gli attributi definiscono la descrizione, il contenuto, le immagini, i prezzi e i vari dati dei tuoi prodotti.

Una comunicazione corretta tra Commerce e Amazon richiede che [!DNL Commerce] gli attributi devono essere mappati correttamente (o abbinati) all’attributo Amazon corrispondente. Durante l’integrazione con Amazon, questi attributi vengono mappati sugli attributi di Amazon. Una volta completato, [!DNL Commerce] può sincronizzare e gestire le tue inserzioni Amazon con il tuo [!DNL Commerce] catalogo dei prodotti.

Ad esempio, immagina di avere lo stesso elemento nel tuo [!DNL Commerce] cataloghi ed inserzioni Amazon. Un attributo del prodotto potrebbe essere il prezzo di vendita dell&#39;articolo. Nome del prezzo di vendita in [!DNL Commerce] potrebbe essere denominato `Price`, mentre il prezzo di vendita di Amazon potrebbe essere denominato `ListingPrice`. Devi istruire [!DNL Commerce] che quando si comunica con Amazon, il [!DNL Commerce] attributo denominato `Price` corrisponde all’attributo Amazon denominato `ListingPrice`. Questo processo è denominato _gestione degli attributi_, e include la creazione di nuovi attributi e la modifica di quelli esistenti. La corretta corrispondenza degli attributi assicura la comunicazione corretta tra [!DNL Commerce] e Amazon.

Quando è impostata la mappatura degli attributi, [!DNL Commerce] può comunicare le informazioni sui prodotti con Amazon. Se hai elenchi di prodotti Amazon, [!DNL Commerce] può importare i tuoi prodotti e dettagli di Amazon nel tuo [!DNL Commerce] consente di gestire le inserzioni Amazon da un unico catalogo centrale di prodotti.

Il canale di vendita Amazon ti consente di accedere, esaminare, creare e gestire gli attributi, a seconda delle necessità, nel [_[!UICONTROL Attributes]_visualizza](./attributes-view.md) nella home page del canale di vendita Amazon. Se aggiungi un attributo al tuo [!DNL Commerce] potrebbe richiedere un aggiornamento di tali valori in tutti i prodotti.

Per ulteriori informazioni su [!DNL Commerce] e i set di attributi e i valori di Amazon, consulta:

- [Gestisci nozioni di base sugli attributi](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}
- [Creare un attributo](./creating-attributes.md#create-an-attribute)
- [Modifica un attributo esistente](./creating-attributes.md#edit-an-attribute)
- [Visualizza mappatura attributi](./amazon-matching-attributes-values.md)
- [Modifica o crea mappatura attributi](./amazon-manually-update-incomplete-listing.md)
