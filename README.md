<details open>
<summary>Analisi Domain Driven</summary>

* <a href="interview.md"> Interviste </a>
* <a href="eventstorming.md"> Event Storming </a>
* <a href="index.md"> Use cases </a>
* <a href="userstories.md"> Domain Story Telling </a>
* <a href="boundedcontext.md"> Bounded Contexts </a>
* Sub-Domain

</details>

# Analisi Domain Driven Design
Questo repository mostra la documentazione generata da tutto il processo di analisi in ottica DDD, quindi design guidato interamente dal dominio, dai cosiddetti Domain Expert ai Bounded Context per definire sottodomini indipendenti da associare a possibili team di sviluppo separati e paralleli.
Seguendo l’approccio di sviluppo Domain Driven, si è partiti dalla fase fondamen-
tale di analisi del dominio, dettagliando e snocciolando la domain knowledge per
ridurre il rischio di incomprensioni, lack of knowledge e requisiti errati. Siamo
partiti dall’analisi dell’ambiente scolastico, semplice nella sua generalità dal pun-
to di vista dello studente ma non banale nei meccanismi, dal punto di vista del
professore. 
## Richiesta del committente 
Di seguito è presente la prima richiesta del committente: 
<br> <br>
<i>
"Salve, vorremmo commissionare un progetto che riguarda la creazione di un siste-
ma integrato allo zaino, con l’obiettivi di poter aiutare studenti e professori nella
gestione del materiale scolastico da portare a lezione. In particolare l’idea è quella
di adattare un qualsiasi zaino con un dispositivo che possa leggere il materiale che
viene inserito, come comunemente vengono letti alla cassa i prodotti acquistati al
supermercato, affinch ́e lo zaino intelligente possa sapere cosa è stato inserito e,
tramite servizi web e applicazione smartphone sviluppata ad hoc, possa ricorda-
re all’utente quale materiale manca per le lezioni del giorno successivo. Tramite
l’applicazione mobile un professore deve poter gestire le lezioni delle proprie classi
mentre uno studente deve poter visualizzare il materiale da portare alle proprie
lezioni. Una cosa essenziale `e il fatto di poter visualizzare realtime il contenuto
dello zaino dall’applicazione ed esser notificato in qualche modo nel caso di qualche
libro o oggetto mancante"
</i>
