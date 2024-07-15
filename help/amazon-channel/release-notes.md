---
title: '[!DNL Amazon Sales Channel] note sulla versione'
description: Consulta le note sulla versione per informazioni su tutte le  [!DNL Amazon Sales Channel]  versioni.
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2010'
ht-degree: 0%

---

# Note sulla versione di [!DNL Amazon Sales Channel]

>[!IMPORTANT]
>
> È possibile installare [!DNL Amazon sales channel] nelle istanze con Magento Open Source, Adobe Commerce e Adobe Commerce nelle versioni 2.3.x e 2.4.x dell&#39;infrastruttura cloud. L’estensione non è più supportata in Adobe Commerce 2.1, Magento Open Source 2.2 o Magento 1.
> <br>Il supporto è disponibile solo per [!DNL Amazon sales channel] versioni 4.0.0 e 4.1.0 nelle versioni Adobe Commerce 2.3.x.
> <br>[!DNL Amazon sales channel] la versione 4.2.0+ è compatibile con le versioni di Adobe Commerce 2.3.x, ma è disponibile il supporto solo per le versioni di Adobe Commerce 2.4.x.
>

Queste note sulla versione descrivono la versione iniziale di [!DNL Amazon sales channel] e includono:

![Nuove](../assets/new.svg) nuove funzionalità
![Problema risolto](../assets/fix.svg) correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti

Consulta [Prossime versioni](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) per il controllo delle versioni, il supporto e la compatibilità.

Consulta [Disponibilità del prodotto](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) per sapere quali versioni di Adobe Commerce supportano questa estensione.

## v4.5.0

*30 agosto 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) Aggiunto il gateway API Adobe.IO, che cambia da MAGI, per una maggiore sicurezza dell&#39;autenticazione. `ServicesId` fornisce una nuova interfaccia utente per gestire le credenziali Adobe.IO, simile ad altri [servizi Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html).

>[!NOTE]
>
>I commercianti devono assicurarsi che le [chiavi API private e pubbliche](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html) siano aggiornate per la produzione.


![È stato risolto un problema](../assets/fix.svg). È stato identificato un problema di impostazione della configurazione ed è stato risolto il flusso di creazione dell&#39;ordine.

## v4.4.4

*7 marzo 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![È stato risolto il problema](../assets/fix.svg) È stato aggiunto il supporto per Adobe Commerce 2.4.6 e PHP 8.2.

![È stato risolto il problema](../assets/fix.svg). Riduzione del rumore nei registri.

![È stato risolto il problema](../assets/fix.svg). È stata migliorata la stabilità degli aggiornamenti di richiamo.

![È stato risolto il problema](../assets/fix.svg). Il processo per l&#39;esecuzione di pull di tipo azione singola o per l&#39;applicazione da CLI è stato semplificato.

![È stato risolto il problema](../assets/fix.svg). È stata aggiornata la dipendenza per `magento/services-connector`.

![È stato risolto il problema](../assets/fix.svg) sono stati risolti i problemi di sincronizzazione negli account del Regno Unito con codice paese non valido.

![Problema risolto](../assets/fix.svg) L&#39;elemento hardcoded entity_type_id per l&#39;entità prodotto catalogo causa problemi con il prezzo Magento Source.

![È stato risolto un problema](../assets/fix.svg) che impediva l&#39;eliminazione dall&#39;interfaccia utente anche degli account eliminati in un back-end da un&#39;altra istanza.

![È stato risolto un problema](../assets/fix.svg) a causa del quale alcune regole del carrello interrompevano l&#39;importazione degli ordini.

## v4.4.3

*7 marzo 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) aggiunta del supporto per Adobe Commerce 2.4.4.

## v4.4.2

*11 novembre 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) dipendenze aggiornate per supportare altre estensioni aggiornate.
![Correzione](../assets/fix.svg) aggiunta del supporto per PHP 8.1.

## v4.4.1

*11 novembre 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) ha cambiato il modo in cui Adobe Commerce riceve il campo _Nome utente_ da Amazon. In precedenza, si era verificato un errore durante la creazione dell&#39;ordine quando il campo _Nome utente_ conteneva caratteri speciali. Adobe Commerce ora riceve i dati di _Nome utente_ e filtra i caratteri speciali in modo che l&#39;ordine possa essere creato correttamente.

