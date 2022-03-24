---
title: Connessione a Commerce Services
description: Collega l'istanza di Channel Manager a [!DNL Commerce services] per abilitare la sincronizzazione dei dati e la comunicazione tra l’istanza Commerce, Channel Manager e altri servizi di supporto.
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Connessione a Commerce Services

Commerce Services Connector integra il servizio Channel Manager con le istanze Adobe Commerce e Magenti Open Source. Il connettore consente la sincronizzazione dei dati e la comunicazione tra [!DNL Commerce] istanza, [!DNL Channel Manager]e altri servizi di supporto.

La configurazione di Commerce Services Connector è un processo una tantum necessario per utilizzare Adobe [Servizi SaaS di Commerce](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;} come [!DNL Channel Manager], [!DNL Live Search]e [!DNL Product Recommendations]. Se hai già configurato il connettore per un altro servizio, salta questo passaggio.

## Prerequisiti

- **Account Commerce**-Per installare il software nelle istanze Commerce, è necessario disporre di un account con accesso Proprietario o Amministratore alla piattaforma Commerce.

   I proprietari dell’account e gli utenti amministratori possono creare nuovi account Admin dall’istanza Commerce o dalla riga di comando utilizzando [!DNL Commerce] Comando CLI `admin:user:create`.

- **Chiave API di produzione Adobe Commerce**-This [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} abilita l&#39;accesso API ai servizi richiesti da Channel Manager. Per questa chiave sono necessarie le credenziali pubbliche e private.

   Per fornire le credenziali, il titolare di una licenza Commerce o il proprietario di un account dispone di opzioni per
   [accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;}, oppure fornisci [Chiave API](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} credenziali a uno sviluppatore fidato.

## Configurare Commerce Services Connector

1. Apri la configurazione dei servizi store.

   - Dall’amministratore, seleziona **[!UICONTROL Stores]**.

   - Sotto *Impostazioni*, seleziona **[!UICONTROL Configuration]**.

   - Espandi **[!UICONTROL Services]** e seleziona **[!UICONTROL Commerce Services Connector]**.

1. Aggiungi le credenziali della chiave API di produzione dal tuo account Adobe Commerce.

   ![[!DNL Commerce Service Connector] nel [!DNL Admin] visualizzare](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Se [!DNL Commerce] l&#39;istanza ha un altro [!DNL Adobe Commerce] servizi come [!DNL Live Search] o [!DNL Product Recommendations] installate, le informazioni sulle credenziali vengono visualizzate nell&#39;interfaccia e non è richiesta alcuna ulteriore configurazione.

1. Configura il progetto SaaS e lo spazio dati in modo che Commerce Services possa inviare dati al servizio Channel Manager.

   ![[!DNL Commerce Service Connector] Configurazione dell’identificatore SaaS nel [!DNL Admin] visualizzare](assets/commerce-services-connector-saas-config.png)

