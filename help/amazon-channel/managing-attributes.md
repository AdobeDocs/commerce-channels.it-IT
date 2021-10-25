---
title: Gestisci attributi
description: Puoi gestire la mappatura degli attributi di prodotto Commerce agli attributi di Amazon per garantire informazioni di prodotto precise tra i sistemi.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Gestire gli attributi

Amazon e [!DNL Commerce] entrambi utilizzano un sistema di proprietà del prodotto, noto come attributi, utilizzato per definire un prodotto. Gli attributi definiscono la descrizione, il contenuto, le immagini, i prezzi e vari dati per i prodotti.

La comunicazione corretta tra Commerce e Amazon richiede che [!DNL Commerce] Gli attributi devono essere mappati correttamente (o confrontati) con l&#39;attributo Amazon corrispondente. Durante l’integrazione con Amazon, associ questi attributi agli attributi di Amazon. Al termine, [!DNL Commerce] può sincronizzare e mantenere gli elenchi Amazon con [!DNL Commerce] catalogo dei prodotti.

Ad esempio, immagina di avere lo stesso elemento nel tuo [!DNL Commerce] elenchi di catalogo e Amazon. Un attributo per il prodotto potrebbe essere il prezzo di listino dell&#39;articolo. Nome del prezzo di listino in [!DNL Commerce] potrebbe essere denominato `Price`, mentre il prezzo di listino per Amazon potrebbe essere denominato `ListingPrice`. Devi istruire [!DNL Commerce] quando comunica con Amazon, la [!DNL Commerce] attributo denominato `Price` è lo stesso dell’attributo Amazon denominato `ListingPrice`. Questo processo si chiama _gestione attributi_ e include la creazione di attributi nuovi e la modifica di attributi esistenti. Assicurati che gli attributi corrispondano correttamente assicura la corretta comunicazione tra [!DNL Commerce] e Amazon.

Quando è impostata la mappatura degli attributi, [!DNL Commerce] può comunicare informazioni sui prodotti avanti e indietro con Amazon. Se hai degli elenchi di prodotti Amazon, [!DNL Commerce] può importare i prodotti e i dettagli Amazon nel tuo [!DNL Commerce] catalogo, che consente di gestire gli elenchi Amazon da un unico catalogo centrale di prodotti.

Il canale di vendita Amazon ti consente di accedere, rivedere, creare e gestire gli attributi, in base alle esigenze, nel [_[!UICONTROL Attributes]_visualizzare](./attributes-view.md) nella home page del canale di vendita Amazon. Se aggiungi un attributo al tuo [!DNL Commerce] catalogo, potrebbe richiedere un aggiornamento di tali valori in tutti i prodotti.

Per ulteriori informazioni [!DNL Commerce] e i set di attributi e i valori di Amazon, vedi:

- [Informazioni di base sulla gestione degli attributi](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [Creare un attributo](./creating-attributes.md#create-an-attribute)
- [Modificare un attributo esistente](./creating-attributes.md#edit-an-attribute)
- [Visualizza mappatura attributi](./amazon-matching-attributes-values.md)
- [Modificare o creare una mappatura degli attributi](./amazon-manually-update-incomplete-listing.md)
