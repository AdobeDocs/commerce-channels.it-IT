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
| 1 | **Un ordine evaso da un commerciante è stato effettuato su Amazon.** Amazon assegna uno stato di `Pending` fino alla verifica delle informazioni sulla carta di credito del cliente. Gli ordini con lo stato `Pending` vengono importati automaticamente nel canale di vendita di Amazon, ma non vengono visualizzati nella scheda _[!UICONTROL Orders]_. |
| 2 | **L&#39;ordine è verificato da Amazon.** Dopo la verifica, Amazon cambia lo stato in `Unshipped`. Con questa modifica di stato, l&#39;ordine viene aggiornato nel canale di vendita di Amazon e viene visualizzato nella scheda _[!UICONTROL Orders]_. |
| 3 | **I dettagli dell&#39;ordine sono stati aggiornati.** Il canale di vendita Amazon aggiorna i dettagli dell&#39;ordine con il prezzo, l&#39;e-mail del cliente e il nome del cliente. Durante questo aggiornamento, l&#39;ordine Amazon crea l&#39;ordine [!DNL Commerce] corrispondente nella pagina di gestione degli ordini. Il numero di ordine [!DNL Commerce] viene visualizzato con le informazioni sull&#39;ordine nella scheda _[!UICONTROL Orders]_. |
| 4 | **È stato creato un nuovo account cliente.** Se è configurato nelle impostazioni dell&#39;ordine e il cliente non esiste nel database [!DNL Commerce], verrà creato un nuovo cliente nel database [!DNL Commerce] utilizzando le informazioni corrispondenti del cliente dell&#39;ordine Amazon. Se si sceglie `No Customer Creation (guest)` nelle impostazioni dell&#39;ordine, l&#39;ordine segue il processo guest [!DNL Commerce] e non crea un cliente nel database. A questo punto, se il sistema [!DNL Commerce] è integrato con un ERP/OMS/WMS, l&#39;ordine viene selezionato in base all&#39;integrazione di un nuovo ordine inserito e creato in [!DNL Commerce]. |
| 5 | **Ordine spedito.** Dalla pagina di elaborazione dell&#39;ordine [!DNL Commerce], spedisci l&#39;ordine e aggiungi un numero di registrazione. Quando tutti gli elementi sono contrassegnati con lo stato `Shipped`:<ul><li>Lo stato dell&#39;ordine [!DNL Commerce] cambia in `Complete`.</li><li>Lo stato dell&#39;ordine del canale di vendita Amazon diventa `Shipped`.</li><li>Il numero di tracciamento è sincronizzato in Amazon e lo stato dell&#39;ordine in Amazon cambia in `Shipped`.</li><li>Le notifiche di spedizione vengono inviate al cliente tramite Amazon, non da [!DNL Commerce] (in base ai criteri di Amazon). |

## Esempio: evaso da Amazon (FBA)

| Passaggio | Descrizione |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Un ordine eseguito da Amazon è stato effettuato su Amazon.** |
| 2 | **Ordine importato.** L&#39;ordine non viene importato nel canale di vendita di Amazon fino a quando Amazon non assegna all&#39;ordine lo stato `Shipped`. Poiché Amazon dispone dell&#39;inventario per questo prodotto, evita interferenze con la gestione di magazzino/inventario. |
| 3 | **I dettagli dell&#39;ordine sono stati aggiornati.** Se configurato nelle [impostazioni ordine](./order-settings.md), l&#39;ordine Amazon crea l&#39;ordine [!DNL Commerce] corrispondente e può essere creato come ordine con stato `Complete`. |
