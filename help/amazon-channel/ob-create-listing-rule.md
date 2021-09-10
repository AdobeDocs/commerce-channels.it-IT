---
title: 'Onboarding: Crea regola di elenco'''
description: Durante il completamento del processo di onboarding del canale di vendita Amazon, crea le regole di annuncio iniziali per generare gli elenchi Amazon per i tuoi prodotti [!DNL Commerce] .
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Onboarding: Crea regola di elenco

Le regole di elenco possono essere definite durante l’onboarding, ma possono anche essere modificate in qualsiasi momento. Dopo l&#39;onboarding, puoi accedere alle [regole di elenco](./listing-rules.md) nello store [dashboard](./amazon-store-dashboard.md).

## Creare una regola di elenco durante l’onboarding

1. Dopo aver connesso lo store, fai clic su **[!UICONTROL View Store]** per lo store aggiunto.

   L&#39;archivio [dashboard](./amazon-store-dashboard.md) viene visualizzato con il messaggio `No products listed to Amazon`.

1. Fare clic su **[!UICONTROL Preview and List Eligible Products]**.

   Viene visualizzata la pagina _[!UICONTROL Listing Rules]_.

1. Definisci le condizioni desiderate per l’idoneità dei prodotti da elencare in Amazon e fai clic su **[!UICONTROL Preview changes]**, oppure fai clic su **[!UICONTROL Preview changes]** per saltare questo passaggio.

   Vedere [Esempio: Definire una condizione](./ob-define-condition-example.md).

1. Rivedi le tue inserzioni nell&#39;anteprima dell&#39;elenco:

   ![Anteprima elenco](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - I prodotti elencati in questa scheda non sono idonei per l’elenco di Amazon in base alle impostazioni correnti della regola di elenco.

      I prodotti non consentiti non vengono pubblicati in Amazon. Se un prodotto non idoneo è già elencato in Amazon e si associa l’elenco Amazon al prodotto di catalogo [!DNL Commerce], la quantità dell’elenco Amazon viene modificata in `0` per impedire la vendita del prodotto. Per rimuovere manualmente un elenco da Amazon, consulta [Terminazione di un elenco Amazon](./end-listings-manually.md). I prodotti non idonei ai requisiti Amazon non sono elencati qui. Tali prodotti sono elencati nella scheda [[!UICONTROL Inactive Listings]](./inactive-listings.md).

      Per modificare un elenco `Ineligible` in un elenco `Eligible`, ripeti questo processo e modifica le regole di elenco.

   - **[!UICONTROL Eligible Listings]** - I prodotti elencati in questa scheda sono idonei per l’inserimento nell’elenco di Amazon in base alla configurazione della regola dell’elenco corrente e sono idonei in base ai requisiti Amazon. Questa scheda include gli elenchi Amazon esistenti importati (se **[!UICONTROL Import Third Party Listings]** è impostato su `Import Listing` nel [Impostazioni elenco](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - I prodotti elencati in questa scheda includono i prodotti di  [!DNL Commerce] catalogo appena idonei per l’inserimento nell’elenco di Amazon in base alla configurazione della regola dell’elenco corrente e creare elenchi di Amazon.

1. Al termine, fai clic su **[!UICONTROL Save and Close]**.

   Viene visualizzato l&#39;archivio [dashboard](./amazon-store-dashboard.md).

Al termine dell&#39;onboarding di uno store, viene avviata la sincronizzazione delle informazioni tra [!DNL Commerce] e Amazon. Gli elenchi Amazon vengono importati in [!DNL Commerce] e tentano di trovare una corrispondenza con i prodotti nel catalogo [!DNL Commerce].

Puoi visualizzare le informazioni sull’ordine di Amazon nella sezione _[!UICONTROL Recent Orders]_del dashboard store. Consulta [Archivia dashboard](./amazon-store-dashboard.md) o [Gestisci ordini](./managing-orders.md).

>[!IMPORTANT]
>
>Ci sono alcune importanti impostazioni store (elenchi, prezzi, regole, evasione, altro) che hanno valori predefiniti per un nuovo negozio. Per verificare che lo store sia configurato per le tue esigenze specifiche, controlla le [impostazioni dello store](./default-store-settings.md) .

![Icona ](assets/btn-next.png) [**SuccessivoImpostazioni store predefinite**](./default-store-settings.md)
