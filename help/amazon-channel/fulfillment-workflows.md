---
title: Flussi di lavoro di evasione di Amazon
description: L'evasione di un ordine da un elenco Amazon segue una sequenza specifica dall'invio dell'ordine alla spedizione.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Flussi di lavoro di implementazione di Amazon

## Esempio: realizzato dal commerciante

| Passaggio | Descrizione |
|----|----|
| 1 | **Un ordine soddisfatto dal commerciante viene inserito su Amazon.** Amazon assegna uno stato di  `Pending` finché non vengono verificate le informazioni sulla carta di credito del cliente. Gli ordini nello stato `Pending` vengono importati automaticamente nel canale di vendita Amazon ma non vengono visualizzati nella scheda _[!UICONTROL Orders]_. |
| 2 | **L’ordine è verificato da Amazon.** Quando viene verificato, Amazon cambia lo stato in  `Unshipped`. Con questa modifica dello stato, l’ordine viene aggiornato nel canale di vendita Amazon e viene visualizzato nella scheda _[!UICONTROL Orders]_. |
| 1 | **I dettagli dell’ordine vengono aggiornati.** Il canale di vendita Amazon aggiorna i dettagli dell’ordine con il prezzo, l’e-mail del cliente e il nome del cliente. Durante questo aggiornamento, l’ordine Amazon crea l’ordine [!DNL Commerce] corrispondente nella pagina di gestione dell’ordine. Il numero dell&#39;ordine [!DNL Commerce] viene visualizzato con le informazioni sull&#39;ordine nella scheda _[!UICONTROL Orders]_. |
| 4 | **Viene creato un nuovo account cliente.** Se configurato nelle impostazioni dell&#39;ordine e il cliente non esiste nel  [!DNL Commerce] database, viene creato un nuovo cliente nel  [!DNL Commerce] database utilizzando le informazioni cliente corrispondenti dell&#39;ordine Amazon. Se hai scelto `No Customer Creation (guest)` nelle impostazioni dell&#39;ordine, l&#39;ordine segue il processo guest [!DNL Commerce] e non crea un cliente nel database. A questo punto, se il sistema [!DNL Commerce] è integrato con un ERP/OMS/WMS, l&#39;ordine viene rilevato in base all&#39;integrazione di un nuovo ordine che viene posizionato e creato all&#39;interno di [!DNL Commerce]. |
| 5 | **L&#39;ordine viene spedito.** Dalla pagina di elaborazione dell’ [!DNL Commerce] ordine, spedisci l’ordine e aggiungi un numero di tracciamento. Quando tutti gli elementi sono contrassegnati con uno stato `Shipped`:<ul><li>Lo stato dell&#39;ordine [!DNL Commerce] diventa `Complete`.</li><li>Lo stato dell&#39;ordine dei canali di vendita Amazon cambia in `Shipped`.</li><li>Il numero di tracciamento viene sincronizzato in Amazon e lo stato dell’ordine in Amazon cambia in `Shipped`.</li><li>Le notifiche di spedizione vengono inviate al cliente tramite Amazon, non da [!DNL Commerce] (in base alle politiche di Amazon). |

## Esempio: soddisfatto da Amazon (FBA)

| Passaggio | Descrizione |
|---|---|
| 1 | **Su Amazon viene effettuato un ordine soddisfatto da Amazon.** |
| 2 | **L&#39;ordine viene importato.** L’ordine non viene importato nel canale di vendita Amazon fino a quando Amazon non assegna all’ordine lo  `Shipped` stato . Poiché Amazon dispone dell’inventario per questo prodotto, evita interferenze con la gestione del magazzino/magazzino. |
| 1 | **I dettagli dell’ordine vengono aggiornati.** Se configurato nelle impostazioni [ ](./order-settings.md)dell’ordine, l’ordine Amazon crea l’ [!DNL Commerce] ordine corrispondente e viene creato come ordine con uno stato  `Complete`. |
