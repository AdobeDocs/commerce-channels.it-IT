---
title: Aggiungere o verificare la chiave API di Amazon
description: Nella configurazione di Commerce, la chiave API Amazon convalidata ti consente di integrare i negozi con l’account Amazon Seller.
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Aggiungere o verificare la chiave API di Amazon

Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon che hai aggiunto nella configurazione dello store. Se convalidata, puoi passare al passaggio successivo, [Integrazione store](./store-integration.md).

Se la chiave API di Amazon è mancante, non valida o scaduta, devi aggiornarla. Viene visualizzato un messaggio che richiede di ottenere una chiave API e di aggiungerla alla configurazione del canale di vendita Amazon.

## Ottieni e aggiungi la chiave API di Amazon come richiesto

La chiave API viene convalidata ogni volta che accedi al tuo canale di vendita Amazon.

1. Accedere all&#39;amministratore [!DNL Commerce].

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Se è la prima volta che accedi al canale di vendita Amazon o se la tua chiave API richiede un aggiornamento, il sistema ti chiederà di completare la procedura.

   ![Ottieni e aggiungi il prompt della chiave API di Amazon](assets/amazon-api-verification-prompt.png){width="500"}

1. Fai clic su **[!UICONTROL Sign in]** per accedere al tuo account Web [!DNL Commerce].

   La pagina Account di Commerce si apre in una nuova scheda del browser.

   - Se hai effettuato l&#39;accesso al tuo account [!DNL Commerce], la sezione _[!UICONTROL API Portal]_della pagina_[!UICONTROL My Account]_ viene visualizzata automaticamente.

   - Se non si è connessi, verrà richiesto di immettere il nome utente e la password dell&#39;account [!DNL Commerce] prima che venga visualizzata la scheda _[!UICONTROL API Portal]_.

   - Se non disponi di un account, visita [la [!DNL Commerce] pagina account](https://account.magento.com/customer/account/login/){target="_blank"} e registrati. Questo account deve far parte della tua azienda o attività.

1. Se necessario, puoi visualizzare e generare le chiavi API nella scheda _[!UICONTROL API Portal]_del tuo account [!DNL Commerce].

   Per creare una chiave API, immetti una descrizione come `Amazon Sales Channel` e fai clic su **[!UICONTROL Add New]**. La nuova chiave viene generata e visualizzata con il nome immesso. Fare clic su **[!UICONTROL Copy]** per copiare la nuova chiave.

   ![Generare o copiare una chiave API](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. Quando la nuova chiave viene generata e copiata, tornare alla scheda _[!UICONTROL Amazon Sales Channel]_nel browser.

1. Nella pagina _[!UICONTROL Welcome to Amazon Sales Channel]_, fare clic su **[!UICONTROL Add the key]**.

   Il browser esce dal canale di vendita Amazon e una pagina di configurazione dello store apre la pagina _[!UICONTROL Api Keys]_nell&#39;amministratore [!DNL Commerce]. Puoi aprire questa pagina manualmente quando scegli **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, espandi **[!UICONTROL Services]** nel pannello a sinistra e scegli **[!UICONTROL Magento Services]**.

1. Incolla la chiave copiata per **[!UICONTROL Production Api key]**.

1. Fare clic su **[!UICONTROL Save Config]**. Ora puoi tornare al canale di vendita Amazon.

   ![Aggiunta della chiave API nella configurazione dell&#39;archivio](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Il nuovo accesso al canale di vendita Amazon attiva [!DNL Commerce] la verifica e la convalida della chiave API e consente di continuare.

   Se viene richiesto di verificare nuovamente la chiave, ripetere il processo _Aggiungi e verifica_.

![Icona successiva](assets/btn-next.png) [**Continua a archiviare l&#39;integrazione**](./store-integration.md)
