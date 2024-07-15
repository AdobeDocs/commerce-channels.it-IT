---
title: "[!DNL (B2B) Business Price] per le inserzioni Amazon"
description: Puoi elencare i tuoi [!DNL Commerce] prodotti store sul sito Amazon Business (B2B) abilitando le attività nel tuo account Amazon [!DNL Seller Central] .
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# [!DNL (B2B) Business Price] per le inserzioni Amazon

(B2B) Le impostazioni del prezzo aziendale fanno parte delle impostazioni dell’inserzione del negozio. Le impostazioni dell&#39;inserzione sono accessibili dal [dashboard dell&#39;archivio Amazon](./amazon-store-dashboard.md).

[!DNL Amazon Business] è un marketplace esclusivo per gli account aziendali registrati di Amazon ed è disponibile solo negli Stati Uniti, in Francia, Germania e Regno Unito. Se il marketplace consente prezzi aziendali B2B, è modificabile all’interno delle impostazioni dell’inserzione.

[!DNL B2B Business Pricing] consente ai commercianti con account aziendali di acquistare tra loro con le prestazioni previste dell&#39;esperienza di acquisto di Amazon. Con il business pricing B2B, le aziende possono offrire prezzi su più livelli in base alla quantità acquistata.

Affinché i tuoi prodotti vengano elencati nel sito [!DNL Amazon Business (B2B)], devi prima abilitare l&#39;attività nel tuo account [!DNL Amazon Seller Central]. Per ulteriori informazioni sulla funzionalità B2B, vedi [Amazon: B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"} (richiede l&#39;accesso a Seller Central).

## Configura impostazioni [!DNL (B2B) Business Price]

1. Fare clic su **[!UICONTROL Listing Settings]** nel dashboard dell&#39;archivio.

1. Espandere la sezione _[!UICONTROL (B2B) Business Price]_.

1. Per **[!UICONTROL Enable Business Pricing]**, scegliere un&#39;opzione.

   - `Disabled` - (Predefinito) Scegliere se non si desidera abilitare le vendite business-to-business. Tutti gli altri campi di questa sezione vengono disattivati quando vengono selezionati.

   - `Enabled` - Scegliere quando abilitare le vendite business-to-business. Quando questa opzione è abilitata, il prezzo aziendale viene impostato come prezzo di listino dopo l&#39;applicazione di tutte le regole di determinazione prezzi. Il prezzo business segue l&#39;ambito di determinazione prezzi del sito Web, se abilitato. Il prezzo di un&#39;attività non può essere inferiore a 1 dollaro.

1. Per **[!UICONTROL Enable Tiered Pricing]**, scegliere un&#39;opzione.

   - `Disabled` - (Predefinito) Scegliere quando si desidera ottenere lo stesso prezzo di vendita per tutte le quantità dell&#39;ordine. Se scelti, tutti i campi _[!UICONTROL Pricing Level]_di questa sezione sono disabilitati.

   - `Enabled` - Scegliere quando abilitare gli adeguamenti dei prezzi in base alla quantità dell&#39;ordine. Se scelti, i campi _[!UICONTROL Pricing Level]_sono abilitati.

1. Completare le impostazioni di **[!UICONTROL Pricing Level]**.

   È possibile definire fino a cinque impostazioni di quantità/sconto per impostare la determinazione dei prezzi per il livello delle inserzioni commerciali. In ogni riga, inserire il valore di soglia della quantità e la percentuale di sconto da applicare. Ad esempio, se si immette `5` nel primo campo della prima riga e `5` nel secondo campo, il prezzo applica uno sconto del 5% quando un&#39;altra azienda acquista una quantità pari o superiore a 5.

1. Al termine, fare clic su **[!UICONTROL Save listing settings]**.

![Amazon Business Pricing (B2B)](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| Campo | Descrizione |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | Opzioni: <ul><li>**[!UICONTROL Disabled]** - (Predefinito) Scegliere se non si desidera abilitare le vendite business-to-business. Quando vengono selezionati, tutti gli altri campi di questa sezione vengono disabilitati.</li><li>**[!UICONTROL Enabled]** - Scegliere quando abilitare le vendite business to business. Quando viene scelto, il prezzo aziendale viene impostato come prezzo di listino dopo l&#39;applicazione di tutte le regole di determinazione prezzi. Il prezzo business segue l&#39;ambito di determinazione prezzi del sito Web, se abilitato. Il prezzo di un&#39;attività non può essere inferiore a 1 dollaro.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | Opzioni (obbligatorio): <ul><li>**[!UICONTROL Disabled]** - (Predefinito) Scegliere quando si desidera ottenere lo stesso prezzo di vendita per tutte le quantità dell&#39;ordine. Se scelti, tutti i campi _[!UICONTROL Pricing Level]_di questa sezione sono disabilitati.</li><li>**[!UICONTROL Enabled]** - Scegliere quando abilitare la determinazione dei prezzi in base alla quantità ordine. Se scelti, i campi _[!UICONTROL Pricing Level]_sono abilitati.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | Quando è abilitata la determinazione prezzi su più livelli, è possibile definire fino a cinque impostazioni di quantità/sconto che impostano la determinazione prezzi su più livelli per le inserzioni aziendali. In ogni riga, inserire il valore di soglia della quantità e la percentuale di sconto da applicare. Ad esempio, se si immette `5` nel primo campo della prima riga e `5` nel secondo campo, il prezzo applica uno sconto del 5% quando un&#39;altra azienda acquista una quantità pari o superiore a cinque. |

**Accesso rapido** - [!UICONTROL Listing Settings] sezioni

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
