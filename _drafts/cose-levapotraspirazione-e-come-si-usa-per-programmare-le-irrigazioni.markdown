---
title: Cos'è l'evapotraspirazione e come si usa per programmare le irrigazioni?
date: 2021-03-09 10:04:00 Z
categories:
- Irrigation
subtitle: Le informazioni sull'evapotraspirazione possono essere usate dagli agricoltori
  per programmare più accuratamente le irrigazioni con l'obiettivo di raggiungere
  le massime rese e migliorare l'efficienza idrica.
image: "/uploads/Schermata%202021-03-16%20alle%2012.56.30.png"
layout: post
---

L'evapotraspirazione (ET) rappresenta il consumo d'acqua di un terreno dovuto alla combinazione di due processi: l'acqua viene persa da un lato dalla superficie del suolo per evaporazione e dall'altro lato dalla coltura per traspirazione. I valori di ET sono tipicamente misurati in millimetri al giorno (mm/giorno) e sono più alti nei mesi estivi e relativamente più bassi in primavera ed autunno. Inoltre i principali fattori che influiscono sul suo valore sono la luce del sole, il vento, l'umidità e la temperatura.

<p align="center">
<img src="/uploads/Schermata%202021-03-09%20alle%2011.57.16.png">
</p>

### Perché dovrei voler usare l'ET per programmare le irrigazioni?
Le informazioni sull'ET permettono agli agricoltori di adattare meglio le irrigazioni alle esigenze delle colture in crescita vegetativa, aiutando così ad ottenere rese maggiori e a migliorare l'efficienza irrigua. Monitorare giornalmente i valori di ET aiuta ad eliminare le incertezze nell'irrigazione. Un piccolo, ma regolare miglioramento nella programmazione dell'irrigazione può aumentare significativamente la produzione e la qualità complessiva delle colture.
Un altro vantaggio dell'uso dell'ET è che i valori sono rilevanti per un intero appezzamento e non in un singolo punto, come nel caso dei sensori di umidità del suolo. Questo permette una programmazione accurata dell'irrigazione considerando la variabilità del tipo di suolo, la capacità di ritenzione idrica del suolo, i tassi di estrazione dell'acqua e l'uniformità dell'irrigazione.

L'animazione in basso mostra la variazione dei valori di ET giornalieri in un terreno coltivato a soia, generati dalla [piattaforma web Irreo](https://irreo.nodriver.ai).  
I valori di ET sono stimati utilizzando diversi **dati satellitari** e vengono forniti all'agricoltore **giornalmente con una risoluzione spaziale di 10 metri** (ogni pixel nell'immagine corrisponde ad un area di 100 metri quadrati).

<p align="center">
<img src="/uploads/gif2.gif">
</p>

Senza informazioni oggettive può essere difficile stabilire il momento migliore per programmare le irrigazioni. Per gli agricoltori è particolare importante fare attenzione ai dati di ET sopratutto nel periodo estivo, quando le richieste d'acqua delle colture sono elevate e i tassi di crescita sono più sensibili alle irrigazioni ritardate.

### Quali sono i principi di base dell'uso della ET per la programmazione dell'irrigazione?

Per far corrispondere l'irrigazione alle esigenze delle colture in crescita vegetativa, l'irrigazioni devono essere programmate in relazione alla **quantità di acqua nel terreno che è prontamente disponibile** per le piante (nota anche come "Readily Available Water" o "RAW").
La RAW è la componente dell'umidità del suolo che può essere prontamente estratta dalle piante prima che soffrano di stress da umidità e di tassi di crescita inferiori.
Il concetto di base è che man mano che le piante estraggono acqua (il cui valore può essere stimato utilizzando i dati di ET giornalieri), il contenuto idrico del suolo diminuisce e raggiunge un valore di soglia oltre il quale l'acqua diventa più fortemente legata al suolo e più difficile da estrarre. 

Quando l'estrazione cumulativa di acqua supera il valore RAW, l'acqua del suolo non può più essere estratta abbastanza rapidamente per soddisfare le esigenze idriche delle colture in crescita vegetativa. Inoltre c'è il rischio di una "siccità verde" se l'intervallo di irrigazione è "allungato" e l'estrazione cumulativa di acqua supera il valore stimato di RAW. Se questo accade, le piante possono apparire sane, ma la crescita è compromessa. Nel caso estremo senza irrigazione o pioggia, alla fine si raggiunge un punto in cui l'assorbimento dell'acqua è zero e le piante appassiscono e muoiono definitivamente.
In genere la RAW varia a seconda della coltura e del tipo di suolo. Ad esempio per il mais ci saranno in genere fino a 60-70 mm di RAW, mentre per l'erba medica la RAW tende ad essere nell'intervallo da 70mm a 100mm.

I metodi tradizionali per il calcolo della RAW su un particolare terreno richiedono l'uso di sonde tensiometriche e di diversi calcoli manuali da effettuare, il risultato è un processo complicato e che richiede molto tempo.
Gli agricoltori da oggi possono usare [Irreo](https://irreo.nodriver.ai) per conoscere esattamente il valore della RAW su un particolare terreno, senza aver bisogno di **nessun sensore da installare** e in maniera **completamente automatica**.  
Questo è possibile grazie alla nostra tecnologia, che combinando diversi dati satellitari ed algoritmi di ["Machine Learning"](https://it.wikipedia.org/wiki/Apprendimento_automatico), è in grado di stimare la struttura del suolo sotto la copertura fogliare, monitorando il processo di infiltrazione dell'acqua. Questo permette ai nostri utenti di analizzare diverse variabili relative all'umidità del suolo, come **la capacità di campo** (FC), il **punto di appassimento permanente** (WP), il **contenuto di acqua prontamente disponibile** (RAW) e **l'acqua totale disponibile** (TAW).

<p align="center">
<img src="/uploads/Schermata%202021-03-17%20alle%2011.45.53.png">
</p>

### Come posso usare i valori di ET per programmare le irrigazioni?
Il momento ottimale per effettuare l'irrigazione è determinato sottraendo i valori giornalieri di ET dal valore massimo stimato della RAW (per esempio, 40 mm), fino a quando il valore diventa prossimo allo zero. Quando il valore della RAW  si trova vicino allo zero, è il momento di irrigare di nuovo. 
Oltre all'assorbimento dell'acqua da parte delle piante, chiaramente anche le precipitazioni influenzano i valori della RAW, dato che provocano un'aumento del contenuto di acqua nel suolo. Inoltre le precipitazioni che non contribuiscono alla riserva di umidità disponibile delle colture (precipitazioni "inefficaci") non dovrebbero essere considerate. Per esempio, la quantità di precipitazioni che viene persa a causa del deflusso superficiale o che tramite infiltrazione supera la zona delle radici deve essere ignorata.

<span class="img_container center" style="display: block;">
<img alt="test" src="/uploads/Schermata%202021-03-17%20alle%2015.02.15.png" style="display:block; margin-left: auto; margin-right: auto;" title="caption" />
<span class="img_caption" style="display: block; text-align: center;">caption</span>
</span>

![tabella](/uploads/Schermata%202021-03-17%20alle%2015.02.15.png)

![grafico](/uploads/graph.png)

[da dove posso iniziare -- Irreo]