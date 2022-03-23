---
title: '''[!DNL Amazon Sales Channel] Note sulla versione'''
description: Consulta le note sulla versione per informazioni su tutti [!DNL Amazon Sales Channel] versioni.
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: adf86495e7de53f9ee7bc916b2a7398f04e7cbd4
workflow-type: tm+mt
source-wordcount: '2130'
ht-degree: 0%

---

# Note sulla versione

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] può essere installato su istanze con Magenti Open Source, Adobe Commerce e Adobe Commerce sulle versioni 2.3.x e 2.4.x dell’infrastruttura cloud. L&#39;estensione non è più supportata in Adobe Commerce 2.1, Magenti Open Source 2.2 o Magento 1.
> <br>Il supporto è disponibile per [!DNL Amazon sales channel]  solo nelle versioni 4.0.0 e 4.1.0 di Adobe Commerce 2.3.x.
> <br>[!DNL Amazon sales channel] La versione 4.2.0+ è compatibile con le versioni Adobe Commerce 2.3.x, ma il supporto è disponibile solo per le versioni Adobe Commerce 2.4.x.

Queste note sulla versione descrivono la versione iniziale di [!DNL Amazon sales channel] e comprendono:

![Nuovo](../assets/new.svg) Nuove funzioni
![Problema risolto](../assets/fix.svg) Correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti

