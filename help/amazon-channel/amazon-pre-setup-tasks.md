---
title: Attività di pre-configurazione
description: Rivedi le attività richieste da completare prima di integrare il tuo archivio Adobe Commerce o Magento Open Source nel Sales Channel Amazon.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# Attività di pre-configurazione

Prima di [Integrazione store](./store-integration.md), è necessario assicurarsi che [!DNL Amazon Seller Central] account e [!DNL Commerce] sono pronti per l’integrazione. Per eseguire correttamente l’integrazione, sono necessarie alcune attività di preconfigurazione.

Quando configuri il primo store Amazon nel canale di vendita Amazon, viene visualizzato un elenco delle attività di configurazione. Si consiglia di rivedere queste attività prima di [aggiungi uno store di Amazon](./store-integration.md). Dopo aver aggiunto il primo negozio, puoi rivedere queste attività nella vista Apprendimento e preparazione del canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## 1. Abilitare le attività in background in [!DNL Commerce]

Tutti i prodotti e i dati sincronizzati tra [!DNL Commerce] e Amazon è gestito da un [lavoro cron](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}. Quando si completano attività quali l&#39;aggiunta o l&#39;aggiornamento di inserzioni e la ricezione di ordini, un OdL cron invia e riceve dati tra i [!DNL Commerce] back-end e [!DNL Amazon Seller Central] account.

- [Abilita [!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}.

- Per ottenere le massime prestazioni, [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target="_blank"} per eseguire una volta ogni cinque minuti.

## 2. Creare [!DNL Amazon Seller Central] account

Prima di iniziare la configurazione del tuo canale di vendita Amazon, devi disporre di un [!DNL Amazon Seller Central] account. Se non disponi già di un account Amazon Seller in [Nord America (US, CA, MX)](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} area geografica, puoi completare il processo di impostazione dell&#39;account del venditore di Amazon.

Il canale di vendita Amazon richiede un [!DNL Professional Seller] account su [!DNL Amazon Seller Central]. Amazon addebita un abbonamento mensile e le tariffe di vendita. Consulta [Amazon: scegli il piano di vendita](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Assicurati di essere un venditore Amazon approvato

Per eseguire l&#39;integrazione, è necessario disporre di un [!DNL Amazon Seller Central] account. Il tuo account non deve avere restrizioni per prodotti o categorie. Alcuni prodotti e categorie richiedono l&#39;approvazione prima di creare inserzioni. Rivedi i criteri di Amazon per l’approvazione di categorie e prodotti per assicurarti che i tuoi prodotti siano approvati. Consulta [Amazon: categorie e prodotti da approvare](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (è richiesto l&#39;accesso centrale del venditore).

È inoltre importante assicurarsi di aver configurato quanto segue nel [!DNL Amazon Seller Central] account:

- Assicurati che i criteri di restituzione siano validi o migliori dei criteri di restituzione di Amazon. Consulta [Amazon: criteri di restituzione](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Verifica che le impostazioni relative alle imposte siano configurate. Consulta [Amazon: Politiche fiscali](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (è richiesto l&#39;accesso centrale del venditore).

- Assicurati che i metodi di spedizione siano configurati correttamente. Per impostare i metodi di spedizione [!DNL Commerce] vengono offerti ai clienti per evadere gli ordini di Amazon, aggiornare [Amazon: impostazioni di spedizione](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} nel tuo [!DNL Amazon Seller Central] account.

## 4. Assicurati che l&#39;IVA sia configurata per i tuoi negozi

(Utilizzato principalmente dai venditori del Regno Unito.) Amazon consiglia di registrarsi al [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. Se scegli un metodo diverso, sei responsabile della conformità IVA.

>[!NOTE]
>
>Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

## 5. Aumentare il numero di corrispondenze automatiche del catalogo

Durante l’onboarding, il canale di vendita Amazon utilizza gli attributi del prodotto per far corrispondere gli elenchi Amazon esistenti (se applicabili) ai prodotti esistenti nel tuo [!DNL Commerce] catalogo. Dopo l’onboarding, questi attributi di prodotto vengono utilizzati per pubblicare [!DNL Commerce] catalogare gli elementi in un’inserzione Amazon e sincronizzare i dati di prodotto tra [!DNL Commerce] e Amazon.

Per avere il numero più alto di [!DNL Commerce] i prodotti corrispondano automaticamente agli elenchi di Amazon, devi creare un set di attributi di prodotto per il tuo [!DNL Commerce] catalogo. Prima di configurare il tuo Amazon Sales Channel Store, devi aggiungere [!DNL Commerce] attributi del prodotto corrispondenti a questi attributi di Amazon, ad esempio: ASIN, EAN, ISBN, UPC o GCID. Consulta [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Configurare la valuta e la conversione (in base alle esigenze)

Se il tuo archivio Amazon utilizza una valuta diversa da quella configurata per il tuo [!DNL Commerce] immagazzinare, [abilita la valuta](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target="_blank"} and set the [currency conversion rate](https://docs.magento.com/user-guide/stores/currency-update.html){target="_blank"}.

## 7. Creare un attributo di condizione del prodotto (in base alle esigenze)

Se le inserzioni Amazon contengono più di una condizione di prodotto (ad esempio _nuovo_, _utilizzato_, o _mi piace nuovo_), crea un [!DNL Commerce] e assegnare valori di condizione. Durante l’onboarding, devi mappare questo attributo all’attributo di prodotto Condizione Amazon. Consulta [Creazione di attributi per Amazon](./ob-creating-magento-attributes.md).

## 8. Configurare [!DNL Amazon Seller Central] metodo di spedizione

Per impostare i metodi di spedizione da offrire per l&#39;esecuzione degli ordini Amazon, fare riferimento a [Impostazioni e impostazioni spedizione][10] nel tuo [!DNL Amazon Seller Central] account.

## Configurazioni aggiuntive

Quando il tuo account Amazon è configurato e attivo, sono presenti diversi [!DNL Commerce] consigli per semplificare il processo di onboarding del canale di vendita Amazon.

### Rivedi e prendi nota di tutti i prodotti da escludere

Potresti non voler mettere in vendita alcuni prodotti su Amazon. Il canale di vendita Amazon dispone di un motore per le regole di inserzione utilizzato per determinare quali prodotti sono idonei per la pubblicazione in Amazon. [Regole di inserzione](./listing-rules.md) consente di selezionare sottoinsiemi di prodotti da pubblicare (o non pubblicare) nel [!DNL Amazon Seller Central] account, ad esempio per selezione di categorie o definendo uno o più attributi di prodotto. Mi piace [!DNL Commerce] [catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"} or [shopping cart](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"} price rules, product attributes used for Amazon listing eligibility must have **[!UICONTROL Use for Promo Rule Conditions]** set to `Yes`. See the **[!UICONTROL Use for Promo Rule Conditions]** in [Product Attributes](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"}.

### Imposta il [!DNL Amazon Seller Central] area geografica da inattiva

Per facilitare la transizione dei dati senza errori durante l’integrazione, si consiglia di impostare l’area geografica di Amazon su `Inactive` stato in Impostazioni > Informazioni account > Impostazioni ferie. Fai riferimento a [Amazon: Elenco dello stato per le vacanze][11]. Al termine della configurazione, torna allo stato `Active` in Amazon.

![Icona Successivo](assets/btn-next.png) [**Continua a creare [!DNL Commerce] Attributi**](./ob-creating-magento-attributes.md)
