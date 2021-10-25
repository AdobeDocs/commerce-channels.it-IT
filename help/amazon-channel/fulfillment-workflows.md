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
| 1 | **Un ordine soddisfatto dal commerciante viene inserito su Amazon.** Amazon assegna uno stato di `Pending` fino alla verifica delle informazioni sulla carta di credito del cliente. Ordini in `Pending` lo stato viene importato automaticamente nel canale di vendita Amazon ma non viene visualizzato nel _[!UICONTROL Orders]_scheda . |
| 2 | **L’ordine è verificato da Amazon.** Quando viene verificato, Amazon cambia lo stato in `Unshipped`. Con questa modifica dello stato, l’ordine viene aggiornato nel canale di vendita Amazon e viene visualizzato nel _[!UICONTROL Orders]_scheda . |
| 3 | **I dettagli dell’ordine vengono aggiornati.** Il canale di vendita Amazon aggiorna i dettagli dell’ordine con il prezzo, l’e-mail del cliente e il nome del cliente. Durante questo aggiornamento, l’ordine Amazon crea il corrispondente [!DNL Commerce] nella pagina di gestione degli ordini. La [!DNL Commerce] viene visualizzato il numero dell&#39;ordine con le informazioni sull&#39;ordine nella _[!UICONTROL Orders]_scheda . |
| 4 | **Viene creato un nuovo account cliente.** Se configurato nelle impostazioni dell&#39;ordine e il cliente non esiste nel [!DNL Commerce] nel database viene creato un nuovo cliente [!DNL Commerce] database utilizzando le informazioni relative al cliente corrispondenti dell’ordine Amazon. Se hai scelto `No Customer Creation (guest)` nelle impostazioni dell&#39;ordine, l&#39;ordine segue [!DNL Commerce] processo guest e non creare un cliente nel database. A questo punto, se [!DNL Commerce] il sistema è integrato con un ERP/OMS/WMS, l&#39;ordine viene prelevato per l&#39;integrazione di un nuovo ordine che viene posizionato e creato all&#39;interno [!DNL Commerce]. |
| 5 | **L&#39;ordine viene spedito.** Da [!DNL Commerce] nella pagina di elaborazione dell&#39;ordine, spedisci l&#39;ordine e aggiungi un numero di tracciamento. Quando tutti gli elementi sono contrassegnati in un `Shipped` stato:<ul><li>Lo stato del [!DNL Commerce] modifica dell&#39;ordine in `Complete`.</li><li>Lo stato dell&#39;ordine del canale di vendita Amazon cambia in `Shipped`.</li><li>Il numero di tracciamento viene sincronizzato in Amazon e lo stato dell’ordine in Amazon cambia in `Shipped`.</li><li>Le notifiche di spedizione vengono inviate al cliente tramite Amazon, non da [!DNL Commerce] (in base ai criteri di Amazon). |

## Esempio: soddisfatto da Amazon (FBA)

| Passaggio | Descrizione |
|---|---|
| 1 | **Su Amazon viene effettuato un ordine soddisfatto da Amazon.** |
| 2 | **L&#39;ordine viene importato.** L&#39;ordine non viene importato nel canale di vendita Amazon finché non viene assegnato l&#39;ordine `Shipped` stato di Amazon. Poiché Amazon dispone dell’inventario per questo prodotto, evita interferenze con la gestione del magazzino/magazzino. |
| 3 | **I dettagli dell’ordine vengono aggiornati.** Se configurato nel [impostazioni ordine](./order-settings.md), l’ordine Amazon crea il corrispondente [!DNL Commerce] e vengono creati come ordine con uno stato `Complete`. |