## v4.4.0

*9 aprile 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![New](../assets/new.svg) ha aggiunto alla configurazione il supporto per la modalità di sola lettura. Vedi [impostazioni canale vendite](sales-channel-settings.md).

![Correzione](../assets/fix.svg) ha modificato il flusso di dati in modo che più copie della stessa istanza possano recuperare gli aggiornamenti contemporaneamente.

![Correzione](../assets/fix.svg) ha modificato il processo di sincronizzazione delle informazioni sull&#39;account. È stato aggiunto un processo cron da sincronizzare con l’account remoto e la stessa funzionalità è stata aggiunta ai comandi CLI.

![Correzione](../assets/fix.svg) aggiunti argomenti e flag di comando CLI per un controllo più preciso.

![Correzione](../assets/fix.svg): le attività in background (cron) di Source sono state corrette nella configurazione del sistema.

![Correzione](../assets/fix.svg) è stato corretto il problema che impediva la creazione di ordini quando il codice del paese era impostato su Porto Rico (PR).

## v4.3.0

*3 marzo 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) <!--CHAN-xxxx-->La funzionalità _Dettagli ordine_ è stata riprogettata e non si basa più sull&#39;impostazione _Importa ordini_. I dettagli dell’ordine vengono ora visualizzati nell’interfaccia di Sales Channel di Amazon per tutti gli ordini.

![Correzione](../assets/fix.svg) Nel menu _[!UICONTROL Marketing]_dell&#39;amministratore, il nome è stato modificato da_[!UICONTROL Amazon]_ a _[!UICONTROL Amazon Sales Channel]_.

![Problema noto](../assets/bug.svg) **Importante**: i problemi noti relativi alla compatibilità con Adobe Commerce 2.4.0 sono stati risolti nella versione Adobe Commerce 2.4.1.

- processi cron di Amazon nello stato `error`
- L’installazione con Commerce 2.4.0 non riesce durante la creazione di archivi nel database
- La creazione del prodotto non riesce quando è installato MSI

## v4.2.0

*3 marzo 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

Se è installata una versione precedente di [!DNL Amazon sales channel] e si tenta di aggiornare Adobe Commerce alla versione 2.4.0, viene richiesto di aggiornare l&#39;estensione prima di poter completare l&#39;aggiornamento di Adobe Commerce.

![Problema noto](../assets/bug.svg) Quando [!DNL Amazon sales channel] 4.2.0 è integrato con la versione 2.4.0 e [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) è abilitato, esiste un problema noto che impedisce l&#39;aggiunta di prodotti nel catalogo Commerce. Questo problema verrà risolto in una versione futura di Commerce.

![Nuovo](../assets/new.svg) [!DNL Amazon sales channel] è stato migliorato per accettare dati di indirizzi basati su testo e confrontarli con formati di indirizzi standardizzati, inclusi città, stato e CAP. Questo aggiornamento consente ai dati di ordine e spedizione di sincronizzarsi (sincronizzarsi) con Amazon senza errori di indirizzo.<br/>Ad esempio, un acquirente inserisce la città, lo stato, il codice postale come `Escondido, californiA 92025-1501`. Il Sales Channel Amazon importa e associa i dati al formato standard come `Escondido, CA 92025`, quindi li sincronizza nuovamente in Amazon in questo formato standard.

![Nuovo](../assets/new.svg) aggiunto supporto per PHP 7.4.

![Nuovo](../assets/new.svg) <!--CHAN-4334-->Aggiunto supporto per Adobe Commerce 2.4.x. Le versioni precedenti possono essere compatibili con Commerce 2.4.x, ma non sono supportate. Consulta [Prossime versioni](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) per informazioni sulla compatibilità delle versioni. Per completare l’aggiornamento di Amazon 2.4.0, è necessario aggiornare il Sales Channel Adobe Commerce alla versione 4.2.0.

![Correzione](../assets/fix.svg) <!--CHAN-4431-->È stato corretto un problema che causava un errore _Accesso negato_ per i clienti del Regno Unito.

