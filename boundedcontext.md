---
title: Bounded Context Canvas
layout: minimal
nav_order: 4
---

# Bounded Contexts
Di seguito sono mostrate le Bounded Context Canvas, ovvero card speciali che mostrano i dettagli di un singolo Bounded Context. Di seguito una piccola leggenda sulle varie classificazioni utilizzate.

## Strategic Classification

### Importanza del BC sul successo del progetto e dell'organizzazione:
- core domain: una iniziativa strategica chiave per il progetto e il suo successo
- supporting domain: necessario allo sviluppo e funzionamento, ma non un ke point tale da differenziarsi nel mercato o portare vantaggio dal punto di vista della concorrenza
- generic: un contesto comune presente in altri domini, anche totalmente differenti
### Ruolo che il BC gioca nel nostro modello di Business:
- revenue generator: le persone pagano per questo preciso servizio o sistema
- engagement creator: agli utenti piace ma non vogliono dover pagare per averlo, quasi fosse scontato per il coinvolgimento degli utenti
- compliance enforcer: protegge il la reputazione e l'esistenza del nostro business nel mercato
### Come verrà sviluppato o evoluto il BC nel suo ciclo di vita:
- genesis: nuovi domini inesplorati
- custom built: compagnie realizzano la loro versione da immettere nel mercato, ognuno con la propria soluzione
- product: versioni off-the-shelf esistono
- commodity: versioni e soluzioni altamente standardizzate esistono

## Domain Roles
Di seguito verranno analizzati i ruoli di dominio utilizzati nella stesura delle canvas, l'elenco completo su cui è stato fatto riferimento è presente al seguente <a href="https://github.com/ddd-crew/bounded-context-canvas/blob/master/resources/model-traits-worksheet.md"> link </a>.
- Approver Context: riceve richieste e determina se queste possono proseguire allo step successivo del processo in questione
- Execution Context: esegue o tiene traccia, monitorando, un lavoro
- Storage Context: gestisce basi di dati permanenti o volatili, in modo da offrire il loro accesso mediante opportune politiche
- Gateway Context: si pone all'estremo di un sistema e gestisce le comunicazioni inbound e outbound

## Sottodomini
I sottodomini analizzati rispiecchiano gli Emerging Bounded Context già visti in fase di Event Storming, ovvero dal raggruppamento naturale scaturito nell'attaccare i post-it alla lavagna virtuale. Più nello specifico, i sottodomini sono i seguenti, con la relativa classificazione strategia:
- Gestione libri
Generic
{: .label .label-green }
- Gestione utenti
Generic
{: .label .label-green }
- Gestione calendario
Supporting
{: .label .label-yellow }
- Reminder Engine
Core
{: .label .label-red }
- Zaino intelligente
Core
{: .label .label-red }
- Creazione etichette (TAG)
Generic
{: .label .label-green }
- Fabbricazione zaini
Generic
{: .label .label-green }
- Gestione materiale per lezioni
Core
{: .label .label-red }
- Applicazione mobile
Core
{: .label .label-red }

<img src="https://lucid.app/publicSegments/view/389c87e1-3ee5-4a43-930f-660df8a70a1b/image.png" style="width:100%; height: auto; border-style: solid;">
