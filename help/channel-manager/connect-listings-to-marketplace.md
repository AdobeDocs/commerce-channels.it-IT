---
title: Collega le inserzioni a Walmart
description: 'Connetti le inserzioni per  [!DNL Commerce] prodotti a [!DNL Walmart Marketplace]per iniziare a vendere.'
feature: Sales Channels, Integration, Products, Tools and External Services
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# Collega le inserzioni a Walmart

Come altri mercati, [!DNL Walmart] consente ai venditori di terze parti di elencare gli articoli venduti da altri.

- [!DNL Walmart Marketplace] utilizza identificatori di prodotto come UPC e GTIN per far corrispondere i prodotti alle inserzioni di [!DNL Walmart Marketplace] esistenti.

- Per i prodotti corrispondenti, l&#39;elenco di Walmart Marketplace viene aggiornato in modo da includere l&#39;offerta di prodotto [!DNL Commerce] quando si connette un prodotto da [!DNL Channel Manager].

- Di solito, le offerte di prodotti con i prezzi più bassi compaiono prima nell&#39;elenco [!DNL Walmart Marketplace], ma anche altri fattori come le recensioni influiscono sul posizionamento.

## Corrispondenza prodotti

Quando si confrontano i prodotti, Channel Manager invia i dati del prodotto a [!DNL Walmart Marketplace] per cercare le inserzioni esistenti con valori di attributo corrispondenti all&#39;attributo di prodotto [!DNL Commerce] mappato. I criteri di corrispondenza sono determinati dalla [configurazione di mappatura degli attributi](map-catalog-attributes.md) per il canale dell&#39;archivio.

Se viene trovata una corrispondenza, l’elenco dei prodotti esistente viene aggiornato per aggiungere la tua offerta.

### Prerequisiti

Prima di associare i prodotti, verifica che i valori degli attributi del catalogo prodotti soddisfino i requisiti di Walmart e configura le impostazioni degli attributi dei prodotti. Vedi [Mappa attributi catalogo](map-catalog-attributes.md).

#### Seleziona e abbina prodotti

1. Apri un canale di vendita connesso.

1. Da **[!UICONTROL Listings]**, selezionare i prodotti per la corrispondenza che sono nello stato *[!UICONTROL Draft]*.

   ![Seleziona i prodotti dalle inserzioni e inviali per la corrispondenza](assets/products-in-marketplace-sales-channel.png){width="500" zoomable="yes"}

1. Selezionare **[!UICONTROL Match Products]**.

   Un messaggio indica il numero di prodotti inviati per la corrispondenza.

   Lo stato dei prodotti selezionati diventa [!UICONTROL *Elaborazione*] fino al completamento dell&#39;operazione di corrispondenza. Il completamento dell&#39;operazione di abbinamento può richiedere fino a 30 minuti per Walmart Marketplace.

### Verifica stato corrispondenza

Al termine della corrispondenza, selezionare **[!UICONTROL Refresh products]** per visualizzare lo stato corrente del prodotto. *Corrispondenza* o *Errore*.

- **[!UICONTROL Match]** indica che il prodotto è stato trovato correttamente. L&#39;offerta di prodotto è stata collegata a un&#39;inserzione esistente di Walmart Marketplace. Se l&#39;archivio [Marketplace non è attivo](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* verrà visualizzato nella colonna *[!UICONTROL Status detail]*. I prodotti in staging vengono connessi automaticamente all&#39;attivazione dell&#39;archivio [!DNL Walmart Marketplace].

- **[!UICONTROL Error]** indica che l&#39;operazione di corrispondenza non è riuscita a causa di uno dei seguenti problemi:

   - [!DNL Channel Manager] non è stato in grado di inviare per la corrispondenza a causa di un problema di connessione.

   - Nessuna corrispondenza trovata.

   - Trovata corrispondenza, ma non è possibile connettere l&#39;inserzione perché [!DNL Walmart Marketplace] ha restituito un codice di errore. Per informazioni sul problema, vedere **[!UICONTROL Error Description]**.

### Controlla l&#39;inserzione su Walmart

Dopo aver individuato i prodotti corrispondenti, esaminare l&#39;elenco dei prodotti aggiornato e verificare i dettagli, il prezzo e la quantità di magazzino dal dashboard [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) per esaminare il prodotto aggiornato.

### Risolvere i problemi relativi agli errori di corrispondenza prodotto

Se l&#39;operazione di corrispondenza prodotto non riesce e viene restituito un errore, il messaggio di errore viene visualizzato nella colonna *[!UICONTROL Status detail]* dell&#39;elenco dei prodotti [!UICONTROL Channel Manager].

Gli errori comuni restituiti sono valori ID prodotto formattati in modo errato o attributi richiesti mancanti.

#### Correggi valori ID prodotto

| Tipo | Descrizione | Esempio |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, il numero a 12 cifre comprensivo di cifra di controllo. </br></br>Se l&#39;UPC è composto da meno di 12 cifre, ad esempio UPC-E, ovvero 8 cifre, aggiungere degli zeri finali per soddisfare il requisito. | Cambia da `45678912345` a `045678912345` |
| GTIN | GTIN-14, il numero a 14 cifre comprendente la cifra di controllo. </br></br>Se il numero di cifre del GTIN è inferiore a 14, aggiungere gli zeri iniziali </br> per soddisfare il requisito. | Cambia `456789123456` in `0045678912345` |
| EAN | GTIN-13, il numero a 13 cifre comprensivo di cifra di controllo. </br></br>Se il numero EAN è inferiore a 13 cifre, aggiungere </br>zeri iniziali per soddisfare il requisito. | Cambia da `4567891234` a `0004567891234` |

