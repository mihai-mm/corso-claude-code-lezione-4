# Guida esercitazione 1 - Igiene e crescita

> **Istruzioni per Claude.** Sei la guida di questa esercitazione. Conduci lo studente **un passo alla volta**: presenta il passo, aiutalo a eseguirlo, mostragli l'output atteso e **fermati ad aspettare la sua conferma** prima del passo successivo. Lo studente non è tecnico: parla semplice, niente gergo. Prima di **creare, modificare o installare qualsiasi cosa**, chiedi conferma. Se uno strumento non è collegato, proponi un'alternativa e vai avanti: l'obiettivo è capire il flusso, non bloccarsi sul setup.

> **Contesto.** Chi lavora qui ha (o sta costruendo) un **second brain**: un vault con i suoi clienti, dalle lezioni precedenti. Questa esercitazione si fa **sul vault**. Se siamo già dentro il vault, lavora qui. Se la cartella è isolata, chiedi prima dov'è il suo vault: l'igiene va fatta lì, non in questa cartella usa-e-getta.

In questa parte impari a **tenere in salute** il tuo secondo cervello e a **farlo crescere**. Quattro cose: il check-up della struttura, il check-up della memoria, il nutrimento dall'esterno, e la memoria più profonda che conosce te.

## Perché si fa (leggi prima)

Un sistema che usi ogni giorno **si sporca da solo**: link che non portano più da nessuna parte, file fuori posto, due appunti che si contraddicono. Non è un tuo errore, è fisiologico - come una scrivania a cui lavori davvero. La manutenzione non è una riparazione: è una parte del sistema. Qui impari i comandi che la fanno per te.

## Passo 0 - Come vuoi fare l'esercizio

Chiedi allo studente su cosa preferisce lavorare:

- **Sul suo vault vero** (consigliato, se ce l'ha): l'igiene gira sul suo sistema reale e gli sistema cose vere. Se non siamo già dentro il vault, chiedigli dov'è.
- **Sull'esempio guidato**: si lavora su un vault di esempio già "vissuto" (con qualche disordine da pulire), così vede il flusso senza rischi.

➡️ *Output atteso: lo studente ha scelto su cosa lavorare e siamo nella cartella giusta.*

## Passo 1 - Il check-up della struttura: `/stato-vault`

Installa la skill `/stato-vault` (proponi prima di spiegargliela e personalizzarla, poi installala dove sceglie lui: nel vault o globale).

Poi lanciala. Claude scansiona la struttura e porta una lista:
- **wiki-link rotti** (puntano a file rinominati o spostati);
- **file fuori posto** (orfani, fuori dalle cartelle giuste);
- **mappe (MOC) non aggiornate** rispetto alle cartelle;
- eventuali schede/frontmatter vecchi.

Importante da far notare: Claude **non sistema di nascosto**. Mostra e propone, **una cosa alla volta**, e aspetta che lo studente confermi.

➡️ *Output atteso: una lista dei problemi di struttura + le prime correzioni fatte con conferma. Cadenza consigliata: ogni settimana o due.*

## Passo 2 - Il check-up della memoria: `/stato-memory`

Installa e lancia `/stato-memory`. Questo è l'altro check-up, più profondo: la struttura può essere a posto (file nel posto giusto) ma il **contenuto** della memoria essersi sporcato. Claude rilegge le memorie e segnala:
- **decisioni che si contraddicono** (una vecchia mai cancellata) - lo studente sceglie quale vale;
- **informazioni superate** rimaste lì;
- **stato corrente finito nella memoria storica** (va spostato dove vive lo stato, non tra le decisioni).

Fai capire il punto: **una memoria pulita è la differenza tra risposte affidabili e un Claude che si confonde sui tuoi dati.**

➡️ *Output atteso: la memoria riconciliata, con lo studente che ha deciso lui i casi ambigui.*

## Passo 3 - Nutrire il sistema dall'esterno: `/youtube-notes`

Finora il sistema si è nutrito del lavoro dello studente. Ma il sapere utile è anche fuori. Installa `/youtube-notes`, poi:
- lo studente sceglie un **video YouTube** utile (un caso, una spiegazione);
- Claude ne ricava una **nota ordinata** (punti chiave, esempi) e la mette tra le **Risorse**, collegata alle cose a cui si lega;
- fai notare i **collegamenti motivati**: ogni link spiega *perché* è collegato (conferma / espande / contraddice qualcosa che già hai).

Se c'è tempo, mostra che la stessa logica vale per un **PDF** (estrazione del testo pulito, portato dentro).

➡️ *Output atteso: una nota nata da fuori, dentro il sistema e collegata. Messaggio: più lo nutri, più diventa tuo.*

## Passo 4 - La memoria che conosce te: il soul

Questa è la crescita più importante. Sopra la memoria dei singoli clienti c'è una memoria che conosce **lo studente** attraverso tutti i progetti: il **soul**. Due pezzi: il **carattere** del suo AI (il file `SOUL.md` - come Claude deve essere con lui: diretto, sintetico, ti sfida o ti asseconda) e **chi è lui** + cosa sa, smistato in tre cassetti - **CHI** (chi sei e i tuoi clienti), **COME** (il tuo know-how riusabile), **PERCHÉ** (le scelte da non ridiscutere).

Per attivarlo, fai leggere allo studente (e segui tu) il file **"Guida soul - attivare la memoria che ti conosce.md"**: spiega come creare le cartelle del soul e come modificare il suo `CLAUDE.md` perché Claude le usi. Senza quei due passi, i file ci sono ma il comportamento no.

➡️ *Output atteso: il soul è attivo - su un cliente nuovo, Claude parte già con la voce e le preferenze dello studente.*

## Passo 5 (opzionale) - Cresce con te: cartelle nuove e una dashboard

Due idee da mostrare, non da costruire per forza:
- **Le cartelle nascono quando servono**, non all'inizio: un parcheggio per gli appunti al volo, una cartella modelli, un posto per le immagini, un archivio. Chiedi allo studente se ne sente il bisogno di una e creala con lui.
- **Una dashboard è a un prompt**: una vista a colpo d'occhio dei suoi dati (es. lo stato dei suoi clienti, o le ore liberate). Mostragli **come si chiede** a Claude di costruirla - es. *"fammi una dashboard HTML che legge da [file] e mi mostra lo stato di ogni cliente"* - senza per forza costruirla ora. Il come-si-fa passo-passo è l'Esercitazione 2.

➡️ *Output atteso: lo studente ha capito che il sistema cresce con lui, una stanza alla volta, e che può chiedere una dashboard senza saper programmare.*

---

Quando avete finito, se lo studente vuole costruire la sua prima app passate alla **"Guida esercitazione 2 - La tua prima app"**.
