---
title: Impostazioni del canale di vendita
description: Per gestire la registrazione, l’origine cron e la sincronizzazione per le funzioni del canale di vendita di Amazon, aggiorna la configurazione di Commerce.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Impostazioni del canale di vendita

Quando [!DNL Amazon Sales Channel] Se l&#39;estensione è installata, i valori predefiniti sono impostati nel canale di vendita Admin for Amazon. Queste impostazioni possono essere modificate nelle impostazioni di configurazione del tuo archivio Amazon. Queste impostazioni includono:

- Intervalli per cancellare la cronologia del registro attività
- Selezione sorgente Cron
- Opzioni di sincronizzazione del registro

## Modificare le impostazioni dei canali Commerce

1. Il giorno _Amministratore_ barra laterale, vai a **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Nel pannello a sinistra, espandi **[!UICONTROL Sales Channels]** e scegli **[!UICONTROL Global Settings]**.

1. Per **[!UICONTROL Clear Log History]**, scegli un’opzione:

   - `Once Daily` - Scegli di cancellare la cronologia delle attività del negozio una volta al giorno.

   - `Once Weekly` - Scegli di cancellare la cronologia delle attività del negozio una volta alla settimana.

   - `Once Monthly` - (Impostazione predefinita) Scegli di cancellare la cronologia delle attività del negozio una volta al mese.

1. Per **[!UICONTROL Background Tasks (CRON) Source]**, scegli `Magento CRON`.

   Questa opzione consente al canale di vendita Amazon di utilizzare [!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) impostazioni per determinare gli intervalli di comunicazione e sincronizzazione dei dati con [!DNL Amazon Seller Central].

1. Per **[!UICONTROL Enable Debug Logging]**, scegli `Enabled` per raccogliere dati di sincronizzazione aggiuntivi quando è necessaria la risoluzione dei problemi.

   La registrazione del canale di vendita Amazon viene scritta in `{Commerce Root}/var/log/channel_amazon.log` e possono essere visualizzati in [modalità sviluppatore](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes). La registrazione deve essere `Enabled` durante la risoluzione dei problemi e deve essere `Disabled` al termine della risoluzione dei problemi.

1. Per **[!UICONTROL Read-Only Mode]**, seleziona `Enabled` per bloccare tutte le richieste API in uscita che cambiano lo stato.

   Con questa impostazione, le modifiche potenziali vengono salvate, ma non inviate, fino al [!UICONTROL Read-Only Mode] è disabilitato. Per abilitare la modalità di sola lettura, è necessario cancellare la cache di configurazione. Per avviare nuovamente i trasferimenti di dati, seleziona `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] è progettato per le copie dell’istanza Production, come staging o QA, e non deve essere utilizzato nell’istanza Production.
   >
   >Quando si esegue la migrazione di un database a una nuova copia dell&#39;istanza (rilevato quando l&#39;URL di un archivio cambia nella configurazione), [!UICONTROL Read-Only Mode] viene attivato automaticamente.

1. Clic **[!UICONTROL Save Config]**.

![Impostazioni configurazione Sales Channel](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
