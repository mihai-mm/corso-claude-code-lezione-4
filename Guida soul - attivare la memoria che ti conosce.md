# Guida soul - attivare la memoria che ti conosce

> **Istruzioni per Claude.** Guida lo studente a creare il suo **soul** e ad attivarlo. Lo studente non è tecnico: spiega in parole semplici, e **prima di creare cartelle o modificare il suo file `CLAUDE.md` chiedi conferma**. Procedi un passo alla volta. Alla fine deve avere: (1) le cartelle del soul, (2) un primo contenuto minimo, (3) il suo `CLAUDE.md` che dice a Claude di leggere il soul a ogni nuova conversazione.

Il **soul** è la memoria più profonda: non quella che conosce *un* cliente, ma quella che conosce **te** attraverso tutti i progetti. È il motivo per cui, anche su un cliente nuovo, Claude parte già con la tua voce e le tue preferenze.

Vive **fuori dal vault** (in `~/.claude/soul/`, una cartella di sistema) e **non si condivide**: è il livello più personale. Per questo lo costruisci tu, sul tuo computer.

## Come è fatto: tre cassetti

L'idea che conta è **cosa va dove**. Tre cassetti:

- **CHI** - chi sei tu (come lavori, come scrivi, cosa preferisci) e chi sono i tuoi clienti.
- **COME** - il tuo know-how: i modi di fare le cose che hai imparato e che valgono su qualunque cliente. Una cosa fatta bene una volta diventa il modo di farla sempre.
- **PERCHÉ** - le scelte importanti che hai preso e che non vuoi ridiscutere ogni volta da capo.

(C'è anche un cassettino per *come scrivi* nei vari canali - email, post, messaggi - ma l'idea è quella: tre cassetti, una regola di smistamento.)

## Passo 1 - Crea le cartelle del soul

Crea questa struttura (chiedi conferma prima):

```
~/.claude/soul/
├── PROFILO.md              ← CHI sei tu
└── knowledge/
    ├── clients/            ← CHI sono i tuoi clienti (un file per cliente)
    ├── know-how/           ← COME: le cose che hai imparato a fare
    └── decisioni/          ← PERCHÉ: le scelte da non ridiscutere
```

➡️ *Output atteso: le cartelle del soul esistono. Per ora sono quasi vuote: è normale, le riempi nel tempo.*

## Passo 2 - Scrivi il primo contenuto (CHI sei)

Apri `PROFILO.md` e aiuta lo studente a buttarci giù poche righe vere, non un tema. Fai qualche domanda e scrivi tu al posto suo:
- che lavoro fa e per chi (il tipo di clienti);
- come gli piace che Claude gli parli (diretto? formale? con esempi?);
- una o due preferenze forti su come scrive (es. "niente paroloni", "frasi corte").

Bastano 10-15 righe. Il soul cresce vivendo, non si compila tutto il primo giorno.

➡️ *Output atteso: un `PROFILO.md` che dice a Claude chi è lo studente e come trattarlo.*

## Passo 3 - Attiva il soul (la modifica che fa la differenza)

Questo è il passo che molti saltano: **avere i file non basta**. Claude li usa solo se glielo dici nel tuo `CLAUDE.md` globale (il file `~/.claude/CLAUDE.md`, le istruzioni che valgono su ogni progetto).

Apri quel file (se non esiste, crealo) e aggiungi un blocco come questo - **chiedi conferma prima di scrivere**:

```markdown
## Soul - la mia memoria profonda

All'inizio di OGNI nuova conversazione, prima di rispondere:
1. Leggi `~/.claude/soul/PROFILO.md` (chi sono e come lavoro).
2. Se sto lavorando su un cliente, leggi il file in `~/.claude/soul/knowledge/clients/` se esiste.

Mentre lavoriamo, quando impari qualcosa di nuovo e durevole su di me,
i miei clienti, o un mio modo di fare le cose:
- aggiorna **silenziosamente** il file giusto del soul (CHI → PROFILO/clients,
  COME → know-how, PERCHÉ → decisioni);
- non chiedere il permesso, fallo e basta;
- tieni i file brevi e concreti.
```

Spiega allo studente cosa fa questo blocco: ordina a Claude di **leggere** il soul a ogni avvio e di **aggiornarlo da solo** quando impara qualcosa. Da qui in poi il sistema si nutre mentre lavora.

➡️ *Output atteso: il `CLAUDE.md` dello studente attiva il soul. Da adesso Claude lo legge a ogni nuova conversazione e lo fa crescere da solo.*

## Passo 4 - Provalo

Apri una **conversazione nuova** e chiedi a Claude qualcosa di semplice (es. "scrivimi due righe per un cliente"). Fai notare allo studente che Claude parte già con la sua voce e le sue preferenze, **senza che lui le ripeta**. È il soul al lavoro.

➡️ *Output atteso: lo studente vede la differenza - Claude lo "conosce" da subito.*

---

Una nota: il soul è la cosa più personale del sistema. Non finisce in nessun repository condiviso, non si pubblica. È tuo, e cresce con te.
