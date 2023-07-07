<details open>
<summary>Analisi Domain Driven</summary>

* <a href="eventstorming.html"> Event Storming </a>
* <a href="boundedcontext.html"> Bounded Contexts </a>
* Sub-Domain

</details>

# Analisi Domain Driven Design
Come punto di partenza per l'analisi del dominio, si è deciso di partire dai casi d'uso del sistema che si vuole progettare, per capire al meglio quali sono le operazioni che gli utenti vedono e vogliono eseguire e quali attori sono coinvolti. L'importanza del loro utilizzo sta nell'identificare (a caratteri generali) quali attori sono coinvolti nelle varie operazioni e quali sono le principali azioni che devono essere sviluppate e/o sulle quali avere maggior riguardo. Per realizzare i casi d'uso c'è stata una forte collaborazione del team con i committenti, sfruttando svariate riunioni, che si sono poi ripetute abitualmente.
## Interazione tra utente e zaino intelligente
Nel seguente schema sono rappresentate le interazioni di un generico attore User e lo zaino intelligente con il sistema.
In particolare:
- L'attore User (studente o professore) può effettuare operazioni come aggiungere o rimuovere un oggetto nello zaino e verificare il materiale interno, per confrontarlo con quello necessario al giorno successivo. E' colui che possiede uno zaino intelligente (Smart Bagpack) e che effettua le operazioni che ne cambiano lo stato, quali aggiunta e rimozione di un oggetto
- Lo zaino viene notificato quando viene aggiunto o rimosso un elemento al suo interno e notifica l'utente qualora si fosse dimenticato un oggetto; questo attore rappresenta lo zaino, la sua componente smart, la quale è aperto a interazioni con l'utente esterno e possiede capacità di connessione per comunicare con l'esterno
<center><img src="https://lucid.app/publicSegments/view/c97f432e-905e-4671-8709-f5471451ed52/image.png" style="width:50%; height: auto; border-style: solid;"> </img></center>

## Gestione istituti e lezioni
Per quanto riguarda invece la gestione degli istituti e lezioni (con conseguente gestione del materiale necessario), dopo una riunione collaborativo si è realizzato il seguente schema Use Case, che mostra i casi d'uso e l'interazione tra i seguenti attori:
- Vendor: è l'attore che identifica un qualsiasi editore di libri; entità che può aggiungere libri con il suo codice ISBN e informazioni standard come titolo
- Istituto: entità che rappresenta un istituto scolastico, il quale detiene la facoltà di eseguire operazioni quali la possibilità di aggiungere/rimuovere e modificare il ruolo dei singoli utenti
- Professore: attore che gestisce le lezioni e tutto ciò che ne compete, può gestire più classi, calendari, materie
- Owner: amministratore del sistema, il quale può aggiungere istituti
- Studente: oltre ad utilizzare lo zaino, può accedere alle materie, calendario e libri necessari per una specifica lezione
<center><img src="https://lucid.app/publicSegments/view/0f28296b-50a1-418c-bec0-d2e30e68c930/image.png" style="width:50%; height: auto; border-style: solid;"> </img></center>

Uno dei principali requisiti che sono scaturiti dagli use cases è la necessità di avere un'utente generale non assegnato a nessun ruolo. Infatti, tutte le azioni del professore e dello studente, possono essere generalizzate e messe sotto permessi speciali, tramite l'utilizzo di un'utente generico che le accomuna. Saranno poi gli istituti, mediante i loro permessi, a modificare i ruoli degli utenti, assegnando studente o professore a seconda di quello che l'utente deve rappresentare.

In particolare, sono stati individuati 5 tipi di utenti diversi con diversi gradi di importanza all'interno del sistema:
- User: Rappresenta l'utente generico, non specializzato e che non appartiene a nessun istituto, rappresenta il ruolo minimo all'interno del sistema;
- Studente: Rappresenta un utente che studia presso un istituto;
- Professore: Rappresenta un utente che lavora come professore presso un istituto. Seguendo i requisiti del problema, non è stato definito alcun vincolo riguardante il professore che può partecipare solamente ad un istituto;
- Istituto: Rappresentazione di una entità in grado di gestire tutti i ruoli e azioni di alto livello sugli utenti che sono registrati al sistema;
- Owner: Entità che rappresenta il proprietario del sistema o tutte le persone che ci possono accedere con i permessi di admin.
