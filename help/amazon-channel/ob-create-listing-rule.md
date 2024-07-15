---
title: Creare una regola di inserimento nell’elenco di Amazon
description: Durante il completamento del processo di onboarding del canale di vendita Amazon, crea le regole di inserzione iniziali per la generazione di inserzioni Amazon per i tuoi  [!DNL Commerce]  prodotti.
role: Admin
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Creare una regola di inserimento nell’elenco di Amazon

Le regole di inserzione possono essere definite durante l’onboarding, ma possono anche essere modificate in qualsiasi momento. Dopo l&#39;onboarding, puoi accedere alle [regole di elenco](./listing-rules.md) nell&#39;archivio [dashboard](./amazon-store-dashboard.md).

## Creare una regola di elenco durante l’onboarding

1. Dopo aver connesso l&#39;archivio, fare clic su **[!UICONTROL View Store]** per l&#39;archivio aggiunto.

   Verrà visualizzato il dashboard [archivio](./amazon-store-dashboard.md) con il messaggio `No products listed to Amazon`.

1. Fare clic su **[!UICONTROL Preview and List Eligible Products]**.

   Viene visualizzata la pagina _[!UICONTROL Listing Rules]_.

1. Definisci le condizioni desiderate per l&#39;idoneità dei prodotti da elencare su Amazon e fai clic su **[!UICONTROL Preview changes]**, oppure fai clic su **[!UICONTROL Preview changes]** per saltare questo passaggio.

   Vedi [Esempio: definire una condizione](./ob-define-condition-example.md).

1. Controlla le inserzioni nell&#39;Anteprima inserzioni:

   ![Anteprima elenco](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - I prodotti elencati in questa scheda non sono idonei per l&#39;inserzione Amazon in base alle impostazioni correnti della regola di inserzione.

     I prodotti non ammissibili non vengono pubblicati in Amazon. Se un prodotto non idoneo è già presente nell&#39;elenco di Amazon e si abbina l&#39;elenco di Amazon al prodotto di catalogo [!DNL Commerce], la quantità dell&#39;elenco di Amazon viene modificata in `0` per impedire le vendite del prodotto. Per rimuovere manualmente un&#39;inserzione da Amazon, vedi [Terminazione di un&#39;inserzione da Amazon](./end-listings-manually.md). I prodotti che non sono idonei in base ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella scheda [[!UICONTROL Inactive Listings]](./inactive-listings.md).

     Per cambiare un&#39;inserzione `Ineligible` in un&#39;inserzione `Eligible`, ripeti questo processo e modifica le regole dell&#39;inserzione.

   - **[!UICONTROL Eligible Listings]** - I prodotti elencati in questa scheda sono idonei per l&#39;inserzione in Amazon in base alla configurazione della regola di inserzione corrente e sono idonei in base ai requisiti Amazon. Questa scheda include le tue inserzioni esistenti di Amazon importate (se hai **[!UICONTROL Import Third Party Listings]** impostato su `Import Listing` nelle [Impostazioni inserzioni](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - I prodotti elencati in questa scheda includono i prodotti del catalogo [!DNL Commerce] che sono appena idonei per l&#39;inserzione in Amazon in base alla configurazione della regola di inserzione corrente e creano inserzioni in Amazon.

1. Al termine, fare clic su **[!UICONTROL Save and Close]**.

   Verrà aperto l&#39;archivio [dashboard](./amazon-store-dashboard.md).

Al termine dell&#39;onboarding di un archivio, viene avviata la sincronizzazione delle informazioni tra [!DNL Commerce] e Amazon. Le tue inserzioni Amazon vengono importate in [!DNL Commerce] e tentano di trovare una corrispondenza con i prodotti nel catalogo [!DNL Commerce].

Puoi visualizzare le informazioni sull&#39;ordine di Amazon nella sezione _[!UICONTROL Recent Orders]_del dashboard dello store. Vedi [Dashboard store](./amazon-store-dashboard.md) o [Gestione ordini](./managing-orders.md).

>[!IMPORTANT]
>
>Alcune importanti impostazioni del negozio (inserzioni, prezzi, regole, evasione, altro) hanno valori predefiniti per un nuovo negozio. Per assicurarsi che il tuo archivio sia configurato per le tue esigenze specifiche, controlla le [impostazioni dello store](./default-store-settings.md).

![Icona Successivo](assets/btn-next.png) [**Passa alle impostazioni di archiviazione predefinite**](./default-store-settings.md)
