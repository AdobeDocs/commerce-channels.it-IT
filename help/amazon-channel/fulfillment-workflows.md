---
title: Flussi di lavoro di evasione di Amazon
description: L'evasione di un ordine da un'inserzione Amazon segue una sequenza specifica dalla sottomissione dell'ordine alla spedizione.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Flussi di lavoro di evasione di Amazon

## Esempio: evaso dal commerciante

| Passaggio | Descrizione |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Un ordine evaso da un esercente viene effettuato su Amazon.** Amazon assegna uno stato di `Pending` fino alla verifica delle informazioni sulla carta di credito del cliente. Ordini in `Pending` lo stato viene importato automaticamente nel canale di vendita di Amazon, ma non viene visualizzato nel _[!UICONTROL Orders]_scheda. |
| 2 | **L’ordine viene verificato da Amazon.** Una volta verificata, Amazon modifica lo stato in `Unshipped`. Con questa modifica di stato, l’ordine viene aggiornato nel canale di vendita di Amazon e viene visualizzato nel _[!UICONTROL Orders]_scheda. |
| 3 | **I dettagli dell’ordine vengono aggiornati.** Il canale di vendita Amazon aggiorna i dettagli dell’ordine con il prezzo, l’e-mail del cliente e il nome del cliente. Durante questo aggiornamento, l’ordine Amazon crea il corrispondente [!DNL Commerce] ordina nella pagina di gestione degli ordini. Il [!DNL Commerce] viene visualizzato il numero dell&#39;ordine con le informazioni sull&#39;ordine _[!UICONTROL Orders]_scheda. |
| 4 | **Viene creato un nuovo account cliente.** Se configurato nelle impostazioni dell&#39;ordine e il cliente non esiste nel tuo [!DNL Commerce] database, viene creato un nuovo cliente nel tuo [!DNL Commerce] utilizzando le informazioni corrispondenti sul cliente dell’ordine di Amazon. Se si sceglie `No Customer Creation (guest)` nelle impostazioni dell’ordine, l’ordine segue il [!DNL Commerce] processo guest e non creare un cliente nel database. A questo punto, se [!DNL Commerce] è integrato con un ERP/OMS/WMS, l&#39;ordine viene selezionato in base all&#39;integrazione di un nuovo ordine inserito e creato all&#39;interno [!DNL Commerce]. |
| 5 | **L&#39;ordine viene spedito.** Dalla sezione [!DNL Commerce] pagina di elaborazione dell&#39;ordine, spedisci l&#39;ordine e aggiungi un numero di tracciamento. Quando tutti gli elementi sono contrassegnati in un `Shipped` stato:<ul><li>Stato del [!DNL Commerce] ordina le modifiche in `Complete`.</li><li>Lo stato dell’ordine del canale di vendita Amazon cambia in `Shipped`.</li><li>Il numero di tracciamento viene sincronizzato in Amazon e lo stato dell’ordine in Amazon cambia in `Shipped`.</li><li>Le notifiche di spedizione vengono inviate al cliente tramite Amazon, non da [!DNL Commerce] (in base ai criteri di Amazon). |

## Esempio: evaso da Amazon (FBA)

| Passaggio | Descrizione |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Un ordine evaso da Amazon viene effettuato su Amazon.** |
| 2 | **L’ordine viene importato.** L’ordine viene importato nel canale di vendita di Amazon solo dopo che gli è stato assegnato l’ordine `Shipped` stato di Amazon. Poiché Amazon dispone dell&#39;inventario per questo prodotto, evita interferenze con la gestione di magazzino/inventario. |
| 3 | **I dettagli dell’ordine vengono aggiornati.** Se configurato in [impostazioni ordine](./order-settings.md), l’ordine Amazon crea il corrispondente [!DNL Commerce] e deve essere creato come ordine con lo stato `Complete`. |
