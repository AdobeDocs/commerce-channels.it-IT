---
title: Logica della priorità del prezzo
description: Il canale di vendita Amazon applica la definizione delle priorità nella determinazione del prezzo pubblicato per un elenco Amazon.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Logica della priorità del prezzo

Nell’esempio seguente, come determina il sistema se pubblicare $31.99, $24.99 o $27.99?

![Campo di applicazione del prezzo del commercio](assets/amazon-price-scope.png)

Per determinare quale prezzo viene utilizzato se un prodotto si trova su due siti web e ha un prezzo variabile per sito web, utilizzare la logica di priorità del prezzo (determinata dal valore [Ordina ordine](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}).

Per visualizzare l&#39;ordinamento degli archivi, passa a **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** nella barra laterale _Amministratore_. Nella colonna _[!UICONTROL Web Site]_, fai clic sul nome del sito web. La pagina_[!UICONTROL Web Site Information]_ mostra l’impostazione _[!UICONTROL Sort Order]_per il sito web, che determina la priorità del sito web. Un valore di `1` indica la priorità più alta.

Se il prezzo del prodotto è impostato su `Use Default`, torna al valore predefinito del prezzo invece del valore del sito web.

## Esempio 1

|  | Priorità sito web | Prezzo (sito web) | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | — |
| Store 1 | 1 | $ 24,99 | No |
| Store 2 | 2 | $ 27,99 | Sì |

- Il **[!UICONTROL Magento Price Source]** (definito nel [Prezzo di listino](./listing-price.md) è impostato sull&#39;attributo `Price`.
- Osserva il sito web con la priorità più elevata, che è Store 1 (definito dal valore [Sort Order](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} ).
- Poiché lo Store 1 è impostato per utilizzare il prezzo del sito web (Use Default = No), il prezzo pubblicato è $24,99.

## Esempio 2

|  | Priorità sito web | Sito Web del prezzo | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | — |
| Store 1 | 1 | $ 24,99 | Sì |
| Store 2 | 2 | $ 27,99 | No |

- Il **[!UICONTROL Magento Price Source]** (definito nel [Prezzo di listino](./listing-price.md) è impostato sull&#39;attributo `Price`.
- Osserva il sito web con la priorità più elevata, che è Store 1 (definito dal valore [sort order](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} ).
- Poiché il Negozio 1 **non è** impostato per utilizzare il prezzo del sito web (Usa predefinito = Sì), guarda il sito Web successivo nell&#39;ordinamento.
- Poiché lo Store 2 **è** impostato per utilizzare il prezzo del sito web (Usa predefinito = No), il prezzo pubblicato è $27,99.

## Esempio 3

|  | Priorità sito web | Sito Web del prezzo | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | $ 30,00 |
| Store 1 | 1 | $ 24,99 | — |
| Store 2 | 2 | $ 27,99 | $ 20,00 |

In questo esempio viene aggiunto il valore non relativo al prezzo, utilizzato se si seleziona un altro valore per _[!UICONTROL Magento Price Source_] (definito nelle impostazioni [Prezzo di listino](./listing-price.md)). Il valore non di prezzo utilizza sempre il prezzo come prezzo di fallback.

- Il **[!UICONTROL Magento Price Source]** (definito nelle impostazioni [[!UICONTROL Listing Price]](./listing-price.md)) è impostato su `Non-Price`.
- Osserva il sito web con la priorità più elevata, che è `Store 1`(definito dal valore [Ordina ordine](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}).
- Poiché lo Store 1 **non è** impostato per utilizzare l&#39;attributo `Non-Price`, controlla il sito Web successivo nell&#39;ordinamento.
- Poiché lo Store 2 **è** impostato per utilizzare l&#39;attributo `Non-Price` (Non-Price [Sito Web] = $20,00), il prezzo pubblicato è $20,00.
