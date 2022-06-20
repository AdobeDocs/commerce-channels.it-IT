---
title: Collegare gli annunci a Walmart
description: Collegare gli elenchi dei prodotti Commerce a [!DNL Walmart Marketplace]per iniziare a vendere.
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 418bb6a91817f49f3c3ae39a8d26370bfeb39099
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Collegare gli annunci a Walmart

Come altri mercati, [!DNL Walmart] consente ai venditori di terze parti di elencare gli articoli venduti da altri.

- [!DNL Walmart Marketplace] utilizza identificatori di prodotto come UPC e GTIN per abbinare i prodotti a quelli esistenti [!DNL Walmart Marketplace] elenchi.

- Per i prodotti associati, l’elenco di Walmart Marketplace viene aggiornato per includere l’offerta di prodotto Commerce quando si collega un prodotto da [!DNL Channel Manager].

- Di solito, le offerte di prodotti con i prezzi più bassi compaiono per prime nel [!DNL Walmart Marketplace] l&#39;inserimento nell&#39;elenco, ma anche altri fattori come le revisioni influiscono sul posizionamento.

## Prodotti abbinati

Quando abbini prodotti, Channel Manager invia i dati del prodotto a [!DNL Walmart Marketplace] per cercare elenchi esistenti con valori di attributo corrispondenti all’attributo di prodotto Commerce mappato. I criteri di corrispondenza sono determinati dal [configurazione di mappatura degli attributi](map-catalog-attributes.md) per il tuo canale store.

Se viene trovata una corrispondenza, l’elenco dei prodotti esistenti viene aggiornato per aggiungere la tua offerta.

### Prerequisiti

Prima di eseguire la corrispondenza con i prodotti, verifica che i valori degli attributi del catalogo dei prodotti soddisfino i requisiti di Walmart e configura le impostazioni degli attributi dei prodotti. Vedi [Mappare gli attributi del catalogo](map-catalog-attributes.md).

#### Selezionare e abbinare i prodotti

1. Apri un canale di vendita collegato.

1. Da **[!UICONTROL Listings]**, seleziona i prodotti per la corrispondenza in *[!UICONTROL Draft]* stato.

   ![Seleziona i prodotti da inserzioni e invia per la corrispondenza](assets/products-in-marketplace-sales-channel.png)

1. Seleziona **[!UICONTROL Match Products]**.

   Un messaggio indica il numero di prodotti inviati per la corrispondenza.

   ![Inviare prodotti al canale di vendita collegato](assets/products-submitted-for-matching.png)

   Lo stato dei prodotti selezionati viene modificato in [!UICONTROL *Elaborazione*] fino al completamento dell’operazione di abbinamento. Per completare l&#39;operazione di match, Walmart Marketplace può richiedere fino a 30 minuti.

### Verifica lo stato di corrispondenza

Al termine della corrispondenza, seleziona il **[!UICONTROL Refresh products]** per visualizzare lo stato corrente del prodotto. *Corrispondenza* o *Errore*.

- **[!UICONTROL Match]** indica che la corrispondenza del prodotto è stata completata. L&#39;offerta di prodotto è stata connessa a un elenco esistente di Walmart Marketplace. Se la [L&#39;archivio Marketplace non è attivo](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* viene visualizzato in *[!UICONTROL Status detail]* colonna. I prodotti di staging vengono collegati automaticamente quando il [!DNL Walmart Marketplace] archivio attivato.

- **[!UICONTROL Error]** indica che l’operazione di corrispondenza non è riuscita a causa di uno dei seguenti problemi:

   - [!DNL Channel Manager] impossibile inviare per la corrispondenza a causa di un problema di connessione.

   - Non è stata trovata alcuna corrispondenza.

   - Trovata corrispondenza, ma l’elenco non può essere collegato perché [!DNL Walmart Marketplace] ha restituito un codice di errore. Consulta la sezione **[!UICONTROL Error Description]** per informazioni sul problema.

### Controlla l&#39;elenco su Walmart