![Correzione](../assets/fix.svg) <!--CHAN-4394-->È stato risolto un problema che impediva la sincronizzazione dello stato di spedizione di Amazon con l&#39;ordine Commerce corrispondente, &quot;bloccando&quot; lo stato di spedizione dell&#39;ordine come `Pending` in Commerce e `Unshipped` in Amazon. Con la nuova funzione di indirizzo standardizzato, questi errori di stato di spedizione sono stati risolti.

![Correzione](../assets/fix.svg) <!--ticket#-->Sincronizzazione ordini aggiornata (sincronizzazione) per ignorare le importazioni degli ordini non riuscite, riducendo così più tentativi di sincronizzazione e consentendo l&#39;elaborazione delle importazioni successive, con richieste di sincronizzazione ordini inviate ogni cinque minuti. Gli errori di sincronizzazione vengono comunque registrati nel registro degli errori, ma contrassegnati come &quot;elaborati&quot; per consentire ulteriori funzioni di registrazione. Inoltre, [!DNL Amazon sales channel] ora rimuove automaticamente i dati in eccesso raccolti per gli ordini non creati in Commerce.

![Correzione](../assets/fix.svg) Registrazione degli errori aggiornata per raccogliere ulteriori informazioni sugli errori non rilevati relativi all&#39;eccezione e all&#39;aggiornamento delle estensioni.

![Correzione](../assets/fix.svg) <!--ticket#-->È stato risolto un problema che causava un errore nella sincronizzazione iniziale dei dati del _prezzo più basso_ a causa di un valore _prezzo_ mancante.

![Correzione](../assets/fix.svg) <!--CHAN-4410-->Sono stati corretti i problemi che causavano errori di filtro nella visualizzazione _Amazon orders_ quando il campo dell&#39;intervallo di date viene lasciato vuoto.

![Correzione](../assets/fix.svg) <!--CHAN-4439-->È stato corretto un problema che causava errori di sincronizzazione di evasione e scorte correlate alla quantità. L’estensione ora arrotonda verso il basso i valori della quantità immessi come decimali prima di sincronizzarli con Amazon.<br/> Ad esempio, quando un commerciante inserisce manualmente una quantità di `2.5`, l&#39;estensione arrotonda il valore a `2` e quindi sincronizza la quantità aggiornata con Amazon.

## v4.1.0

*7 maggio 2020*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) <!--4247, 4230-->Il processo di importazione degli ordini è stato modificato per allinearlo ai requisiti degli ordini di Commerce. Queste modifiche correggono i problemi che impedivano a Commerce di creare l’ordine corrispondente per un ordine importato. Per informazioni sui blocchi ordini e sulle soluzioni, consulta [Gestione ordini](managing-orders.md).

