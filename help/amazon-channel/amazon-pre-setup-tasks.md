---
title: Attività di preinstallazione per  [!DNL Amazon sales channel]
description: Rivedi le attività richieste da completare prima di integrare il tuo archivio Adobe Commerce o Magento Open Source nel Sales Channel Amazon.
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Attività di preconfigurazione per [!DNL Amazon sales channel]

Prima di [Integrazione store](./store-integration.md), è necessario assicurarsi che l&#39;account [!DNL Amazon Seller Central] e l&#39;account [!DNL Commerce] siano pronti per l&#39;integrazione. Per eseguire correttamente l’integrazione, sono necessarie alcune attività di preconfigurazione.

Quando configuri il primo store Amazon nel canale di vendita Amazon, viene visualizzato un elenco delle attività di configurazione. È consigliabile rivedere queste attività prima di [aggiungere un archivio Amazon](./store-integration.md). Dopo aver aggiunto il primo store, puoi rivedere queste attività nella vista Apprendimento e preparazione della pagina principale del canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## 1. Abilitare le attività in background in [!DNL Commerce]

Tutti i prodotti e i dati sincronizzati tra [!DNL Commerce] e Amazon sono gestiti da un [processo cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). Quando si completano attività quali l&#39;aggiunta o l&#39;aggiornamento di inserzioni e la ricezione di ordini, un processo cron invia e riceve dati tra il backend [!DNL Commerce] e l&#39;account [!DNL Amazon Seller Central].

