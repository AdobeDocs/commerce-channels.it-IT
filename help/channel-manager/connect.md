---
title: 'Connetti a [!DNL Commerce] Servizi'
description: "Connetti Channel Manager a [!DNL Commerce] servizi per consentire la sincronizzazione dei dati e la comunicazione tra [!DNL Commerce] , Channel Manager e altri servizi di supporto."
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# Connetti a [!DNL Commerce] Servizi

Il [!DNL Commerce Services Connector] integra il servizio Channel Manager con Adobe Commerce e le istanze di Magento Open Source. Il connettore consente la sincronizzazione dei dati e la comunicazione tra [!DNL Commerce] istanza, [!DNL Channel Manager]e altri servizi di supporto.

[!DNL Commerce Services Connector] la configurazione è un processo una tantum necessario per utilizzare [Servizi SaaS di Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target="_blank"} come [!DNL Channel Manager], [!DNL Live Search], e [!DNL Product Recommendations]. Se hai già configurato il connettore per un altro servizio, salta questo passaggio.

## Requisiti

- **Account Commerce**-Per installare il software su [!DNL Commerce] istanze, è necessario disporre di un account con accesso Proprietario o Amministratore al [!DNL Commerce] piattaforma.

   I proprietari degli account e gli utenti con privilegi avanzati possono creare account amministratore dal [!DNL Commerce] o dalla riga di comando utilizzando [!DNL Commerce] Comando CLI `admin:user:create`.

- **Chiave API di produzione Adobe Commerce**-Questo [chiave](https://docs.magento.com/user-guide/system/saas.html#apikey){target="_blank"} consente l’accesso API ai servizi richiesti da Channel Manager. Sono necessarie le credenziali pubbliche e private per questa chiave.

>[!TIP]
>
>Per fornire le credenziali, è necessario [!DNL Commerce] il titolare della licenza o il proprietario dell’account dispone di opzioni per [accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html){target="_blank"}, or give the [API Key](https://docs.magento.com/user-guide/system/saas.html#apikey){target="_blank"} credenziali a uno sviluppatore attendibile.

## Configurare [!DNL Commerce Services Connector]

1. Apri Configurazione servizi di archiviazione.

   - Dall’amministratore, seleziona **[!UICONTROL Stores]**.

   - Sotto *[!UICONTROL Settings]*, seleziona **[!UICONTROL Configuration]**.

   - Espandi **[!UICONTROL Services]** e seleziona **[!UICONTROL Commerce Services Connector]**.

1. Aggiungi le credenziali della chiave API di produzione dal tuo account Adobe Commerce.

   ![[!DNL Commerce Services Connector] servizio in [!DNL Admin] visualizza](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Se il [!DNL Commerce] l&#39;istanza ha altro [!DNL Adobe Commerce] servizi come [!DNL Live Search] o [!DNL Product Recommendations] installate, le informazioni sulle credenziali vengono visualizzate nell’interfaccia e non è richiesta alcuna ulteriore configurazione.

1. Configura il progetto SaaS e lo spazio dati in modo che Commerce Services possa inviare dati al servizio Channel Manager.

   ![[!DNL Commerce Services Connector] Configurazione dell’identificatore SaaS in [!DNL Admin] visualizza](assets/commerce-services-connector-saas-config.png)

