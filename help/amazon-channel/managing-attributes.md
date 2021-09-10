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

Sia Amazon che [!DNL Commerce] utilizzano un sistema di proprietà del prodotto, note come attributi, utilizzato per definire un prodotto. Gli attributi definiscono la descrizione, il contenuto, le immagini, i prezzi e vari dati per i prodotti.

La comunicazione corretta tra Commerce e Amazon richiede che gli attributi [!DNL Commerce] siano mappati correttamente (o abbinati) all’attributo Amazon corrispondente. Durante l’integrazione con Amazon, associ questi attributi agli attributi di Amazon. Una volta completato, [!DNL Commerce] può sincronizzare e mantenere gli elenchi Amazon con il catalogo di prodotti [!DNL Commerce].

Ad esempio, immagina di avere lo stesso elemento nel catalogo [!DNL Commerce] e negli elenchi di Amazon. Un attributo per il prodotto potrebbe essere il prezzo di listino dell&#39;articolo. Il nome del prezzo di listino in [!DNL Commerce] potrebbe essere denominato `Price`, mentre il prezzo di listino per Amazon potrebbe essere denominato `ListingPrice`. È necessario indicare a [!DNL Commerce] che, durante la comunicazione con Amazon, l&#39;attributo [!DNL Commerce] denominato `Price` è lo stesso dell&#39;attributo Amazon denominato `ListingPrice`. Questo processo si chiama _gestione attributi_ e include la creazione di attributi nuovi e la modifica di attributi esistenti. Assicurati che la corrispondenza degli attributi sia corretta garantisce la corretta comunicazione tra [!DNL Commerce] e Amazon.

Quando è impostata la mappatura degli attributi, [!DNL Commerce] può comunicare le informazioni sul prodotto avanti e indietro con Amazon. Se disponi di elenchi di prodotti Amazon, [!DNL Commerce] può importare i prodotti e i dettagli Amazon nel catalogo [!DNL Commerce], per gestire gli elenchi Amazon da un unico catalogo centrale di prodotti.

Il canale di vendita Amazon ti consente di accedere, rivedere, creare e gestire gli attributi, in base alle esigenze, nella [_[!UICONTROL Attributes]_view](./attributes-view.md) nella home page del canale di vendita Amazon. Se aggiungi un attributo al catalogo [!DNL Commerce], potrebbe essere necessario un aggiornamento di tali valori per tutti i prodotti.

Per ulteriori informazioni sui set e i valori di attributi [!DNL Commerce] e Amazon, consulta:

- [Nozioni di base sugli attributi di gestione](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [Creare un attributo](./creating-attributes.md#create-an-attribute)
- [Modificare un attributo esistente](./creating-attributes.md#edit-an-attribute)
- [Visualizza mappatura attributi](./amazon-matching-attributes-values.md)
- [Modificare o creare una mappatura degli attributi](./amazon-manually-update-incomplete-listing.md)
