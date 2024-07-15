---
title: Impostazioni del canale di vendita
description: Per gestire la registrazione, l’origine cron e la sincronizzazione per le funzioni del canale di vendita di Amazon, aggiorna la configurazione di Commerce.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Impostazioni del canale di vendita

Quando l&#39;estensione [!DNL Amazon Sales Channel] è installata, i valori predefiniti vengono impostati nel canale di vendita Admin for Amazon. Queste impostazioni possono essere modificate nelle impostazioni di configurazione del tuo archivio Amazon. Queste impostazioni includono:

- Intervalli per cancellare la cronologia del registro attività
- Selezione sorgente Cron
- Opzioni di sincronizzazione del registro

## Modificare le impostazioni dei canali di Commerce

1. Nella barra laterale _Admin_, passa a **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Nel pannello a sinistra, espandi **[!UICONTROL Sales Channels]** e scegli **[!UICONTROL Global Settings]**.

1. Per **[!UICONTROL Clear Log History]**, scegliere un&#39;opzione:

   - `Once Daily` - Scegliere di cancellare la cronologia delle attività dello store una volta al giorno.

   - `Once Weekly` - Scegliere di cancellare la cronologia delle attività dello store una volta alla settimana.

   - `Once Monthly` - (predefinito) Scegli di cancellare la cronologia delle attività dello store una volta al mese.

1. Per **[!UICONTROL Background Tasks (CRON) Source]**, scegliere `Magento CRON`.

   Questa opzione consente al canale di vendita Amazon di utilizzare le impostazioni [!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) per determinare gli intervalli di sincronizzazione delle comunicazioni e dei dati con [!DNL Amazon Seller Central].

1. Per **[!UICONTROL Enable Debug Logging]**, scegliere `Enabled` per raccogliere dati di sincronizzazione aggiuntivi quando è necessaria la risoluzione dei problemi.

   La registrazione del canale di vendita Amazon è scritta nel file `{Commerce Root}/var/log/channel_amazon.log` e può essere visualizzata in [modalità sviluppatore](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes). La registrazione deve essere solo `Enabled` durante la risoluzione dei problemi e deve essere `Disabled` al termine della risoluzione dei problemi.

1. Per **[!UICONTROL Read-Only Mode]**, selezionare `Enabled` per bloccare tutte le richieste API in uscita che modificano lo stato.

   Con questa impostazione, le modifiche potenziali vengono salvate, ma non inviate, fino a quando [!UICONTROL Read-Only Mode] non viene disabilitato. Per abilitare la modalità di sola lettura, è necessario cancellare la cache di configurazione. Per riavviare i trasferimenti di dati, selezionare `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] è progettato per le copie dell&#39;istanza Production, ad esempio staging o QA, e non deve essere utilizzato nell&#39;istanza Production.
   >
   >Quando si esegue la migrazione di un database a una nuova copia dell&#39;istanza (rilevata quando l&#39;URL di un archivio cambia nella configurazione), [!UICONTROL Read-Only Mode] viene abilitato automaticamente.

1. Fare clic su **[!UICONTROL Save Config]**.

![Impostazioni di configurazione Sales Channel](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
