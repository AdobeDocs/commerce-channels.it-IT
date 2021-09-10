---
title: Impostazioni Sales Channel
description: Per gestire la registrazione, l’origine cron e la sincronizzazione per le funzioni del canale di vendita Amazon, aggiorna la configurazione Commerce.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Impostazioni Sales Channel

Quando l&#39;estensione [!DNL Amazon Sales Channel] è installata, i valori predefiniti vengono impostati nell&#39;Admin per il canale di vendita Amazon. Queste impostazioni possono essere modificate nelle impostazioni di configurazione per il tuo archivio Amazon. Queste impostazioni includono:

- Intervalli per la cancellazione della cronologia del registro attività
- Selezione della sorgente cron
- Opzioni di sincronizzazione del registro

## Modificare le impostazioni dei canali Commerce

1. Nella barra laterale _Amministratore_, vai a **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Nel pannello a sinistra, espandi **[!UICONTROL Sales Channels]** e scegli **[!UICONTROL Global Settings]**.

1. Per **[!UICONTROL Clear Log History]**, scegli un’opzione:

   - `Once Daily` - Scegliere di cancellare la cronologia delle attività del negozio una volta al giorno.

   - `Once Weekly` - Scegliere di cancellare la cronologia delle attività del negozio una volta alla settimana.

   - `Once Monthly` - (Impostazione predefinita) Scegli di cancellare la cronologia delle attività del negozio una volta al mese.

1. Per **[!UICONTROL Background Tasks (CRON) Source]**, scegli `Magento CRON`.

   Questa opzione consente al canale di vendita Amazon di utilizzare le impostazioni [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) per determinare gli intervalli di comunicazione e sincronizzazione dei dati con [!DNL Amazon Seller Central].

1. Per **[!UICONTROL Enable Debug Logging]**, scegli `Enabled` per raccogliere dati di sincronizzazione aggiuntivi quando è necessaria una risoluzione dei problemi.

   La registrazione dei canali di vendita Amazon viene scritta nel file `{Commerce Root}/var/log/channel_amazon.log` e può essere visualizzata in [modalità sviluppatore](https://docs.magento.com/user-guide/magento/installation-modes.html){:target=&quot;_blank&quot;}. La registrazione deve essere solo `Enabled` durante la risoluzione dei problemi e deve essere `Disabled` al termine della risoluzione dei problemi.

1. Fare clic su **[!UICONTROL Save Config]**.

![Impostazioni di configurazione del Sales Channel](assets/config-sales-channel-global-settings.png)
