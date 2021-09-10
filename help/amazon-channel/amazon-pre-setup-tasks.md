---
title: Attività pre-installazione
description: Rivedi le attività necessarie da completare prima di integrare Adobe Commerce o Magenti Open Source Store in Amazon Sales Channel.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Attività pre-installazione

Prima di [archiviare l&#39;integrazione](./store-integration.md), è necessario assicurarsi che l&#39;account [!DNL Amazon Seller Central] e l&#39;account [!DNL Commerce] siano pronti per l&#39;integrazione. Per eseguire l&#39;integrazione, sono necessarie alcune attività di preinstallazione.

Quando si imposta il primo negozio Amazon nel canale di vendita Amazon, viene visualizzato un elenco delle attività di configurazione. È consigliabile rivedere queste attività prima di [aggiungere un archivio Amazon](./store-integration.md). Dopo aver aggiunto il tuo primo negozio, puoi rivedere queste attività nella vista Apprendimento e preparazione del canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## 1. Abilita le attività in background in [!DNL Commerce]

Tutti i prodotti e i dati sincronizzati tra [!DNL Commerce] e Amazon sono gestiti da un [lavoro cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}. Quando si completano attività quali l’aggiunta o l’aggiornamento di elenchi e la ricezione di ordini, un processo cron invia e riceve dati tra il backend [!DNL Commerce] e l’account [!DNL Amazon Seller Central].

- [ [!DNL Commerce] Enablecron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}.

- Per prestazioni massime, [impostare [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;} per l&#39;esecuzione una volta ogni cinque minuti.

## 2. Crea il tuo account [!DNL Amazon Seller Central]

Prima di iniziare a configurare il canale di vendita Amazon, devi disporre di un account [!DNL Amazon Seller Central] attivo. Se nell&#39;area [Nord America (Stati Uniti, CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;} o [Europa (Regno Unito)](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;} non è presente un account venditore esistente, è possibile completare il processo di configurazione dell&#39;account venditore Amazon.

Il canale di vendita Amazon richiede un account [!DNL Professional Seller] su [!DNL Amazon Seller Central]. Amazon impone un abbonamento mensile e tariffe per la vendita. Consulta [Amazon: Scegli il piano di vendita](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.

## 3. Assicurati di essere un venditore Amazon approvato

Per eseguire l&#39;integrazione, è necessario disporre di un account [!DNL Amazon Seller Central] approvato. Il tuo account non deve avere restrizioni per prodotti o categorie. Alcuni prodotti e categorie richiedono l’approvazione prima di creare elenchi. Rivedi i criteri Amazon per l’approvazione di prodotti e categorie per assicurarti che i tuoi prodotti siano approvati. Consulta [Amazon: Categorie e prodotti che richiedono l&#39;approvazione](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;} (accesso a Seller Central richiesto).

È inoltre importante assicurarsi di aver configurato quanto segue nel proprio account [!DNL Amazon Seller Central]:

- Assicurati che i criteri di restituzione siano buoni o migliori dei criteri di restituzione di Amazon. Consulta [Amazon: Restituisce Policy](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}.

- Assicurati che le tue impostazioni fiscali siano configurate. Consulta [Amazon: Informativa fiscale](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;} (accesso a Seller Central richiesto).

- Assicurati che i tuoi metodi di spedizione siano configurati con precisione. Per impostare i metodi di spedizione [!DNL Commerce] offerti ai clienti per soddisfare i tuoi ordini Amazon, aggiorna l’ [Amazon: Impostazioni di spedizione](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;} nel tuo account [!DNL Amazon Seller Central].

## 4. Assicurati che l&#39;IVA sia configurata per i tuoi negozi

(Utilizzato principalmente dai venditori britannici). Amazon consiglia di registrarsi per il [servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}. Se scegli un metodo diverso, sei responsabile della conformità IVA.

>[!NOTE]
>
>Potrebbero essere necessari 10-14 giorni perché Amazon verifichi e attivi il tuo account Servizio di calcolo dell&#39;IVA.

## 5. Aumentare il numero di corrispondenze automatiche al catalogo

Durante l’onboarding, il canale di vendita Amazon utilizza gli attributi di prodotto per far corrispondere gli elenchi Amazon esistenti (se applicabili) ai prodotti esistenti nel catalogo [!DNL Commerce]. Dopo l’onboarding, questi attributi di prodotto vengono utilizzati per pubblicare gli elementi di catalogo [!DNL Commerce] in un elenco Amazon e per sincronizzare i dati di prodotto tra [!DNL Commerce] e Amazon.

Per far corrispondere automaticamente il numero più alto di prodotti [!DNL Commerce] con gli elenchi di Amazon, crea un set di attributi di prodotto per il catalogo [!DNL Commerce]. Prima di configurare l&#39;archivio dei canali di vendita di Amazon, è necessario aggiungere gli attributi di prodotto [!DNL Commerce] in modo che corrispondano a questi attributi di Amazon, ad esempio: ASIN, EAN, ISBN, UPC o GCID. Consulta [Creare un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Configura la valuta e la conversione (in base alle esigenze)

Se l&#39;archivio Amazon utilizza una valuta diversa da quella configurata per l&#39;archivio [!DNL Commerce], [abilita la valuta](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} e imposta il [tasso di conversione della valuta](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}.

## 7. Crea un attributo Product Condition (in base alle esigenze)

Se gli elenchi Amazon contengono più di una condizione di prodotto (ad esempio _new_, _used_ o _like new_), crea un attributo [!DNL Commerce] e assegna valori di condizione. È necessario mappare questo attributo durante l’onboarding sull’attributo di prodotto Amazon Condition . Consulta [Creazione di attributi per Amazon](./ob-creating-magento-attributes.md).

## 8. Configura il tuo metodo di spedizione [!DNL Amazon Seller Central]

Per impostare i metodi di spedizione che si desidera offrire per soddisfare gli ordini Amazon, fare riferimento a [Impostazioni e impostazioni di spedizione][10] nel tuo account [!DNL Amazon Seller Central].

## Configurazioni aggiuntive

Quando il tuo account Amazon è configurato e attivo, ci sono diversi [!DNL Commerce] consigli che aiutano a semplificare il processo di onboarding dei canali di vendita Amazon.

### Rivedi e prendi nota di tutti i prodotti che desideri escludere

Potresti non volere elencare alcuni prodotti in Amazon. Il canale di vendita Amazon dispone di un motore di regole di elenco utilizzato per determinare quali prodotti sono idonei per la pubblicazione in Amazon. [Le ](./listing-rules.md) regole di elenco ti consentono di selezionare sottoinsiemi di prodotti da pubblicare (o non pubblicare) nel tuo  [!DNL Amazon Seller Central] account, ad esempio per selezione di categorie o definendo uno o più attributi di prodotto. Come per le regole di prezzo [!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} o [carrello](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}, gli attributi di prodotto utilizzati per l&#39;idoneità all&#39;elenco Amazon devono avere **[!UICONTROL Use for Promo Rule Conditions]** impostato su `Yes`. Vedi **[!UICONTROL Use for Promo Rule Conditions]** in [Attributi del prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

### Imposta l&#39;area [!DNL Amazon Seller Central] su inattiva

Per facilitare la transizione dei dati senza errori durante l’integrazione, è consigliabile impostare lo stato di Amazon su `Inactive` in Impostazioni > Informazioni account > Impostazioni vacanza. Fai riferimento a [Amazon: Stato elenco per le vacanze][11]. Al termine della configurazione, modifica nuovamente lo stato in `Active` in Amazon.

![Icona ](assets/btn-next.png) [**SuccessivoContinua alla creazione di  [!DNL Commerce] attributi**](./ob-creating-magento-attributes.md)
