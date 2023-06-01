---
title: "Onboarding [!DNL Amazon Sales Channel]"
description: Scopri le attività preliminari alla configurazione, i passaggi di onboarding e come Amazon funziona con il Sales Channel Amazon in Adobe Commerce e Magenti Open Source.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Onboarding [!DNL Amazon Sales Channel]

Questa sezione descrive le attività preliminari alla configurazione, i passaggi per l’onboarding e alcuni concetti chiave sul funzionamento di Amazon con il canale di vendita Amazon in Adobe Commerce e Magenti Open Source.

Il [!DNL Amazon Sales Channel] L&#39;estensione supporta più store di Amazon. Per un singolo [!DNL Amazon Seller Central] che opera nell’area geografica Amazon Stati Uniti/Canada/Messico, crea tre negozi Amazon (uno per le vendite negli Stati Uniti, in Messico e in Canada). Ognuno dei tre negozi definisce il paese del marketplace durante la sua creazione. Se ne hai più di uno [!DNL Amazon Seller Central] account, potresti avere fino a tre store di Amazon per ciascuno dei tuoi [!DNL Amazon Seller Central] account. Se vendi anche nel Regno Unito, avrai un quarto negozio Amazon.

>[!TIP]
>
>A [Account venditore professionale](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>L’onboarding è semplice: crea il negozio e quindi collegalo al tuo [!DNL Amazon Seller Central] account.
>Quando il negozio è connesso, il canale Amazon tenta di importare le inserzioni Amazon e di farle corrispondere al catalogo, in base al [mappatura attributi](./attributes-view.md).<br><br>
>Le impostazioni del canale di vendita Amazon influiscono sulle inserzioni Amazon. Le impostazioni iniziali dell&#39;inserzione, dei prezzi e dei prodotti sono predefinite. Puoi modificare i [impostazioni store](./ob-store-review.md) (inserzioni, prezzi, ordini e rapporti) dopo la connessione del tuo Negozio al tuo [!DNL Amazon Seller Central] account.

| Passaggi | Cosa succede |
|--- |--- |
| [Attività di pre-configurazione](./amazon-pre-setup-tasks.md) | Prima di iniziare l’onboarding, assicurati di disporre di un [!DNL Amazon Seller Central] account. Ci sono anche alcuni [!DNL Commerce] requisiti e raccomandazioni da completare prima dell’onboarding. |
| [Verifica la chiave API di Amazon](./amazon-verify-api-key.md) | Quando si accede al canale di vendita Amazon, [!DNL Commerce] verifica e convalida automaticamente la chiave API di Amazon aggiunta nella configurazione dell’archivio. Se la chiave API non è stata aggiunta o non è valida, viene richiesto di: [aggiungere o aggiornare la chiave API di Amazon](./amazon-verify-api-key.md). |
| [Integrazione store](./store-integration.md) | Questo passaggio include la creazione di un negozio di canali di vendita Amazon e la successiva connessione al tuo [!DNL Amazon Seller Central] account. Sono necessarie le credenziali di accesso primarie per [!DNL Amazon Seller Central] account (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore) per questo passaggio. |
| [Crea regola di inserzione](./ob-create-listing-rule.md) | Dopo aver collegato il tuo Amazon Sales Channel Store, ti viene richiesto di creare una regola per l’inserzione. Questo passaggio è consigliato, ma puoi anche saltarlo per avviare il processo di importazione dell’inserzione. Puoi anche accedere al tuo [impostazioni di archiviazione ed elenco](./ob-store-review.md) in negozio [dashboard](./amazon-store-dashboard.md). |