![Nuovo](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->È stata aggiornata la sezione _Ordini recenti_ del dashboard dello store ed è stata aggiunta una nuova visualizzazione _Tutti gli ordini_ che mostra tutti gli ordini Amazon, incluse le opzioni di filtro e l&#39;impaginazione per visualizzare altri ordini. Consulta [Dashboard di Amazon Store](amazon-store-dashboard.md) e [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) Aggiunta della colonna _[!UICONTROL Order Notes]_della tabella_[!UICONTROL Amazon Orders]_ riprogettata nelle visualizzazioni _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_. _[!UICONTROL Order Notes]_informa il commerciante che esiste un problema con l&#39;importazione dell&#39;ordine. Vedi [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) <!--CHAN-4013-->Parametri di condizione del prodotto aggiornati per l&#39;allineamento con il programma [Amazon Renewed](https://sell.amazon.com/programs/renewed). Vedi [Prodotti rinnovati](renewed-products.md).

![Nuovo](../assets/new.svg) <!--CHAN-3680-->Aggiornamento di [Dettagli ordine Amazon](amazon-order-details.md) per includere &quot;dati generici&quot; per gli ordini evasi da Amazon. Vedi [Completato da](fulfilled-by.md).

![Correzione](../assets/fix.svg) <!--CHAN-4069-->È stato risolto un problema che causava la distorsione delle icone sulla scheda dello store.

![Correzione](../assets/fix.svg) <!--CHAN-4165-->È stato corretto un errore che impediva la visualizzazione della schermata _Accesso_ dopo il timeout della sessione.

![Correzione](../assets/fix.svg) <!--CHAN-4211-->È stato risolto un problema che impediva l&#39;importazione dell&#39;importo dell&#39;imposta dell&#39;ordine Amazon nel nuovo ordine Commerce.

![Correzione](../assets/fix.svg) <!--CHAN-4234-->È stato corretto un problema a causa del quale i totali delle entrate visualizzati nel dashboard dello store includevano ordini con stato `Canceled` o `Error`.

![Correzione](../assets/fix.svg) <!--CHAN-4326-->È stato corretto un problema che causava errori di importazione degli ordini associati alle estensioni di terze parti che utilizzano i metodi _Magento Shipping_ per la creazione degli ordini.

![Correzione](../assets/fix.svg) <!--CHAN-4357-->È stato corretto un problema che causava errori durante l&#39;esecuzione della sincronizzazione cron. È stato aggiunto un blocco al comando CLI che impedisce la sincronizzazione simultanea di due processi cron.

![Correzione](../assets/fix.svg) criteri di sicurezza del contenuto aggiornati per il supporto con Commerce versione 2.3.5.

## v4.0.0

*25 marzo 2020*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 non è supportato per Adobe Commerce 2.3.5. Per il supporto con Adobe Commerce 2.3.5, effettua l’aggiornamento ad Amazon Sales Channel 4.1.0.

![Nuovo](../assets/new.svg) è stata introdotta una nuova home page del [Sales Channel Amazon](amazon-sales-channel-home.md) con una &quot;vista a schede&quot; migliorata per le informazioni del tuo archivio.

![Nuovo](../assets/new.svg) ha introdotto un nuovo [dashboard dello store](amazon-store-dashboard.md) con informazioni su elenchi, ordini recenti e impostazioni dello store.

![Nuovo](../assets/new.svg) ha introdotto un [processo di onboarding](amazon-onboarding-home.md) più semplice e semplificato e [impostazioni store predefinite](default-store-settings.md) per integrare più rapidamente i tuoi store.

![Problema noto](../assets/bug.svg) <!--CHAN-4102--> Quando [crea attributi](managing-attributes.md) per importare immagini dagli elenchi e **Viste archivio** è impostato su `All Store Views (Global)`, esiste un problema noto che impedisce l&#39;importazione di immagini in tutte le viste archivio. Se si modifica l&#39;impostazione per **Viste archivio (per importare valori in)** in un archivio specifico, le immagini vengono importate per tale archivio.

## v3.0.1

*11 novembre 2019*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) **Impostazioni campo numerico**: <!--CHAN-3779-->I campi che richiedono un valore basato su numeri sono stati aggiornati per accettare solo caratteri numerici. Esempio: Impostazioni regola determinazione prezzi > campo Importo adeguamento

![Correzione](../assets/fix.svg) **Collegamenti alla Guida utente**: <!--CHAN-3778-->I collegamenti alla _Guida utente_ non sono corretti.

![Correzione](../assets/fix.svg) **Elenchi Amazon duplicati**: <!--CHAN-3593-->È stato corretto un problema segnalato in precedenza che causava la duplicazione degli elenchi Amazon. Prima di questa versione, l’estensione aggiungeva il codice paese per l’area geografica Amazon ai valori SKU durante l’importazione delle inserzioni. L’inserzione corrisponde all’elemento del catalogo, ma l’estensione ha creato una nuova inserzione duplicata con lo SKU aggiunto. Con questa versione, l’estensione non modifica lo SKU per le inserzioni importate e non viene apportata alcuna modifica alle inserzioni esistenti. Puoi utilizzare l&#39;opzione [!UICONTROL End Listing(s)] su Amazon per rimuovere le inserzioni duplicate.

## v3.0.0

*7 ottobre 2019*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) **Amazon UK Marketplace ora disponibile**: gli utenti possono scegliere il marketplace per il Regno Unito durante la creazione e l&#39;integrazione di un archivio Commerce. Questo aggiornamento per il Regno Unito include supporto aggiuntivo per:

- [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Informazioni sul codice fiscale](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}.

