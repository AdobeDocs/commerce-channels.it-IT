---
title: Creare e modificare le sostituzioni del canale di vendita Amazon
description: Utilizza le sostituzioni del Sales Channel Amazon per applicare le modifiche a una singola inserzione Amazon o a più inserzioni.
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Creare e modificare le sostituzioni

È possibile creare e sostituire un&#39;inserzione oppure modificare o rimuovere un&#39;esclusione applicata a un&#39;inserzione. Sostituisce imposta un valore definito per un elenco specifico.

## Creare una sostituzione per una singola inserzione

L&#39;azione _[!UICONTROL Create Override]_è disponibile quando si visualizzano le inserzioni nelle schede_[!UICONTROL Inactive]_, _[!UICONTROL Active]_e_[!UICONTROL Ineligible]_.

1. Visualizzare un&#39;inserzione in una pagina _[!UICONTROL Products Listings]_(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_e_[!UICONTROL Ineligible]_ schede).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Create Override]**per aprire la pagina delle sostituzioni dell&#39;elenco di prodotti.

   ![crea sostituzione elenco Amazon](assets/amazon-select-create-override.png){width="220"}

1. Per assicurarsi di visualizzare l&#39;inserzione corretta, verificare _[!UICONTROL Listing Details]_.

1. Determinare il tipo di sostituzione che si sta creando.

   Puoi definire un singolo tipo di sostituzione o qualsiasi combinazione di tipi per l’inserzione (prezzo, tempo di gestione, condizione, note del venditore).

   - **Prezzo** - Fare clic su **[!UICONTROL Change Listing Price]** e immettere il valore di prezzo definito per **[!UICONTROL Price Override]**.
   - **Tempo di gestione** - Fare clic su **[!UICONTROL Change Handling Time]** e immettere il valore di tempo definito (in giorni) per **[!UICONTROL Handling Time Override]**.
   - **Condizione** - Fare clic su **[!UICONTROL Change Condition]** e scegliere l&#39;opzione corretta per **[!UICONTROL Condition Override]**.
   - **Note del venditore** - Fai clic su **[!UICONTROL Change Seller Notes]** e immetti il testo delle note per **[!UICONTROL Seller Notes Override]**.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_si chiude. Lo stato della voce cambia in `Relist in Progress`. La modifica verrà pubblicata in Amazon con la prossima sincronizzazione dati (come configurato nelle impostazioni cron). L&#39;inserzione viene aggiunta anche alla scheda_[!UICONTROL Overrides]_.

L&#39;esempio seguente mostra una sostituzione che definisce un nuovo prezzo di `$55`, un nuovo tempo di imballaggio di `1 day`, una nuova condizione di `Used; Like New` e un nuovo testo della Nota del venditore.

