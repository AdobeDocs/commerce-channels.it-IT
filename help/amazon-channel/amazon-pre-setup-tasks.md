---
title: Attività pre-installazione
description: Esamina le attività necessarie da completare prima di integrare l’Adobe Commerce o l’archivio Magenti Open Source in Amazon Sales Channel.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Attività pre-installazione

Prima [Integrazione store](./store-integration.md), assicurati che [!DNL Amazon Seller Central] l&#39;account [!DNL Commerce] l’account è pronto per l’integrazione. Per eseguire l&#39;integrazione, sono necessarie alcune attività di preinstallazione.

Quando si imposta il primo negozio Amazon nel canale di vendita Amazon, viene visualizzato un elenco delle attività di configurazione. Prima di eseguire questa operazione, è consigliabile rivedere queste attività [aggiungere un archivio Amazon](./store-integration.md). Dopo aver aggiunto il tuo primo negozio, puoi rivedere queste attività nella vista Apprendimento e preparazione del canale di vendita Amazon [home page](./amazon-sales-channel-home.md).

## 1. Abilitare le attività in background in [!DNL Commerce]

Tutti i prodotti e i dati sincronizzati tra [!DNL Commerce] e Amazon è gestito da un [cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}. Quando si completano attività quali aggiungere o aggiornare elenchi e ricevere ordini, un processo cron invia e riceve dati tra le [!DNL Commerce] back-end e [!DNL Amazon Seller Central] conto.