![Nuovo](../assets/new.svg) **Registrazione migliorata**: <!--CHAN-3642, 3672-->È stata implementata la funzionalità **Abilita registrazione debug** per raccogliere ulteriori dati di sincronizzazione quando è necessaria la risoluzione dei problemi. Consulta l&#39;argomento [Impostazioni Sales Channel](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) nella documentazione sulla configurazione.

![Correzione](../assets/fix.svg) **Catalogo prodotti**: <!--CHAN-3687-->È stato risolto un problema che impediva l&#39;applicazione delle immagini importate con un elenco Amazon al corrispondente prodotto catalogo Commerce.

![Correzione](../assets/fix.svg) **Creazione ordine**: <!--CHAN-3708-->È stato risolto un problema che impediva a Commerce di creare ordini per un ordine Amazon che non corrisponde a un prodotto catalogo Commerce.

![Problema noto](../assets/bug.svg) **Elenco Amazon duplicato**: <!--CHAN-3593-->Il problema fa sì che il catalogo crei un elemento per un elenco importato, utilizzando lo stesso SKU ma con un codice di area aggiunto alla fine. Amazon elabora quindi lo SKU modificato come nuovo elemento e crea un’inserzione. Questo problema verrà affrontato in una versione futura.

## v2.0.0

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

>[!NOTE]
>
>La versione 1.0.0 era disponibile solo in versione limitata.

![Nuovo](../assets/new.svg) **Onboarding e manutenzione semplificati**: aggiungi e integra con il tuo account Amazon Seller tramite un processo dettagliato con istruzioni dettagliate disponibili tramite l&#39;amministratore. Gestisci i tuoi negozi, gli account e i prodotti elencati tramite un unico dashboard.

![Nuovo](../assets/new.svg) **Supporto di più account**: gestisci e monitora più marchi Amazon e aree del marketplace tramite l&#39;amministratore.

![Nuovo](../assets/new.svg) **Intelligent Pricing**: imposta le regole di rideterminazione prezzi automatizzata per aumentare le probabilità per l&#39;ambito Buy Box. Impostare i prezzi per adeguarli in modo dinamico al prezzo Buy Box corrente o al prezzo concorrente più basso. Imposta i limiti per la revisione dei prezzi al fine di proteggere il tuo margine.

![Nuovo](../assets/new.svg) **Gestione delle inserzioni**: automatizza le inserzioni dei prodotti e sincronizza il catalogo Commerce con Amazon Marketplace utilizzando le regole per le inserzioni. Aggiungi sostituzioni specifiche per controllare in modo preciso le offerte. Controlla e gestisci tutte le tue inserzioni direttamente dall&#39;Amministratore.

![Nuovo](../assets/new.svg) **Inventory management coerente**: mantieni le quantità di inventario di Commerce e Amazon in sincronia costante.

![Nuovo](../assets/new.svg) **Gestione ordini ed evasione**: tieni traccia degli ordini di Amazon attraverso il dashboard, con comunicazioni e aggiornamenti dell&#39;inventario senza soluzione di continuità. Completa e tieni traccia delle spedizioni degli ordini evase da Amazon, evasa dal commerciante o con una combinazione di metodi.

![Problema noto](../assets/bug.svg) Potrebbero verificarsi tempi di attesa più lunghi per l&#39;aggiornamento delle quantità di prodotti. La sincronizzazione degli aggiornamenti per la quantità di prodotto potrebbe richiedere circa due ore.

![Problema noto](../assets/bug.svg) Gli ordini importati possono avere un tipo di _Prime_ o _Premium_ ordini. Devi verificare questi ordini nel tuo account Amazon Seller.

![Problema noto](../assets/bug.svg) I prodotti in bundle non idonei potrebbero essere visualizzati come idonei per l&#39;inserimento nell&#39;elenco in Amazon. Uno dei prodotti inclusi nel pacchetto potrebbe non essere idoneo. In caso di problemi, controlla lo stato di idoneità per gli articoli in bundle.

![Problema noto](../assets/bug.svg) Quando si utilizza Inventory management per Commerce 2.3.x, potrebbe non essere possibile attivare una reindicizzazione parziale delle azioni al momento della creazione di un ordine. La quantità vendibile viene ricalcolata ogni ora e ciò può causare la vendita eccessiva durante l&#39;intervallo di aggiornamento.
