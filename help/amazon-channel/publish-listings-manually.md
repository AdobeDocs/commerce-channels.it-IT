---
title: Pubblicare manualmente le inserzioni in Amazon
description: Se necessario, puoi pubblicare manualmente le inserzioni Amazon scadute dall’amministratore Commerce.
feature: Sales Channels, Products, Merchandising
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Pubblicare manualmente le inserzioni in Amazon

Puoi pubblicare manualmente una o più inserzioni Amazon scadute.

1. Visualizza una o più inserzioni nella scheda _[!UICONTROL Ended]_della pagina [Inserzioni prodotto](./managing-product-listings.md) (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_o_[!UICONTROL Ineligible]_).

1. Nella colonna sinistra, fai clic su per controllare ciascuna delle inserzioni che desideri ripubblicare.

1. In _[!UICONTROL Actions]_, fare clic su **[!UICONTROL Publish Product to Amazon]**.

1. Fare clic su **[!UICONTROL OK]** nel messaggio di conferma.

   Viene visualizzato un messaggio per confermare che le inserzioni selezionate sono in fase di elaborazione per la pubblicazione in Amazon.

   Le informazioni sull’inserzione vengono pubblicate in Amazon in base alle impostazioni della tua cron. Le informazioni sull’inserzione vengono inviate ad Amazon alla prossima sincronizzazione dei dati. Fino a quando Amazon non risponde con la conferma dell&#39;inserzione, le inserzioni pubblicate manualmente rimangono nella scheda _Pronto per l&#39;elenco_ con lo stato `List in Progress`. Quando la conferma dell&#39;inserzione viene ricevuta da Amazon, le inserzioni vengono spostate nella scheda _Active_ con stato `Active`.