- [Abilita [!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}.

- Per prestazioni massime, [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;} da eseguire una volta ogni cinque minuti.

## 2. Crea il tuo [!DNL Amazon Seller Central] account

Prima di iniziare a configurare il canale di vendita Amazon, devi disporre di un [!DNL Amazon Seller Central] conto. Se non disponi di un account Amazon Seller esistente nella sezione [Nord America (Stati Uniti, CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;} o [Europeo (Regno Unito)](https://sell.amazon.co.uk/sell-online/beginners-guide)Area {target=&quot;_blank&quot;}, è possibile completare il processo di configurazione dell&#39;account venditore di Amazon.

Il canale di vendita Amazon richiede un [!DNL Professional Seller] conto su [!DNL Amazon Seller Central]. Amazon impone un abbonamento mensile e tariffe per la vendita. Vedi [Amazon: Scegli il piano di vendita](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.

## 3. Assicurati di essere un venditore Amazon approvato

Per eseguire l&#39;integrazione, è necessario disporre di un [!DNL Amazon Seller Central] conto. Il tuo account non deve avere restrizioni per prodotti o categorie. Alcuni prodotti e categorie richiedono l’approvazione prima di creare elenchi. Rivedi i criteri Amazon per l’approvazione di prodotti e categorie per assicurarti che i tuoi prodotti siano approvati. Vedi [Amazon: Categorie e prodotti che richiedono l&#39;omologazione](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;} (accesso al centro rivenditori richiesto).

È inoltre importante assicurarsi di aver configurato quanto segue nel [!DNL Amazon Seller Central] account:

- Assicurati che i criteri di restituzione siano buoni o migliori dei criteri di restituzione di Amazon. Vedi [Amazon: Criteri di ritorno](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}.

- Assicurati che le tue impostazioni fiscali siano configurate. Vedi [Amazon: Politiche fiscali](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;} (accesso al centro rivenditori richiesto).

- Assicurati che i tuoi metodi di spedizione siano configurati con precisione. Per impostare i metodi di spedizione che [!DNL Commerce] sono offerti ai clienti per soddisfare i tuoi ordini Amazon, aggiornare [Amazon: Impostazioni di spedizione](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;} nel tuo [!DNL Amazon Seller Central] conto.

## 4. Assicurati che l&#39;IVA sia configurata per i tuoi negozi

(Utilizzato principalmente dai venditori britannici). Amazon consiglia di iscriversi al [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}. Se scegli un metodo diverso, sei responsabile della conformità IVA.

>[!NOTE]
>
>Potrebbero essere necessari 10-14 giorni perché Amazon verifichi e attivi il tuo account Servizio di calcolo dell&#39;IVA.

## 5. Aumentare il numero di corrispondenze automatiche al catalogo

Durante l’onboarding, il canale di vendita Amazon utilizza gli attributi di prodotto per far corrispondere gli elenchi Amazon esistenti (se applicabili) ai prodotti esistenti nel tuo [!DNL Commerce] catalogo. Dopo l’onboarding, questi attributi di prodotto vengono utilizzati per pubblicare il tuo [!DNL Commerce] catalogare gli elementi in un elenco Amazon e sincronizzare i dati dei prodotti tra [!DNL Commerce] e Amazon.

Per avere il numero più alto di [!DNL Commerce] i prodotti corrispondono automaticamente agli elenchi di Amazon, devi creare un set di attributi di prodotto per [!DNL Commerce] catalogo. Prima di configurare il tuo archivio canali di vendita Amazon, devi aggiungere [!DNL Commerce] gli attributi del prodotto in modo che corrispondano a questi attributi di Amazon, ad esempio: ASIN, EAN, ISBN, UPC o GCID. Vedi [Crea un attributo di prodotto in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Configura la valuta e la conversione (in base alle esigenze)

Se l&#39;archivio Amazon utilizza una valuta diversa da quella configurata per la [!DNL Commerce] negozio, [abilitare la valuta](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} e imposta il [tasso di conversione della valuta](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}.

## 7. Crea un attributo Product Condition (in base alle esigenze)

Se gli elenchi Amazon contengono più di una condizione di prodotto (ad esempio _nuovo_, _usato_ oppure _come nuovo_), crea un [!DNL Commerce] attribuire e assegnare valori di condizione. È necessario mappare questo attributo durante l’onboarding sull’attributo di prodotto Amazon Condition . Vedi [Creazione di attributi per Amazon](./ob-creating-magento-attributes.md).

## 8. Configura il tuo [!DNL Amazon Seller Central] metodo di spedizione

Per impostare i metodi di spedizione che si desidera offrire per soddisfare gli ordini Amazon, fare riferimento a [Impostazioni e impostazioni di spedizione][10] nel tuo [!DNL Amazon Seller Central] conto.

## Configurazioni aggiuntive

Quando il tuo account Amazon è configurato e attivo, sono disponibili diversi [!DNL Commerce] consigli che semplificano il processo di onboarding dei canali di vendita Amazon.

### Rivedi e prendi nota di tutti i prodotti che desideri escludere

Potresti non volere elencare alcuni prodotti in Amazon. Il canale di vendita Amazon dispone di un motore di regole di elenco utilizzato per determinare quali prodotti sono idonei per la pubblicazione in Amazon. [Regole di elenco](./listing-rules.md) consente di selezionare sottoinsiemi di prodotti da pubblicare (o non pubblicare) nel [!DNL Amazon Seller Central] , ad esempio per selezione di categorie o definendo uno o più attributi di prodotto. Simile [!DNL Commerce] [catalogo](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} o [carrello](https://docs.magento.com/user-guide/marketing/price-rules-cart.html)Le regole di prezzo {target=&quot;_blank&quot;}, gli attributi di prodotto utilizzati per l&#39;elenco di idoneità di Amazon devono avere **[!UICONTROL Use for Promo Rule Conditions]** impostato su `Yes`. Consulta la sezione **[!UICONTROL Use for Promo Rule Conditions]** in [Attributi del prodotto](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

### Imposta le [!DNL Amazon Seller Central] da regione a inattiva

Per facilitare la transizione dei dati senza errori durante l’integrazione, è consigliabile impostare la propria area geografica Amazon su `Inactive` stato in Impostazioni > Informazioni account > Impostazioni vacanza. Fai riferimento a [Amazon: Stato dell&#39;elenco per le vacanze][11]. Al termine della configurazione, reimposta lo stato su `Active` in Amazon.

![Icona Successivo](assets/btn-next.png) [**Continua a creare [!DNL Commerce] Attributi**](./ob-creating-magento-attributes.md)
