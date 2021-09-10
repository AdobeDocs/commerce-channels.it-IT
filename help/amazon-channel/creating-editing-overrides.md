---
title: Creare e modificare sostituzioni
description: Utilizza le sostituzioni dei Sales Channel Amazon per applicare le modifiche a un singolo elenco Amazon o a più elenchi.
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Creare e modificare le sostituzioni

È possibile creare e sostituire un elenco oppure modificare o rimuovere un override applicato a un elenco. Le sostituzioni impostano un valore definito per un elenco specifico.

## Creare un override per un singolo elenco

L’azione _[!UICONTROL Create Override]_è disponibile quando visualizzi gli elenchi nelle schede_[!UICONTROL Inactive]_, _[!UICONTROL Active]_e_[!UICONTROL Ineligible]_ .

1. Visualizza un elenco in una scheda _[!UICONTROL Products Listings]_(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_e_[!UICONTROL Ineligible]_ ).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Create Override]**per aprire la pagina Sostituzioni elenco prodotti .

   ![crea override elenco Amazon](assets/amazon-select-create-override.png)

1. Per verificare di aver visualizzato l&#39;elenco corretto, verifica il _[!UICONTROL Listing Details]_.

1. Determinare il tipo di sostituzione che si sta creando.

   È possibile definire un singolo tipo di sostituzione o qualsiasi combinazione di tipi per l&#39;inserzione (prezzo, tempo di gestione, condizione, note sul venditore).

   - **Prezzo**  - Fai clic  **[!UICONTROL Change Listing Price]** e inserisci il valore del prezzo definito per  **[!UICONTROL Price Override]**.
   - **Tempo di gestione** : fai clic su  **[!UICONTROL Change Handling Time]** e immetti il valore temporale definito (in giorni) per  **[!UICONTROL Handling Time Override]**.
   - **Condizione**  - Fai clic  **[!UICONTROL Change Condition]** e scegli l’opzione corretta per  **[!UICONTROL Condition Override]**.
   - **Note venditore**  - Fai clic su  **[!UICONTROL Change Seller Notes]** e inserisci il testo delle note per  **[!UICONTROL Seller Notes Override]**.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_viene chiusa. Lo stato dell’elenco diventa `Relist in Progress`. La modifica verrà pubblicata in Amazon con la successiva sincronizzazione dati (come configurata nelle impostazioni cron). L’elenco viene aggiunto anche alla scheda_[!UICONTROL Overrides]_ .

L&#39;esempio seguente mostra un override che definisce un nuovo prezzo di `$55`, un nuovo tempo di movimentazione di `1 day`, una nuova condizione di `Used; Like New` e un nuovo testo di Note venditore.

![Esempio di sostituzione dell’elenco Amazon](assets/amazon-overrides-edit.png)

## Modificare o rimuovere una sostituzione per un singolo elenco {#edit-override-single-listing}

L’azione _[!UICONTROL Edit Overrides]_è disponibile quando visualizzi gli elenchi nella scheda_[!UICONTROL Overrides]_ .

1. Visualizza un elenco nella scheda _[!UICONTROL Product Listings]_(_[!UICONTROL Overrides]_ ).

1. Nella colonna _[!UICONTROL Action]_, fai clic su **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   Viene visualizzata la pagina _[!UICONTROL Product Listing Overrides]_.

   ![Seleziona un override per l’elenco Amazon](assets/amazon-select-edit-overrides.png)

1. Per sovrascrivere l&#39;elenco corretto, verifica il _[!UICONTROL Listing Details]_.

1. Per modificare le impostazioni _[!UICONTROL Override]_, definisci le sezioni relative al tipo da modificare (Prezzo, Tempo di gestione, Condizione, Note sul venditore).

   Per mantenere lo stesso tipo di sostituzione, selezionare `No Change To <override type>` (impostazione predefinita). Questa impostazione lascia invariato il valore di sostituzione precedentemente definito.

   - **Prezzo**  - Fai clic  **[!UICONTROL Change Listing Price]** e inserisci il valore del prezzo definito per  **[!UICONTROL Price Override]**.
   - **Tempo di gestione** : fai clic su  **[!UICONTROL Change Handling Time]** e immetti il valore temporale definito (in giorni) per  **[!UICONTROL Handling Time Override]**.
   - **Condizione**  - Fai clic  **[!UICONTROL Change Condition]** e scegli l’opzione corretta per  **[!UICONTROL Condition Override]**.
   - **Note venditore**  - Fai clic su  **[!UICONTROL Change Seller Notes]** e inserisci il testo delle note per  **[!UICONTROL Seller Notes Override]**.

1. Per rimuovere un tipo di sostituzione, fare clic su **Rimuovi** per ciascuno dei tipi che si desidera rimuovere. Se non viene rimosso, il valore definito in precedenza rimane nella sostituzione.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_viene chiusa. Lo stato dell’elenco diventa `Relist in Progress`. La modifica verrà pubblicata in Amazon con la successiva sincronizzazione dati (come configurata nelle impostazioni cron). Se non è già presente nell’elenco, anche gli elenchi vengono aggiunti alla scheda_[!UICONTROL Overrides]_ .

