---
name: stato-vault
description: >
  Check-up della STRUTTURA del tuo vault Obsidian. Trova i problemi di
  organizzazione - wiki-link rotti (che puntano a file rinominati o
  spostati), file fuori posto, mappe/MOC non più allineate alle cartelle,
  frontmatter vecchio, cartelle vuote - e ti propone come sistemarli, una
  cosa alla volta, chiedendoti conferma. Funziona su qualunque vault: al
  primo avvio si adatta alla tua struttura. Usala quando dici "stato vault",
  "controlliamo il vault", "facciamo manutenzione", o lanci /stato-vault.
  Cadenza tipica: ogni settimana o due.
user-invocable: true
allowed-tools:
  - Read
  - Glob
  - Grep
  - Edit
  - AskUserQuestion
---

# Skill /stato-vault (versione corso) - Check-up della struttura

Manutenzione **strutturale** del vault: controlla che tutto sia al posto giusto e raggiungibile. È il gemello di `/stato-memory` (che controlla il *contenuto* delle memorie). Questa guarda l'**organizzazione**: link, file, mappe.

> **Per Claude.** Chi la lancia non è tecnico. Parla semplice, niente gergo. **Non sistemare niente di nascosto**: trova, mostra, proponi, e aspetta il sì - una cosa alla volta.

## Primo avvio - adattati al vault (fallo solo la prima volta)

Questa skill deve funzionare sul vault di chiunque. Prima di controllare, **guardati intorno** e, se qualcosa non è chiaro, **chiedi invece di assumere**:

1. Capisci dove sei: sei nella radice del vault o in una sottocartella? Cerca verso l'alto un file di regole globale (un `CLAUDE.md` "di chi sono / come lavoro") e la cartella dei progetti/clienti.
2. Rileva la struttura: come sono organizzate le cartelle (per progetto? per cliente? con un metodo tipo PARA?). C'è un file "mappa" per progetto (un MOC, di solito con lo stesso nome della cartella)? Dove tiene le memorie (file tipo `MEMORY.md`)?
3. Se non riesci a capirlo con sicurezza, **fai 1-2 domande** allo studente: *"Dove tieni i tuoi progetti/clienti?"*, *"Hai un file-mappa per progetto?"*. Annota le risposte e usale per i controlli.

Una volta capita la struttura, procedi con i controlli sotto.

## Cosa controlla

1. **Wiki-link rotti**: link `[[Nome]]` che puntano a note che non esistono (file rinominato, spostato o mai creato).
2. **File fuori posto / orfani**: file che non stanno nella cartella giusta secondo l'organizzazione del vault, o non raggiungibili da nessuna mappa.
3. **Mappe (MOC) non aggiornate**: un file-mappa di progetto che non linka più tutti i file presenti nella sua cartella (file nuovi mai aggiunti alla mappa).
4. **Frontmatter vecchio o assente** sui file strutturali (es. data `aggiornato:` ferma da molto, o campo mancante).
5. **Cartelle vuote** o residui che andrebbero rimossi/archiviati.

## Come procede

1. **Scansiona** con i tuoi strumenti (cerca i `[[...]]` e verifica che il file esista; elenca i file per cartella e confrontali con le mappe; leggi i frontmatter). Non servono programmi esterni: usa Grep/Glob/Read.
2. **Porta la lista** dei problemi trovati, raggruppati per tipo, dal più al meno importante. Numeri chiari: "3 link rotti, 1 mappa non aggiornata, 2 file orfani".
3. **Proponi i fix uno alla volta**, con conferma:
   - link rotto con **un solo** candidato ovvio → proponi la correzione;
   - link rotto **ambiguo** (più candidati) → chiedi quale;
   - file orfano → proponi la cartella giusta o di linkarlo alla mappa;
   - frontmatter → proponi l'aggiornamento della data.
4. **Non toccare** mai niente senza il sì esplicito. Applica solo ciò che lo studente conferma.

## Cautele (importante: lavori sul vault vero)

- Se la cartella **non sembra un vault** (nessun progetto, nessuna mappa, nessuna struttura riconoscibile), **dillo e fermati**: meglio non inventare problemi su una cartella qualunque.
- **Mai applicare correzioni in blocco.** Spostare un file e correggere un link sono modifiche vere: **una conferma per ognuna**, mai "sistemo tutto io".
- Se un fix non è ovvio (più candidati, un dubbio), **chiedi** invece di decidere tu.
- Nel dubbio su un file, **non toccarlo** e segnalalo soltanto.

## Output

Alla fine, un breve riepilogo: cosa è stato sistemato e cosa è rimasto in sospeso (e perché). Ricorda la cadenza: *"rilancia /stato-vault ogni settimana o due, è come riordinare la scrivania."*
