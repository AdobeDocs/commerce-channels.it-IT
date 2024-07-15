---
title: "Onboarding [!DNL Amazon Sales Channel]"
description: Scopri le attività preliminari alla configurazione, i passaggi di onboarding e come Amazon funziona con il Sales Channel Amazon in Adobe Commerce e Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Onboarding [!DNL Amazon Sales Channel]

Questa sezione descrive le attività preliminari alla configurazione, i passaggi per l’onboarding e alcuni concetti chiave sul funzionamento di Amazon con il canale di vendita Amazon in Adobe Commerce e Magento Open Source.

L&#39;estensione [!DNL Amazon Sales Channel] supporta più archivi Amazon. Per un singolo account [!DNL Amazon Seller Central] che opera nell&#39;area Amazon Stati Uniti/Canada/Messico, creare tre negozi Amazon (uno per le vendite negli Stati Uniti, in Messico e in Canada). Ognuno dei tre negozi definisce il paese del marketplace durante la sua creazione. Se hai più di un account [!DNL Amazon Seller Central], potresti avere fino a tre store Amazon per ciascuno dei tuoi account [!DNL Amazon Seller Central]. Se vendi anche nel Regno Unito, avrai un quarto negozio Amazon.

>[!TIP]
>
>È necessario un [account venditore professionale](https://sell.amazon.com/){target="_blank"} su [!DNL Amazon Seller Central] nell&#39;area Nord America o Europa (Regno Unito). Amazon addebita un abbonamento mensile e le tariffe di vendita. Vedi [Amazon: scegli il tuo piano di vendita](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>L&#39;onboarding è semplice: crea il tuo archivio e poi collegalo al tuo account [!DNL Amazon Seller Central].
>Quando il tuo archivio è connesso, il canale Amazon tenta di importare le tue inserzioni Amazon e di abbinarle al catalogo, in base alla [mappatura attributi](./attributes-view.md).<br><br>
>Le impostazioni del canale di vendita Amazon influiscono sulle inserzioni Amazon. Le impostazioni iniziali dell&#39;inserzione, dei prezzi e dei prodotti sono predefinite. Puoi modificare le [impostazioni dello store](./ob-store-review.md) (inserzioni, prezzi, ordini e rapporti) dopo che lo store è connesso al tuo account [!DNL Amazon Seller Central].

| Passaggi | Cosa succede |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Attività preliminari](./amazon-pre-setup-tasks.md) | Prima di iniziare, è necessario assicurarsi di disporre di un account [!DNL Amazon Seller Central] attivo e approvato. Ci sono anche alcuni requisiti e consigli per [!DNL Commerce] da completare prima dell&#39;onboarding. |
| [Verifica la chiave API di Amazon](./amazon-verify-api-key.md) | Quando accedi al canale di vendita Amazon, [!DNL Commerce] controlla e convalida automaticamente la chiave API Amazon che hai aggiunto nella configurazione dello store. Se la chiave API non è stata aggiunta o non è valida, verrà richiesto di [aggiungere o aggiornare la chiave API di Amazon](./amazon-verify-api-key.md). |
| [Integrazione store](./store-integration.md) | Questo passaggio include la creazione di un Amazon Sales Channel Store e la successiva connessione al tuo account [!DNL Amazon Seller Central]. Per questo passaggio sono necessarie le credenziali di accesso primarie per l&#39;account [!DNL Amazon Seller Central] (l&#39;e-mail o il telefono utilizzato per creare l&#39;account del venditore). |
| [Crea Regola Di Inserzione](./ob-create-listing-rule.md) | Dopo aver collegato il tuo Amazon Sales Channel Store, ti viene richiesto di creare una regola per l’inserzione. Questo passaggio è consigliato, ma puoi anche saltarlo per avviare il processo di importazione dell’inserzione. Puoi anche accedere alle tue [impostazioni per store ed inserzioni](./ob-store-review.md) nell&#39;archivio [dashboard](./amazon-store-dashboard.md). |
