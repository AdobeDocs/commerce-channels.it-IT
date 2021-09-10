---
title: Sales Channel Amazon integrato
description: 'Scopri le attività di preconfigurazione, i passaggi di onboarding e il funzionamento di Amazon con Amazon Sales Channel in Adobe Commerce e Magenti Open Source.'
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html: 
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 0%

---

# Canale di vendita Amazon integrato

Questa sezione descrive le attività di preconfigurazione, i passaggi per l’onboarding e alcuni concetti chiave su come Amazon funziona con il canale di vendita Amazon in Commerce e Magento Open Source di Adobe.

L&#39;estensione [!DNL Amazon Sales Channel] supporta più store Amazon. Per un singolo account [!DNL Amazon Seller Central] che opera nell&#39;area Amazon U.S./Canada/Messico, crea tre negozi Amazon (uno ciascuno per le vendite negli Stati Uniti, in Messico e in Canada). Ognuno dei tre negozi definisce il paese del mercato durante la sua creazione. Se disponi di più account [!DNL Amazon Seller Central], puoi potenzialmente avere fino a tre store Amazon per ciascuno dei tuoi account [!DNL Amazon Seller Central]. Se vendete anche nel Regno Unito, avrete un quarto negozio Amazon.

>[!TIP]
>
>È necessario un account [Venditore professionale](https://sell.amazon.com/){target=&quot;_blank&quot;} su [!DNL Amazon Seller Central] nell&#39;area Nord America o Europea (UK). Amazon impone un abbonamento mensile e tariffe per la vendita. Consulta [Amazon: Scegli il piano di vendita](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.<br><br>
>L&#39;onboarding è semplice: crea lo store e quindi collegalo al tuo account [!DNL Amazon Seller Central].
>Quando lo store è connesso, il canale Amazon tenta di importare gli elenchi Amazon e di farli corrispondere al catalogo, in base alla [mappatura attributi](./attributes-view.md).<br><br>
>Le impostazioni del canale di vendita Amazon influiscono sugli elenchi di Amazon. Per impostazione predefinita, vengono utilizzati l&#39;elenco iniziale, il prezzo e le impostazioni del prodotto. È possibile modificare le impostazioni [store](./ob-store-review.md) (inserzioni, prezzi, ordini e rapporti) dopo la connessione dello store all&#39;account [!DNL Amazon Seller Central].

| Passaggi | Cosa succede |
|--- |--- |
| [Attività pre-installazione](./amazon-pre-setup-tasks.md) | Prima di salire a bordo, è necessario assicurarsi di disporre di un account [!DNL Amazon Seller Central] attivo e approvato. Sono inoltre disponibili alcuni requisiti e raccomandazioni [!DNL Commerce] da completare prima dell’onboarding. |
| [Verificare la chiave API di Amazon](./amazon-verify-api-key.md) | Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon aggiunta nella configurazione dello store. Se la chiave API non è stata aggiunta o non è valida, ti viene richiesto di [aggiungere o aggiornare la chiave API Amazon](./amazon-verify-api-key.md). |
| [Integrazione store](./store-integration.md) | Questo passaggio include la creazione di un archivio dei canali di vendita Amazon e la successiva connessione al tuo account [!DNL Amazon Seller Central]. Per questo passaggio sono necessarie le credenziali di accesso principali per il tuo account [!DNL Amazon Seller Central] (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore). |
| [Crea regola di inserimento nell’elenco](./ob-create-listing-rule.md) | Dopo aver collegato l&#39;archivio canali di vendita Amazon, ti viene richiesto di creare una regola di elenco. Questo passaggio è consigliato, ma puoi anche saltare per avviare il processo di importazione dell’elenco. Puoi anche accedere alle [impostazioni store ed elencare](./ob-store-review.md) sullo store [dashboard](./amazon-store-dashboard.md). |