Vedi [Versioni future](https://devdocs.magento.com/release/){target=&quot;_blank&quot;} per il controllo delle versioni, il supporto e la compatibilità.

## v4.4.3

[!DNL Amazon sales channel]  4.4.3 è compatibile con le versioni 2.3.x e 2.4.0 di Adobe Commerce, ma è supportato solo per le versioni 2.4.1+, ad Magento Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

Questa versione di [!DNL Amazon sales channel] include la seguente correzione.

![Correzione](../assets/fix.svg) È stato aggiunto il supporto per Adobe Commerce 2.4.4.

## v4.4.2

[!DNL Amazon sales channel]  4.4.2 è compatibile con le versioni 2.3.x e 2.4.0 di Adobe Commerce, ma è supportato solo per le versioni 2.4.1+, ad Magento Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

Questa versione di [!DNL Amazon sales channel] include le seguenti correzioni.

![Correzione](../assets/fix.svg) Sono state aggiornate le dipendenze per supportare altre estensioni aggiornate.
![Correzione](../assets/fix.svg) È stato aggiunto il supporto per PHP 8.1.

## v4.4.1

[!DNL Amazon sales channel] 4.4.1 è compatibile con le versioni 2.3.x e 2.4.0 di Adobe Commerce, ma è supportato solo per le versioni 2.4.1+, ad Magento Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

Questa versione di [!DNL Amazon sales channel]  include la seguente correzione.

![Correzione](../assets/fix.svg) È stato modificato il modo in cui Adobe Commerce riceve il _Nome utente_ campo da Amazon. In precedenza, si verificava un errore durante la creazione dell&#39;ordine quando la _Nome utente_ il campo conteneva caratteri speciali. Adobe Commerce ora riceve il _Nome utente_ e filtra i caratteri speciali in modo che l’ordine possa essere creato correttamente.

## v4.4.0

[!DNL Amazon sales channel] 4.4.0 è compatibile con le versioni 2.3.x e 2.4.0 di Adobe Commerce, ma è supportato solo per le versioni 2.4.1+, ad Magento Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

Questa versione di [!DNL Amazon sales channel] include i miglioramenti e le correzioni seguenti.

![Nuovo](../assets/new.svg) È stato aggiunto il supporto per la modalità di sola lettura alla configurazione. Vedi [impostazioni del canale di vendita](sales-channel-settings.md).

![Correzione](../assets/fix.svg) È stato modificato il flusso di dati in modo che più copie della stessa istanza possano recuperare gli aggiornamenti contemporaneamente.

![Correzione](../assets/fix.svg) È stato modificato il processo di sincronizzazione per la sincronizzazione delle informazioni sull’account. È stato aggiunto un processo cron da sincronizzare con l’account remoto e ha aggiunto la stessa funzionalità ai comandi CLI.

![Correzione](../assets/fix.svg) Sono stati aggiunti argomenti di comando e flag CLI per un controllo più preciso.

![Correzione](../assets/fix.svg) Correzione dell&#39;origine attività in background (cron) nella configurazione del sistema.

![Correzione](../assets/fix.svg) È stato corretto il problema che impediva la creazione di ordini quando il codice del paese era impostato su Porto Rico (PR).

## v4.3.0

[!DNL Amazon sales channel] 4.3.0 è compatibile con le versioni 2.3.x e 2.4.0 di Adobe Commerce. Il supporto è disponibile solo per le versioni 2.4.1+, ad Magento Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

Questa versione di [!DNL Amazon sales channel] include i miglioramenti e le correzioni seguenti.

![Correzione](../assets/fix.svg) <!--CHAN-xxxx-->La _Dettagli ordine_ è stata riprogettata e non si basa più sul _Importa ordini_ impostazione. I dettagli dell’ordine vengono ora visualizzati nell’interfaccia di Amazon Sales Channel per tutti gli ordini.

![Correzione](../assets/fix.svg) In _[!UICONTROL Marketing]_in Admin, il nome è stato modificato da_[!UICONTROL Amazon]_ a _[!UICONTROL Amazon Sales Channel]_.

![Problema noto](../assets/bug.svg) **Importante**: I problemi noti relativi alla compatibilità Adobe Commerce 2.4.0 vengono risolti nella versione Adobe Commerce 2.4.1.

- Processi cron Amazon in `error` stato
- L’installazione con Commerce 2.4.0 non riesce quando si creano archivi nel database
- La creazione del prodotto non riesce quando MSI è installato

## v4.2.0

[!DNL Amazon sales channel] 4.2.0 è compatibile con Adobe Commerce versione 2.3.x ma supportato solo per le versioni 2.4.x di Magenti Open Source, Adobe Commerce e Adobe Commerce su infrastruttura cloud. Se hai un [!DNL Amazon sales channel] È stata installata la versione e si tenta di aggiornare Adobe Commerce alla versione 2.4.0. Viene richiesto di aggiornare l’estensione prima di completare l’aggiornamento Adobe Commerce.

Questa versione di [!DNL Amazon sales channel] include una nuova funzionalità, miglioramenti e correzioni.

![Problema noto](../assets/bug.svg) Quando [!DNL Amazon sales channel] 4.2.0 è integrato con la versione 2.4.0 e [Inventory management](https://docs.magento.com/user-guide/catalog/inventory.html) è attivato, esiste un problema noto che impedisce l’aggiunta di prodotti nel catalogo Commerce. Questo problema verrà risolto in una futura versione Commerce.

![Nuovo](../assets/new.svg) [!DNL Amazon sales channel] è stato migliorato per accettare dati di indirizzi basati su testo e farli corrispondere a formati di indirizzi standardizzati, quali città, stato e codice postale. Questo aggiornamento consente la sincronizzazione dei dati relativi all’ordine e alla spedizione (sincronizzazione) con Amazon senza errori di indirizzo.<br/>Ad esempio, un acquirente immette la città, lo stato e il codice postale come `Escondido, californiA 92025-1501`. Il Sales Channel Amazon importa e corrisponde ai dati nel formato standard come `Escondido, CA 92025`, quindi sincronizzalo nuovamente con Amazon in questo formato standard.

![Nuovo](../assets/new.svg) È stato aggiunto il supporto per PHP 7.4.

![Nuovo](../assets/new.svg) <!--CHAN-4334-->È stato aggiunto il supporto per Adobe Commerce 2.4.x. Le versioni precedenti possono essere compatibili con Commerce 2.4.x, ma non sono supportate. Vedi [Versioni future](https://devdocs.magento.com/release/){:target=&quot;_blank&quot;} per la compatibilità delle versioni. È necessario aggiornare Amazon Sales Channel alla versione 4.2.0 prima di completare l’aggiornamento ad Adobe Commerce 2.4.0.

![Correzione](../assets/fix.svg) <!--CHAN-4431-->È stato corretto un problema che causava un _Accesso negato_ errore per i clienti britannici.

![Correzione](../assets/fix.svg) <!--CHAN-4394-->È stato corretto un problema che impediva la sincronizzazione dello stato di spedizione di Amazon con l’ordine Commerce corrispondente, bloccando in tal modo lo stato di spedizione dell’ordine come `Pending` nel commercio e `Unshipped` in Amazon. Con la nuova funzione indirizzo standardizzato, questi errori di stato di spedizione sono stati risolti.

![Correzione](../assets/fix.svg) <!--ticket#-->Sincronizzazione dell&#39;ordine aggiornata per ignorare le importazioni di ordini non riusciti, riducendo così i tentativi di sincronizzazione multipli e consentendo l&#39;elaborazione delle importazioni successive, con le richieste di sincronizzazione degli ordini inviate ogni cinque minuti. Gli errori di sincronizzazione vengono ancora registrati nel registro degli errori, ma contrassegnati come &quot;elaborati&quot; per consentire ulteriori funzioni di registrazione. Inoltre, [!DNL Amazon sales channel] ora rimuove automaticamente i dati in eccesso raccolti per gli ordini che non possono essere creati in Commerce.

![Correzione](../assets/fix.svg) Registrazione degli errori aggiornata per raccogliere ulteriori informazioni sugli errori di eccezione e aggiornamento dell&#39;estensione non rilevati.

![Correzione](../assets/fix.svg) <!--ticket#-->È stato corretto un problema che causava la sincronizzazione iniziale del _prezzo più basso_ dati non riusciti a causa di un _prezzo_ valore.

![Correzione](../assets/fix.svg) <!--CHAN-4410-->Sono stati corretti i problemi che causavano errori di filtro nel _Ordini Amazon_ visualizza quando il campo intervallo di date viene lasciato vuoto.

![Correzione](../assets/fix.svg) <!--CHAN-4439-->È stato corretto un problema che causava errori di sincronizzazione delle scorte e di evasione relativi alla quantità. L&#39;estensione ora arrotonda i valori di quantità immessi come decimale prima della sincronizzazione con Amazon.<br/> Ad esempio, quando un commerciante immette manualmente una quantità di `2.5`, l&#39;estensione arrotonda il valore a `2` quindi sincronizza la quantità aggiornata con Amazon.

## v4.1.0

Amazon Sales Channel 4.1.0 è compatibile con Adobe Commerce 2.3.x di Commerce Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud. Questa versione di Amazon Sales Channel include miglioramenti all&#39;interfaccia utente e correzioni di bug minori.

![Nuovo](../assets/new.svg) <!--4247, 4230-->È stato modificato il processo di importazione dell’ordine per allinearlo ai requisiti dell’ordine Commerce. Queste modifiche correggono i problemi che impedivano a Commerce di creare l’ordine corrispondente per un ordine importato. Vedi [Gestisci ordini](managing-orders.md) per informazioni sui blocchi degli ordini e sulle soluzioni.

![Nuovo](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->È stato aggiornato il _Ordini recenti_ sezione del dashboard store e aggiunto un nuovo _Tutti gli ordini_ visualizza tutti gli ordini di Amazon, incluse le opzioni di filtro e l’impaginazione per la visualizzazione di più ordini. Vedi [Dashboard di Amazon Store](amazon-store-dashboard.md) e [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) È stato aggiunto il _[!UICONTROL Order Notes]_della colonna riprogettata_[!UICONTROL Amazon Orders]_ tabella in entrambi _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_ visualizzazioni. _[!UICONTROL Order Notes]_informi il commerciante che c&#39;è un problema con l&#39;importazione dell&#39;ordine. Vedi [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) <!--CHAN-4013-->Sono stati aggiornati i parametri di condizione del prodotto per l’allineamento con [Amazon rinnovato](https://sell.amazon.com/programs/renewed) programma. Vedi [Prodotti rinnovati](renewed-products.md).

![Nuovo](../assets/new.svg) <!--CHAN-3680-->Aggiornato [Dettagli ordine Amazon](amazon-order-details.md) includere &quot;dati generici&quot; per gli ordini che sono soddisfatti da Amazon. Vedi [Completato da](fulfilled-by.md).

![Correzione](../assets/fix.svg) <!--CHAN-4069-->È stato risolto un problema che causava la distorsione delle icone sulla scheda del negozio.

![Correzione](../assets/fix.svg) <!--CHAN-4165-->È stato corretto un errore che impediva la _Login_ la schermata viene visualizzata dopo l’interruzione della sessione.

![Correzione](../assets/fix.svg) <!--CHAN-4211-->È stato risolto un problema che impediva l’importazione dell’importo dell’imposta ordine Amazon nel nuovo ordine Commerce.

![Correzione](../assets/fix.svg) <!--CHAN-4234-->È stato corretto un problema a causa del quale i totali dei ricavi visualizzati nel dashboard archivio includevano gli ordini in `Canceled` o `Error` stato.

![Correzione](../assets/fix.svg) <!--CHAN-4326-->È stato corretto un problema che causava errori di importazione dell’ordine associati a estensioni di terze parti che utilizzano _Magento Shipping_ metodi per la creazione di ordini.

![Correzione](../assets/fix.svg) <!--CHAN-4357-->È stato corretto un problema che causava errori durante l’esecuzione della sincronizzazione cron. È stato aggiunto un blocco al comando CLI che impedisce la sincronizzazione simultanea di due processi cron.

![Correzione](../assets/fix.svg) È stata aggiornata la policy di sicurezza dei contenuti per il supporto con Commerce versione 2.3.5.

## v4.0.0

Amazon Sales Channel 4.0.0 è compatibile con le versioni 2.3.0, 2.3.1, 2.3.2, 2.3.3 e 2.3.4 di Magenti Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud. Questa versione di Amazon Sales Channel include molti aggiornamenti dell&#39;interfaccia utente, insieme a correzioni di bug minori.

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 non è supportato per Adobe Commerce 2.3.5. Per il supporto con Adobe Commerce 2.3.5, effettua l’aggiornamento ad Amazon Sales Channel 4.1.0.

![Nuovo](../assets/new.svg) Introduzione di un nuovo [Sales Channel Amazon](amazon-sales-channel-home.md) home page con &quot;vista a schede&quot; migliorata per le informazioni del negozio.

![Nuovo](../assets/new.svg) Introduzione di un nuovo [dashboard store](amazon-store-dashboard.md) con inserzioni, ordini recenti e informazioni sulle impostazioni di archiviazione.

![Nuovo](../assets/new.svg) Introduzione di un sistema più semplice e semplificato [processo di onboarding](amazon-onboarding-home.md) e [impostazioni store predefinite](default-store-settings.md) per velocizzare l&#39;integrazione dei negozi.

![Problema noto](../assets/bug.svg) <!--CHAN-4102--> Quando [creazione di attributi](managing-attributes.md) per l&#39;importazione di immagini da elenchi e **Visualizzazioni store** è impostato su `All Store Views (Global)`, esiste un problema noto che impedisce l’importazione di immagini in tutte le viste store. Se si modifica l&#39;impostazione per **Memorizza visualizzazioni (per importare valori in)** in un archivio specifico, le immagini vengono importate per tale archivio.

## v3.0.1

Amazon Sales Channel 3.0.1 è compatibile con le versioni 2.2.4+ e 2.3.x di Magenti Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

![Correzione](../assets/fix.svg) **Impostazioni campo numerico**: <!--CHAN-3779-->I campi che richiedono un valore numerico sono stati aggiornati per accettare solo caratteri numerici. Esempio: Impostazioni regola determinazione prezzi > Campo Importo adeguamento

![Correzione](../assets/fix.svg) **Collegamenti alla guida utente**: <!--CHAN-3778-->Errato _Guida utente_ i collegamenti sono stati corretti.

![Correzione](../assets/fix.svg) **Duplica elenchi Amazon**: <!--CHAN-3593-->È stato corretto un problema precedentemente segnalato che causava la duplicazione degli elenchi di Amazon. Prima di questa versione, l’estensione aggiungeva il codice del paese per l’area Amazon ai valori SKU al momento dell’importazione degli elenchi. L’elenco corrisponde all’elemento del catalogo, ma l’estensione ha creato un nuovo elenco duplicato con lo SKU aggiunto. Con questa versione, l’estensione non modifica lo SKU per gli elenchi importati e non vengono apportate modifiche agli elenchi esistenti. È possibile utilizzare [!UICONTROL End Listing(s)] su Amazon per rimuovere gli elenchi duplicati.

## v3.0.0

Amazon Sales Channel 3.0.0 è compatibile con le versioni 2.2.4+ e 2.3.x di Magenti Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

![Nuovo](../assets/new.svg) **Amazon UK Marketplace ora disponibile**: Gli utenti possono scegliere il marketplace del Regno Unito durante la creazione e l&#39;integrazione di un negozio Commerce. Questo aggiornamento del Regno Unito include supporto aggiuntivo per:

- [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources){target=&quot;_blank&quot;}

- [Codice fiscale prodotto](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US)Informazioni su {target=&quot;_blank&quot;}.

![Nuovo](../assets/new.svg) **Registrazione migliorata**: <!--CHAN-3642, 3672-->Implementato il **Abilita registrazione debug** funzionalità per la raccolta di dati di sincronizzazione aggiuntivi quando è necessaria una risoluzione dei problemi. Consulta la sezione [Impostazioni Sales Channel](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) in Riferimento configurazione.

![Correzione](../assets/fix.svg) **Catalogo dei prodotti**: <!--CHAN-3687-->È stato risolto un problema che impediva l’applicazione delle immagini importate con un elenco Amazon al prodotto catalogo Commerce corrispondente.

![Correzione](../assets/fix.svg) **Creazione di ordini**: <!--CHAN-3708-->È stato corretto un problema che impediva a Commerce di creare ordini per un ordine Amazon non corrispondente a un prodotto catalogo Commerce.

![Problema noto](../assets/bug.svg) **Duplica elenchi Amazon**: <!--CHAN-3593-->Questo problema fa sì che il catalogo crei un articolo per un elenco importato, utilizzando lo stesso SKU ma con un codice di regione aggiunto alla fine. Amazon elabora quindi lo SKU modificato come nuovo elemento e crea un elenco. Questo problema verrà risolto in una versione futura.

## v2.0.0

Amazon Sales Channel 2.0.0 è compatibile con le versioni 2.2.4+ e 2.3.x di Magenti Open Source, Adobe Commerce e Adobe Commerce sull’infrastruttura cloud.

>[!NOTE]
>
>La versione 1.0.0 era disponibile solo nella versione limitata.

![Nuovo](../assets/new.svg)  **Onboarding e manutenzione semplificati**: Aggiungi e integra con il tuo account Amazon Seller tramite una procedura dettagliata con istruzioni dettagliate disponibili tramite l’amministratore. Gestisci i tuoi negozi, account e prodotti elencati tramite un dashboard.

![Nuovo](../assets/new.svg)  **Supporto di più account**: Gestisci e monitora più marchi Amazon e aree di marketplace tramite l’amministratore.

![Nuovo](../assets/new.svg)  **Prezzi intelligenti**: Imposta regole di rideterminazione dei prezzi automatizzate per aumentare le tue possibilità per l&#39;ambito Buy Box. Impostare i prezzi in modo da adattarsi dinamicamente al prezzo Buy Box corrente o al prezzo più basso della concorrenza. Imposta i limiti per la rideterminazione dei prezzi per proteggere il tuo margine.

![Nuovo](../assets/new.svg)  **Gestione degli elenchi**: Automatizza gli elenchi dei prodotti e sincronizza il catalogo Commerce con Amazon Marketplace utilizzando le regole di elenco. Aggiungi sostituzioni specifiche per controllare con precisione le offerte. Monitora e gestisci tutti gli elenchi direttamente dall’amministratore.

![Nuovo](../assets/new.svg)  **Inventory management coerente**: Mantieni le quantità di inventario Commerce e Amazon in sincronizzazione costante.

![Nuovo](../assets/new.svg)  **Gestione dell&#39;ordine e dell&#39;evasione**: Monitora gli ordini di Amazon attraverso il dashboard, con comunicazioni e aggiornamenti di inventario senza soluzione di continuità. Completare e tenere traccia delle spedizioni degli ordini come soddisfatte da Amazon, dagli esercenti adempiuti o da una combinazione di metodi.

![Problema noto](../assets/bug.svg)  È possibile che si verifichino tempi di attesa più lunghi per l’aggiornamento delle quantità di prodotti. La sincronizzazione degli aggiornamenti per la quantità di prodotto potrebbe richiedere circa due ore.

![Problema noto](../assets/bug.svg)  Gli ordini importati possono avere un tipo di _Prime_ o _Premium_ ordini. Devi verificare questi ordini nel tuo account Amazon Seller.

![Problema noto](../assets/bug.svg)  I prodotti bundle non consentiti possono essere visualizzati come Idonei per l’inserimento nell’elenco su Amazon. Uno dei prodotti inclusi nel prodotto abbinato potrebbe non essere ammissibile. In caso di problemi, controlla lo stato di idoneità per gli elementi dei prodotti raggruppati.

![Problema noto](../assets/bug.svg)  Quando si utilizza Inventory management for Commerce 2.3.x, non è possibile che venga attivato un reindice azionario parziale alla creazione di un ordine. La quantità vendibile ricalcola ogni ora, il che può causare la vendita in eccesso durante questo intervallo di aggiornamento.
