---
title: Aggiungere o verificare la chiave API di Amazon
description: Nella configurazione Commerce, la chiave API di Amazon convalidata ti consente di integrare gli store con il tuo account Seller Amazon.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Aggiungi o verifica la chiave API di Amazon

Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon che hai aggiunto nella configurazione del tuo negozio. Se convalidato, puoi passare al passaggio successivo, [Integrazione store](./store-integration.md).

Se la chiave API di Amazon è mancante, non valida o scaduta, devi aggiornare la chiave. Viene visualizzato un messaggio che richiede di ottenere una chiave API e di aggiungerla alla configurazione del canale di vendita Amazon.

## Ottieni e aggiungi la chiave API Amazon come richiesto

La chiave API viene convalidata ogni volta che accedi al tuo canale di vendita Amazon.

1. Accedi al [!DNL Commerce] Amministratore.

1. Sulla _[!UICONTROL Admin]_barra laterale, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Se è la prima volta che accedi al canale di vendita Amazon o se la chiave API richiede un aggiornamento, il sistema ti chiede di seguire il processo.

   ![Ottieni e aggiungi il prompt chiave API di Amazon](assets/amazon-api-verification-prompt.png)

1. Fai clic su **[!UICONTROL Sign in]** per accedere al [!DNL Commerce] account web.

   La pagina Account Commerce viene visualizzata in una nuova scheda del browser.

   - Se hai effettuato l’accesso al tuo [!DNL Commerce] il conto _[!UICONTROL API Portal]_della sezione_[!UICONTROL My Account]_ la pagina viene visualizzata automaticamente.

   - Se non hai effettuato l&#39;accesso, ti viene richiesto di immettere il tuo [!DNL Commerce] nome utente e password dell&#39;account prima del _[!UICONTROL API Portal]_viene visualizzata la scheda .

   - Se non disponi di un account, visita [la [!DNL Commerce] pagina account](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;} e registra. Questo account deve far parte della tua azienda o attività.

1. Se necessario, puoi visualizzare e generare le chiavi API in _[!UICONTROL API Portal]_nella scheda [!DNL Commerce] conto.

   Per creare una chiave API, immetti una descrizione come `Amazon Sales Channel` e fai clic su **[!UICONTROL Add New]**. La nuova chiave viene generata e visualizzata con il nome inserito. Fai clic su **[!UICONTROL Copy]** per copiare la nuova chiave.

   ![Generare o copiare una chiave API](assets/amazon-add-api-key.png)

1. Con la nuova chiave generata e copiata, torna alla _[!UICONTROL Amazon Sales Channel]_nel browser.

1. Sulla _[!UICONTROL Welcome to Amazon Sales Channel]_pagina, fai clic su **[!UICONTROL Add the key]**.

   Il browser esce dal canale di vendita Amazon e viene aperta una pagina di configurazione del negozio _[!UICONTROL Api Keys]_nella pagina [!DNL Commerce] Amministratore. Puoi aprire manualmente questa pagina quando vai a **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, espandi **[!UICONTROL Services]** nel pannello a sinistra e scegliete **[!UICONTROL Magento Services]**.

1. Incolla la chiave copiata per **[!UICONTROL Production Api key]**.

1. Fai clic su **[!UICONTROL Save Config]**. Ora puoi tornare al canale di vendita Amazon.

   ![Aggiunta della chiave API nella configurazione dell&#39;archivio](assets/config-magento-services-api-screen.png)

1. Sulla _[!UICONTROL Admin]_barra laterale, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Riaccesso ai trigger dei canali di vendita Amazon [!DNL Commerce] verifica e convalida la chiave API e ti consente di continuare.

   Se viene richiesto di verificare nuovamente la chiave, ripetilo _Aggiungi e verifica_ processo.

![Icona Successivo](assets/btn-next.png) [**Continua a archiviare l’integrazione**](./store-integration.md)
