---
title: 'Onboarding: Crea regola di elenco'''
description: Durante il completamento del processo di onboarding del canale di vendita Amazon, crea le regole di annuncio iniziali per generare gli elenchi Amazon per il tuo [!DNL Commerce] prodotti.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Onboarding: Crea regola di elenco

Le regole di elenco possono essere definite durante l’onboarding, ma possono anche essere modificate in qualsiasi momento. Dopo l’onboarding, puoi accedere al [regole di elenco](./listing-rules.md) sul negozio [dashboard](./amazon-store-dashboard.md).

## Creare una regola di elenco durante l’onboarding

1. Dopo aver connesso lo store, fai clic su **[!UICONTROL View Store]** per l&#39;archivio aggiunto.

   Il negozio [dashboard](./amazon-store-dashboard.md) appare con `No products listed to Amazon` messaggio.

1. Fai clic su **[!UICONTROL Preview and List Eligible Products]**.

   La _[!UICONTROL Listing Rules]_viene visualizzata la pagina .

1. Definisci le condizioni desiderate per l’idoneità dei prodotti da elencare in Amazon e fai clic su **[!UICONTROL Preview changes]** o fai clic su **[!UICONTROL Preview changes]** per saltare questo passaggio.

   Vedi [Esempio: Definire una condizione](./ob-define-condition-example.md).

1. Rivedi le tue inserzioni nell&#39;anteprima dell&#39;elenco:

   ![Anteprima elenco](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - I prodotti elencati in questa scheda non sono idonei per l’elenco di Amazon in base alle impostazioni correnti della regola di elenco.

      I prodotti non consentiti non vengono pubblicati in Amazon. Se un prodotto non idoneo è già elencato in Amazon e l’elenco Amazon corrisponde al tuo [!DNL Commerce] prodotto catalogo, la quantità per l’elenco di Amazon cambia in `0` per impedire la vendita del prodotto. Per rimuovere manualmente un elenco da Amazon, vedi [Terminazione di un elenco Amazon](./end-listings-manually.md). I prodotti non idonei ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella [[!UICONTROL Inactive Listings] scheda](./inactive-listings.md).

      Per modificare un `Ineligible` inserimento in un elenco `Eligible` elencare, ripetere questo processo e modificare le regole di inserzione.

   - **[!UICONTROL Eligible Listings]** - I prodotti elencati in questa scheda sono idonei per l’inserimento nell’elenco di Amazon in base alla configurazione della regola dell’elenco corrente e sono idonei in base ai requisiti Amazon. Questa scheda include gli elenchi di Amazon esistenti importati (se hai **[!UICONTROL Import Third Party Listings]** impostato su `Import Listing` nel tuo [Impostazioni elenco](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - I prodotti elencati in questa scheda includono [!DNL Commerce] prodotti di catalogo che sono appena idonei per l’inserimento nell’elenco di Amazon in base alla configurazione della regola dell’elenco corrente e creare elenchi Amazon.

1. Al termine, fai clic su **[!UICONTROL Save and Close]**.

   Il negozio [dashboard](./amazon-store-dashboard.md) si apre.

Al termine dell&#39;onboarding di uno store, le informazioni vengono sincronizzate tra [!DNL Commerce] e Amazon è stato avviato. Gli elenchi Amazon vengono importati in [!DNL Commerce] e cerca di abbinare i prodotti nel tuo [!DNL Commerce] Catalogo.

Puoi visualizzare le informazioni sull’ordine Amazon nella sezione _[!UICONTROL Recent Orders]_della dashboard del negozio. Vedi [Dashboard del Negozio](./amazon-store-dashboard.md) o [Gestisci ordini](./managing-orders.md).

>[!IMPORTANT]
>
>Ci sono alcune importanti impostazioni store (elenchi, prezzi, regole, evasione, altro) che hanno valori predefiniti per un nuovo negozio. Per assicurarti che lo store sia configurato per le tue esigenze specifiche, rivedi il tuo [impostazioni store](./default-store-settings.md) .

![Icona Successivo](assets/btn-next.png) [**Continua con le impostazioni store predefinite**](./default-store-settings.md)
