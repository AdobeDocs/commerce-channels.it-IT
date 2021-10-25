---
title: Logica della priorità del prezzo
description: Il canale di vendita Amazon applica la definizione delle priorità nella determinazione del prezzo pubblicato per un elenco Amazon.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Logica della priorità del prezzo

Nell’esempio seguente, come determina il sistema se pubblicare $31.99, $24.99 o $27.99?

![Campo di applicazione del prezzo del commercio](assets/amazon-price-scope.png)

Per determinare quale prezzo viene utilizzato se un prodotto si trova su due siti web e ha un prezzo variabile per sito web, utilizza la logica di priorità del prezzo (determinata dalla [Ordinamento](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target=&quot;_blank&quot;} value).

Per visualizzare l&#39;ordinamento dei negozi, vai a **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** in _Amministratore_ barra laterale. In _[!UICONTROL Web Site]_fare clic sul nome del sito Web. La_[!UICONTROL Web Site Information]_ mostra la pagina _[!UICONTROL Sort Order]_impostazione per il sito web, che determina la priorità del sito web. Un valore di `1` indica la priorità più alta.

Se il prezzo del prodotto è impostato su `Use Default`, torna al valore di prezzo predefinito invece del valore di prezzo del sito web.

## Esempio 1

|  | Priorità sito web | Prezzo (sito web) | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | — |
| Store 1 | 1 | $ 24,99 | No |
| Store 2 | 2 | $ 27,99 | Sì |

- La **[!UICONTROL Magento Price Source]** (definito nella [Prezzo di listino](./listing-price.md) è impostato su `Price` attributo.
- Osserva il sito web con la priorità più elevata, che è Store 1 (definito dalla [Ordinamento](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target=&quot;_blank&quot;} value).
- Poiché lo Store 1 è impostato per utilizzare il prezzo del sito web (Use Default = No), il prezzo pubblicato è $24,99.

## Esempio 2

|  | Priorità sito web | Sito Web del prezzo | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | — |
| Store 1 | 1 | $ 24,99 | Sì |
| Store 2 | 2 | $ 27,99 | No |

- La **[!UICONTROL Magento Price Source]** (definito nella [Prezzo di listino](./listing-price.md) è impostato su `Price` attributo.
- Osserva il sito web con la priorità più elevata, che è Store 1 (definito dalla [ordinamento](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target=&quot;_blank&quot;} value).
- Dal Negozio 1 **non** impostato per utilizzare il prezzo del sito web (Usa predefinito = Sì), guarda il sito Web successivo nell&#39;ordinamento.
- Dal Negozio 2 **è** impostato per utilizzare il prezzo del sito web (Usa predefinito = No), il prezzo pubblicato è $27,99.

## Esempio 3

|  | Priorità sito web | Sito Web del prezzo | Usa predefinito |
|---|---|---|---|
| Predefinito | 0 | $ 31,99 | $ 30,00 |
| Store 1 | 1 | $ 24,99 | — |
| Store 2 | 2 | $ 27,99 | $ 20,00 |

In questo esempio viene aggiunto il valore non relativo al prezzo, utilizzato se si seleziona un altro valore per _[!UICONTROL Magento Price Source_] (definito nella [Prezzo di listino](./listing-price.md) impostazioni). Il valore non di prezzo utilizza sempre il prezzo come prezzo di fallback.

- La **[!UICONTROL Magento Price Source]** (definito nella [[!UICONTROL Listing Price]](./listing-price.md) è impostato su `Non-Price`.
- Guarda il sito web con la massima priorità del sito web, che è `Store 1`(definito dalla [Ordinamento](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target=&quot;_blank&quot;} value).
- Dal Negozio 1 **non** impostato per utilizzare `Non-Price` , guarda il sito Web successivo nell&#39;ordinamento.
- Dal Negozio 2 **è** impostato per utilizzare `Non-Price` attributo (Non-Price) [Sito Web] = $ 20,00), il prezzo pubblicato è $ 20,00.
