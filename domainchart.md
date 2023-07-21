---
title: Strategic Design
layout: minimal
nav_order: 7
---

# Domain Chart
Una volta analizzati i sottodomini nella sezione <i> Strategic Design </i>, possiamo passare ad un livello di analisi più avanzato, aggiungendo al campo visuale aspetti chiave come:
- vantaggio competitivo
- complessità (alta, potenzialmente alta, semplice)
- volatilità del contesto o del sottodominio preso in considerazione durante il suo futuro ciclo di vita
- tipo di soluzione che si vuole adottare (in-house, outsourcing o build-from-scratch)
- tipo del problema (interessante, risolto o ovvio nella sua risoluzione)

A tal scopo. è riportata sotto la Domain Chart, ovvero un grafico determinato da due assi: il primo riguarda la complessità del modello, ovvero il livello di complessità interna che richiede quel preciso componente o bounded context (sottodominio); la seconda riguarda il livello di differenziazione nel mercato, nel business in cui vogliamo operare e dentro al quale inseriamo il prodotto. Entrambi questi livelli possono spaziare tra basso e alto, senza una quantificazione meramente numerica, ma secondo una possibile stima teorica.
Chiaramente, i sottodomini <i style="color: red"> CORE </i> li troviamo nella parte in alto a destra del grafico, in quanto per definizione portano ad una elevata differenziazione sul mercato, dato per l'innovazione o per la creatività, e la sua intrinseca complessità, in quanto sicuramente non è banale dal punto di vista progettuale (essendo un prodotto nuovo o non presente nel mercato con tali peculiarità).
Sottodomini <i style="color: green"> GENERIC </i> non portano a vantaggi lato business, ma possono nascondere complessità elevate, stessa cosa per sottodomini di <i style="color: yellow"> SUPPORT </i>,i quali possono anche portare vantaggi lato business ma non esserne il core fondamentale (a patto che siano di facile implementazione o altamente standardizzati).

Nell'immagine che segue è possibile vedere la classificazione dei sottodomini precedentemente analizzati, con qualche dettaglio aggiuntivo.

## Decisive Core
Questi sono domini core con estrema complessità e offrono un alta differenziazione nel mercato, con un carattere decisivo nell'imporre il vantaggio del prodotto. Questi sono:
- l'applicazione mobile
- lo zaino intelligente
- il reminder engine, seppur prevedendo una minor complessità rispetto ai primi due

## Short Term core
Questi tipi di sottodomini presentano un potenziale iniziale alto dal punto di vista della differenziazione sul mercato, prevista però ad abbassarsi a causa della sua scarsa complessità, vulnerabilità che potrebbe causare l'analisi e la relativa copia da parte dei competitor. Per questo la gestione del materiale per le lezioni si suppone passerà prima o poi da core a generico.

## Considerazioni
Una considerazione va fatta sulla gestione dei device lato cloud: oltre all'utilizzo di un dispositivo fisico da installare all'interno dello zaino adattato, è necessario dare una rappresentazione digitale del dispositivo anche sul cloud, in modo che sia accessibile ovunque e da qualsiasi sorgente: per questo si è deciso di sfruttare una piattaforma esterna, quindi outsourcing, in modo da eliminare la progettazione di un sistema from-scratch e delegarne le funzionalità a soluzioni già esistenti.

<center><img src="https://lucid.app/publicSegments/view/0fe87968-11d7-46fa-91cf-46a4464db4d5/image.png" style="width:100%; height: auto; border-style: solid;"> </center>
