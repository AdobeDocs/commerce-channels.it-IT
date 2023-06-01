---
title: Integrazione store con un [!DNL Amazon Seller Account]
description: Prima di iniziare il processo di onboarding, devi creare (aggiungere) un archivio di Sales Channel di Amazon e collegarlo al tuo account Amazon Seller.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Integrazione store con un [!DNL Amazon Seller Account]

Per iniziare a utilizzare il canale di vendita Amazon, devi creare (aggiungere) un negozio del canale di vendita Amazon e collegarlo al tuo [!DNL Amazon Seller Account]. Questi due passaggi integrano [!DNL Commerce] e account Amazon per condividere dati, sincronizzare prodotti e altro ancora.

_Sono necessarie le credenziali di accesso primarie per [!DNL Amazon Seller Central] account (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore) per collegare il tuo negozio._

>[!NOTE]
>
>Dopo la prima integrazione del negozio, ti verrà chiesto di rinnovare ogni anno la connessione del canale di vendita Amazon ad Amazon concedendo nuovamente l’accesso. Puoi rinnovare o revocare questa autorizzazione in _Autorizzazioni correnti_ tabella in _Autorizzazioni per sviluppatori Amazon MWS_ sezione del **Impostazioni** > **Autorizzazioni utente** pagina del tuo account Seller Central.

## Aggiungi uno store di Amazon

1. Il giorno _Amministratore_ barra laterale, vai a **Marketing** > _Canali_ > **Sales Channel Amazon**.

   Quando aggiungi il tuo primo negozio canale di vendita Amazon, il _Attività di pre-configurazione_ viene visualizzata la finestra modale. Dopo aver aggiunto il primo store, è possibile accedere alle attività di preconfigurazione sul [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina in _Apprendimento e preparazione_ nel menu a sinistra.

1. Clic **[!UICONTROL Add Amazon Store]**.

   Il _[!UICONTROL Add Amazon sales channel]_viene visualizzata la pagina.

   ![Aggiungi il negozio del canale di vendita Amazon](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. Per **[!UICONTROL Magento Website to use for Amazon Listing]**, scegli quale [!DNL Commerce] siti Web da connettere per questo negozio del canale di vendita Amazon.

   Questa impostazione definisce anche il valore [!DNL Commerce] memorizza per [importazione di ordini Amazon](./order-settings.md).

1. Per **[!UICONTROL Email Address]**, immetti l’indirizzo e-mail di contatto preferito.

1. Per **[!UICONTROL New Store Name]**, immetti un nome descrittivo per il nuovo negozio del canale di vendita Amazon.

   >[!NOTE]
   >
   >Questo nome viene utilizzato come [!DNL Commerce] solo riferimento e identifica l’archivio sul [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina. Desideri che sia qualcosa che il tuo team possa facilmente identificare. Ad esempio, il nome del tuo store Amazon che vende negli Stati Uniti `Amazon Store USA`.

1. Per **[!UICONTROL Amazon Marketplace Country]**, scegli l’area geografica in cui questo negozio del canale di vendita Amazon vende i prodotti. Opzioni:

   - Stati Uniti
   - Canada
   - Messico
   - Regno Unito

1. In _[!UICONTROL Map your Magento attributes to Amazon]_eseguire le operazioni seguenti:

   - Per **[!UICONTROL Product ID on the Amazon market]**, scegli l&#39;attributo Amazon da mappare al [!DNL Commerce] di seguito.

      Questo ID aiuta a far corrispondere correttamente i prodotti corrispondenti nel tuo [!DNL Commerce] catalogo.

   - Per **[!UICONTROL Map a Magento attribute]**, scegli il [!DNL Commerce] attributo prodotto da mappare all’attributo Amazon selezionato in precedenza.

      [Mappatura degli attributi](./ob-creating-magento-attributes.md) consente di garantire che l’inserzione di Amazon corrisponda correttamente al prodotto corrispondente nel tuo [!DNL Commerce] catalogo.

1. Clic **[!UICONTROL Connect]**.

   La finestra di dialogo si chiude e il nuovo archivio viene visualizzato sul [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina con un messaggio di conferma.

## Connetti un negozio a [!DNL Amazon Seller Central]

1. Nel dashboard del negozio, fai clic su **[!UICONTROL Connect store]** sulla scheda dello store per avviare [!DNL Amazon Seller Central] in una nuova scheda.

1. Immetti il [!DNL Amazon Seller Central] credenziali account e fai clic su **[!UICONTROL Sign in]**.

   Per completare la connessione, devi accedere al tuo [!DNL Amazon Seller Central] account utilizzando le credenziali di accesso per l&#39;utente principale (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore).

1. Se richiesto, completa l’autorizzazione a due fattori di Amazon (2FA) immettendo il codice ricevuto da Amazon e fai clic su **[!UICONTROL Sign in]**.

1. Il giorno _[!UICONTROL Amazon Marketplace Web Service]_pagina di conferma, seleziona la &quot;[!UICONTROL I understand...]&quot; e fai clic su **[!UICONTROL Next]**.

1. Il giorno _[!UICONTROL You are almost done]_messaggio, fai clic su **[!UICONTROL Continue]**.

   Hai concesso al canale di vendita Amazon l’autorizzazione per accedere e condividere i dati con il tuo [!DNL Amazon Seller Central] account. La pagina Amazon si chiude e viene visualizzato un messaggio di conferma.

   Il [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) viene visualizzata la pagina con le tue schede del negozio Amazon.

   Per visualizzare il dashboard del negozio, fai clic su **[!UICONTROL View Store]** sulla scheda del negozio.

![Home del canale di vendita Amazon con nuova scheda del negozio](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

Il tuo nuovo canale di vendita Amazon è ora collegato al tuo [!DNL Amazon Seller Central] account.

![Icona Successivo](assets/btn-next.png) [**Continua a creare una regola di elenco**](./ob-create-listing-rule.md)
