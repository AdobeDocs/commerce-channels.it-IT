---
title: Onboarding [!DNL Channel Manager]
description: '''Connetti l''istanza al servizio [!DNL Channel Manager] completando alcuni passaggi di onboarding.'''
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---


# Onboarding [!DNL Channel Manager]

Dopo aver completato il processo di onboarding di Channel Manager, puoi accedere, configurare e gestire le operazioni di vendita dei canali di Walmart Marketplace da Adobe Commerce. Channel Manager è disponibile dall&#39;opzione [!UICONTROL Channel Manager] nel menu [!UICONTROL Commerce Admin Marketing].

Opzione ![[!DNL Channel Manager] nella visualizzazione Amministratore](assets/channel-manager-admin-view.png){width="500"}

## Requisiti

Controlla i requisiti per l’utilizzo di Channel Manager e raccogli le informazioni e le credenziali dell’account necessarie per scaricare, installare e configurare l’estensione.

- **[Requisiti di Walmart Marketplace](walmart-requirements.md)**-Verificare di soddisfare i requisiti per l&#39;integrazione con Channel Manager, tra cui [configurazione dell&#39;account del venditore](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) e generazione della chiave API per abilitare l&#39;integrazione.

- **Informazioni sull&#39;account Commerce**-Il download e l&#39;installazione di [!DNL Channel Manager] richiede un [account Commerce](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html). È necessario disporre di un ID account e di credenziali con accesso di proprietario o amministratore all&#39;istanza [!DNL Adobe Commerce] o [!DNL Magento Open Source].

   - **ID IMMAGINE**-[Accedi](https://account.magento.com/customer/account/login/) all&#39;account [!DNL Commerce] per ottenere l&#39;ID da **[!UICONTROL My Account - Magento settings]**.

     ![[!DNL MAGEID] su [!DNL Commerce] impostazioni account](assets/mageid-my-commerce-account.png){width="250"}

   - **Chiavi di accesso-** Ottenere le chiavi di autenticazione per scaricare [!DNL Commerce] estensioni dall&#39;archivio del Compositore [!DNL Commerce] `([!DNL repo.magento.com]`).

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Nei progetti Adobe Commerce e Magento Open Source, il proprietario può impostare [Accesso condiviso](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) per consentire ai dipendenti e ai provider di servizi attendibili di scaricare estensioni utilizzando le credenziali dell&#39;account Proprietario o del titolare della licenza.

     Per [!DNL Adobe Commerce] sui progetti di infrastruttura cloud, i programmi di installazione software devono avere il seguente accesso all&#39;istanza [!DNL Commerce]:

      - Accesso utente privilegiato al progetto Cloud
      - Accesso amministratore a un ambiente specifico
      - un account [!DNL Adobe Commerce] con autorizzazioni di accesso all&#39;archivio del Compositore

     Consulta [Gestire l&#39;accesso utente](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) nella *Guida all&#39;infrastruttura cloud di Commerce*.

- **Esperienza con Composer e[!DNL Commerce CLI]**-Per informazioni sull&#39;utilizzo di questi strumenti per installare e gestire le estensioni sulle piattaforme [!DNL Adobe Commerce] o [!DNL Magento Open Source], vedere [Installare un&#39;estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) nella *Guida all&#39;installazione*.

- **[[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Se hai attivato [!DNL Amazon Sales Channel] per i tuoi siti [!DNL Commerce], verifica che nella piattaforma [!DNL Commerce] sia installata la versione 4.4.2 o successiva prima di installare [!DNL Channel Manager].

- Estensione **[!DNL Inventory Management]per Adobe Commerce e Magento Open Source**

  Se prevedi di utilizzare Channel Manager per la gestione dell’inventario e degli ordini, devi aver installato e abilitato l’estensione Inventory management nell’istanza Adobe Commerce e di Magento Open Source. In genere, questa estensione viene installata e abilitata per impostazione predefinita in Adobe Commerce e [!DNL Magento Open Source] 2.3.x e versioni successive.

  Se hai aggiornato Commerce dalla versione 2.2.x o hai disabilitato Inventory management, aggiorna l’installazione per includere i moduli richiesti. Consulta [Installare Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html) nella *Guida di Inventory management*.

### Requisiti di sistema

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7.3 / 7.4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [Compositore 1.x o versione successiva](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Se hai attivato [!DNL Amazon Sales Channel] per i tuoi siti [!DNL Commerce], verifica che nella piattaforma [!DNL Commerce] sia installata la versione 4.4.2 prima di installare [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### Piattaforme supportate

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce on premise (EE) : 2.4.x
- Magento Open Source 2.4.x

## Passaggi di onboarding

1. [Configura il tuo account venditore Walmart](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installa  [!DNL Channel Manager] estensione](install.md).

1. [Connettiti a Commerce Services](connect.md) per integrare Channel Manager con l&#39;istanza di Commerce e altri servizi di supporto.

1. [Connetti il tuo archivio [!DNL Commerce] a [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Completare la configurazione dell&#39;archivio](complete-sales-channel-store-setup.md).
