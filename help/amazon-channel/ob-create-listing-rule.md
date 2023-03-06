---
title: "Onboarding: crea regola di inserzione"
description: Durante il completamento del processo di onboarding del canale di vendita Amazon, crea le regole di inserzione iniziali per la generazione di inserzioni Amazon per il tuo [!DNL Commerce] prodotti.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Onboarding: crea regola di inserzione

Le regole di inserzione possono essere definite durante l’onboarding, ma possono anche essere modificate in qualsiasi momento. Dopo l’onboarding, puoi accedere al [regole di inserzione](./listing-rules.md) in negozio [dashboard](./amazon-store-dashboard.md).

## Creare una regola di elenco durante l’onboarding

1. Dopo aver connesso il tuo Negozio, fai clic su **[!UICONTROL View Store]** per lo store aggiunto.

   Il negozio [dashboard](./amazon-store-dashboard.md) viene visualizzato con `No products listed to Amazon` messaggio.

1. Clic **[!UICONTROL Preview and List Eligible Products]**.

   Il _[!UICONTROL Listing Rules]_viene visualizzata.

1. Definisci le condizioni desiderate per l’idoneità dei prodotti a essere elencati su Amazon e fai clic su **[!UICONTROL Preview changes]**, o fai clic su **[!UICONTROL Preview changes]** per saltare questo passaggio.

   Consulta [Esempio: definire una condizione](./ob-define-condition-example.md).

1. Controlla le inserzioni nell&#39;Anteprima inserzioni:

   ![Anteprima elenco](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - I prodotti elencati in questa scheda non sono idonei per l’inserzione in Amazon in base alle impostazioni correnti della regola di inserzione.

      I prodotti non ammissibili non vengono pubblicati in Amazon. Se un prodotto non idoneo è già presente nell’elenco di Amazon e l’inserzione di Amazon corrisponde a [!DNL Commerce] prodotto del catalogo, la quantità per l’elenco Amazon diventa `0` per impedire la vendita del prodotto. Per rimuovere manualmente un’inserzione da Amazon, consulta [Chiusura di un’inserzione di Amazon](./end-listings-manually.md). I prodotti che non sono idonei in base ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella [[!UICONTROL Inactive Listings] scheda](./inactive-listings.md).

      Per modificare una `Ineligible` inserimento in un elenco `Eligible` inserzione, ripeti questa procedura e modifica le regole di inserzione.

   - **[!UICONTROL Eligible Listings]** - I prodotti elencati in questa scheda sono idonei per l’inserzione in Amazon in base alla configurazione della regola di inserzione corrente e sono idonei in base ai requisiti di Amazon. Questa scheda include le tue inserzioni esistenti di Amazon che vengono importate (se hai **[!UICONTROL Import Third Party Listings]** imposta su `Import Listing` nel tuo [Impostazioni elenco](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - I prodotti elencati in questa scheda includono [!DNL Commerce] cataloga i prodotti appena idonei per l’inserzione in Amazon in base alla configurazione della regola di inserzione corrente e crea inserzioni in Amazon.

1. Al termine, fai clic su **[!UICONTROL Save and Close]**.

   Il negozio [dashboard](./amazon-store-dashboard.md) viene aperto.

Al termine dell’onboarding di un archivio, le informazioni si sincronizzano tra [!DNL Commerce] e viene avviato Amazon. Le tue inserzioni Amazon vengono importate in [!DNL Commerce] e tentare di abbinare con i prodotti nel tuo [!DNL Commerce] Catalogo.

Puoi visualizzare le informazioni sull’ordine di Amazon in _[!UICONTROL Recent Orders]_sezione del dashboard del negozio. Consulta [Dashboard store](./amazon-store-dashboard.md) o [Gestisci ordini](./managing-orders.md).

>[!IMPORTANT]
>
>Alcune importanti impostazioni del negozio (inserzioni, prezzi, regole, evasione, altro) hanno valori predefiniti per un nuovo negozio. Per essere certi che il tuo negozio sia configurato per le tue esigenze specifiche, controlla [impostazioni store](./default-store-settings.md) .

![Icona Successivo](assets/btn-next.png) [**Passa alle impostazioni predefinite dello store**](./default-store-settings.md)
