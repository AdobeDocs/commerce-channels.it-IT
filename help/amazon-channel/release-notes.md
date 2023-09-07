---
title: '''[!DNL Amazon Sales Channel] note sulla versione'
description: Consulta le note sulla versione per informazioni su tutte [!DNL Amazon Sales Channel] versioni.
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2024'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] note sulla versione

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] può essere installato nelle istanze con Magento Open Source, Adobe Commerce e Adobe Commerce nelle versioni 2.3.x e 2.4.x dell’infrastruttura cloud. L’estensione non è più supportata in Adobe Commerce 2.1, Magento Open Source 2.2 o Magento 1.
> <br>Supporto disponibile per [!DNL Amazon sales channel]  versioni 4.0.0 e 4.1.0 solo sulle versioni Adobe Commerce 2.3.x.
> <br>[!DNL Amazon sales channel] la versione 4.2.0+ è compatibile con le versioni di Adobe Commerce 2.3.x, ma è disponibile il supporto solo per le versioni di Adobe Commerce 2.4.x.
>

Queste note sulla versione descrivono la versione iniziale di [!DNL Amazon sales channel] e includono:

![Nuovo](../assets/new.svg) Nuove funzioni
![Problema risolto](../assets/fix.svg) Correzioni e miglioramenti
![Problema noto](../assets/bug.svg) Problemi noti

Consulta [Prossime versioni](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) per controllo delle versioni, supporto e compatibilità.

Consulta [Disponibilità del prodotto](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) per scoprire quali versioni di Adobe Commerce supportano questa estensione.

## v4.5.0

*30 agosto 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) È stato aggiunto il gateway API Adobe.IO, che cambia da MAGI, per una maggiore sicurezza dell’autenticazione. `ServicesId` fornisce una nuova interfaccia utente per gestire le credenziali Adobe.IO, simile ad altre [Servizi Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html).

>[!NOTE]
>
>I commercianti devono garantire che [chiavi API pubbliche e private](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html) vengono aggiornati per la produzione.


![Problema risolto](../assets/fix.svg) È stato identificato un problema di impostazione della configurazione ed è stato risolto il flusso di creazione dell’ordine.

## v4.4.4

*7 marzo 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Problema risolto](../assets/fix.svg) È stato aggiunto il supporto per Adobe Commerce 2.4.6 e PHP 8.2.

![Problema risolto](../assets/fix.svg) Riduzione del rumore nei registri.

![Problema risolto](../assets/fix.svg) È stata migliorata la stabilità del richiamo degli aggiornamenti.

![Problema risolto](../assets/fix.svg) Semplificazione del processo di esecuzione di pull single action-like o per l&#39;applicazione da CLI.

![Problema risolto](../assets/fix.svg) È stata aggiornata la dipendenza per `magento/services-connector`.

![Problema risolto](../assets/fix.svg) Sono stati risolti dei problemi di sincronizzazione negli account del Regno Unito con codice paese non valido.

![Problema risolto](../assets/fix.svg) Se l’elemento entity_type_id per l’entità prodotto del catalogo è codificato in modo non corretto, si verificano problemi con l’Origine prezzo Magento.

![Problema risolto](../assets/fix.svg) È stato risolto un problema che impediva agli account eliminati in un backend da un’altra istanza di essere eliminati anche dall’interfaccia utente.

![Problema risolto](../assets/fix.svg) È stato risolto un problema a causa del quale alcune regole del carrello interrompevano l’importazione degli ordini.

## v4.4.3

*7 marzo 2023*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) È stato aggiunto il supporto per Adobe Commerce 2.4.4.

## v4.4.2

*11 novembre 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) Sono state aggiornate le dipendenze per supportare altre estensioni aggiornate.
![Correzione](../assets/fix.svg) È stato aggiunto il supporto per PHP 8.1.

## v4.4.1

*11 novembre 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) È stato modificato il modo in cui Adobe Commerce riceve _Nome utente_ da Amazon. In precedenza, si verificava un errore durante la creazione dell’ordine quando _Nome utente_ il campo conteneva caratteri speciali. Adobe Commerce ora riceve il _Nome utente_ e filtra i caratteri speciali in modo che l’ordine possa essere creato correttamente.

## v4.4.0

*9 aprile 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) Alla configurazione è stato aggiunto il supporto per la modalità di sola lettura. Consulta [impostazioni del canale di vendita](sales-channel-settings.md).

![Correzione](../assets/fix.svg) È stato modificato il flusso di dati in modo che più copie della stessa istanza possano recuperare gli aggiornamenti contemporaneamente.

![Correzione](../assets/fix.svg) È stato modificato il processo di sincronizzazione per la sincronizzazione delle informazioni sull&#39;account. È stato aggiunto un processo cron da sincronizzare con l’account remoto e la stessa funzionalità è stata aggiunta ai comandi CLI.

![Correzione](../assets/fix.svg) Sono stati aggiunti argomenti e flag del comando CLI per un controllo più preciso.

![Correzione](../assets/fix.svg) È stata corretta l’origine delle attività in background (cron) nella configurazione del sistema.

![Correzione](../assets/fix.svg) È stato corretto il problema che impediva la creazione di ordini quando il prefisso del paese era impostato su Porto Rico (PR).

## v4.3.0

*3 marzo 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) <!--CHAN-xxxx-->Il _Dettagli ordine_ è stata riprogettata e non si basa più sul _Ordini di importazione_ impostazione. I dettagli dell’ordine vengono ora visualizzati nell’interfaccia di Sales Channel di Amazon per tutti gli ordini.

![Correzione](../assets/fix.svg) In _[!UICONTROL Marketing]_in Admin, il nome è stato modificato da_[!UICONTROL Amazon]_ a _[!UICONTROL Amazon Sales Channel]_.

![Problema noto](../assets/bug.svg) **Importante**: i problemi noti relativi alla compatibilità con Adobe Commerce 2.4.0 sono stati risolti con Adobe Commerce 2.4.1.

- Processi Amazon cron in `error` stato
- L’installazione con Commerce 2.4.0 non riesce quando si creano archivi nel database
- La creazione del prodotto non riesce quando è installato MSI

## v4.2.0

*3 marzo 2021*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

Se hai un precedente [!DNL Amazon sales channel] versione installata e tentare di aggiornare Adobe Commerce alla versione 2.4.0, viene richiesto di aggiornare l’estensione prima di poter completare l’aggiornamento di Adobe Commerce.

![Problema noto](../assets/bug.svg) Quando [!DNL Amazon sales channel] 4.2.0 è integrato con la versione 2.4.0 e [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) è abilitato, esiste un problema noto che impedisce l’aggiunta di prodotti nel catalogo Commerce. Questo problema verrà affrontato in una futura versione di Commerce.

![Nuovo](../assets/new.svg) [!DNL Amazon sales channel] è stato migliorato per accettare dati di indirizzi basati su testo e confrontarli con formati di indirizzi standardizzati, tra cui città, stato e codice postale. Questo aggiornamento consente ai dati di ordine e spedizione di sincronizzarsi (sincronizzarsi) con Amazon senza errori di indirizzo.<br/>Ad esempio, un acquirente inserisce città, stato, codice postale come `Escondido, californiA 92025-1501`. Il Sales Channel Amazon importa e abbina i dati al formato standard come `Escondido, CA 92025`, quindi lo sincronizza nuovamente con Amazon in questo formato standardizzato.

![Nuovo](../assets/new.svg) È stato aggiunto il supporto per PHP 7.4.

![Nuovo](../assets/new.svg) <!--CHAN-4334-->È stato aggiunto il supporto per Adobe Commerce 2.4.x. Le versioni precedenti possono essere compatibili con Commerce 2.4.x, ma non sono supportate. Consulta [Versioni future](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) per la compatibilità delle versioni. Per completare l’aggiornamento di Amazon 2.4.0, è necessario aggiornare il Sales Channel Adobe Commerce alla versione 4.2.0.

![Correzione](../assets/fix.svg) <!--CHAN-4431-->È stato risolto un problema che causava un errore in un _Accesso negato_ per i clienti britannici.

![Correzione](../assets/fix.svg) <!--CHAN-4394-->È stato risolto un problema che impediva la sincronizzazione dello stato di spedizione di Amazon con l’ordine Commerce corrispondente, bloccando così lo stato di spedizione dell’ordine come `Pending` in Commerce e `Unshipped` in Amazon. Con la nuova funzione di indirizzo standardizzato, questi errori di stato di spedizione sono stati risolti.

![Correzione](../assets/fix.svg) <!--ticket#-->È stata aggiornata la sincronizzazione degli ordini (sync) per ignorare le importazioni degli ordini non riuscite, riducendo in tal modo più tentativi di sincronizzazione e consentendo l’elaborazione delle importazioni successive, con richieste di sincronizzazione degli ordini inviate ogni cinque minuti. Gli errori di sincronizzazione vengono comunque registrati nel registro degli errori, ma contrassegnati come &quot;elaborati&quot; per consentire ulteriori funzioni di registrazione. Inoltre, [!DNL Amazon sales channel] ora rimuove automaticamente i dati in eccesso raccolti per gli ordini che non vengono creati in Commerce.

![Correzione](../assets/fix.svg) È stata aggiornata la registrazione degli errori per raccogliere ulteriori informazioni sugli errori non rilevati relativi all’eccezione e all’aggiornamento dell’estensione.

![Correzione](../assets/fix.svg) <!--ticket#-->È stato risolto un problema che causava la sincronizzazione iniziale di _prezzo più basso_ dati non riusciti a causa di un errore _prezzo_ valore.

![Correzione](../assets/fix.svg) <!--CHAN-4410-->Sono stati risolti i problemi che causavano errori di filtro in _Ordini Amazon_ visualizza quando il campo intervallo di date viene lasciato vuoto.

![Correzione](../assets/fix.svg) <!--CHAN-4439-->È stato risolto un problema che causava errori di sincronizzazione di scorte e evasioni relativi alla quantità. L’estensione ora arrotonda verso il basso i valori della quantità immessi come decimali prima di sincronizzarli con Amazon.<br/> Ad esempio, quando un commerciante inserisce manualmente una quantità di `2.5`, l’estensione arrotonda il valore per difetto a `2` e quindi sincronizza la quantità aggiornata con Amazon.

## v4.1.0

*7 maggio 2020*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) <!--4247, 4230-->Il processo di importazione degli ordini è stato modificato per allinearlo ai requisiti degli ordini Commerce. Queste modifiche correggono i problemi che impedivano a Commerce di creare l’ordine corrispondente per un ordine importato. Consulta [Gestisci ordini](managing-orders.md) per informazioni su blocchi degli ordini e soluzioni.

![Nuovo](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->È stato aggiornato il _Ordini recenti_ sezione del dashboard dello store e ha aggiunto una nuova _Tutti gli ordini_ visualizzazione che mostra tutti gli ordini di Amazon, incluse le opzioni di filtro e la paginazione per visualizzare più ordini. Consulta [Dashboard di Amazon Store](amazon-store-dashboard.md) e [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) È stata aggiunta la _[!UICONTROL Order Notes]_colonna del riprogettato_[!UICONTROL Amazon Orders]_ tabella in entrambi _[!UICONTROL Recent Orders]_e_[!UICONTROL All Orders]_ visualizzazioni. _[!UICONTROL Order Notes]_comunicare al commerciante che esiste un problema con l&#39;importazione dell&#39;ordine. Consulta [Visualizza ordini Amazon](amazon-orders-all.md).

![Nuovo](../assets/new.svg) <!--CHAN-4013-->Sono stati aggiornati i parametri delle condizioni del prodotto per allinearli al [Amazon rinnovato](https://sell.amazon.com/programs/renewed) programma. Consulta [Prodotti rinnovati](renewed-products.md).

![Nuovo](../assets/new.svg) <!--CHAN-3680-->Aggiornato [Dettagli ordine Amazon](amazon-order-details.md) per includere &quot;dati generici&quot; per gli ordini evasi da Amazon. Consulta [Soddisfatto da](fulfilled-by.md).

![Correzione](../assets/fix.svg) <!--CHAN-4069-->È stato risolto un problema che causava la distorsione delle icone sulla scheda dello store.

![Correzione](../assets/fix.svg) <!--CHAN-4165-->È stato corretto un errore che impediva il corretto funzionamento di _Login_ schermo non venga visualizzato dopo il timeout della sessione.

![Correzione](../assets/fix.svg) <!--CHAN-4211-->È stato risolto un problema che impediva l’importazione dell’importo dell’imposta sugli ordini di Amazon nel nuovo ordine di Commerce.

![Correzione](../assets/fix.svg) <!--CHAN-4234-->È stato corretto un problema a causa del quale i totali dei ricavi visualizzati nel dashboard del negozio includevano gli ordini in `Canceled` o `Error` stato.

![Correzione](../assets/fix.svg) <!--CHAN-4326-->È stato risolto un problema che causava errori di importazione degli ordini associati alle estensioni di terze parti che utilizzavano _Magento Shipping_ metodi per creare gli ordini.

![Correzione](../assets/fix.svg) <!--CHAN-4357-->È stato risolto un problema che causava errori durante l’esecuzione della sincronizzazione cron. È stato aggiunto un blocco al comando CLI che impedisce la sincronizzazione simultanea di due processi cron.

![Correzione](../assets/fix.svg) Criteri di sicurezza dei contenuti aggiornati per il supporto con Commerce versione 2.3.5.

## v4.0.0

*25 marzo 2020*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 non è supportato per Adobe Commerce 2.3.5. Per il supporto con Adobe Commerce 2.3.5, effettua l’aggiornamento ad Amazon Sales Channel 4.1.0.

![Nuovo](../assets/new.svg) Presentato un nuovo [Sales Channel Amazon](amazon-sales-channel-home.md) home page con la visualizzazione migliorata delle schede per le informazioni del tuo negozio.

![Nuovo](../assets/new.svg) Presentato un nuovo [dashboard store](amazon-store-dashboard.md) con informazioni sull&#39;elenco, sugli ordini recenti e sulle impostazioni del punto vendita.

![Nuovo](../assets/new.svg) Introduzione di una soluzione più semplice e [processo di onboarding](amazon-onboarding-home.md) e [impostazioni store predefinite](default-store-settings.md) per integrare più rapidamente i punti vendita.

![Problema noto](../assets/bug.svg) <!--CHAN-4102--> Quando [creazione di attributi](managing-attributes.md) per importare immagini dalle inserzioni e **Visualizzazioni store** è impostato su `All Store Views (Global)`, esiste un problema noto che impedisce l’importazione delle immagini in tutte le visualizzazioni dello store. Se si modifica l&#39;impostazione per **Visualizzazioni store (per importare valori in)** in un archivio specifico, le immagini vengono importate per tale archivio.

## v3.0.1

*11 novembre 2019*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Correzione](../assets/fix.svg) **Impostazioni campo numerico**: <!--CHAN-3779-->I campi che richiedono un valore numerico sono stati aggiornati per accettare solo caratteri numerici. Esempio: Impostazioni regola determinazione prezzi > campo Importo adeguamento

![Correzione](../assets/fix.svg) **Collegamenti alla guida utente**: <!--CHAN-3778-->Errato _Guida utente_ i collegamenti sono stati corretti.

![Correzione](../assets/fix.svg) **Elenchi Amazon duplicati**: <!--CHAN-3593-->Ora viene risolto un problema segnalato in precedenza che causava la duplicazione degli elenchi di Amazon. Prima di questa versione, l’estensione aggiungeva il codice paese per l’area geografica Amazon ai valori SKU durante l’importazione delle inserzioni. L’inserzione corrisponde all’elemento del catalogo, ma l’estensione ha creato una nuova inserzione duplicata con lo SKU aggiunto. Con questa versione, l’estensione non modifica lo SKU per le inserzioni importate e non viene apportata alcuna modifica alle inserzioni esistenti. È possibile utilizzare [!UICONTROL End Listing(s)] su Amazon per rimuovere le inserzioni duplicate.

## v3.0.0

*7 ottobre 2019*

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

![Nuovo](../assets/new.svg) **Amazon UK Marketplace ora disponibile**: gli utenti possono scegliere il marketplace del Regno Unito durante la creazione e l’integrazione di un Commerce store. Questo aggiornamento per il Regno Unito include supporto aggiuntivo per:

- [Servizio di calcolo IVA Amazon](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Codice imposta prodotto](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} informazioni.

![Nuovo](../assets/new.svg) **Registrazione migliorata**: <!--CHAN-3642, 3672-->Implementazione di **Abilita registrazione debug** per raccogliere dati di sincronizzazione aggiuntivi quando è necessaria la risoluzione dei problemi. Consulta la [Impostazioni Sales Channel](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) nella Guida di riferimento della configurazione.

![Correzione](../assets/fix.svg) **Catalogo prodotti**: <!--CHAN-3687-->È stato risolto un problema che impediva l’applicazione delle immagini importate con un elenco Amazon al corrispondente prodotto del catalogo Commerce.

![Correzione](../assets/fix.svg) **Creazione ordine**: <!--CHAN-3708-->È stato risolto un problema che impediva a Commerce di creare ordini per un ordine Amazon che non corrispondeva a un prodotto del catalogo Commerce.

![Problema noto](../assets/bug.svg) **Elenchi Amazon duplicati**: <!--CHAN-3593-->Questo problema fa sì che il catalogo crei un elemento per un’inserzione importata, utilizzando lo stesso SKU ma con un codice regionale aggiunto alla fine. Amazon elabora quindi lo SKU modificato come nuovo elemento e crea un’inserzione. Questo problema verrà affrontato in una versione futura.

## v2.0.0

[!BADGE Supportato]{type=Informative tooltip="Supportato"}

>[!NOTE]
>
>La versione 1.0.0 era disponibile solo in versione limitata.

![Nuovo](../assets/new.svg)  **Onboarding e manutenzione semplificati**: aggiungi e integra con il tuo account Amazon Seller tramite una procedura dettagliata con istruzioni dettagliate disponibili tramite l’Amministratore. Gestisci i tuoi negozi, gli account e i prodotti elencati tramite un unico dashboard.

![Nuovo](../assets/new.svg)  **Supporto di più account**: gestisci e monitora più marchi Amazon e aree del marketplace tramite l’amministratore.

![Nuovo](../assets/new.svg)  **Prezzi intelligenti**: imposta le regole di rideterminazione prezzi automatizzata per aumentare le opportunità per l’ambito Buy Box. Impostare i prezzi per adeguarli in modo dinamico al prezzo Buy Box corrente o al prezzo concorrente più basso. Imposta i limiti per la revisione dei prezzi al fine di proteggere il tuo margine.

![Nuovo](../assets/new.svg)  **Gestione elenchi**: automatizza gli elenchi dei prodotti e sincronizza il catalogo Commerce con Amazon Marketplace utilizzando le regole per gli elenchi. Aggiungi sostituzioni specifiche per controllare in modo preciso le offerte. Controlla e gestisci tutte le tue inserzioni direttamente dall&#39;Amministratore.

![Nuovo](../assets/new.svg)  **Inventory management coerente**: mantieni le quantità di magazzino di Commerce e Amazon in sincronizzazione costante.

![Nuovo](../assets/new.svg)  **Gestione ordini e evasione**: tieni traccia degli ordini di Amazon attraverso il dashboard, con comunicazioni e aggiornamenti dell’inventario senza soluzione di continuità. Completa e tieni traccia delle spedizioni degli ordini evase da Amazon, evasa dal commerciante o con una combinazione di metodi.

![Problema noto](../assets/bug.svg)  Potrebbero verificarsi tempi di attesa più lunghi per aggiornare le quantità di prodotto. La sincronizzazione degli aggiornamenti per la quantità di prodotto potrebbe richiedere circa due ore.

![Problema noto](../assets/bug.svg)  Gli ordini importati possono avere un tipo di _Prime_ o _Premium_ ordini. Devi verificare questi ordini nel tuo account Amazon Seller.

![Problema noto](../assets/bug.svg)  I prodotti in bundle non ammissibili possono essere visualizzati come idonei per l’inserimento nell’elenco su Amazon. Uno dei prodotti inclusi nel pacchetto potrebbe non essere idoneo. In caso di problemi, controlla lo stato di idoneità per gli articoli in bundle.

![Problema noto](../assets/bug.svg)  Quando si utilizza Inventory management for Commerce 2.3.x, potrebbe non essere possibile attivare una reindicizzazione parziale delle azioni al momento della creazione di un ordine. La quantità vendibile viene ricalcolata ogni ora e ciò può causare la vendita eccessiva durante l&#39;intervallo di aggiornamento.
