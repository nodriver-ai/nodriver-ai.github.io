---
title: Come programmare le irrigazioni con Irreo analizzando il bilanciamento idrico sui tuoi terreni?
date: 2021-05-10 10:28:00 Z
categories:
- Irrigation
subtitle: Come utilizzare Irreo per programmare in maniera ottimale le irrigazioni attraverso il bilanciamento idrico del suolo senza installare nessun sensore sui propri appezzamenti
card-title: Scopri quando è il momento ottimale per irrigare, monitorando il bilancio idrico sui tuoi appezzamenti.
image: "/uploads/blog2.png"
layout: post
---
Il fabbisogno d'acqua di una coltura in crescita vegetativa deve essere soddisfatto per raggiungere massime rese e aumentare la qualità dei prodotti finali.  
Come abbiamo visto nel precedente [articolo]({{ site.baseurl }}{% link _posts/2021-04-12-cose-levapotraspirazione-e-come-si-usa-per-programmare-le-irrigazioni.markdown %}), il fabbisogno idrico è anche chiamato [evapotraspirazione]({{ site.baseurl }}{% link _posts/2021-04-12-cose-levapotraspirazione-e-come-si-usa-per-programmare-le-irrigazioni.markdown %}) delle colture ed è solitamente rappresentato come ET<sub>c</sub>.
Tale fabbisogno può essere fornito dall'acqua immagazzinata nel suolo, dalle precipitazioni e dall'irrigazione. L'irrigazione è necessaria quando l'ET<sub>c</sub> (la domanda d'acqua delle colture) supera la fornitura d'acqua del suolo e delle precipitazioni.
Poiché l'ET<sub>c</sub> varia con lo stadio di sviluppo della coltura e delle condizioni meteorologiche, decidere sia la quantità che i tempi di irrigazione ottimali diventa fondamentale.

Il suolo nella zona delle radici ha un limite superiore e un limite inferiore di acqua che può immagazzinare e che può essere usata dalle colture. Il limite superiore è chiamato **capacità di campo** (FC), che è la quantità di acqua che può essere trattenuta dal suolo contro la gravità dopo essere stata saturata e drenata. Il limite inferiore è chiamato **punto di appassimento permanente** (WP), che è la quantità di acqua che rimane nel suolo quando la pianta appassisce definitivamente perché non può più estrarre acqua. La **capacità idrica disponibile** (TAW), o acqua totale disponibile, del suolo è la quantità di acqua tra questi due limiti (AWC = FC - PWP) ed è la quantità massima di acqua che può essere estratta dalle piante dal suolo.
<p align="center">
<img src="/uploads/Diapositiva2.png">
</p>

Questi paramentri sono difficili da stimare sul campo, infatti i metodi tradizionali richiedono uso di sonde, analisi del suolo in laboratorio e di diversi calcoli manuali da effettuare, il risultato è un processo complicato e costoso, che richiede oltretutto molto tempo. Combinando diversi dati satellitari ed algoritmi sviluppati internamente, [Irreo](https://irreo.nodriver.ai) è in grado di stimare la struttura del suolo sotto la copertura fogliare, monitorare il processo di infiltrazione dell'acqua e quindi stimare in maniera **completamente automatica** e senza **nessun sensore da installare** la capacità di campo, il punto di appassimento permanente e la capacità idrica disponibile.

### Come funziona il bilanciamento idrico del suolo?
Man mano che la coltura cresce ed estrae acqua dal suolo per soddisfare il suo fabbisogno di ET<sub>c</sub>, l'acqua immagazzinata nel suolo si esaurisce gradualmente. In generale, il fabbisogno irriguo netto è la quantità d'acqua necessaria per riportare nuovamente il contenuto d'acqua del suolo nella zona delle radici fino alla capacità del campo. Questa quantità, che è la differenza tra la capacità del campo e il livello attuale di acqua del suolo, corrisponde al **deficit idrico** del suolo (D). Il responsabile dell'irrigazione deve tenere traccia di D, dato che corrisponde alla quantità netta di acqua da applicare attraverso l'irrigazione. 
Su base giornaliera, D può essere stimato usando la seguente formula che tiene conto di tutti gli elementi che incidono sul deficit idrico del suolo nella zona delle radici:

<img src="http://www.sciweavers.org/tex2img.php?eq=D_c = D_p %2B ET_c - P - Irr %2B RO %2B DP&bc=White&fc=Black&im=jpg&fs=16&ff=arev&edit=" style="margin-bottom: 0;">

dove D<sub>c</sub> è il deficit idrico del suolo (fabbisogno irriguo netto) nella zona delle radici, D<sub>p</sub> è il deficit idrico del giorno precedente, ET<sub>c</sub> è il tasso di evapotraspirazione della coltura, P corrisponde alle precipitazioni, Irr è la quantità netta di irrigazione infiltrata nel suolo per il giorno corrente, RO è il deflusso superficiale e DP è la percolazione dell’acqua in profondità o il drenaggio.
Utilizzando [Irreo](https://irreo.nodriver.ai) potrai **monitorare giornalmente i valori di deficit idrico** sul tuo appezzamento senza costosi sensori e centraline meteo da installare e manutenere. Infatti analizzando dati satellitari multispettrali, termici e meteorologici siamo in grado di stimare le precipitazioni e l'ET<sub>c</sub> giornaliera ed attraverso diversi modelli idrologici il deflusso superficiale e il drenaggio dell'acqua sul particolare terreno.

### Come scegliere la propria startegie di irrigazione con Irreo
Scegliere la propria strategia di irrigazione, significa capire quando è il momento ottimale per irrigare con l'obiettivo di evitare che le colture soffrino di stress idrico.
Per capire ciò bisogna considerare che solo una percentuale della TAW può essere esaurita prima che la coltura inizi a sperimentare stress idrico. Pertanto, deve essere scelta una **soglia di intervento**, ovvero la quantità massima di deficit idrico consentito. Tale soglia può essere espressa anche come una percentuale della TAW.

Considerando la composizione del terreno, il tipo di coltura e lo stato fenologico, [Irreo](https://irreo.nodriver.ai) stima la **soglia di intervento ottimale**, chiamata RAW, ovvero la percentuale di acqua disponibile nel suolo che può essere esaurita tra due
interventi irrigui successivi senza che la coltura soffri di stress idrico.

<p align="center">
<img src="/uploads/diapositiva3.gif">
</p>

Allo stesso tempo, [Irreo](https://irreo.nodriver.ai) consente agli agricoltori di decidere e **personalizzare la soglia di intervento** a seconda delle proprie strategie irrigue. Ad esempio, se si possiede un sistema di irrigazione che ha una portata inferiore alla RAW consigliata, allora l'agricoltore può diminuire la soglia di intervento ed impostarla uguale alla portata massima in millimetri che il proprio impianto è in grado di effettuare in un singolo turno irriguo. Chiaramente diminuire la soglia di intervento sotto il valore della RAW porta ad irrigazioni più frequenti. 
<p align="center">
<img src="/uploads/diapositiva4.gif">
</p>

Se invece si vuole attuare una startegia di irrigazione a **deficit controllato**, l'agricoltore può aumentare la soglia di intervento superando la RAW. Chiaramente attuando tale strategia bisogna stare attenti a non provocare eccessivi stress che potrebbero comportare una diminuizione dell'evapotranspirazione e di conseguenza anche la biomassa prodotta.
<p align="center">
<img src="/uploads/diapositiva5.gif">
</p>