Dopo aver eseguito la corrispondenza dei prodotti, rivedi l’elenco dei prodotti aggiornato e verifica i dettagli dei prodotti, il prezzo e la quantità di scorte dalla [[!UICONTROL Walmart Marketplace Seller Account Items] dashboard](https://seller.walmart.com/items-and-inventory/manage-items) per rivedere il prodotto aggiornato.

### Risolvere i problemi relativi agli errori di corrispondenza del prodotto

Se l’operazione di corrispondenza del prodotto non riesce e viene visualizzato un errore, nel *[!UICONTROL Status detail]* nella colonna [!UICONTROL Channel Manager] elenco dei prodotti.

Gli errori comuni restituiti sono valori ID prodotto formattati in modo non corretto o attributi richiesti mancanti.

#### Correggere i valori ID prodotto

| Tipo | Descrizione | Esempio |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, il numero a 12 cifre, compresa la cifra di controllo. </br></br>Se l&#39;UPC ha meno di 12 cifre, ad esempio UPC-E a 8 cifre, aggiungere zeri finali per soddisfare il requisito. | Cambia da `45678912345` a `045678912345` |
| GTIN | GTIN-14, il numero a 14 cifre, compresa la cifra di controllo. </br></br>Se il valore GTIN è inferiore a 14 cifre, aggiungere zeri iniziali </br>per soddisfare il requisito. | Modifica `456789123456` a `0045678912345` |
| EAN | GTIN-13, il numero a 13 cifre, compresa la cifra di controllo. </br></br>Se l&#39;EAN ha meno di 13 cifre, aggiungi l&#39;interlinea </br>zero per soddisfare il requisito. | Cambia da `4567891234` a `0004567891234` |

Per informazioni dettagliate sui codici di errore di Walmart Marketplace, consulta la sezione [Aiuto per i venditori di Walmart](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Carica nuovi elenchi di prodotti

Per i prodotti che non hanno corrispondenza su Walmart Marketplace, utilizza un modello Excel di categoria di prodotti Walmart per caricare in massa gli elenchi di prodotti. Compilare il modello Walmart utilizzando i dati del catalogo di prodotto esportati dalla tua istanza Commerce.

Per i nuovi elenchi di prodotti, controlla il catalogo dei prodotti per assicurarsi che i prodotti che intendi vendere su Walmart Marketplace abbiano gli attributi necessari per gli elenchi di prodotti di Walmart Marketplace.

**Elenchi di Marketplace Walmart-Requisiti degli attributi**

| **Attributo** | **Livello del requisito** |
|--------------------------|-----------------------|
| SKU | Obbligatorio |
| Nome del prodotto | Obbligatorio |
| Tipo di ID prodotto | Obbligatorio |
| ID prodotto | Obbligatorio |
| Brand | Obbligatorio |
| Breve descrizione | Obbligatorio |
| Prezzo di vendita | Obbligatorio |
| Descrizione del sito | Obbligatorio |
| URL immagine principale | Obbligatorio |
| Peso della spedizione | Obbligatorio |
| Funzioni principali | Consigliato |
| Numero del modello | Consigliato |
| Nome del produttore | Consigliato |
| Numero parte costruttore | Consigliato |
| Dimensione | Consigliato |
| Colore | Consigliato |
| URL immagine principale | Facoltativo |
| URL immagine aggiuntivo | Facoltativo |
| Produttore | Facoltativo |

### Prerequisiti

- Verifica che la [Requisiti di Walmart](walmart-requirements.md).

- Nel catalogo del prodotto Commerce, verifica che la configurazione del catalogo per i prodotti da elencare su Walmart Marketplace abbia tutti gli attributi richiesti e soddisfi le linee guida per i contenuti di Walmart Marketplace.

- Verifica che il processo cron sia in esecuzione per completare l&#39;operazione di esportazione.

   - Per le istanze locali, vedi [Configurare ed eseguire cron](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - Ad Adobe, l’infrastruttura cloud, vedi [Imposta lavori cron](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Crea il file di dati prodotto da caricare

1. Dal tuo [Account venditore Walmart](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), scarica un modello di elenco dei prodotti dal Centro Venditori Walmart.

   - Dalla pagina Elementi catalogo prodotti , seleziona **[!UICONTROL Add Items]**. Quindi, seleziona **[!UICONTROL Add items in bulk]**.

      ![Aggiunta di elementi in modalità collettiva nella configurazione di elementi di Walmart Marketplace](assets/walmart-seller-account-add-items-bulk.png)

   - Nella pagina di download, seleziona **[!UICONTROL Full Setup]**. Quindi, seleziona una categoria di articoli e scarica il modello di categoria.

      ![Opzione Scarica modello di categoria nella configurazione di elementi di Walmart Marketplace](assets/walmart-seller-account-full-setup-download.png)

   - Verifica che il modello includa gli attributi richiesti e consigliati per l’elenco dei prodotti.

1. Da [!DNL Commerce] Amministratore, seleziona i dati di prodotto da esportare dal tuo sito Adobe Commerce.

   - Dall’amministratore, seleziona [!UICONTROL **Sistema** > Trasferimento dati > **Esporta**].

   - Sulla [!UICONTROL Export] nella pagina [!UICONTROL Entity Type] campo , seleziona [!UICONTROL **Prodotti**].

   - In [!UICONTROL Entity Attributes] configura i criteri di selezione per l’esportazione dei dati di prodotto.
   ![Esporta la pagina dei dati di prodotto in [!UICONTROL Commerce Admin]](assets/walmart-seller-account-full-setup-download.png)

   Utilizza i filtri per selezionare e configurare i valori degli attributi applicabili alle categorie di prodotti che vendi. Accertati di includere gli attributi richiesti e consigliati di Walmart (consulta [Esporta dati](https://docs.magento.com/user-guide/system/data-export.html) nella Guida utente di Adobe Commerce per istruzioni dettagliate.)

   Per omettere un attributo dall’esportazione, seleziona la [!UICONTROL **Escludi**] all’inizio della riga.

1. Scorri fino alla fine della tabella degli attributi e seleziona [!UICONTROL **Continua**] per avviare l’esportazione dei dati.

   Il file di esportazione CSV viene elaborato tramite una coda di messaggi utilizzando i lavori cron e salvato nel `var/export/folder`. (Vedi [Gestire le code dei messaggi](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) in *Guida per gli sviluppatori di Commerce*.)

1. Aprire il modello Excel per la categoria di prodotto Walmart Marketplace e utilizzare le funzionalità macro di Excel per unire i dati di prodotto esportati nel modello Excel.

1. Carica il file Excel con i dati di prodotto esportati.

   - Torna alla pagina Elementi catalogo prodotti nella [Centro Venditori Walmart](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Seleziona [!UICONTROL **Aggiungi elementi** > **Aggiungi elementi in blocco**].
   - Trascina il foglio di calcolo completato nella sezione Carica .
   - Seleziona [!UICONTROL **Invia**].
   - Seleziona la [!UICONTROL  **Feed attività**] per visualizzare lo stato di avanzamento.

Per istruzioni complete, consulta [Aggiungi elementi in blocco utilizzando la specifica completa dell&#39;elemento](https://sellerhelp.walmart.com/s/guide?article=000007680) in [!DNL *Aiuto per i venditori di Walmart*].
