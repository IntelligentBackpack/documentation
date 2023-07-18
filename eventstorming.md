# Event Storming
Durante una delle prime riunioni si è deciso di spendere un congruo tempo in anticipo per effettuare un brainstorming collettivo, per iniziare a disegnare i contorni del Domain Knowledge e delle tempistiche stimate sul sistema da realizzare. Esplorando il dominio per la prima volta infatti, è risultata in un'attività fondamentale per delineare concetti, opportunità, attori e sistemi esterni, su cui ci siamo poi basati per gli sviluppi futuri sia lato progettazione, sia implementazione. Alla sessione di Event Storming ha partecipato l'intero team di sviluppo e gli esperti di dominio.
Abbiamo adottato il classico sistema di <i> Sticky Notes </i>, in un ambiente virtuale e collaborativo offerto dallo strumento online Lucidchart. 

Per una migliore lettura della lavagna virtuale di post-it, a lato è presente una leggenda, molto similare a quella convenzionale, che associa il colore del post-it utilizzando al suo significato.

<img src="https://lucid.app/publicSegments/view/03a8b62d-c0ea-4cd0-956a-fa881d82025f/image.png" style="width:100%; height: auto; border-style: solid;"> </img>

Come possiamo notare, sono rappresentate una serie di informazioni fondamentali, necessarie per una comprensione iniziale del dominio e una base da cui partire per una ulteriore analisi più raffinata. Per quanto riguarda l'andamento temporale che si è supposto fin da subito, risulta abbastanza parallelizzabile in termini di task da portare a termine, partendo da due <i> swim lanes </i> fino ad arrivare alla fine con circa quattro linee di sviluppo separate.
In particolare si possono già notare i cosiddetti <i> Pivotal Events </i>, ovvero gli eventi ritenuti più importanti che si dovranno gestire nel corso dello sviluppo e che rappresenteranno delle milestone nel progetto:
- Gestione della creazione di un'utente e di un registro utenti (stessa cosa per gli owner del sistema)
- Gestione dei calendari
- Insieme di funzionalità che permettono all'utente di gestire il proprio materiale personale all'interno dello zaino intelligente, come registrare oggetti nuovi quali libri e registrare un nuovo zaino
- Sviluppo dell'interazione tra lo zaino intelligente e l'utente (ad esempio inserimento oggetti)

## Emerging Bounded Context
Com'è possibile notare, si distinguono visibilmente degli agglomerati di post-it, i quali rappresentano primi indicatori dei possibili Bounded Context che andremo a progettare, un punto di partenza per un'analisi più approfondita.
Più in particolare, questi agglomerati di eventi simili possono essere raggruppati per tipologie, in modo tra l'altro molto simile alle swim lanes individuate:
- Gestione dei libri riconosciuti dal sistema
- Gestione dei ruoli degli utenti e tutte le possibili azioni che potranno effettuare sul sistema
- Tutto ciò che riguarda i calendari, lezioni e giorni scolastici
- Gestione del proprio materiale da parte degli studenti e professori
- Notifica di elementi mancanti nello zaino a fronte di una lista di oggetti richiesti
- Gestione dello zaino, del contenuto e del suo aggiornamento di stato

## Opportunità
Sono state individuate due opportunità, ovvero due possibili requisiti non indicati nella richiesta di progetto del committente, ma comunque aspetti di valore che potrebbero essere sviluppate in un secondo momento grazie alla terminazione di un qualche componente, che ne rivela appunto il possibile valore e l'effettiva possibilità di realizzazione.
Uno di questi è la possibilità di eliminare tutte le lezioni in un certo periodo di tempo per determinate materie, opportunità che richiede almeno l'implementazione della semplice aggiunta, rimozione o swap di lezioni in un preciso giorno, stando quindi a rappresentare una funzionalità aggiunta di possibile interesse per il cliente ma non richiesta.
La seconda riguarda invece un hotspot, ovvero una questione con pensieri conflittuali all'interno del team e che non trova un'effettivo riscontro nella richiesta del committente: in questo caso parliamo della possibilità di creare un proprio evento da parte dello studente, ovvero la possibilità di creare un evento (come una lezione ma non necessariamente) che richieda del materiale necessario da avere con se. Questo hotspot, se implementato, potrebbe dar vita ad una opportunità, ovvero rendere l'applicazione e l'intero sistema, più propenso ad un utilizzo generico, collegabile ad un calendario personale oltre che ad un calendario scolastico.