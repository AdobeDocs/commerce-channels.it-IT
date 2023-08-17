---
title: Onboarding [!DNL Channel Manager]
description: "Connetti l’istanza a [!DNL Channel Manager] completando alcuni passaggi di onboarding."
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# Onboarding [!DNL Channel Manager]

Dopo aver completato il processo di onboarding di Channel Manager, puoi accedere, configurare e gestire le operazioni di vendita dei canali di Walmart Marketplace da Adobe Commerce. Channel Manager è disponibile dal [!UICONTROL Channel Manager] opzione sul [!UICONTROL Commerce Admin Marketing] menu.

![[!DNL Channel Manager] Opzione in visualizzazione Amministratore](assets/channel-manager-admin-view.png){width="500"}

## Requisiti

Controlla i requisiti per l’utilizzo di Channel Manager e raccogli le informazioni e le credenziali dell’account necessarie per scaricare, installare e configurare l’estensione.

- **[Requisiti di Walmart Marketplace](walmart-requirements.md)**-Verificare che siano soddisfatti i requisiti per l&#39;integrazione con Channel Manager, tra cui [configurazione dell&#39;account del venditore](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) e la generazione della chiave API per abilitare l’integrazione.

- **Informazioni account Commerce**-Download e installazione [!DNL Channel Manager] richiede un [Account Commerce](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html). È necessario disporre di un ID account e delle credenziali con accesso Proprietario o Amministratore al [!DNL Adobe Commerce] o [!DNL Magento Open Source] dell&#39;istanza.

   - **ID IMMAGINE**-[Accedi](https://account.magento.com/customer/account/login/) al [!DNL Commerce] account da cui ottenere l’ID **[!UICONTROL My Account - Magento settings]**.

     ![[!DNL MAGEID] il [!DNL Commerce] impostazioni account](assets/mageid-my-commerce-account.png){width="250"}

   - **Tasti di accesso-** Ottieni chiavi di autenticazione da scaricare [!DNL Commerce] estensioni da [!DNL Commerce] Repository del compositore `([!DNL repo.magento.com]`).

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Nei progetti Adobe Commerce e di Magento Open Source, il proprietario può impostare [Accesso condiviso](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) per consentire ai dipendenti e ai fornitori di servizi attendibili di scaricare estensioni utilizzando le credenziali dell&#39;account Proprietario o del titolare della licenza.

     Per [!DNL Adobe Commerce] nei progetti di infrastruttura cloud, i programmi di installazione del software devono disporre dei seguenti diritti di accesso [!DNL Commerce] istanza:

      - Accesso utente privilegiato al progetto Cloud
      - Accesso amministratore a un ambiente specifico
      - un [!DNL Adobe Commerce] account con autorizzazioni per accedere all’archivio del Compositore

     Consulta [Gestire l’accesso degli utenti](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) nel *Guida di Commerce su infrastruttura cloud*.

- **Esperienza utilizzando Compositore e[!DNL Commerce CLI]**-Vedere [Installare un’estensione](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) nel *Guida all’installazione* per informazioni sull&#39;utilizzo di questi strumenti per installare e gestire le estensioni su [!DNL Adobe Commerce] o [!DNL Magento Open Source] piattaforme.

- **[[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Se è stato attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che il tuo [!DNL Commerce] sulla piattaforma è installata la versione 4.4.2 o successiva prima dell’installazione [!DNL Channel Manager].

- **[!DNL Inventory Management]estensione per Adobe Commerce e Magento Open Source**

  Se prevedi di utilizzare Channel Manager per la gestione dell’inventario e degli ordini, devi aver installato e abilitato l’estensione Inventory management nell’istanza Adobe Commerce e di Magento Open Source. In genere, questa estensione viene installata e abilitata per impostazione predefinita in Adobe Commerce e [!DNL Magento Open Source] 2.3.x e versioni successive.

  Se hai aggiornato Commerce dalla versione 2.2.x o se hai disabilitato Inventory management, aggiorna l’installazione per includere i moduli richiesti. Consulta [Installare Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html) nel *Guida di Inventory management*.

### Requisiti di sistema

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7,3 / 7,4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [Compositore 1.x o versione successiva](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Se è stato attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che il tuo [!DNL Commerce] sulla piattaforma è installata la versione 4.4.2 prima dell’installazione [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### Piattaforme supportate

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce on premise (EE) : 2.4.x
- Magento Open Source 2.4.x

## Passaggi di onboarding

1. [Configura il tuo account del venditore Walmart](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installare [!DNL Channel Manager] estensione](install.md).

1. [Connetti a Commerce Services](connect.md) integrare Channel Manager con l’istanza Commerce e altri servizi di supporto.

1. [Connetti [!DNL Commerce] memorizza in [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Completa la configurazione del negozio](complete-sales-channel-store-setup.md).
