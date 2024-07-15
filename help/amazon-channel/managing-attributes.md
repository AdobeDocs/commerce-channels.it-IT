---
title: Gestisci gli attributi per le inserzioni Amazon
description: Puoi gestire la mappatura degli attributi del prodotto Commerce agli attributi Amazon per garantire informazioni accurate sul prodotto tra i sistemi.
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Gestisci gli attributi per le inserzioni Amazon

Amazon e [!DNL Commerce] utilizzano entrambi un sistema di proprietà del prodotto, note come attributi, utilizzate per definire un prodotto. Gli attributi definiscono la descrizione, il contenuto, le immagini, i prezzi e i vari dati dei tuoi prodotti.

Una comunicazione corretta tra Commerce e Amazon richiede che gli attributi [!DNL Commerce] siano mappati correttamente (o abbinati) all&#39;attributo Amazon corrispondente. Durante l’integrazione con Amazon, questi attributi vengono mappati sugli attributi di Amazon. Una volta completato, [!DNL Commerce] può sincronizzare e gestire le tue inserzioni Amazon con il tuo catalogo prodotti [!DNL Commerce].

Immagina ad esempio di avere lo stesso elemento nel catalogo [!DNL Commerce] e nelle inserzioni Amazon. Un attributo del prodotto potrebbe essere il prezzo di vendita dell&#39;articolo. Il nome del prezzo di vendita in [!DNL Commerce] potrebbe essere `Price`, mentre il prezzo di vendita per Amazon potrebbe essere `ListingPrice`. È necessario indicare a [!DNL Commerce] che quando si comunica con Amazon, l&#39;attributo [!DNL Commerce] denominato `Price` è uguale all&#39;attributo Amazon denominato `ListingPrice`. Questo processo è denominato _gestione degli attributi_ e include la creazione di nuovi attributi e la modifica di quelli esistenti. Verificare che gli attributi corrispondano correttamente per garantire una comunicazione corretta tra [!DNL Commerce] e Amazon.

Quando è impostata la mappatura degli attributi, [!DNL Commerce] può comunicare le informazioni sul prodotto avanti e indietro con Amazon. Se disponi di elenchi di prodotti Amazon, [!DNL Commerce] può importare i tuoi prodotti e dettagli Amazon nel tuo catalogo [!DNL Commerce], consentendoti di gestire i tuoi elenchi Amazon da un unico catalogo centrale di prodotti.

Il canale di vendita Amazon ti consente di accedere, esaminare, creare e gestire gli attributi, in base alle esigenze, nella visualizzazione [_[!UICONTROL Attributes]_](./attributes-view.md) della home page del canale di vendita Amazon. Se si aggiunge un attributo al catalogo [!DNL Commerce], potrebbe essere necessario aggiornare tali valori in tutti i prodotti.

Per ulteriori informazioni sui set di attributi e i valori [!DNL Commerce] e Amazon, vedere:

- [Nozioni di base su come gestire gli attributi](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [Creare un attributo](./creating-attributes.md#create-an-attribute)
- [Modifica un attributo esistente](./creating-attributes.md#edit-an-attribute)
- [Visualizza mappatura attributi](./amazon-matching-attributes-values.md)
- [Modifica o crea mappatura attributi](./amazon-manually-update-incomplete-listing.md)
