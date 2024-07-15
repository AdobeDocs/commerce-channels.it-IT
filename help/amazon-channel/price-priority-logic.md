---
title: Canale di vendita Amazon - Logica di priorità prezzo
description: Nel determinare il prezzo pubblicato per un’inserzione Amazon, il canale di vendita Amazon applica la priorità.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%

---

# Logica priorità prezzo

Nell&#39;esempio seguente, in che modo il sistema determina se è necessario pubblicare $31,99, $24,99 o $27,99?

![Ambito prezzo Commerce](assets/amazon-price-scope.png){width="400"}

Per determinare quale prezzo viene utilizzato se un prodotto si trova su due siti Web e ha un prezzo variabile per sito Web, utilizzare la logica di priorità del prezzo (determinata dal valore [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)).

Per visualizzare l&#39;ordinamento dei negozi, passa a **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** nella barra laterale _Amministratore_. Nella colonna _[!UICONTROL Web Site]_fare clic sul nome del sito Web. Nella pagina_[!UICONTROL Web Site Information]_ è visualizzata l&#39;impostazione _[!UICONTROL Sort Order]_per il sito Web, che determina la priorità del sito Web. Il valore `1` indica la priorità più alta.

Se il prezzo del prodotto è impostato su `Use Default`, viene ripristinato il valore di prezzo predefinito anziché il valore del prezzo del sito Web.

## Esempio 1

|         | Priorità sito Web | Prezzo (sito Web) | Usa predefinito |
|---------|------------------|-----------------|-------------|
| Predefinito | 0 | 31,99 $ | — |
| Store 1 | 1 | 24,99 $ | No |
| Store 2 | 2 | 27,99 $ | Sì |

- **[!UICONTROL Magento Price Source]** (definito nel [Prezzo d&#39;inserzione](./listing-price.md) è impostato sull&#39;attributo `Price`.
- Esaminare il sito Web con la priorità più elevata, ovvero Archivio 1 (definito dal valore [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)).
- Poiché il Negozio 1 è impostato per utilizzare il prezzo del sito Web (Usa predefinito = No), il prezzo pubblicato è $24,99.

## Esempio 2

|         | Priorità sito Web | Sito Web prezzi | Usa predefinito |
|---------|------------------|---------------|-------------|
| Predefinito | 0 | 31,99 $ | — |
| Store 1 | 1 | 24,99 $ | Sì |
| Store 2 | 2 | 27,99 $ | No |

- **[!UICONTROL Magento Price Source]** (definito nel [Prezzo d&#39;inserzione](./listing-price.md) è impostato sull&#39;attributo `Price`.
- Esaminare il sito Web con la priorità più elevata, ovvero Archivio 1 (definito dal valore [sort](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)).
- Poiché il Negozio 1 **non è** impostato per utilizzare il prezzo del sito Web (Usa predefinito = Sì), controllare il sito Web successivo nell&#39;ordinamento.
- Poiché lo Store 2 **è** impostato per utilizzare il prezzo del sito Web (Usa predefinito = No), il prezzo pubblicato è $27,99.

## Esempio 3

|         | Priorità sito Web | Sito Web prezzi | Usa predefinito |
|---------|------------------|---------------|-------------|
| Predefinito | 0 | 31,99 $ | 30,00 $ |
| Store 1 | 1 | 24,99 $ | — |
| Store 2 | 2 | 27,99 $ | 20,00 $ |

In questo esempio viene aggiunto il valore non di prezzo, che viene utilizzato se si seleziona un altro valore per _[!UICONTROL Magento Price Source_] (definito nelle impostazioni [Listing Price](./listing-price.md)). Il valore non relativo al prezzo utilizza sempre il prezzo come prezzo di fallback.

- **[!UICONTROL Magento Price Source]** (definito nelle impostazioni [[!UICONTROL Listing Price]](./listing-price.md)) è impostato su `Non-Price`.
- Esaminare il sito Web con la priorità più alta, ovvero `Store 1` (definito dal valore [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)).
- Poiché l&#39;archivio 1 **non è** impostato per l&#39;utilizzo dell&#39;attributo `Non-Price`, controllare il sito Web successivo nell&#39;ordinamento.
- Poiché l&#39;archivio 2 **is** è impostato per utilizzare l&#39;attributo `Non-Price` (non prezzo [sito Web] = $20,00), il prezzo pubblicato è $20,00.
