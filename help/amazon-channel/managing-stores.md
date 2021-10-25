---
title: Amazon Stores View
description: Vai alla vista Amazon Store per esaminare rapidamente le statistiche di base per ciascuno dei tuoi store Amazon e le opzioni di gestione degli accessi.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Vista Amazon Stores

Quando visualizzi la home page del canale di vendita Amazon, la _Amazon Stores_ per impostazione predefinita viene aperta la vista.

![Vista Amazon Stores](assets/amazon-sales-channel-home-tabs.png)

La _[!UICONTROL Amazon Stores]_visualizza una &quot;scheda store&quot; per ogni negozio Amazon, insieme ad alcune statistiche di base e ad alcune opzioni di gestione. Le informazioni di riepilogo visualizzate in ogni scheda includono lo stato dell&#39;archivio, la data di creazione, l&#39;ultima data di aggiornamento, gli elenchi che richiedono attenzione (ad esempio: Inserzioni incomplete) e i dati assegnati [!DNL Commerce] sito web.

Quando visualizzi la _[!UICONTROL Amazon Store]_visualizza, ogni scheda del negozio consente di:

- Per aprire uno store [dashboard](./amazon-store-dashboard.md), fai clic su **[!UICONTROL View Store]**.

- Per modificare lo stato di un archivio o eliminare un archivio, fare clic su **[!UICONTROL Action]** e scegli:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Scegliere di modificare lo stato dell&#39;archivio in `Active` o `Inactive`, rispettivamente.

      Modifica di un `Inactive` archiviare `Active` lo stato attiva le inserzioni e l&#39;attività dell&#39;ordine per l&#39;archivio, utilizzando le impostazioni dell&#39;archivio corrente (ad esempio le impostazioni dell&#39;elenco, le regole del prezzo e le sostituzioni).

      Modifica dello stato di un archivio da `Active` a `Inactive` lo stato sospende gli elenchi e l&#39;attività dell&#39;ordine per l&#39;archivio. Un archivio inattivo conserva tutte le impostazioni e gli elenchi degli archivi, ma interrompe temporaneamente la sincronizzazione di prezzi, quantità e gestione degli ordini fino a quando lo store non viene modificato in `Active` stato. Questa funzione ti consente di controllare l&#39;attività del tuo negozio a livello regionale senza la necessità di ricreare o reintegrare il tuo negozio Amazon o la perdita di dati storici sugli ordini e sulle vendite.

   - **[!UICONTROL Delete]** - Scegliere di eliminare uno store non più necessario.

      Scegli quando eliminare un archivio Amazon esistente e le relative impostazioni di integrazione con il tuo [!DNL Amazon Seller Central] conto. L&#39;eliminazione dell&#39;account rimuove l&#39;archivio dal canale di vendita Amazon, insieme a tutte le impostazioni dell&#39;account, gli elenchi, i registri e altre informazioni relative a questo archivio. Impossibile recuperare l&#39;archivio dopo l&#39;eliminazione. È necessario creare un nuovo archivio.

>[!NOTE]
>Per modificare il sito Web assegnato allo store durante l&#39;integrazione, è necessario eliminare lo store e aggiungere di nuovo lo store con il sito Web diverso definito durante l&#39;integrazione con lo store.

| Scheda Store | Descrizione |
|--- |--- |
| Sezione superiore | Include: <br>Icona della regione per lo store, definita durante [integrazione store](./store-integration.md).<br> Assegnato _[!UICONTROL Magento Website]_, definito durante l&#39;integrazione dell&#39;archivio.<br>La_[!UICONTROL Status]_ del tuo negozio. Opzioni: **[!UICONTROL Active]** - L’integrazione del negozio è completa e verificata con Amazon ed è disponibile per le attività di vendita. **[!UICONTROL Inactive]** - L&#39;integrazione del negozio è completa, ma non è in uso o disponibile per l&#39;attività di vendita. Quando `Inactive`, le tue vendite Amazon sono in pausa. Quando `Active`, le entrate di vendita e le impostazioni aggiuntive vengono salvate per essere aggiornate prima dell’attivazione.<br>La *[!UICONTROL Last Updated]* data della modifica più recente alla configurazione dell’archivio Amazon.<br>La *[!UICONTROL Created]* data di creazione dell&#39;archivio Amazon nel canale di vendita Amazon. |
| Sezione centrale | Include un grafico di riepilogo delle attività del negozio per gli ultimi 30 giorni e include e segnala eventuali inserzioni che richiedono attenzione. |
| Sezione inferiore | Include le opzioni Visualizza archivio e Azione.<br>Per aprire lo store [dashboard](./amazon-store-dashboard.md), fai clic su **[!UICONTROL View Store]**.<br>Per attivare, disattivare o eliminare un archivio, fare clic su **[!UICONTROL Actions]**. |