Piggybackup sull&#39;esempio _Crea un override_. L’esempio seguente mostra una modifica alla sostituzione creata in precedenza che definisce un nuovo prezzo di `$50`, rimuove la sostituzione del tempo di gestione e mantiene le sostituzioni precedenti di Condition e Seller Notes.

![Modifica o rimozione di un override](assets/amazon-overrides-edit-2.png)
__

## Modificare o rimuovere un override per più elenchi {#edit-override-multiple-listings}

L’azione _[!UICONTROL Edit Listing Overrides]_è disponibile nelle schede_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ e _[!UICONTROL Ineligible]_.

>[!NOTE]
>
>Poiché modifichi le sostituzioni per più elenchi, la sezione _[!UICONTROL Listing Details]_non viene visualizzata come quando modifichi un singolo elenco.

1. Visualizza l’elenco in una scheda _[!UICONTROL Products Listings]_(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ e _[!UICONTROL Ineligible]_).

1. Seleziona la casella di controllo nella colonna a sinistra per ciascuno degli elenchi da modificare.

1. In _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Edit Listing Overrides]**.

   Viene visualizzata la pagina _[!UICONTROL Product Listing Overrides]_.

   ![Seleziona un override per l’elenco Amazon](assets/amazon-actions-edit-listing-overrides.png)

1. Per modificare le impostazioni _[!UICONTROL Override]_, definisci le sezioni relative al tipo da modificare (Prezzo, Tempo di gestione, Condizione, Note sul venditore).

   Per mantenere uguale un override, selezionare `No Change To <override type>` (impostazione predefinita). Questa impostazione lascia invariato il valore di sostituzione precedentemente definito.

   - **Prezzo**  - Fai clic  **[!UICONTROL Change Listing Price]** e inserisci il valore del prezzo definito per  **[!UICONTROL Price Override]**.
   - **Tempo di gestione** : fai clic su  **[!UICONTROL Change Handling Time]** e immetti il valore temporale definito (in giorni) per  **[!UICONTROL Handling Time Override]**.
   - **Condizione**  - Fai clic  **[!UICONTROL Change Condition]** e scegli l’opzione corretta per  **[!UICONTROL Condition Override]**.
   - **Note venditore**  - Fai clic su  **[!UICONTROL Change Seller Notes]** e inserisci il testo delle note per  **[!UICONTROL Seller Notes Override]**.

1. Per rimuovere un tipo di sostituzione, fare clic su **[!UICONTROL Remove]** per ciascuno dei tipi che si desidera rimuovere. Se non viene rimosso, il valore definito in precedenza rimane nella sostituzione.

1. Fare clic su **[!UICONTROL Save Listing Override]**.

   La pagina _[!UICONTROL Product Listing Overrides]_viene chiusa. Lo stato degli elenchi cambia in `Relist in Progress`. La modifica verrà pubblicata in Amazon con la successiva sincronizzazione dati (come configurata nelle impostazioni cron). Se non è già presente nell’elenco, anche gli elenchi vengono aggiunti alla scheda_[!UICONTROL Overrides]_ .

### Tipi di sostituzione

| Override | Descrizione |
|--- |--- |
| [!UICONTROL Price Override] | Una sostituzione del prezzo definisce il prezzo delle inserzioni. Questa sostituzione ha la priorità su tutte le impostazioni automatizzate fino a quando la sostituzione non viene rimossa.<br><br>Per ignorare il prezzo del prodotto, scegli  **[!UICONTROL Change Listing Price]** e inserisci il nuovo prezzo per  **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | Una sostituzione dei tempi di gestione definisce il tempo (in giorni) necessario per elaborare e spedire i prodotti. Una sostituzione del tempo di gestione ha la priorità su tutte le impostazioni di tempo di gestione automatizzata e predefinita fino a quando la sostituzione non viene rimossa.<br><br>Il valore presente nella  _[!UICONTROL Handling Time Override]_casella può essere rappresentato dal tempo di gestione predefinito definito nell&#39; [elenco ](./listing-settings.md) o dal tempo di gestione predefinito. Se si rimuove una sostituzione del tempo di gestione, per impostazione predefinita l&#39;elenco riporta il tempo di gestione definito nelle impostazioni dell&#39;elenco.<br><br>Per definire una sostituzione del tempo di gestione, scegliere **[!UICONTROL Change Handling Time]**e immettere il nuovo tempo di gestione (in giorni) per **[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | Per ignorare la condizione di elenco, scegli **[!UICONTROL Change Condition]** e scegli la nuova condizione da **Condizione di sostituzione**. |
| [!UICONTROL Seller Notes Override] | Per i prodotti del catalogo definiti con una condizione diversa da `New`, è possibile aggiungere una nota al venditore per fornire ulteriori dettagli sul prodotto e sulle sue condizioni ai potenziali acquirenti. È possibile inserire una sostituzione di nota venditrice per un prodotto a condizione `New`, ma Amazon non visualizza la nota.<br><br>Per ignorare le note sul venditore, scegli  **[!UICONTROL Change Seller Notes]** e inserisci la nuova nota per  **[!UICONTROL Seller Notes Override]**. |
