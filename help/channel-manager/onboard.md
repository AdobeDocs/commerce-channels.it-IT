---
title: '"A bordo [!DNL Channel Manager]"'
description: Collega l’istanza a [!DNL Channel Manager] per completare alcune fasi di onboarding.
role: User
level: Intermediate
source-git-commit: ff87f31fec7a689385a93b8cab260fd93ff15f90
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Onboard [!DNL Channel Manager]

Channel Manager integrato installando l&#39;estensione Channel Manager sul tuo [!DNL Commerce] istanza e configurazione delle connessioni API per abilitare la comunicazione e la sincronizzazione dei dati tra la tua istanza Commerce e Walmart Marketplace.

Dopo aver completato l&#39;onboarding, puoi configurare e gestire le operazioni sui canali di vendita da [!UICONTROL Channel Manager] l&#39;opzione [!UICONTROL Commerce Admin Marketing] menu.

![[!DNL Channel Manager] in visualizzazione Amministratore](assets/channel-manager-admin-view.png)

## Panoramica sull’onboarding

1. [Installa il [!DNL Channel Manager] estensione](install.md).

1. [Configura le [!DNL Commerce Services Connector]](connect.md) per integrare Channel Manager con l’istanza Commerce e altri servizi di supporto.

1. [Collega il tuo [!DNL Commerce] archiviare [!DNL Walmart Marketplace]](connect.md).

## Prerequisiti

- Verifica di avere Walmart Marketplace Seller AccountWalmart requisiti per la vendita su Walmart Marketplace

- **Informazioni sull’account Commerce**- Download e installazione [!DNL Channel Manager] richiede un ID e le credenziali di un [Account Commerce](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;} con accesso del proprietario al [!DNL Adobe Commerce] o [!DNL Magento Open Source] istanza.

   - **ID MAGLIA**-[Accedere](https://account.magento.com/customer/account/login/) all’account Commerce per ottenere l’ID da [!UICONTROL My Account - Magento settings]. È necessario questo ID per registrarsi al [!DNL Channel Manager] servizio Beta.

      ![[!DNL MAGEID] sulle impostazioni dell’account Commerce](assets/mageid-my-commerce-account.png)

   - **Tasti di accesso-** Ottieni le chiavi di autenticazione per scaricare estensioni Commerce dall’archivio Commerce Composer ([!DNL repo.magento.com]).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Nei progetti Adobe Commerce e Magenti Open Source, il proprietario può configurare [Accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html) per consentire ai dipendenti e ai fornitori di servizi attendibili di scaricare estensioni utilizzando le credenziali dell’account proprietario o del titolare della licenza.

      On [!DNL Adobe Commerce] nei progetti di infrastruttura cloud, gli utenti devono disporre delle seguenti autorizzazioni per installare il software [!DNL Commerce] istanza:

      - Accesso utente privilegiato al progetto Cloud
      - Accesso dell’amministratore a un ambiente specifico
      - un [!DNL Adobe Commerce] o [!DNL Magento Open Source] account con autorizzazioni per accedere all’archivio Composer. Vedi [Gestire l’accesso utente](https://devdocs.magento.com/cloud/project/user-admin.html).

- **Autorizzazione per scaricare il pacchetto del Compositore canali**- Fornisci l’ID MAGINE dall’account Commerce utilizzato per gestire il servizio al rappresentante Adobe che coordina il programma Beta per la tua organizzazione.
- **Esperienza con Compositore e[!DNL Commerce CLI]** -Vedi [Installazione generale CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} per informazioni sull&#39;utilizzo di questi strumenti per installare e gestire le estensioni su A[!DNL Adobe Commerce] o [!DNL Magento Open Source] piattaforme.
- Per le istanze Commerce con Amazon Sales Channel installato, verifica che [Amazon Sales Channel versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) è installato prima dell&#39;installazione di Channel Manager.


### Requisiti

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Compositore 1.x o successivo](https://devdocs.magento.com/cloud/reference/cloud-composer.html)


### Piattaforme supportate

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce nei locali (EE) : 2.4.x
- Magenti Open Source 2.4.x
