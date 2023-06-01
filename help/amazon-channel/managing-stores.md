---
title: "[!UICONTROL Amazon Stores] view"
description: Vai alla vista Amazon Stores per rivedere rapidamente le statistiche di base per ciascuno dei tuoi store Amazon e accedere alle opzioni di gestione.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores] visualizza

Quando si visualizza la home page del canale di vendita Amazon, il _Amazon Stores_ la vista viene aperta per impostazione predefinita.

![Vista Amazon Stores](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

Il _[!UICONTROL Amazon Stores]_visualizza mostra una &quot;scheda store&quot; per ciascuno dei tuoi store Amazon insieme ad alcune statistiche di base e opzioni di gestione. Le informazioni di riepilogo visualizzate in ogni scheda includono lo stato di ogni negozio, la data di creazione, la data dell&#39;ultimo aggiornamento, le inserzioni che richiedono attenzione (ad esempio: Inserzioni incomplete) e il [!DNL Commerce] sito Web.

Quando si visualizza _[!UICONTROL Amazon Store]_visualizzazione, ogni scheda dello store consente di:

- Per aprire un negozio [dashboard](./amazon-store-dashboard.md), fai clic su **[!UICONTROL View Store]**.

- Per modificare lo stato di un archivio o eliminare un archivio, fare clic su **[!UICONTROL Action]** e scegli:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Scegliere di cambiare lo stato del negozio in `Active` o `Inactive`, rispettivamente.

      Modifica di un `Inactive` memorizza in `Active` stato attiva le inserzioni e l&#39;attività di ordinazione per il negozio, utilizzando le impostazioni del negozio corrente (ad esempio le impostazioni delle inserzioni, le regole di prezzo e le sostituzioni).

      Modifica dello stato di uno store da `Active` a `Inactive` lo stato sospende le inserzioni e l&#39;attività di ordinazione per lo store. Un archivio inattivo conserva tutte le impostazioni del negozio e le inserzioni, ma interrompe temporaneamente la sincronizzazione di determinazione prezzi, quantità e gestione degli ordini fino a quando il negozio non viene ripristinato `Active` stato. Questa funzione consente di controllare l’attività del negozio a livello regionale senza la necessità di ricreare o reintegrare il negozio Amazon o la perdita di dati storici relativi a ordini e vendite.

   - **[!UICONTROL Delete]** - Scegli di eliminare un archivio non più necessario.

      Scegli quando eliminare un archivio Amazon esistente e le relative impostazioni di integrazione con il tuo [!DNL Amazon Seller Central] account. L’eliminazione dell’account rimuove il negozio dal canale di vendita Amazon, insieme a tutte le impostazioni dell’account, le inserzioni, i registri e altre informazioni relative a questo negozio. Impossibile recuperare l&#39;archivio dopo l&#39;eliminazione. È necessario creare un nuovo archivio.

>[!NOTE]
>Per cambiare il sito web assegnato al negozio durante l’integrazione, devi eliminare il negozio e aggiungerlo nuovamente con il diverso sito web definito durante l’integrazione del negozio.

| Scheda store | Descrizione |
|--- |--- |
| Sezione superiore | Include: <br>L’icona dell’area geografica del negozio, definita durante [integrazione store](./store-integration.md).<br> Il valore assegnato _[!UICONTROL Magento Website]_, definito durante l’integrazione dello store.<br>Il_[!UICONTROL Status]_ del tuo negozio. Opzioni: **[!UICONTROL Active]** - L&#39;integrazione del negozio è stata completata e verificata con Amazon ed è disponibile per le attività di vendita. **[!UICONTROL Inactive]** - L&#39;integrazione dello store è stata completata, ma non è in uso o non è disponibile per attività di vendita. Quando `Inactive`, le vendite di Amazon vengono sospese. Quando `Active`, ricavi di vendita e altre impostazioni salvate per l&#39;aggiornamento prima dell&#39;attivazione.<br>Il *[!UICONTROL Last Updated]* data della modifica più recente alla configurazione di Amazon store.<br>Il *[!UICONTROL Created]* data di creazione del negozio Amazon nel canale di vendita Amazon. |
| Sezione centrale | Include un grafico di riepilogo dell&#39;attività del punto vendita per gli ultimi 30 giorni e include e un avviso per tutte le inserzioni che richiedono attenzione. |
| Sezione inferiore | Include le opzioni Visualizza store e Azione.<br>Per aprire il negozio [dashboard](./amazon-store-dashboard.md), fai clic su **[!UICONTROL View Store]**.<br>Per attivare, disattivare o eliminare un archivio, fare clic su **[!UICONTROL Actions]**. |
