---
title: Integrazione store
description: Prima di avviare il processo di onboarding, devi creare (aggiungere) un archivio Sales Channel Amazon e connetterlo al tuo account venditore Amazon.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Integrazione store

Per iniziare a utilizzare il canale di vendita Amazon, devi creare (aggiungere) un negozio di canali di vendita Amazon e collegarlo al tuo account venditore Amazon. Questi due passaggi integrano gli account [!DNL Commerce] e Amazon per condividere dati, sincronizzare prodotti e altro ancora.

_Per collegare il tuo negozio è necessario disporre delle credenziali di accesso principali per il tuo  [!DNL Amazon Seller Central] account (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore)._

>[!NOTE]
>
>Dopo l&#39;integrazione del primo negozio, ogni anno ti verrà richiesto di rinnovare la connessione del canale di vendita Amazon ad Amazon concedendo nuovamente l&#39;accesso. Puoi rinnovare o revocare questa autorizzazione nella tabella _Autorizzazioni correnti_ nella sezione _Autorizzazioni per sviluppatori Amazon MWS_ della pagina **Impostazioni** > **Autorizzazioni utente** del tuo account centrale rivenditore.

## Aggiungere un archivio Amazon

1. Nella barra laterale _Amministratore_, vai a **Marketing** > _Canali_ > **Sales Channel Amazon**.

   Quando aggiungi il tuo primo archivio canali di vendita Amazon, viene visualizzato il modale _Attività pre-installazione_ . Dopo l&#39;aggiunta del primo negozio, è possibile accedere alle attività di preconfigurazione nella pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) in _Apprendimento e preparazione_ nel menu a sinistra.

1. Fare clic su **[!UICONTROL Add Amazon Store]**.

   Viene visualizzata la pagina _[!UICONTROL Add Amazon sales channel]_.

   ![Aggiungi l&#39;archivio canali di vendita Amazon](assets/amazon-store-integration.png)

1. Per **[!UICONTROL Magento Website to use for Amazon Listing]**, scegli quale dei tuoi [!DNL Commerce] siti web per connettersi a questo archivio canali di vendita Amazon.

   Questa impostazione definisce anche l&#39;archivio [!DNL Commerce] predefinito per [l&#39;importazione di ordini Amazon](./order-settings.md).

1. Per **[!UICONTROL Email Address]**, inserisci l&#39;indirizzo e-mail di contatto preferito.

1. Per **[!UICONTROL New Store Name]**, immetti un nome descrittivo per il nuovo archivio canali di vendita Amazon.

   >[!NOTE]
   >
   >Questo nome viene utilizzato solo come riferimento [!DNL Commerce] e identifica lo store nella pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md). Vuoi renderlo qualcosa che il tuo team può facilmente identificare. Ad esempio, il nome del tuo negozio Amazon che vende nell’area degli Stati Uniti potrebbe essere `Amazon Store USA`.

1. Per **[!UICONTROL Amazon Marketplace Country]**, scegli la regione/il paese in cui questo negozio di canale di vendita Amazon vende prodotti. Opzioni:

   - Stati Uniti
   - Canada
   - Messico
   - Regno Unito

1. Nella sezione _[!UICONTROL Map your Magento attributes to Amazon]_, procedi come segue:

   - Per **[!UICONTROL Product ID on the Amazon market]**, scegli l’attributo Amazon da mappare all’attributo [!DNL Commerce] selezionato di seguito.

      Questo ID aiuta a far corrispondere correttamente i prodotti corrispondenti nel catalogo [!DNL Commerce].

   - Per **[!UICONTROL Map a Magento attribute]**, scegli l’ [!DNL Commerce] attributo di prodotto da mappare all’attributo Amazon selezionato in precedenza.

      [Gli ](./ob-creating-magento-attributes.md) attributi di mappatura consentono di garantire che l’elenco Amazon corrisponda correttamente al prodotto corrispondente nel  [!DNL Commerce] catalogo.

1. Fare clic su **[!UICONTROL Connect]**.

   La finestra di dialogo si chiude e il nuovo negozio viene visualizzato sulla pagina [Amazon sales channel home](./amazon-sales-channel-home.md) con un messaggio di conferma.

## Connetti uno store a [!DNL Amazon Seller Central]

1. Nel dashboard dello store, fai clic su **[!UICONTROL Connect store]** nella scheda dello store per avviare [!DNL Amazon Seller Central] in una nuova scheda.

1. Immetti le credenziali dell&#39;account [!DNL Amazon Seller Central] e fai clic su **[!UICONTROL Sign in]**.

   Per completare questa connessione, devi accedere al tuo account [!DNL Amazon Seller Central] utilizzando le credenziali di accesso per l&#39;utente principale (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore).

1. Se richiesto, completa Amazon Two-Factor Authorization (2FA) immettendo il codice ricevuto da Amazon e fai clic su **[!UICONTROL Sign in]**.

1. Nella pagina di conferma _[!UICONTROL Amazon Marketplace Web Service]_, seleziona la casella di controllo &quot;[!UICONTROL I understand...]&quot; e fai clic su **[!UICONTROL Next]**.

1. Nel messaggio _[!UICONTROL You are almost done]_, fai clic su **[!UICONTROL Continue]**.

   Hai concesso l’autorizzazione del canale di vendita Amazon per accedere e condividere i dati con il tuo account [!DNL Amazon Seller Central]. La pagina Amazon viene chiusa e viene visualizzato un messaggio di conferma.

   Viene visualizzata la pagina [Home del canale di vendita Amazon](./amazon-sales-channel-home.md) con le schede del tuo negozio Amazon.

   Per visualizzare il dashboard dello store, fai clic su **[!UICONTROL View Store]** nella scheda dello store.

![Casa del canale di vendita Amazon con nuova carta del negozio](assets/asc-dashboard-after-2fa.png)

Il tuo nuovo archivio canali di vendita Amazon è ora connesso al tuo account [!DNL Amazon Seller Central].

![Icona successiva](assets/btn-next.png) [**Continua a creare una regola di elenco**](./ob-create-listing-rule.md)
