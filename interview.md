---
title: Knowledge Crunching
layout: default
nav_order: 1
---

# Knowledge Crunching
La primissima fase per un buon design di qualsiasi progetto è rappresentata dal processo di Knowledge Crunching, ovvero l'arte di rilevare e carpire le informazioni più importanti e sui quali porre più attenzione dal dominio in studio. Quest'attività ci ha portato a creare i modelli corretti e la definizione dei casi d'uso che rispecchiamo il modello e le logiche di business.
Tramite questa operazione siamo in grado anche di separare i concetti e argomento meno conosciuti (<i> technical gaps </i>), quelli che generano più dubbi sulla loro natura o possibile realizzazione, in modo da esplorarli a fondo per una visione a 360 gradi di tutto il dominio. L'aspetto chiave nel Knowledge Crunching è la collaborazione, per cui sono state organizzate discussioni di gruppo in cui esperti di dominio, analisti e team di sviluppo si sono incontrati semplicemente per parlare e chiarire tutti gli aspetti importanti, tramite interviste opportune, il cui estratto è riportato di seguito.

## Interviste

### Ambiente scolastico

<b> Ciao! Raccontaci un po' dell'ambiente scolastico, chi organizza le lezioni? </b> <br>
Le lezioni vengono di norma gestite dalla segreteria, che ha la responsabilità di gestire l'orario delle lezioni durante l'anno. Per effettuare ciò, si avvale di diverse azioni. Vorremmo includere in questa attività anche i professori, in modo che siano in grado di spostare lezioni o modificarne in totale autonomia, in modo veloce e facile e cosicché gli studenti possano saperlo in tempi brevi.

<b> Perfetto, quali meccanismi prevedono la gestione delle lezioni? </b> <br>
Un professore per definire una lezione deve specificare la materia di interesse e il giorno della settimana in cui si svolge, ripetuta nelle settimane del ciclo scolastico annuale, l'orario d'inizio, quello di fine e la classe che dovrà frequentarla.

<b> Chiarissimo, per quanto riguarda invece modifiche al calendario, quali sono ammesse e come dovrebbero esser gestite? </b> <br>
Diciamo che in generale le operazioni che si vogliono effettuare sono le classiche, ovvero aggiungere o rimuovere una o più lezione, che sia solo di un giorno o di un interavallo.
Inoltre è possibile che le lezioni vengano spostate una da un determinato giorno e orario ad una nuova posizione nel calendario, anche in questo caso può essere per un solo giorno o per più gioni (periodo).

<b> Interessante, stessa cosa vale anche per il materiale necessario in una determinata lezione? </b> <br>
Assolutamente, si vuole lasciare piena libertà lato professore, esso deve poter cambiare il materiale disponibile per una data lezione in caso di errore di inserimento o cambi di programma.

<b> Quindi, se ho capito bene, c'è differenza tra giorno settimanale e data di una lezione </b> <br>
Un calendario settimanale mostra i giorni della settimana e gli orari in cui si svolgono lezione in quelli giorni, ripetute quindi durante l'anno ogni settimana. Un giorno è definito come l'etichetta del giorno settimanale in questione e un orario, invece una data  rappresenta un giorno specifico ben formattato seguendo le tipiche convenzioni di rappresentazione. Una lezione è riferita ad un giorno settimanale, quindi è ripetuta, ecco perché è presente il periodo di riferimento con inizio e fine.

<b> Quindi, quando si chiede le lezioni in giorno bisogna sia considerare le lezioni che sono presenti in quell'giorno della settimana che quelle in quella data, giusto? </b> <br>
Esattamente, bisogna anche tenere conto dei cambiamenti apportati all'orario.
Come detto prima le lezioni possono essere aggiunte, cancellate o spostate.

<b> Perfetto, passiamo ad un aspetto un po' più interessante per gli studenti: come deve esser gestito il materiale da portare a lezione? </b> <br>
Uno studente, accedendo al proprio profilo, vedrà le lezioni dell'anno scolastico o corso, insieme al materiale assegnato da portare ripetutamente per quella lezione, ovvero ad esempio nelle lezioni di mercoledi alle ore 9:00.
Nel caso generale si tratta di libri e quindi gli studenti dovranno portare la propria copia del libro.

