---
title: Sales Channel Amazon integrato
description: Scopri le attività di preconfigurazione, i passaggi di onboarding e come Amazon funziona con Amazon Sales Channel in Adobe Commerce e Magenti Open Source.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Canale di vendita Amazon integrato

Questa sezione descrive le attività di preconfigurazione, i passaggi per l’onboarding e alcuni concetti chiave su come Amazon funziona con il canale di vendita Amazon in Adobe Commerce e Magenti Open Source.

La [!DNL Amazon Sales Channel] L&#39;estensione supporta più store Amazon. Per un singolo [!DNL Amazon Seller Central] account che opera nell&#39;area Amazon Stati Uniti/Canada/Messico, crea tre negozi Amazon (uno ciascuno per le vendite degli Stati Uniti, vendite del Messico e vendite del Canada). Ognuno dei tre negozi definisce il paese del mercato durante la sua creazione. Se ne hai più di uno [!DNL Amazon Seller Central] account, potresti potenzialmente avere fino a tre store Amazon per ciascuno dei tuoi [!DNL Amazon Seller Central] conti. Se vendete anche nel Regno Unito, avrete un quarto negozio Amazon.

>[!TIP]
>
>A [Account del venditore professionale](https://sell.amazon.com/){target=&quot;_blank&quot;} su [!DNL Amazon Seller Central] nell&#39;area del Nord America o dell&#39;Europa (Regno Unito) è necessario. Amazon impone un abbonamento mensile e tariffe per la vendita. Vedi [Amazon: Scegli il piano di vendita](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.<br><br>
>L&#39;onboarding è semplice: crea il tuo negozio e quindi collegalo al tuo [!DNL Amazon Seller Central] conto.
>Quando lo store è connesso, il canale Amazon tenta di importare gli elenchi Amazon e di farli corrispondere al catalogo, in base al [mappatura attributi](./attributes-view.md).<br><br>
>Le impostazioni del canale di vendita Amazon influiscono sugli elenchi di Amazon. Per impostazione predefinita, vengono utilizzati l&#39;elenco iniziale, il prezzo e le impostazioni del prodotto. Puoi modificare il tuo [impostazioni store](./ob-store-review.md) (elenco, prezzi, ordine e reporting) dopo che il tuo negozio è collegato al tuo [!DNL Amazon Seller Central] conto.

| Passaggi | Cosa succede |
|--- |--- |
| [Attività pre-installazione](./amazon-pre-setup-tasks.md) | Prima di salire a bordo, assicurati di disporre di un [!DNL Amazon Seller Central] conto. Ci sono anche alcuni [!DNL Commerce] requisiti e raccomandazioni da completare prima dell’onboarding. |
| [Verificare la chiave API di Amazon](./amazon-verify-api-key.md) | Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon che hai aggiunto nella configurazione del tuo negozio. Se la chiave API non è stata aggiunta o non è valida, viene richiesto di [aggiungi o aggiorna la chiave API di Amazon](./amazon-verify-api-key.md). |
| [Integrazione store](./store-integration.md) | Questo passaggio include la creazione di un archivio canali di vendita Amazon e la successiva connessione al tuo [!DNL Amazon Seller Central] conto. Sono necessarie le credenziali di accesso principali per [!DNL Amazon Seller Central] account (e-mail o telefono utilizzato per creare l&#39;account del venditore) per questo passaggio. |
| [Crea regola di inserimento nell’elenco](./ob-create-listing-rule.md) | Dopo aver collegato l&#39;archivio canali di vendita Amazon, ti viene richiesto di creare una regola di elenco. Questo passaggio è consigliato, ma puoi anche saltare per avviare il processo di importazione dell’elenco. Puoi anche accedere al tuo [memorizzare ed elencare le impostazioni](./ob-store-review.md) sul negozio [dashboard](./amazon-store-dashboard.md). |
