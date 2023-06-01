---
user-guide-title: Guida utente del Sales Channel Amazon
user-guide-description: Genera vendite tramite Amazon integrando Adobe Commerce o Magenti Open Source con il tuo [!DNL Amazon Seller Central] account.
breadcrumb-title: Canale di vendita Amazon
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# Canale di vendita Amazon - [!DNL channel manager] per Adobe Commerce {#amazon}

- [Guida utente del Sales Channel Amazon](guide-overview.md)
- [Introduzione al canale di vendita Amazon](overview.md)
- Introduzione {#getting-started}
   - [Informazioni su Amazon Marketplace](about-amazon-marketplace.md)
   - [Amazon e il catalogo Commerce](about-listings-and-catalog.md)
   - [Best practice e limitazioni](amazon-best-practices.md)
   - [Installare l’estensione](install.md)
- Onboarding {#onboarding}
   - [Canale di vendita Amazon integrato](amazon-onboarding-home.md)
   - [Attività di pre-configurazione](amazon-pre-setup-tasks.md)
   - [Crea [!DNL Commerce] attributi per Amazon](ob-creating-magento-attributes.md)
   - [Verifica la chiave API di Amazon](amazon-verify-api-key.md)
   - [Integrazione store](store-integration.md)
   - [Crea regola di elenco](ob-create-listing-rule.md)
   - [Impostazioni store predefinite](default-store-settings.md)
- Gestire il canale di vendita {#manage}
   - [Home page](amazon-sales-channel-home.md)
   - [Negozi Amazon](managing-stores.md)
   - [Controlli di Workspace](workspace-controls.md)
   - [Apprendimento e preparazione](learning-preparation.md)
   - Attributi {#attributes}
      - [Visualizza attributi](attributes-view.md)
      - [Gestisci attributi](managing-attributes.md)
      - [Creare e modificare gli attributi](creating-attributes.md)
      - [Visualizza mappatura attributi](amazon-matching-attributes-values.md)
   - [Impostazioni amministratore canale di vendita](sales-channel-settings.md)
   - [Dashboard store di Amazon](amazon-store-dashboard.md)
   - [Impostazioni store](ob-store-review.md)
- Impostazioni elenco {#listing-settings}
   - [Visualizza impostazioni elenco](listing-settings.md)
   - [Azioni per l’elenco dei prodotti](product-listing-actions.md)
   - [Inserzioni di terze parti](third-party-listing-settings.md)
   - [Prezzo d&#39;inserzione](listing-price.md)
   - [(B2B) prezzi commerciali](business-pricing.md)
   - [Magazzino/quantità](stock-quantity.md)
   - [Soddisfatto da](fulfilled-by.md)
   - [Ricerca nel catalogo](catalog-search.md)
   - [Condizione di elenco prodotti](product-listing-condition.md)
   - [Prodotti rinnovati](renewed-products.md)
- [Impostazioni ordine](order-settings.md)
- [Impostazioni integrazione store](store-integration-settings.md)
- Regole di inserzione e determinazione prezzi {#rules}
   - [Regole di inserzione](listing-rules.md)
   - Regole di determinazione prezzi {#pricing-rules}
      - [Gestire i prezzi](pricing-products.md)
      - [Aggiungi nuova regola di determinazione prezzi](add-pricing-rule.md)
      - [Impostazioni generali regola prezzo](pricing-rule-general-settings.md)
      - [Condizioni della regola di prezzo](pricing-rule-conditions.md)
      - [Azioni regola prezzi](pricing-rule-actions.md)
      - [Regola prezzo standard](standard-price-rules.md)
      - [Regola di rideterminazione prezzi intelligente](intelligent-repricing-rules.md)
      - [Varianze condizionali del concorrente](competitor-conditional-variances.md)
      - [Rettifica prezzo](price-adjustment.md)
      - [Prezzo base](floor-price.md)
      - [Prezzo massimo opzionale](optional-ceiling-price.md)
      - [Limite di prezzo](price-scope.md)
      - [Logica priorità prezzo](price-priority-logic.md)
      - [Prezzo Buy Box concorrente](buy-box-competitor-pricing.md)
      - [Prezzi del concorrente più basso](lowest-competitor-pricing.md)
   - Esempi {#rules-examples}
      - [Definire una condizione](ob-define-condition-example.md)
      - [Esempi di regole di prezzo](price-rule-examples.md)
- Rapporti e registri {#reports-logs}
   - [Registra e archivia i rapporti](amazon-logs-reports.md)
   - Memorizza report {#store-reports}
      - [Analisi dei prezzi competitivi](competitive-price-analysis.md)
      - [Miglioramenti alle inserzioni](listing-improvements.md)
   - Registri {#logs}
      - [Registro delle modifiche alle inserzioni](listing-changes-log.md)
      - [Registro degli errori di comunicazione](communication-errors-log.md)
- Gestisci le inserzioni {#admin-listings}
   - [Gestire le inserzioni Amazon](managing-product-listings.md)
   - Per stato/scheda {#status-tab}
      - [Gestisci per stato/scheda](managing-listings-by-tab.md)
      - [Inserzioni incomplete](incomplete-listings.md)
      - [Nuove inserzioni di terze parti](new-third-party-listings.md)
      - [Pronto per l&#39;elenco](ready-to-list.md)
      - [Inserzioni inattive](inactive-listings.md)
      - [Inserzioni in corso](active-listings.md)
      - [Sostituzioni](overrides.md)
      - [Inserzioni non ammissibili](ineligible-listings.md)
      - [Inserzioni scadute](ended-listings.md)
   - Per azioni {#actions}
      - [Gestisci per azioni](managing-listings-by-action.md)
      - [Creazione e assegnazione di prodotti catalogo](creating-assigning-catalog-products.md)
      - [Creare e modificare le sostituzioni](creating-editing-overrides.md)
      - [Crea un SKU del venditore di alias](create-alias-seller-sku.md)
      - [Modificare un codice ASIN assegnato](edit-assigned-asin.md)
      - [Terminare un’inserzione in Amazon](end-listings-manually.md)
      - [Pubblicare un’inserzione in Amazon](publish-listings-manually.md)
      - [Aggiorna informazioni richieste](amazon-manually-update-incomplete-listing.md)
      - [Visualizza dettagli](product-listing-details.md)
- Gestire gli ordini {#admin-orders}
   - [Gestire gli ordini](managing-orders.md)
   - [Visualizza ordini Amazon](amazon-orders-all.md)
   - [Visualizza dettagli ordine Amazon](amazon-order-details.md)
   - [Attività comuni di elaborazione degli ordini](common-order-processing.md)
   - [Flussi di lavoro di evasione](fulfillment-workflows.md)
   - [Annulla ordini non spediti](cancel-unshipped-order.md)
- [Note sulla versione](release-notes.md)
