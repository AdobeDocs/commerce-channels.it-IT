---
title: Impostazioni Sales Channel
description: Per gestire la registrazione, l’origine cron e la sincronizzazione per le funzioni del canale di vendita Amazon, aggiorna la configurazione Commerce.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Impostazioni Sales Channel

Quando il [!DNL Amazon Sales Channel] l&#39;estensione è installata, i valori predefiniti sono impostati nell&#39;Admin per il canale di vendita Amazon. Queste impostazioni possono essere modificate nelle impostazioni di configurazione per il tuo archivio Amazon. Queste impostazioni includono:

- Intervalli per la cancellazione della cronologia del registro attività
- Selezione della sorgente cron
- Opzioni di sincronizzazione del registro

## Modificare le impostazioni dei canali Commerce

1. Sulla _Amministratore_ barra laterale, vai a **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Nel pannello a sinistra, espandi **[!UICONTROL Sales Channels]** e scegli **[!UICONTROL Global Settings]**.

1. Per **[!UICONTROL Clear Log History]**, scegli un’opzione:

   - `Once Daily` - Scegliere di cancellare la cronologia delle attività del negozio una volta al giorno.

   - `Once Weekly` - Scegliere di cancellare la cronologia delle attività del negozio una volta alla settimana.

   - `Once Monthly` - (Impostazione predefinita) Scegli di cancellare la cronologia delle attività del negozio una volta al mese.

1. Per **[!UICONTROL Background Tasks (CRON) Source]**, scegli `Magento CRON`.

   Questa opzione consente al canale di vendita Amazon di utilizzare [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) impostazioni per determinare gli intervalli di comunicazione e sincronizzazione dati con [!DNL Amazon Seller Central].

1. Per **[!UICONTROL Enable Debug Logging]**, scegli `Enabled` per raccogliere dati di sincronizzazione aggiuntivi quando è necessaria una risoluzione dei problemi.

   La registrazione dei canali di vendita Amazon viene scritta nel `{Commerce Root}/var/log/channel_amazon.log` e può essere visualizzato in [modalità sviluppatore](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}. La registrazione deve essere `Enabled` durante la risoluzione dei problemi e `Disabled` quando la risoluzione dei problemi è completa.

1. Fai clic su **[!UICONTROL Save Config]**.

![Impostazioni di configurazione del Sales Channel](assets/config-sales-channel-global-settings.png)
