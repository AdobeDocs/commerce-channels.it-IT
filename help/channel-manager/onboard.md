---
title: Onboard [!DNL Channel Manager]
description: '''Collega l''istanza a [!DNL Channel Manager] completando alcuni passaggi di onboarding."'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 738c48b8b8075e7c8bbf883c58cc8de39bca355c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Onboard [!DNL Channel Manager]

Dopo aver completato il processo di onboarding di Channel Manager, puoi accedere, configurare e gestire le operazioni di vendita dei canali di Walmart Marketplace da Adobe Commerce. Channel Manager è disponibile dal [!UICONTROL Channel Manager] l&#39;opzione [!UICONTROL Commerce Admin Marketing] menu.

![[!DNL Channel Manager] in visualizzazione Amministratore](assets/channel-manager-admin-view.png)

## Requisiti

Rivedi i requisiti per l’utilizzo di Channel Manager e raccogli le informazioni e le credenziali dell’account necessarie per scaricare, installare e configurare l’estensione.

- **[Requisiti di Marketplace di Walmart](walmart-requirements.md)**- Verifica di soddisfare i requisiti per l&#39;integrazione con Channel Manager, tra cui [configurazione del tuo account Seller](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) e genera la chiave API per abilitare l’integrazione.

- **Informazioni sull’account Commerce**- Download e installazione [!DNL Channel Manager] richiede un [Account Commerce](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. È necessario un ID account e le credenziali con accesso Proprietario o Amministratore al [!DNL Adobe Commerce] o [!DNL Magento Open Source] istanza.

   - **ID MAGLIA**-[Accedere](https://account.magento.com/customer/account/login/) al [!DNL Commerce] per ottenere l&#39;ID da **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] su [!DNL Commerce] impostazioni account](assets/mageid-my-commerce-account.png)

   - **Tasti di accesso-** Scarica le chiavi di autenticazione [!DNL Commerce] estensioni da [!DNL Commerce] Archivio compositore `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Nei progetti Adobe Commerce e Magenti Open Source, il proprietario può configurare [Accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html) per consentire ai dipendenti e ai fornitori di servizi attendibili di scaricare estensioni utilizzando le credenziali dell’account proprietario o del titolare della licenza.

      Per [!DNL Adobe Commerce] nei progetti di infrastruttura cloud, i programmi di installazione del software devono avere i seguenti accessi [!DNL Commerce] istanza:

      - Accesso utente privilegiato al progetto Cloud
      - Accesso dell’amministratore a un ambiente specifico
      - un [!DNL Adobe Commerce] account con autorizzazioni per accedere all&#39;archivio Composer

      Vedi [Gestire l’accesso utente](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Esperienza con Compositore e[!DNL Commerce CLI]**-Vedi [Installazione generale CLI](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} per informazioni sull&#39;utilizzo di questi strumenti per installare e gestire le estensioni in [!DNL Adobe Commerce] o [!DNL Magento Open Source] piattaforme.

- **[[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Se attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che [!DNL Commerce] prima dell’installazione di Platform è installata la versione 4.4.2 o successiva [!DNL Channel Manager].

- **[!DNL Inventory Management]estensione per Adobe Commerce e Magenti Open Source**

   Se intendi utilizzare Channel Manager per la gestione dell&#39;inventario e dell&#39;ordine, devi avere l&#39;estensione Inventory management installata e abilitata nell&#39;istanza Adobe Commerce e Magenti Open Source. In genere, questa estensione viene installata e abilitata per impostazione predefinita su Adobe Commerce e [!DNL Magento Open Source] 2.3.x e versioni successive.

   Se hai aggiornato Commerce dalla versione 2.2.x o se hai disabilitato Inventory management, aggiorna l’installazione per includere i moduli richiesti. Vedi [Installare Inventory management](https://devdocs.magento.com/extensions/inventory-management/) nella documentazione per sviluppatori di Adobe Commerce.

### Requisiti di sistema

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Compositore 1.x o successivo](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] versione 4.4.2 o successiva](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Se hai attivato [!DNL Amazon Sales Channel] per [!DNL Commerce] siti, verifica che [!DNL Commerce] la versione 4.4.2 di platform è installata prima dell&#39;installazione [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### Piattaforme supportate

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce nei locali (EE) : 2.4.x
- Magenti Open Source 2.4.x

## Passaggi di onboarding

1. [Imposta il tuo account Venditore Walmart](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installa il [!DNL Channel Manager] estensione](install.md).

1. [Connessione a Commerce Services](connect.md) per integrare Channel Manager con l’istanza Commerce e altri servizi di supporto.

1. [Collega il tuo [!DNL Commerce] archiviare [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Configurazione completa dello store](complete-sales-channel-store-setup.md).
