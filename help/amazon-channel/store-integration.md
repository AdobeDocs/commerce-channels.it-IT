---
title: Archivia integrazione con un  [!DNL Amazon Seller Account]
description: Prima di iniziare il processo di onboarding, devi creare (aggiungere) un archivio di Sales Channel di Amazon e collegarlo al tuo account Amazon Seller.
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Archivia l&#39;integrazione con un [!DNL Amazon Seller Account]

Per iniziare a utilizzare il canale di vendita Amazon, devi creare (aggiungere) un negozio del canale di vendita Amazon e collegarlo al tuo [!DNL Amazon Seller Account]. Questi due passaggi integrano gli account [!DNL Commerce] e Amazon per condividere dati, sincronizzare prodotti e altro ancora.

_Per connettere il tuo Negozio, devi disporre delle credenziali di accesso primarie per il tuo account [!DNL Amazon Seller Central] (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore)._

>[!NOTE]
>
>Dopo la prima integrazione del negozio, ti verrà chiesto di rinnovare ogni anno la connessione del canale di vendita Amazon ad Amazon concedendo nuovamente l’accesso. Puoi rinnovare o revocare questa autorizzazione nella tabella _Autorizzazioni correnti_ della sezione _Autorizzazioni per sviluppatori Amazon MWS_ della pagina **Impostazioni** > **Autorizzazioni utente** del tuo account Seller Central.

## Aggiungi uno store di Amazon

1. Nella barra laterale _Amministratore_, passa a **Marketing** > _Canali_ > **Sales Channel Amazon**.

   Quando aggiungi il tuo primo store del canale di vendita Amazon, viene visualizzata la finestra modale _Attività di pre-installazione_. Dopo aver aggiunto il primo store, puoi accedere alle attività di preconfigurazione nella pagina [Home del canale di vendita di Amazon](./amazon-sales-channel-home.md) in _Apprendimento e preparazione_ nel menu a sinistra.

1. Fare clic su **[!UICONTROL Add Amazon Store]**.

   Verrà aperta la pagina _[!UICONTROL Add Amazon sales channel]_.

   ![Aggiungi l&#39;Amazon Sales Channel Store](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. Per **[!UICONTROL Magento Website to use for Amazon Listing]**, scegli quale dei tuoi siti Web [!DNL Commerce] connetterti per questo store del canale di vendita Amazon.

   Questa impostazione definisce anche l&#39;archivio predefinito [!DNL Commerce] per [l&#39;importazione di ordini Amazon](./order-settings.md).

1. Per **[!UICONTROL Email Address]**, immetti l&#39;indirizzo e-mail di contatto preferito.

1. Per **[!UICONTROL New Store Name]**, immetti un nome descrittivo per il nuovo negozio del canale di vendita Amazon.

   >[!NOTE]
   >
   >Questo nome viene utilizzato solo come riferimento [!DNL Commerce] e identifica lo store nella [pagina Home del canale di vendita Amazon](./amazon-sales-channel-home.md). Desideri che sia qualcosa che il tuo team possa facilmente identificare. Ad esempio, il tuo Amazon store che vende negli Stati Uniti potrebbe essere denominato `Amazon Store USA`.

1. Per **[!UICONTROL Amazon Marketplace Country]**, scegli l&#39;area geografica o il paese in cui questo negozio del canale di vendita Amazon vende i prodotti. Opzioni:

   - Stati Uniti
   - Canada
   - Messico
   - Regno Unito

1. Nella sezione _[!UICONTROL Map your Magento attributes to Amazon]_eseguire le operazioni seguenti:

   - Per **[!UICONTROL Product ID on the Amazon market]**, scegliere l&#39;attributo Amazon da mappare all&#39;attributo [!DNL Commerce] selezionato di seguito.

     Questo ID consente di associare correttamente i prodotti corrispondenti nel catalogo [!DNL Commerce].

   - Per **[!UICONTROL Map a Magento attribute]**, scegli l&#39;attributo di prodotto [!DNL Commerce] da mappare all&#39;attributo di Amazon selezionato in precedenza.

     [La mappatura degli attributi](./ob-creating-magento-attributes.md) consente di garantire che l&#39;inserzione di Amazon corrisponda correttamente al prodotto corrispondente nel catalogo [!DNL Commerce].

1. Fare clic su **[!UICONTROL Connect]**.

   La finestra di dialogo si chiude e il nuovo store viene visualizzato nella pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) con un messaggio di conferma.

## Connetti un archivio a [!DNL Amazon Seller Central]

1. Nel dashboard dello store, fare clic su **[!UICONTROL Connect store]** sulla scheda dello store per avviare [!DNL Amazon Seller Central] in una nuova scheda.

1. Immettere le credenziali dell&#39;account [!DNL Amazon Seller Central] e fare clic su **[!UICONTROL Sign in]**.

   Per completare la connessione, devi accedere al tuo account [!DNL Amazon Seller Central] utilizzando le credenziali di accesso per l&#39;utente principale (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore).

1. Se richiesto, completare l&#39;autorizzazione a due fattori di Amazon (2FA) immettendo il codice ricevuto da Amazon e fare clic su **[!UICONTROL Sign in]**.

1. Nella pagina di conferma _[!UICONTROL Amazon Marketplace Web Service]_, selezionare la casella di controllo &quot;[!UICONTROL I understand...]&quot; e fare clic su **[!UICONTROL Next]**.

1. Nel messaggio _[!UICONTROL You are almost done]_, fare clic su **[!UICONTROL Continue]**.

   Hai concesso al canale di vendita Amazon l&#39;autorizzazione per accedere e condividere i dati con il tuo account [!DNL Amazon Seller Central]. La pagina Amazon si chiude e viene visualizzato un messaggio di conferma.

   Viene visualizzata la pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) con le schede del tuo Negozio Amazon.

   Per visualizzare il dashboard dello store, fare clic su **[!UICONTROL View Store]** sulla scheda dello store.

![Pagina principale del canale di vendita Amazon con nuova scheda del negozio](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

Il nuovo Amazon Sales Channel Store è ora connesso al tuo account [!DNL Amazon Seller Central].

![Icona Successiva](assets/btn-next.png) [**Continua a creare una regola per le inserzioni**](./ob-create-listing-rule.md)
