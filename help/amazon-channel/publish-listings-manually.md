---
title: Pubblicare manualmente le inserzioni in Amazon
description: Se necessario, puoi pubblicare manualmente le inserzioni Amazon scadute dall’amministratore di Commerce.
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Pubblicare manualmente le inserzioni in Amazon

Puoi pubblicare manualmente una o più inserzioni Amazon scadute.

1. Visualizza una o più inserzioni sul _[!UICONTROL Ended]_scheda della [Elenco prodotti](./managing-product-listings.md) page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, o_[!UICONTROL Ineligible]_ ).

1. Nella colonna sinistra, fai clic su per controllare ciascuna delle inserzioni che desideri ripubblicare.

1. Sotto _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Publish Product to Amazon]**.

1. Clic **[!UICONTROL OK]** nel messaggio di conferma.

   Viene visualizzato un messaggio per confermare che le inserzioni selezionate sono in fase di elaborazione per la pubblicazione in Amazon.

   Le informazioni sull’inserzione vengono pubblicate in Amazon in base alle impostazioni della tua cron. Le informazioni sull’inserzione vengono inviate ad Amazon alla prossima sincronizzazione dei dati. Fino a quando Amazon non risponde con la conferma dell’inserzione, le inserzioni pubblicate manualmente rimangono sul _Pronto per l&#39;elenco_ scheda con `List in Progress` stato. Quando la conferma dell’inserzione viene ricevuta da Amazon, le inserzioni vengono spostate nel _Attivo_ scheda con un `Active` stato.
