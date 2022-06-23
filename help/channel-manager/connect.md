---
title: '''Connetti a [!DNL Commerce] servizi"'
description: '''Connetti Channel Manager a [!DNL Commerce] servizi per abilitare la sincronizzazione dei dati e la comunicazione tra [!DNL Commerce] istanza, Channel Manager e altri servizi di supporto."'
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 7e7a3e854bbc6062e2d15c1962ddf787451e7275
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Connetti a [!DNL Commerce] servizi

La [!DNL Commerce Services Connector] integra il servizio Channel Manager con le istanze Adobe Commerce e Magenti Open Source. Il connettore consente la sincronizzazione dei dati e la comunicazione tra [!DNL Commerce] istanza, [!DNL Channel Manager]e altri servizi di supporto.

[!DNL Commerce Services Connector] la configurazione è un processo una tantum necessario per utilizzare [Servizi SaaS di Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;}, ad esempio [!DNL Channel Manager], [!DNL Live Search]e [!DNL Product Recommendations]. Se hai già configurato il connettore per un altro servizio, salta questo passaggio.

## Requisiti

- **Account Commerce**-Per installare il software su [!DNL Commerce] istanze, devi disporre di un account con accesso Proprietario o Amministratore alla [!DNL Commerce] piattaforma.

   I proprietari dell&#39;account e gli utenti privilegiati possono creare account amministratore da [!DNL Commerce] istanza o dalla riga di comando utilizzando [!DNL Commerce] Comando CLI `admin:user:create`.

- **Chiave API di produzione Adobe Commerce**-This [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} abilita l&#39;accesso API ai servizi richiesti da Channel Manager. Per questa chiave sono necessarie le credenziali pubbliche e private.

>[!TIP]
>
>Per fornire le credenziali, [!DNL Commerce] il titolare della licenza o il proprietario dell&#39;account ha opzioni per [accesso condiviso](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;}, oppure fornisci [Chiave API](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} credenziali a uno sviluppatore fidato.

## Configura le [!DNL Commerce Services Connector]

1. Apri la configurazione dei servizi store.

   - Dall’amministratore, seleziona **[!UICONTROL Stores]**.

   - Sotto *[!UICONTROL Settings]*, seleziona **[!UICONTROL Configuration]**.

   - Espandi **[!UICONTROL Services]** e seleziona **[!UICONTROL Commerce Services Connector]**.

1. Aggiungi le credenziali della chiave API di produzione dal tuo account Adobe Commerce.

   ![[!DNL Commerce Services Connector] nel [!DNL Admin] visualizzare](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Se [!DNL Commerce] l&#39;istanza ha un altro [!DNL Adobe Commerce] servizi come [!DNL Live Search] o [!DNL Product Recommendations] installate, le informazioni sulle credenziali vengono visualizzate nell&#39;interfaccia e non è richiesta alcuna ulteriore configurazione.

1. Configura il progetto SaaS e lo spazio dati in modo che Commerce Services possa inviare dati al servizio Channel Manager.

   ![[!DNL Commerce Services Connector] Configurazione dell’identificatore SaaS nel [!DNL Admin] visualizzare](assets/commerce-services-connector-saas-config.png)