Per informazioni dettagliate sui codici di errore di Walmart Marketplace, consultare la [Guida del venditore di Walmart](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Carica nuovi elenchi di prodotti

Per i prodotti che non hanno alcuna corrispondenza su Walmart Marketplace, utilizza un modello Excel della categoria di prodotti Walmart per caricare in blocco gli elenchi di prodotti. Compilare il modello Walmart utilizzando i dati del catalogo prodotti esportati dall&#39;istanza [!DNL Commerce].

Per i nuovi elenchi di prodotti, controlla il catalogo dei prodotti per assicurarti che i prodotti che intendi vendere su Walmart Marketplace dispongano degli attributi richiesti per gli elenchi di prodotti di Walmart Marketplace.

**Inserzioni su Walmart Marketplace - Requisiti degli attributi**

| **Attributo** | **Livello di fabbisogno** |
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

- Verifica di soddisfare i [requisiti di Walmart](walmart-requirements.md).

- Nel catalogo prodotti [!DNL Commerce], verificare che la configurazione del catalogo per i prodotti da elencare in Walmart Marketplace disponga di tutti gli attributi necessari e soddisfi le linee guida per i contenuti di Walmart Marketplace.

- Verificare che il processo cron sia in esecuzione per completare l&#39;operazione di esportazione.

   - Per le istanze locali, vedere [Configurare ed eseguire cron](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/configure-cron-jobs.html).

   - Ad Adobe, per l&#39;infrastruttura cloud, vedere [Configurare i processi cron](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/properties/crons-property.html).

### Creare il file di dati del prodotto da caricare

1. Dal tuo account [Walmart Seller](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), scarica un modello di inserzione di prodotti dal Walmart Seller Center.

   - Dalla pagina Elementi del catalogo prodotti, selezionare **[!UICONTROL Add Items]**. Quindi, selezionare **[!UICONTROL Add items in bulk]**.

     ![Opzione Aggiungi elementi in blocco nella configurazione di elementi di Walmart Marketplace](assets/walmart-seller-account-add-items-bulk.png){width="600" zoomable="yes"}

   - Nella pagina di download, selezionare **[!UICONTROL Full Setup]**. Quindi, seleziona una categoria di elementi e scarica il modello di categoria.

     ![Opzione Scarica modello di categoria nella configurazione elemento di Walmart Marketplace](assets/walmart-seller-account-full-setup-download.png){width="600" zoomable="yes"}

   - Verifica che il modello includa gli attributi richiesti e consigliati per l’elenco dei prodotti.

1. Dall&#39;amministratore [!DNL Commerce], seleziona i dati del prodotto da esportare dal sito di Adobe [!DNL Commerce].

   - Dall&#39;amministratore, selezionare [!UICONTROL **Sistema** > Trasferimento dati > **Esporta**].

   - Nella pagina [!UICONTROL Export] nel campo [!UICONTROL Entity Type], seleziona [!UICONTROL **Prodotti**].

   - Nella tabella [!UICONTROL Entity Attributes] configurare i criteri di selezione per l&#39;esportazione dei dati del prodotto.

     Utilizza i filtri per selezionare e configurare i valori degli attributi applicabili alle categorie di prodotti venduti in. Assicurati di includere gli attributi richiesti e consigliati di Walmart. Per istruzioni dettagliate, vedere [Esporta dati](https://experienceleague.adobe.com/docs/commerce-admin/systems/data-transfer/data-export.html) nella Guida utente di Adobe [!DNL Commerce].

     Per omettere un attributo dall&#39;esportazione, selezionare la casella di controllo [!UICONTROL **Escludi**] all&#39;inizio della riga.

1. Scorri fino alla fine della tabella degli attributi e seleziona [!UICONTROL **Continua**] per avviare l&#39;esportazione dei dati.

   Il file di esportazione CSV viene elaborato tramite una coda di messaggi utilizzando i processi cron e salvato in `var/export/folder`. (Vedi [Gestione delle code di messaggi](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/message-queues/manage-message-queues.html) nella *Guida alla configurazione*.)

1. Aprire il modello di Excel per la categoria di prodotti Walmart Marketplace e utilizzare le funzionalità macro di Excel per unire i dati di prodotto esportati nel modello di Excel.

1. Carica il file Excel con i dati del prodotto esportato.

   - Torna alla pagina Elementi del catalogo prodotti nel [Centro venditori Walmart](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Seleziona [!UICONTROL **Aggiungi elementi** > **Aggiungi elementi in blocco**].
   - Trascina il foglio di calcolo completato nella sezione Carica.
   - Seleziona [!UICONTROL **Invia**].
   - Seleziona [!UICONTROL  **Feed attività**] per visualizzare l&#39;avanzamento.

Per istruzioni complete, consulta [Aggiungi oggetti in blocco utilizzando la specifica dell&#39;oggetto completa](https://sellerhelp.walmart.com/s/guide?article=000007680) nella [!DNL *Guida di Walmart Seller*].
