---
title: Onboard [!DNL Channel Manager]
description: Collega l’istanza a [!DNL Channel Manager] per completare alcune fasi di onboarding.
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 41a6afec60edbb23492627bd8e80632d3c952caf
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---


# Onboard [!DNL Channel Manager]

Channel Manager integrato installando l&#39;estensione Channel Manager sul tuo [!DNL Commerce] istanza e configurazione delle connessioni API. Queste connessioni consentono la comunicazione e la sincronizzazione dei dati tra la tua istanza Commerce e [!DNL Walmart Marketplace].

Dopo aver completato l&#39;onboarding, configura e gestisci le operazioni sui canali di vendita dal [!UICONTROL Channel Manager] l&#39;opzione [!UICONTROL Commerce Admin Marketing] menu.

![[!DNL Channel Manager] in visualizzazione Amministratore](assets/channel-manager-admin-view.png)

## Panoramica sull’onboarding

1. [Installa il [!DNL Channel Manager] estensione](install.md).

1. [Configura le [!DNL Commerce Services Connector]](connect.md) per integrare Channel Manager con l’istanza Commerce e altri servizi di supporto.

1. [Collega il tuo [!DNL Commerce] archiviare [!DNL Walmart Marketplace]](connect.md).

1. [Configurazione completa dello store](complete-store-setup.md).

## Prerequisiti

- Verifica di disporre dei requisiti necessari [Prerequisiti per Walmart Marketplace](walmart-prerequisites.md) per l’integrazione con Channel Manager.

- **Informazioni sull’account Commerce**- Download e installazione [!DNL Channel Manager] richiede un [Account Commerce](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. È necessario un ID account e le credenziali con accesso Proprietario o Amministratore al [!DNL Adobe Commerce] o [!DNL Magento Open Source] istanza.

   - **ID MAGLIA**-[Accedere](https://account.magento.com/customer/account/login/) all’account Commerce per ottenere l’ID da **[!UICONTROL My Account - Magento settings]**. È necessario questo ID per registrarsi al [!DNL Channel Manager] servizio Beta.

      ![[!DNL MAGEID] sulle impostazioni dell’account Commerce](assets/mageid-my-commerce-account.png)

   - **Tasti di accesso-** Ottenere le chiavi di autenticazione per scaricare estensioni Commerce dall’archivio Commerce Composer `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Nei progetti Adobe Commerce e Magenti Open Source, il proprietario può configurare [Accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html) per consentire ai dipendenti e ai fornitori di servizi attendibili di scaricare estensioni utilizzando le credenziali dell’account proprietario o del titolare della licenza.

      Per [!DNL Adobe Commerce] nei progetti di infrastruttura cloud, i programmi di installazione del software devono avere i seguenti accessi [!DNL Commerce] istanza:

      - Accesso utente privilegiato al progetto Cloud
      - Accesso dell’amministratore a un ambiente specifico
      - un [!DNL Adobe Commerce] o [!DNL Magento Open Source] account con autorizzazioni per accedere all&#39;archivio Composer

      Vedi [Gestire l’accesso utente](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Autorizzazione per scaricare il pacchetto del Compositore canali**- Fornisci al coordinatore beta per Adobe Channel l&#39;ID MAGE del [!DNL Commerce] account utilizzato per gestire il servizio per la tua organizzazione.
- **Esperienza con Compositore e[!DNL Commerce CLI]** -Vedi [Installazione generale CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} per informazioni sull&#39;utilizzo di questi strumenti per installare e gestire le estensioni in [!DNL Adobe Commerce] o [!DNL Magento Open Source] piattaforme.
- [[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Se hai attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che [!DNL Commerce] la versione 4.42 di platform è installata prima dell’installazione [!DNL Channel Manager].

### Requisiti

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Compositore 1.x o successivo](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Se hai attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che [!DNL Commerce] la versione 4.42 di platform è installata prima dell’installazione [!DNL Channel Manager].
- [!DNL Inventory Management]


### Piattaforme supportate

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce nei locali (EE) : 2.4.x
- Magenti Open Source 2.4.x
