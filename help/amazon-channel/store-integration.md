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

Per iniziare a utilizzare il canale di vendita Amazon, devi creare (aggiungere) un negozio di canali di vendita Amazon e collegarlo al tuo account venditore Amazon. Questi due passaggi integrano i [!DNL Commerce] e account Amazon per condividere dati, sincronizzare prodotti e altro ancora.

_Sono necessarie le credenziali di accesso principali per [!DNL Amazon Seller Central] account (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore) per collegare il tuo negozio._

>[!NOTE]
>
>Dopo l&#39;integrazione del primo negozio, ogni anno ti verrà richiesto di rinnovare la connessione del canale di vendita Amazon ad Amazon concedendo nuovamente l&#39;accesso. Puoi rinnovare o revocare questa autorizzazione nel _Autorizzazioni correnti_ nella tabella _Autorizzazioni per sviluppatori Amazon MWS_ della sezione **Impostazioni** > **Autorizzazioni utente** pagina del tuo account Seller Central.

## Aggiungere un archivio Amazon

1. Sulla _Amministratore_ barra laterale, vai a **Marketing** > _Canali_ > **Sales Channel Amazon**.

   Quando aggiungi il tuo primo archivio canali di vendita Amazon, la _Attività pre-installazione_ viene visualizzato modale. Dopo l&#39;aggiunta del primo store, è possibile accedere alle attività pre-installazione nel [Pagina principale del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina sotto _Apprendimento e preparazione_ nel menu a sinistra.

1. Clic **[!UICONTROL Add Amazon Store]**.

   La _[!UICONTROL Add Amazon sales channel]_viene visualizzata la pagina .

   ![Aggiungi l&#39;archivio canali di vendita Amazon](assets/amazon-store-integration.png)

1. Per **[!UICONTROL Magento Website to use for Amazon Listing]**, scegli quale [!DNL Commerce] siti web da collegare a questo archivio canali di vendita Amazon.

   Questa impostazione definisce anche il valore predefinito [!DNL Commerce] memorizzare [importazione di ordini Amazon](./order-settings.md).

1. Per **[!UICONTROL Email Address]**, inserisci l&#39;indirizzo e-mail del contatto preferito.

1. Per **[!UICONTROL New Store Name]**, inserisci un nome descrittivo per il nuovo archivio canali di vendita Amazon.

   >[!NOTE]
   >
   >Questo nome viene utilizzato come [!DNL Commerce] solo il riferimento e identifica l&#39;archivio sul [Pagina principale del canale di vendita Amazon](./amazon-sales-channel-home.md) pagina. Vuoi renderlo qualcosa che il tuo team può facilmente identificare. Ad esempio, potrebbe essere denominato il tuo negozio Amazon che vende nell’area degli Stati Uniti `Amazon Store USA`.

1. Per **[!UICONTROL Amazon Marketplace Country]**, scegli la regione/il paese in cui questo negozio di canale di vendita Amazon vende prodotti. Opzioni:

   - Stati Uniti
   - Canada
   - Messico
   - Regno Unito

1. In _[!UICONTROL Map your Magento attributes to Amazon]_eseguire le operazioni seguenti:

   - Per **[!UICONTROL Product ID on the Amazon market]**, scegli l’attributo Amazon da mappare al [!DNL Commerce] attributo selezionato di seguito.

      Questo ID aiuta a far corrispondere correttamente i prodotti corrispondenti nel tuo [!DNL Commerce] catalogo.

   - Per **[!UICONTROL Map a Magento attribute]**, scegli [!DNL Commerce] attributo di prodotto da mappare all’attributo Amazon selezionato in precedenza.

      [Attributi di mappatura](./ob-creating-magento-attributes.md) garantisce che l’elenco di Amazon corrisponda correttamente al prodotto corrispondente nel tuo [!DNL Commerce] catalogo.

1. Clic **[!UICONTROL Connect]**.

   La finestra di dialogo si chiude e il nuovo archivio viene visualizzato sul [Pagina principale del canale di vendita Amazon](./amazon-sales-channel-home.md) con un messaggio di conferma.

## Collegare uno store a [!DNL Amazon Seller Central]

1. Nel dashboard dello store, fai clic su **[!UICONTROL Connect store]** sulla scheda del negozio da avviare [!DNL Amazon Seller Central] in una nuova scheda.

1. Inserisci il tuo [!DNL Amazon Seller Central] credenziali account e fai clic su **[!UICONTROL Sign in]**.

   Per completare questa connessione, devi accedere al tuo [!DNL Amazon Seller Central] account che utilizza le credenziali di accesso per l&#39;utente principale (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore).

1. Se richiesto, completa Amazon Two-Factor Authorization (2FA) immettendo il codice ricevuto da Amazon e fai clic su **[!UICONTROL Sign in]**.

1. Sulla _[!UICONTROL Amazon Marketplace Web Service]_nella pagina di conferma, seleziona &quot;[!UICONTROL I understand...]&quot; e fai clic su **[!UICONTROL Next]**.

1. Sulla _[!UICONTROL You are almost done]_messaggio, fai clic su **[!UICONTROL Continue]**.

   Hai concesso l’autorizzazione del canale di vendita Amazon per accedere e condividere i dati con il tuo [!DNL Amazon Seller Central] conto. La pagina Amazon viene chiusa e viene visualizzato un messaggio di conferma.

   La [Pagina principale del canale di vendita Amazon](./amazon-sales-channel-home.md) vengono visualizzate le schede Amazon store.

   Per visualizzare il dashboard dell&#39;archivio, fai clic su **[!UICONTROL View Store]** sulla scheda del negozio.

![Casa del canale di vendita Amazon con nuova carta del negozio](assets/asc-dashboard-after-2fa.png)

Il tuo nuovo archivio canali di vendita Amazon è ora connesso al tuo [!DNL Amazon Seller Central] conto.

![Icona Successivo](assets/btn-next.png) [**Continua a creare una regola di elenco**](./ob-create-listing-rule.md)
