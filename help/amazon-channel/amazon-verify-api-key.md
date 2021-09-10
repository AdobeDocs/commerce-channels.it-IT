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

Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon aggiunta nella configurazione dello store. Se convalidato, puoi passare al passaggio successivo, [Memorizza integrazione](./store-integration.md).

Se la chiave API di Amazon è mancante, non valida o scaduta, devi aggiornare la chiave. Viene visualizzato un messaggio che richiede di ottenere una chiave API e di aggiungerla alla configurazione del canale di vendita Amazon.

## Ottieni e aggiungi la chiave API Amazon come richiesto

La chiave API viene convalidata ogni volta che accedi al tuo canale di vendita Amazon.

1. Accedi all&#39;amministratore [!DNL Commerce].

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Se è la prima volta che accedi al canale di vendita Amazon o se la chiave API richiede un aggiornamento, il sistema ti chiede di seguire il processo.

   ![Ottieni e aggiungi il prompt chiave API di Amazon](assets/amazon-api-verification-prompt.png)

1. Fai clic su **[!UICONTROL Sign in]** per accedere al tuo account web [!DNL Commerce].

   La pagina Account Commerce viene visualizzata in una nuova scheda del browser.

   - Se hai effettuato l’accesso al tuo account [!DNL Commerce], la sezione _[!UICONTROL API Portal]_della pagina_[!UICONTROL My Account]_ viene visualizzata automaticamente.

   - Se non hai effettuato l&#39;accesso, ti viene richiesto di immettere il nome utente e la password dell&#39;account [!DNL Commerce] prima che venga visualizzata la scheda _[!UICONTROL API Portal]_.

   - Se non disponi di un account, visita [la  [!DNL Commerce] pagina dell&#39;account](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;} e registra. Questo account deve far parte della tua azienda o attività.

1. Se necessario, puoi visualizzare e generare chiavi API nella scheda _[!UICONTROL API Portal]_del tuo account [!DNL Commerce] .

   Per creare una chiave API, immetti una descrizione come `Amazon Sales Channel` e fai clic su **[!UICONTROL Add New]**. La nuova chiave viene generata e visualizzata con il nome inserito. Fai clic su **[!UICONTROL Copy]** per copiare la nuova chiave.

   ![Generare o copiare una chiave API](assets/amazon-add-api-key.png)

1. Con la nuova chiave generata e copiata, torna alla scheda _[!UICONTROL Amazon Sales Channel]_nel browser.

1. Nella pagina _[!UICONTROL Welcome to Amazon Sales Channel]_, fai clic su **[!UICONTROL Add the key]**.

   Il browser esce dal canale di vendita Amazon e una pagina di configurazione del negozio apre la pagina _[!UICONTROL Api Keys]_nell’ [!DNL Commerce] Admin. Puoi aprire manualmente questa pagina quando vai su **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, espandi **[!UICONTROL Services]** nel pannello di sinistra e scegli **[!UICONTROL Magento Services]**.

1. Incolla la chiave copiata per **[!UICONTROL Production Api key]**.

1. Fare clic su **[!UICONTROL Save Config]**. Ora puoi tornare al canale di vendita Amazon.

   ![Aggiunta della chiave API nella configurazione dell&#39;archivio](assets/config-magento-services-api-screen.png)

1. Nella barra laterale _[!UICONTROL Admin]_, vai a **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Il nuovo accesso ai trigger del canale di vendita Amazon [!DNL Commerce] verifica e convalida la chiave API e ti consente di continuare.

   Se ti viene richiesto di verificare nuovamente la chiave, ripeti questo processo _Aggiungi e verifica_.

![Icona ](assets/btn-next.png) [**SuccessivaContinua a archiviare l’integrazione**](./store-integration.md)
