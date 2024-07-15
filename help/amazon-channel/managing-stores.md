---
title: "[!UICONTROL Amazon Stores] visualizzazione"
description: Vai alla vista Amazon Stores per rivedere rapidamente le statistiche di base per ciascuno dei tuoi store Amazon e accedere alle opzioni di gestione.
feature: Sales Channels, Storefront
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores] visualizzazione

Quando si visualizza la home page del canale di vendita Amazon, per impostazione predefinita viene aperta la visualizzazione _Amazon Stores_.

![Visualizzazione archivi Amazon](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

La visualizzazione _[!UICONTROL Amazon Stores]_mostra una &quot;scheda dello store&quot; per ciascuno degli store Amazon insieme ad alcune statistiche di base e opzioni di gestione. Le informazioni di riepilogo visualizzate in ogni scheda includono lo stato di ogni negozio, la data di creazione, la data dell&#39;ultimo aggiornamento, le inserzioni che richiedono attenzione (ad esempio: Inserzioni incomplete) e il sito Web [!DNL Commerce] assegnato.

Quando si visualizza la visualizzazione _[!UICONTROL Amazon Store]_, ogni scheda dello store consente di:

- Per aprire un archivio [dashboard](./amazon-store-dashboard.md), fare clic su **[!UICONTROL View Store]**.

- Per modificare lo stato di un archivio o eliminare un archivio, fare clic su **[!UICONTROL Action]** e scegliere:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Scegliere di cambiare lo stato dell&#39;archivio rispettivamente in `Active` o `Inactive`.

     La modifica dello stato di un archivio `Inactive` in `Active` attiva le inserzioni e l&#39;attività di ordinazione per il negozio, utilizzando le impostazioni correnti del negozio (ad esempio le impostazioni di inserzione, le regole di prezzo e le sostituzioni).

     La modifica dello stato di un archivio da `Active` a `Inactive` sospende le inserzioni e l&#39;attività dell&#39;ordine per l&#39;archivio. Un archivio inattivo mantiene tutte le impostazioni e le inserzioni del negozio, ma interrompe temporaneamente la sincronizzazione di determinazione prezzi, quantità e gestione degli ordini fino a quando non viene ripristinato lo stato `Active`. Questa funzione consente di controllare l’attività del negozio a livello regionale senza la necessità di ricreare o reintegrare il negozio Amazon o la perdita di dati storici relativi a ordini e vendite.

   - **[!UICONTROL Delete]** - Scegliere di eliminare un archivio non più necessario.

     Scegli quando eliminare un Amazon Store esistente e le relative impostazioni di integrazione con il tuo account [!DNL Amazon Seller Central]. L’eliminazione dell’account rimuove il negozio dal canale di vendita Amazon, insieme a tutte le impostazioni dell’account, le inserzioni, i registri e altre informazioni relative a questo negozio. Impossibile recuperare l&#39;archivio dopo l&#39;eliminazione. È necessario creare un nuovo archivio.

>[!NOTE]
>Per cambiare il sito web assegnato al negozio durante l’integrazione, devi eliminare il negozio e aggiungerlo nuovamente con il diverso sito web definito durante l’integrazione del negozio.

| Scheda store | Descrizione |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sezione superiore | Include: <br>L&#39;icona dell&#39;area geografica per l&#39;archivio, definita durante [l&#39;integrazione dell&#39;archivio](./store-integration.md).<br> L&#39;assegnato _[!UICONTROL Magento Website]_, definito durante l&#39;integrazione dello store.<br>Il_[!UICONTROL Status]_ del tuo archivio. Opzioni: **[!UICONTROL Active]** - L&#39;integrazione dello store è stata completata e verificata con Amazon ed è disponibile per l&#39;attività di vendita. **[!UICONTROL Inactive]** - L&#39;integrazione dello store è stata completata, ma non è in uso o disponibile per l&#39;attività di vendita. Quando `Inactive`, le vendite Amazon vengono sospese. Quando `Active`, i ricavi di vendita e le impostazioni aggiuntive vengono salvati per l&#39;aggiornamento prima dell&#39;attivazione.<br>Data *[!UICONTROL Last Updated]* della modifica più recente alla configurazione dell&#39;archivio Amazon.<br>La data *[!UICONTROL Created]* in cui è stato creato il negozio Amazon nel canale di vendita Amazon. |
| Sezione centrale | Include un grafico di riepilogo dell&#39;attività del punto vendita per gli ultimi 30 giorni e include e un avviso per tutte le inserzioni che richiedono attenzione. |
| Sezione inferiore | Include le opzioni Visualizza store e Azione.<br>Per aprire l&#39;archivio [dashboard](./amazon-store-dashboard.md), fare clic su **[!UICONTROL View Store]**.<br>Per attivare, disattivare o eliminare un archivio, fare clic su **[!UICONTROL Actions]**. |