![Esempio di sostituzione dell&#39;elenco di Amazon](assets/amazon-overrides-edit.png){width="600" zoomable="yes"}

## Modificare o rimuovere una sostituzione per una singola inserzione {#edit-override-single-listing}

L&#39;azione _[!UICONTROL Edit Overrides]_è disponibile quando si visualizzano le inserzioni nella scheda_[!UICONTROL Overrides]_.

1. Visualizza un&#39;inserzione nella pagina _[!UICONTROL Product Listings]_(scheda_[!UICONTROL Overrides]_).

1. Nella colonna _[!UICONTROL Action]_, fare clic su **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   Verrà aperta la pagina _[!UICONTROL Product Listing Overrides]_.

   ![Seleziona una sostituzione dell&#39;inserzione Amazon](assets/amazon-select-edit-overrides.png){width="125"}

1. Per assicurarsi di ignorare l&#39;inserzione corretta, verificare _[!UICONTROL Listing Details]_.

1. Per modificare le impostazioni di _[!UICONTROL Override]_, definire le sezioni per il tipo che si desidera modificare (prezzo, tempo di imballaggio, condizione, note del venditore).

   Per mantenere lo stesso tipo di sostituzione, selezionare `No Change To <override type>` (impostazione predefinita). Questa impostazione lascia invariato il valore di sostituzione definito in precedenza.

   - **Prezzo** - Fare clic su **[!UICONTROL Change Listing Price]** e immettere il valore di prezzo definito per **[!UICONTROL Price Override]**.
   - **Tempo di gestione** - Fare clic su **[!UICONTROL Change Handling Time]** e immettere il valore di tempo definito (in giorni) per **[!UICONTROL Handling Time Override]**.
   - **Condizione** - Fare clic su **[!UICONTROL Change Condition]** e scegliere l&#39;opzione corretta per **[!UICONTROL Condition Override]**.
   - **Note del venditore** - Fai clic su **[!UICONTROL Change Seller Notes]** e immetti il testo delle note per **[!UICONTROL Seller Notes Override]**.

1. Per rimuovere un tipo di sostituzione, fare clic su **Rimuovi** per ognuno dei tipi che si desidera rimuovere. Se non viene rimosso, il valore definito in precedenza rimane nell&#39;override.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_si chiude. Lo stato della voce cambia in `Relist in Progress`. La modifica verrà pubblicata in Amazon con la prossima sincronizzazione dati (come configurato nelle impostazioni cron). Se non sono già elencate, le inserzioni verranno aggiunte anche alla scheda_[!UICONTROL Overrides]_.

Piggybacking nell&#39;esempio _Crea un override_. L&#39;esempio seguente mostra una modifica alla sostituzione creata in precedenza che definisce un nuovo prezzo di `$50`, rimuove la sostituzione del tempo di gestione e mantiene le sostituzioni precedenti di Condizione e Note del venditore.

![Modifica o rimozione di una sostituzione](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## Modifica o rimuovi una sostituzione per più inserzioni {#edit-override-multiple-listings}

L&#39;azione _[!UICONTROL Edit Listing Overrides]_è disponibile nelle schede_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ e _[!UICONTROL Ineligible]_.

>[!NOTE]
>
>Poiché si stanno modificando le sostituzioni per più inserzioni, la sezione _[!UICONTROL Listing Details]_non viene visualizzata come quando si modifica una singola inserzione.

1. Visualizza l&#39;elenco in una pagina _[!UICONTROL Products Listings]_(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ e _[!UICONTROL Ineligible]_schede).

1. Seleziona la casella di controllo nella colonna a sinistra per ciascuna delle inserzioni che desideri modificare.

1. In _[!UICONTROL Actions]_, fare clic su **[!UICONTROL Edit Listing Overrides]**.

   Verrà aperta la pagina _[!UICONTROL Product Listing Overrides]_.

   ![Seleziona una sostituzione dell&#39;inserzione Amazon](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. Per modificare le impostazioni di _[!UICONTROL Override]_, definire le sezioni per il tipo che si desidera modificare (prezzo, tempo di imballaggio, condizione, note del venditore).

   Per mantenere la stessa sostituzione, selezionare `No Change To <override type>` (impostazione predefinita). Questa impostazione lascia invariato il valore di sostituzione definito in precedenza.

   - **Prezzo** - Fare clic su **[!UICONTROL Change Listing Price]** e immettere il valore di prezzo definito per **[!UICONTROL Price Override]**.
   - **Tempo di gestione** - Fare clic su **[!UICONTROL Change Handling Time]** e immettere il valore di tempo definito (in giorni) per **[!UICONTROL Handling Time Override]**.
   - **Condizione** - Fare clic su **[!UICONTROL Change Condition]** e scegliere l&#39;opzione corretta per **[!UICONTROL Condition Override]**.
   - **Note del venditore** - Fai clic su **[!UICONTROL Change Seller Notes]** e immetti il testo delle note per **[!UICONTROL Seller Notes Override]**.

1. Per rimuovere un tipo di sostituzione, fare clic su **[!UICONTROL Remove]** per ciascuno dei tipi che si desidera rimuovere. Se non viene rimosso, il valore definito in precedenza rimane nell&#39;override.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_si chiude. Lo stato delle inserzioni diventa `Relist in Progress`. La modifica verrà pubblicata in Amazon con la prossima sincronizzazione dati (come configurato nelle impostazioni cron). Se non sono già elencate, le inserzioni verranno aggiunte anche alla scheda_[!UICONTROL Overrides]_.

### Sostituisci tipi

| Ignora | Descrizione |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | Una sostituzione prezzo definisce il prezzo per le inserzioni. Questa sostituzione ha la priorità su tutte le impostazioni automatizzate fino a quando non viene rimossa.<br><br>Per sostituire il prezzo del prodotto, scegliere **[!UICONTROL Change Listing Price]** e immettere il nuovo prezzo per **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | Una sostituzione del tempo di gestione definisce il tempo necessario (in giorni) per elaborare e spedire i prodotti. Una sostituzione del tempo di gestione ha la priorità su tutte le impostazioni automatizzate e predefinite del tempo di gestione fino a quando la sostituzione non viene rimossa.<br><br>Il valore presente nella casella _[!UICONTROL Handling Time Override]_è il tempo di imballaggio predefinito definito nelle [impostazioni dell&#39;inserzione](./listing-settings.md) oppure il tempo di imballaggio dell&#39;override definito. Se si rimuove una sostituzione del tempo di gestione, per impostazione predefinita viene utilizzato il tempo di gestione definito nelle impostazioni dell&#39;inserzione.<br><br>Per definire una sostituzione del tempo di gestione, scegliere **[!UICONTROL Change Handling Time]**e immettere il nuovo tempo di gestione (in giorni) per **[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | Per ignorare la condizione dell&#39;elenco, scegliere **[!UICONTROL Change Condition]** e scegliere la nuova condizione da **Sostituzione condizione**. |
| [!UICONTROL Seller Notes Override] | Per i prodotti del catalogo definiti con una condizione diversa da `New`, è possibile aggiungere una nota del venditore per fornire maggiori dettagli sul prodotto e sulla relativa condizione ai potenziali acquirenti. È possibile immettere una sostituzione nota del venditore per un prodotto con condizione `New`, ma Amazon non visualizza la nota.<br><br>Per ignorare le note del venditore, scegli **[!UICONTROL Change Seller Notes]** e inserisci la nuova nota per **[!UICONTROL Seller Notes Override]**. |
