---
title: 'Connetti a [!DNL Commerce] Servizi'
description: '''Connetti Channel Manager ai servizi [!DNL Commerce] per abilitare la sincronizzazione dei dati e la comunicazione tra l''istanza [!DNL Commerce] , Channel Manager e altri servizi di supporto.'''
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Connetti a [!DNL Commerce] servizi

[!DNL Commerce Services Connector] integra il servizio Channel Manager con le istanze Adobe Commerce e Magento Open Source. Il connettore consente la sincronizzazione dei dati e la comunicazione tra l&#39;istanza [!DNL Commerce], [!DNL Channel Manager] e altri servizi di supporto.

L&#39;installazione di [!DNL Commerce Services Connector] è un processo occasionale necessario per utilizzare [i servizi SaaS di Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) quali [!DNL Channel Manager], [!DNL Live Search] e [!DNL Product Recommendations]. Se hai già configurato il connettore per un altro servizio, salta questo passaggio.

## Requisiti

- **Account Commerce**-Per installare il software nelle istanze di [!DNL Commerce], è necessario disporre di un account con accesso proprietario o amministratore alla piattaforma [!DNL Commerce].

  I proprietari degli account e gli utenti privilegiati possono creare account amministratore dall&#39;istanza [!DNL Commerce] o dalla riga di comando utilizzando il comando CLI [!DNL Commerce] `admin:user:create`.

- **Chiave API di produzione Adobe Commerce**-Questa [chiave](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) consente l&#39;accesso API ai servizi richiesti da Channel Manager. Sono necessarie le credenziali pubbliche e private per questa chiave.

>[!TIP]
>
>Per fornire le credenziali, il titolare di licenza o il proprietario dell&#39;account [!DNL Commerce] dispone delle opzioni per [condividere l&#39;accesso](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) o assegnare le credenziali per la [chiave API](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) a uno sviluppatore attendibile.

## Configura [!DNL Commerce Services Connector]

1. Apri Configurazione servizi di archiviazione.

   - Dall&#39;amministratore, selezionare **[!UICONTROL Stores]**.

   - In *[!UICONTROL Settings]*, selezionare **[!UICONTROL Configuration]**.

   - Espandere **[!UICONTROL Services]** e selezionare **[!UICONTROL Commerce Services Connector]**.

1. Aggiungi le credenziali della chiave API di produzione dal tuo account Adobe Commerce.

   Servizio ![[!DNL Commerce Services Connector] nella visualizzazione [!DNL Admin]](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > Se nell&#39;istanza di [!DNL Commerce] sono installati altri servizi [!DNL Adobe Commerce] come [!DNL Live Search] o [!DNL Product Recommendations], le informazioni sulle credenziali vengono visualizzate nell&#39;interfaccia e non è richiesta alcuna ulteriore configurazione.

1. Configurare il progetto SaaS e lo spazio dati in modo che i servizi Commerce possano inviare dati al servizio Channel Manager.

   Configurazione dell&#39;identificatore SaaS ![[!DNL Commerce Services Connector] nella visualizzazione [!DNL Admin]](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

