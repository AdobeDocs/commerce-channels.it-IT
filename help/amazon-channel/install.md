---
title: Installare l’estensione
description: Per integrare il  [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] e vendere tramite [!DNL Amazon Marketplace], scarica e installa l’estensione Amazon Sales Channel.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installare l’estensione

>[!IMPORTANT]
>
>Solo le versioni [!DNL Amazon Sales Channel] dell&#39;estensione 4.0+ sono supportate per Adobe Commerce e Magenti Open Source 2.4.x . Se esegui una versione 2.3.x, consulta la documentazione relativa alla versione [canale di vendita Amazon compatibile](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}. Per ulteriori informazioni sulla compatibilità delle versioni, consulta la pagina [Disponibilità](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.

L’ estensione [!UICONTROL Amazon Sales Channel] installa e aggiunge funzionalità per integrare il catalogo Commerce con [!DNL Amazon Seller Accounts] per la vendita tramite [!DNL Amazon Marketplace]. Per ulteriori informazioni, consulta la pagina [Sales Channel Amazon](https://marketplace.magento.com/magento-module-amazon.html) in [!DNL Commerce Marketplace] e le [note sulla versione](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) nella documentazione per gli sviluppatori.

## Requisiti

- **Istanza** Commerce: L’ [!DNL Amazon Sales Channel] estensione può essere installata su istanze con Magenti Open Source, Adobe Commerce e Adobe Commerce sulle versioni 2.3.x o successive dell’infrastruttura cloud. Non è più supportato nelle versioni 2.1, 2.2 o 1.x.
- **Account** Web Commerce: Devi disporre di un account web Commerce, utilizzato per creare e monitorare una chiave API.
- **Chiave** API: Crea una chiave API del canale di vendita Amazon tramite il tuo account web Commerce. Le istruzioni seguenti includono questi passaggi.

## Installa

Per informazioni più dettagliate sull&#39;utilizzo di Composer per questo processo, consulta le istruzioni [extension installation](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Fare clic sulla scheda **[!UICONTROL Marketplace]**, quindi fare clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione , seleziona la versione .

1. Per il nome e la versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Utilizza il nome e le informazioni sulla versione per aggiornare la voce del connettore servizi nel file `composer.json`.

   - Aggiungi il nome e la versione dell&#39;estensione al file `composer.json`.

   - Passa alla directory di progetto [!DNL Commerce] e aggiorna il file `composer.json`.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Immetti le [chiavi di autenticazione](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}. La tua chiave pubblica è il tuo nome utente; la tua chiave privata è la tua password.

   - Attendi che Compositore completi l’aggiornamento delle dipendenze del progetto e assicurati che non ci siano errori.


1. [Verifica l&#39;estensione](https://devdocs.magento.com/extensions/install/#verify-the-extension) {target=&quot;_blank&quot;}.

## Aggiungi la chiave API del canale di vendita Amazon

Dopo l&#39;installazione, immetti una [chiave API](./amazon-verify-api-key.md) per completare la configurazione.

## Impostare le opzioni di configurazione del canale Amazon

Hai le seguenti opzioni per configurare il canale di vendita Amazon. Non è necessario modificare queste impostazioni per iniziare l’onboarding e la vendita su Amazon. È consigliabile che gli amministratori avanzati considerino queste opzioni.

1. Accedi all’amministratore.

1. Nella barra laterale _Amministratore_, vai a **Negozi** > _Impostazioni_ > **Configurazione**.

1. Fare clic su **Sales Channel**, quindi su **Impostazioni globali**.

1. Per **Cancella cronologia log**, definire l&#39;intervallo per la cancellazione dei log raccolti.

   Le opzioni disponibili sono `Once Daily`, `Once Weekly` e `Once Monthly` (predefinito).

1. (Facoltativo) Per **Origine attività in background (CRON)**, modificare l&#39;impostazione su `Command Line (CLI) CRON`.

   Questa impostazione è consigliata per **_utenti/amministratori avanzati_**.

1. Fare clic su **[!UICONTROL Save Config]**.

## Aggiorna l&#39;estensione

1. Accedi a [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. Fare clic sulla scheda **[!UICONTROL Marketplace]**, quindi fare clic su **[!UICONTROL My Purchases]**.

1. Individua e seleziona **[!UICONTROL Amazon Sales Channel]**.

1. Nella pagina dell&#39;estensione , seleziona la versione .

1. Per il nome e la versione del componente, fai clic su **[!UICONTROL Technical Details]**.

1. Completa le [istruzioni per l&#39;aggiornamento dell&#39;estensione](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;} nella documentazione per gli sviluppatori.