<b> Quindi, dato un titolo di libro, o magari meglio ancora un codice univoco come l'ISBN lo studente deve portare la propria copia? </b> <br>
Esatto, ovviamente la copia è personale per ogni studente.

<b> É possibile identificare una copia di un libro di uno studente? </b> <br>
Alcuni studente mettono il nome all'interno, ma in generele le copie sono identiche tra di loro.

<i> Considerazioni </i>
Dall'intervista precendente risulta evidente che sia necessario idetificare in qualche modo le copie dei libri degli studenti. Per questo motivo si decide si usare la tecnologia RFID mettendo un tag univoco all'interno della copia del libro in modo da inentificarla dalle altre.


### Tipi di utenti
<b> Cambiando tematica, quali sono i tipi di utenti che vorreste differenziare? </b> <br>
Sono due i tipi di utenti finali del servizio che vorremmo offrire, ovvero lo studente e il professore, entrambi potranno accedere alla piattaforma tramite una semplice applicazione mobile.

<b> Immagino abbiano ruoli e quindi funzionalità diverse all'interno del sistema </b> <br>
Esattamente, uno studente, essendo iscritto in un istituto e in una classe, potrà vedere il suo calendario di lezioni programmato e il materiale necessario da portare per una data lezione. Un professore, al contrario, avrà la possibilità di gestire i calendari delle proprie classi e aggiornare il materiale necessario per una data lezione.

<b> Avranno anche funzionalità in comune... </b> <br>
Si, è esatto. Sia studente che professore dovrebbero avere uno zaino intelligente, quindi entrambi i tipi di utenti possono gestire il proprio zaino dall'applicazione mobile, inserire oggetti e vedere il contenuto realtime, nonché esser notificato in qualche modo in caso manchi qualche materiale per la lezione del giorno dopo.

### Peculiarità del sistema che si vuole realizzare
<b> Ci spieghi la sua idea di zaino che vorrebbe </b> <br>
Uno zaino intelligente lo immagino proprio come uno classico, sarebbe l'ideale avere tecnologia presente ma non visibile e non fastidiosa per lo studente (o professore) che ne fa utilizzo.

<b> Quali interazioni si aspetta tra lo zaino e lo smartphone? </b> <br>
Qualsiasi operazione naturale venga fatta con uno zaino classico, ovvero aggiungere e rimuovere oggetti o libri, in modo più naturale possibile, anche se un minimo di abitudine nell'inserirli con cautela è necessario, per ovvie ragioni di lettura del materiale inserito. Infine l'applicazione mobile dovrebbe mostrare in tempo reale, o quasi, il contenuto dello zaino e fornire tutte le funzionalità già discusse.

<b> Quindi, se ho capito bene, il cloud ha un aspetto fondamentale. L'applicazione mobile invece? Quali funzionalità pensa che dovrebbe avere? </b> <br>
Oltre a quelle elencate nella richiesta e nelle precedenti domande, una bella comodità sarebbe rappresentata dal poter registrare uno zaino per un determinato studente sfruttando l'applicazione, senza interazioni dirette con lo zaino, come ad esempio la scannerizzazione di un codice, veloce e intuitivo.

## Impact Mapping
Per avere un'iniziale chiara visione del dominio su cui il sistema opererà, si è scelto di cominciare nelle prime riunioni a fare mente locale con un piccolo brainstorming collettivo, trascrivendo su una mappa concettuale tutte le idee che sorgevano.

In particolare, dalla mappa si riesce già a delineare quali saranno le attività principali che rappresenteranno le principali milestone del progetto, quali sono le attività più corpose (interne, riassumibili nel completamento di una milestone) e quelle più basilari (esterne alla rete, rappresentano funzionalità base) e quali sono i requisiti che vincolano le varie attività.

<center><img src="https://lucid.app/publicSegments/view/98b306f7-c90c-4b41-b69e-9e5a67920b1c/image.png" style="width:100%; height: auto; border-style: solid;"> </center>