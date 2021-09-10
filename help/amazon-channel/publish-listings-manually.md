---
title: Pubblicare manualmente gli elenchi Amazon
description: Se necessario, puoi pubblicare manualmente gli annunci Amazon terminati dal tuo amministratore Commerce.
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Pubblicazione manuale degli elenchi di Amazon

Puoi pubblicare manualmente uno o più elenchi Amazon terminati.

1. Visualizza uno o più elenchi nella scheda _[!UICONTROL Ended]_della pagina [Elenco prodotti](./managing-product-listings.md) (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_o_[!UICONTROL Ineligible]_ ).

1. Nella colonna a sinistra, fai clic su per controllare ciascuno degli elenchi da ripubblicare.

1. In _[!UICONTROL Actions]_, fai clic su **[!UICONTROL Publish Product to Amazon]**.

1. Fai clic su **[!UICONTROL OK]** nel messaggio di conferma.

   Viene visualizzato un messaggio per confermare che gli elenchi selezionati sono in fase di elaborazione per la pubblicazione in Amazon.

   Le informazioni di elenco vengono pubblicate su Amazon in base alle impostazioni cron. Le informazioni sull’elenco vengono inviate ad Amazon alla successiva sincronizzazione dati. Fino a quando Amazon non risponde con la conferma dell’inserimento nell’elenco, gli elenchi pubblicati manualmente rimangono nella scheda _Ready to List_ con uno stato `List in Progress` . Quando Amazon riceve la conferma dell’inserimento nell’elenco, gli elenchi vengono spostati nella scheda _Attivo_ con uno stato `Active` .
