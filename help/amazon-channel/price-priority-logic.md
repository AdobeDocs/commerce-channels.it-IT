---
title: Canale di vendita Amazon - Logica di priorità prezzo
description: Nel determinare il prezzo pubblicato per un’inserzione Amazon, il canale di vendita Amazon applica la priorità.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# Logica priorità prezzo

Nell&#39;esempio seguente, in che modo il sistema determina se è necessario pubblicare $31,99, $24,99 o $27,99?

![Ambito prezzo Commerce](assets/amazon-price-scope.png){width="400"}

Per determinare quale prezzo viene utilizzato se un prodotto si trova su due siti web e ha un prezzo variabile per sito web, utilizza la logica di priorità del prezzo (determinata dalla [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) valore).

Per visualizzare l&#39;ordinamento dei negozi, vai a **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** nel _Amministratore_ barra laterale. In _[!UICONTROL Web Site]_, fare clic sul nome del sito Web. Il_[!UICONTROL Web Site Information]_ mostra la pagina _[!UICONTROL Sort Order]_impostazione per il sito Web, che determina la priorità del sito Web. Un valore di `1` indica la priorità più alta.

Se il prezzo del prodotto è impostato su `Use Default`, torna al valore di prezzo predefinito invece del valore di prezzo del sito web.

## Esempio 1

|         | Priorità sito Web | Prezzo (sito Web) | Usa predefinito |
|---------|------------------|-----------------|-------------|
| Predefinito | 0 | $31.99 | — |
| Store 1 | 1 | $24.99 | No |
| Store 2 | 2 | $27.99 | Sì |

- Il **[!UICONTROL Magento Price Source]** (definito nel [Prezzo di vendita](./listing-price.md) è impostato su `Price` attributo.
- Guarda il sito web con la priorità più alta, che è Store 1 (definito da [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) valore).
- Poiché il Negozio 1 è impostato per utilizzare il prezzo del sito Web (Usa predefinito = No), il prezzo pubblicato è $24,99.

## Esempio 2

|         | Priorità sito Web | Sito Web prezzi | Usa predefinito |
|---------|------------------|---------------|-------------|
| Predefinito | 0 | $31.99 | -- |
| Store 1 | 1 | $24.99 | Sì |
| Store 2 | 2 | $27.99 | No |

- Il **[!UICONTROL Magento Price Source]** (definito nel [Prezzo di vendita](./listing-price.md) è impostato su `Price` attributo.
- Guarda il sito web con la priorità più alta, che è Store 1 (definito da [ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) valore).
- Dal punto vendita 1 **non è** impostato per utilizzare il prezzo del sito Web (Usa predefinito = Sì), esaminare il sito Web successivo nell&#39;ordinamento.
- Da Store 2 **è** impostato per utilizzare il prezzo del sito Web (Usa predefinito = No), il prezzo pubblicato è $ 27,99.

## Esempio 3

|         | Priorità sito Web | Sito Web prezzi | Usa predefinito |
|---------|------------------|---------------|-------------|
| Predefinito | 0 | $31.99 | $30.00 |
| Store 1 | 1 | $24.99 | -- |
| Store 2 | 2 | $27.99 | $20.00 |

In questo esempio viene aggiunto il valore non di prezzo, che viene utilizzato se si seleziona un altro valore per _[!UICONTROL Magento Price Source_] (definito nel [Prezzo di vendita](./listing-price.md) ). Il valore non relativo al prezzo utilizza sempre il prezzo come prezzo di fallback.

- Il **[!UICONTROL Magento Price Source]** (definito in [[!UICONTROL Listing Price]](./listing-price.md) ) è impostato su `Non-Price`.
- Guarda il sito web con la priorità più alta, che è `Store 1`(definito da [Ordinamento](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) valore).
- Dal punto vendita 1 **non è** impostato per utilizzare `Non-Price` , controllare il sito Web successivo in base all&#39;ordinamento.
- Da Store 2 **è** impostato per utilizzare `Non-Price` Attributo (non di prezzo) [Sito Web] = $ 20,00), il prezzo pubblicato è $ 20,00.
