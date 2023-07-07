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
