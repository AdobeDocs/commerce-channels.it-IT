---
title: Collega le inserzioni a Walmart
description: '''Connetti inserzioni per [!DNL Commerce] prodotti a [!DNL Walmart Marketplace]per iniziare a vendere."'
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 0%

---

# Collega le inserzioni a Walmart

Come altri mercati, [!DNL Walmart] consente ai venditori di terze parti di elencare gli articoli venduti da altri.

- [!DNL Walmart Marketplace] utilizza identificatori di prodotto come UPC e GTIN per abbinare i prodotti a quelli esistenti [!DNL Walmart Marketplace] inserzioni.

- Per i prodotti corrispondenti, l&#39;elenco di Walmart Marketplace viene aggiornato in modo da includere [!DNL Commerce] offerta prodotto quando si collega un prodotto da [!DNL Channel Manager].

- Di solito, le offerte di prodotti con i prezzi più bassi appaiono per prime nel [!DNL Walmart Marketplace] ma anche altri fattori come le recensioni influenzano il posizionamento.

## Corrispondenza prodotti

Quando si abbinano i prodotti, Channel Manager invia i dati di prodotto a [!DNL Walmart Marketplace] per cercare le inserzioni esistenti con valori di attributo corrispondenti a quelli mappati [!DNL Commerce] attributo del prodotto. I criteri di corrispondenza sono determinati da [configurazione mapping attributi](map-catalog-attributes.md) per il canale del tuo negozio.

Se viene trovata una corrispondenza, l’elenco dei prodotti esistente viene aggiornato per aggiungere la tua offerta.

### Prerequisiti

Prima di associare i prodotti, verifica che i valori degli attributi del catalogo prodotti soddisfino i requisiti di Walmart e configura le impostazioni degli attributi dei prodotti. Consulta [Mappa attributi catalogo](map-catalog-attributes.md).

#### Seleziona e abbina prodotti

1. Apri un canale di vendita connesso.

1. Da **[!UICONTROL Listings]**, seleziona i prodotti da abbinare che si trovano in *[!UICONTROL Draft]* stato.

   ![Seleziona i prodotti dalle inserzioni e inviali per la corrispondenza](assets/products-in-marketplace-sales-channel.png)

1. Seleziona **[!UICONTROL Match Products]**.

   Un messaggio indica il numero di prodotti inviati per la corrispondenza.

   Lo stato dei prodotti selezionati cambia in [!UICONTROL *Elaborazione*] fino al completamento dell’operazione di corrispondenza. Il completamento dell&#39;operazione di abbinamento può richiedere fino a 30 minuti per Walmart Marketplace.

### Verifica stato corrispondenza

Al termine della corrispondenza, seleziona la **[!UICONTROL Refresh products]** per visualizzare lo stato corrente del prodotto. *Corrispondenza* o *Errore*.

- **[!UICONTROL Match]** indica che il prodotto ha restituito una corrispondenza. L&#39;offerta di prodotto è stata collegata a un&#39;inserzione esistente di Walmart Marketplace. Se il [L’archivio del marketplace non è attivo](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* viene visualizzato in *[!UICONTROL Status detail]* colonna. I prodotti in staging vengono collegati automaticamente quando [!DNL Walmart Marketplace] store è attivato.

- **[!UICONTROL Error]** indica che l&#39;operazione di corrispondenza non è riuscita a causa di uno dei problemi seguenti:

   - [!DNL Channel Manager] impossibile inviare per la corrispondenza a causa di un problema di connessione.

   - Nessuna corrispondenza trovata.

   - È stata trovata una corrispondenza, ma l’inserzione non può essere connessa perché [!DNL Walmart Marketplace] ha restituito un codice di errore. Consulta la **[!UICONTROL Error Description]** per informazioni sul problema.

### Controlla l&#39;inserzione su Walmart

Dopo aver confrontato i prodotti, rivedi l’elenco dei prodotti aggiornato e verifica i dettagli del prodotto, il prezzo e la quantità di magazzino dall’elenco [[!UICONTROL Walmart Marketplace Seller Account Items] dashboard](https://seller.walmart.com/items-and-inventory/manage-items) per rivedere il prodotto aggiornato.

### Risolvere i problemi relativi agli errori di corrispondenza prodotto

Se l’operazione di corrispondenza del prodotto non riesce e viene visualizzato un errore, il messaggio di errore viene visualizzato nel *[!UICONTROL Status detail]* colonna nella [!UICONTROL Channel Manager] elenco prodotti.

Gli errori comuni restituiti sono valori ID prodotto formattati in modo errato o attributi richiesti mancanti.

#### Correggi valori ID prodotto

| Tipo | Descrizione | Esempio |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, il numero a 12 cifre comprensivo di cifra di controllo. </br></br>Se l&#39;UPC è composto da meno di 12 cifre, ad esempio UPC-E, ovvero 8 cifre, aggiungere zeri finali per soddisfare il requisito. | Cambia da `45678912345` a `045678912345` |
| GTIN | GTIN-14, il numero a 14 cifre comprendente la cifra di controllo. </br></br>Se il numero di cifre del GTIN è inferiore a 14, aggiungere zeri iniziali </br>per soddisfare il requisito. | Cambia `456789123456` a `0045678912345` |
| EAN | GTIN-13, il numero a 13 cifre comprensivo di cifra di controllo. </br></br>Se il numero EAN è inferiore a 13 cifre, aggiungere interlinea </br>zero per soddisfare il requisito. | Cambia da `4567891234` a `0004567891234` |

Per informazioni dettagliate sui codici di errore di Walmart Marketplace, vedere [Aiuto per i venditori di Walmart](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Carica nuovi elenchi di prodotti

Per i prodotti che non hanno alcuna corrispondenza su Walmart Marketplace, utilizza un modello Excel della categoria di prodotti Walmart per caricare in blocco gli elenchi di prodotti. Popola il modello Walmart utilizzando i dati del catalogo dei prodotti esportati dal [!DNL Commerce] dell&#39;istanza.

Per i nuovi elenchi di prodotti, controlla il catalogo dei prodotti per assicurarti che i prodotti che intendi vendere su Walmart Marketplace dispongano degli attributi richiesti per gli elenchi di prodotti di Walmart Marketplace.

**Inserzioni Walmart Marketplace - Requisiti degli attributi**

| **Attributo** | **Livello del requisito** |
|--------------------------|-----------------------|
| SKU | Obbligatorio |
| Nome del prodotto | Obbligatorio |
| Tipo di ID prodotto | Obbligatorio |
| ID prodotto | Obbligatorio |
| Marchio | Obbligatorio |
| Breve descrizione | Obbligatorio |
| Prezzo di vendita | Obbligatorio |
| Descrizione del sito | Obbligatorio |
| URL immagine principale | Obbligatorio |
| Peso spedizione | Obbligatorio |
| Funzioni principali | Consigliato |
| Numero modello | Consigliato |
| Nome del produttore | Consigliato |
| Numero parte produttore | Consigliato |
| Dimensione | Consigliato |
| Colore | Consigliato |
| URL immagine principale | Facoltativo |
| URL immagine aggiuntivo | Facoltativo |
| Produttore | Facoltativo |

### Prerequisiti

- Verifica di soddisfare i requisiti [Requisiti di Walmart](walmart-requirements.md).

- Nel tuo [!DNL Commerce] catalogo prodotti, verificare che la configurazione del catalogo per i prodotti da elencare su Walmart Marketplace disponga di tutti gli attributi richiesti e soddisfi le linee guida per i contenuti di Walmart Marketplace.

- Verificare che il processo cron sia in esecuzione per completare l&#39;operazione di esportazione.

   - Per le istanze locali, consulta [Configurare ed eseguire cron](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - Ad Adobe, l’infrastruttura cloud, consulta [Imposta processi cron](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Creare il file di dati del prodotto da caricare

1. Dal tuo [Account del venditore Walmart](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), scarica un modello per l&#39;elenco dei prodotti dal Walmart Seller Center.

   - Dalla pagina Elementi del catalogo dei prodotti, seleziona **[!UICONTROL Add Items]**. Quindi, seleziona **[!UICONTROL Add items in bulk]**.

      ![Opzione Aggiungi elementi in blocco nella configurazione degli elementi di Walmart Marketplace](assets/walmart-seller-account-add-items-bulk.png)

   - Nella pagina di download, seleziona **[!UICONTROL Full Setup]**. Quindi, seleziona una categoria di elementi e scarica il modello di categoria.

      ![Opzione Scarica modello di categoria nella configurazione dell’elemento di Walmart Marketplace](assets/walmart-seller-account-full-setup-download.png)

   - Verifica che il modello includa gli attributi richiesti e consigliati per l’elenco dei prodotti.

1. Dalla sezione [!DNL Commerce] Amministratore, seleziona dall’Adobe i dati del prodotto da esportare [!DNL Commerce] sito.

   - Dall’amministratore, seleziona [!UICONTROL **Sistema** > Trasferimento dati > **Esporta**].

   - Il giorno [!UICONTROL Export] pagina in [!UICONTROL Entity Type] campo, seleziona [!UICONTROL **Prodotti**].

   - In [!UICONTROL Entity Attributes] , configura i criteri di selezione per l’esportazione dei dati del prodotto.
   ![Esporta la pagina dei dati del prodotto in [!UICONTROL [!DNL Commerce] Admin]](assets/walmart-seller-account-full-setup-download.png)

   Utilizza i filtri per selezionare e configurare i valori degli attributi applicabili alle categorie di prodotti venduti in. Assicurati di includere gli attributi richiesti e consigliati di Walmart. (vedere [Esporta dati](https://docs.magento.com/user-guide/system/data-export.html) nell’Adobe [!DNL Commerce] Guida utente per istruzioni dettagliate).

   Per omettere un attributo dall&#39;esportazione, selezionare [!UICONTROL **Escludi**] all’inizio della riga.

1. Scorrere fino alla fine della tabella degli attributi e selezionare [!UICONTROL **Continua**] per avviare l’esportazione dei dati.

   Il file di esportazione CSV viene elaborato tramite una coda di messaggi utilizzando i processi cron e salvato in `var/export/folder`. (vedere [Gestire le code dei messaggi](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) nel *Guida per gli sviluppatori di Commerce*.)

1. Aprire il modello di Excel per la categoria di prodotti Walmart Marketplace e utilizzare le funzionalità macro di Excel per unire i dati di prodotto esportati nel modello di Excel.

1. Carica il file Excel con i dati del prodotto esportato.

   - Torna alla pagina Elementi del catalogo prodotti in [Centro Vendite Walmart](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Seleziona [!UICONTROL **Aggiungi elementi** > **Aggiungi elementi in blocco**].
   - Trascina il foglio di calcolo completato nella sezione Carica.
   - Seleziona [!UICONTROL **Invia**].
   - Seleziona la [!UICONTROL  **Feed attività**] per visualizzare lo stato.

Per istruzioni complete, consulta [Aggiungi articoli in blocco utilizzando la specifica articolo completa](https://sellerhelp.walmart.com/s/guide?article=000007680) nel [!DNL *Aiuto per i venditori di Walmart*].