- [Attiva [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- Per ottenere le massime prestazioni, [imposta [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) da eseguire una volta ogni cinque minuti.

## 2. Crea il tuo account [!DNL Amazon Seller Central]

Prima di iniziare la configurazione del canale di vendita Amazon, è necessario disporre di un account [!DNL Amazon Seller Central] attivo. Se non disponi di un account Amazon Seller esistente nell&#39;area [Nord America (USA, CA, MX)](https://sell.amazon.com/){target="_blank"} o [Europa (Regno Unito)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"}, puoi completare la procedura di configurazione dell&#39;account Amazon Seller.

Il canale di vendita Amazon richiede un account [!DNL Professional Seller] su [!DNL Amazon Seller Central]. Amazon addebita un abbonamento mensile e le tariffe di vendita. Vedi [Amazon: scegli il tuo piano di vendita](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Assicurati di essere un venditore Amazon approvato

Per eseguire l&#39;integrazione, è necessario disporre di un account [!DNL Amazon Seller Central] approvato. Il tuo account non deve avere restrizioni per prodotti o categorie. Alcuni prodotti e categorie richiedono l&#39;approvazione prima di creare inserzioni. Rivedi i criteri di Amazon per l’approvazione di categorie e prodotti per assicurarti che i tuoi prodotti siano approvati. Consulta [Amazon: categorie e prodotti che richiedono l&#39;approvazione](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (accesso centrale del venditore richiesto).

È inoltre importante assicurarsi di aver configurato quanto segue nel proprio account [!DNL Amazon Seller Central]:

- Assicurati che i criteri di restituzione siano validi o migliori dei criteri di restituzione di Amazon. Vedere [Amazon: Criteri restituiti](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Verifica che le impostazioni relative alle imposte siano configurate. Vedi [Amazon: Criteri fiscali](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (accesso centrale del venditore richiesto).

- Assicurati che i metodi di spedizione siano configurati correttamente. Per impostare i metodi di spedizione offerti ai clienti [!DNL Commerce] per l&#39;evasione degli ordini Amazon, aggiornare [Amazon: Impostazioni spedizione](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} nell&#39;account [!DNL Amazon Seller Central].

## 4. Assicurati che l&#39;IVA sia configurata per i tuoi negozi

(Utilizzato principalmente dai venditori del Regno Unito.) Amazon consiglia di iscriversi al [Servizio di calcolo IVA di Amazon](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. Se scegli un metodo diverso, sei responsabile della conformità IVA.

>[!NOTE]
>
>Potrebbero essere necessari 10-14 giorni affinché Amazon verifichi e attivi il tuo account del Servizio di calcolo dell’IVA.

## 5. Aumentare il numero di corrispondenze automatiche del catalogo

Durante l&#39;onboarding, il canale di vendita Amazon utilizza gli attributi del prodotto per far corrispondere le inserzioni esistenti di Amazon (se applicabile) ai prodotti esistenti nel catalogo [!DNL Commerce]. Dopo l&#39;onboarding, questi attributi di prodotto vengono utilizzati per pubblicare gli elementi del catalogo [!DNL Commerce] in un&#39;inserzione di Amazon e per sincronizzare i dati di prodotto tra [!DNL Commerce] e Amazon.

Affinché il numero più elevato di [!DNL Commerce] prodotti corrisponda automaticamente alle inserzioni di Amazon, è necessario creare un set di attributi di prodotto per il catalogo [!DNL Commerce]. Prima di configurare il tuo Amazon Sales Channel Store, devi aggiungere [!DNL Commerce] attributi di prodotto corrispondenti a questi attributi Amazon, ad esempio: ASIN, EAN, ISBN, UPC o GCID. Vedi [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Configurare la valuta e la conversione (in base alle esigenze)

Se il tuo archivio Amazon utilizza una valuta diversa da quella configurata per il tuo archivio [!DNL Commerce], [abilita la valuta](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) e imposta il [tasso di conversione valuta](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7. Creare un attributo di condizione del prodotto (in base alle esigenze)

Se le inserzioni Amazon contengono più di una condizione di prodotto (ad esempio _nuovo_, _usato_ o _come nuovo_), crea un attributo [!DNL Commerce] e assegna i valori della condizione. Durante l’onboarding, devi mappare questo attributo all’attributo di prodotto Condizione Amazon. Consulta [Creazione di attributi per Amazon](./ob-creating-magento-attributes.md).

## 8. Configurare il metodo di spedizione [!DNL Amazon Seller Central]

Per impostare i metodi di spedizione che desideri offrire per l&#39;esecuzione degli ordini Amazon, fai riferimento a _Impostazioni e impostazioni di spedizione_ nel tuo account [!DNL Amazon Seller Central].

## Configurazioni aggiuntive

Quando il tuo account Amazon è configurato e attivo, ci sono diversi [!DNL Commerce] consigli che aiutano a semplificare il processo di onboarding del canale di vendita Amazon.

### Rivedi e prendi nota di tutti i prodotti da escludere

Potresti non voler mettere in vendita alcuni prodotti su Amazon. Il canale di vendita Amazon dispone di un motore per le regole di inserzione utilizzato per determinare quali prodotti sono idonei per la pubblicazione in Amazon. [Le regole di elenco](./listing-rules.md) consentono di selezionare sottoinsiemi di prodotti da pubblicare (o non pubblicare) nell&#39;account [!DNL Amazon Seller Central], ad esempio selezionando una categoria o definendo uno o più attributi di prodotto. Come le regole di prezzo [!DNL Commerce] [catalogo](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) o [carrello](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html), gli attributi del prodotto utilizzati per l&#39;idoneità all&#39;inserzione Amazon devono avere **[!UICONTROL Use for Promo Rule Conditions]** impostato su `Yes`. Vedi **[!UICONTROL Use for Promo Rule Conditions]** in [Attributi del prodotto](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### Imposta l&#39;area geografica [!DNL Amazon Seller Central] su inattiva

Per facilitare la transizione dei dati senza errori durante l’integrazione, si consiglia di impostare lo stato dell’area geografica di Amazon su `Inactive` in Impostazioni > Informazioni account > Impostazioni ferie. Al termine dell&#39;installazione, torna allo stato `Active` in Amazon.

![Icona successiva](assets/btn-next.png) [**Continua con la creazione di [!DNL Commerce] attributi**](./ob-creating-magento-attributes.md)
