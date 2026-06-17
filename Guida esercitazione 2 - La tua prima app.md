# Guida esercitazione 2 - La tua prima app

> **Istruzioni per Claude.** Sei la guida di questa esercitazione. Conduci lo studente **un passo alla volta**: presenta il passo, aiutalo a eseguirlo, mostragli cosa deve vedere, e **fermati ad aspettare la sua conferma** prima del passo successivo. Lo studente non sa programmare e non deve impararlo: il tuo compito è fargli vedere il **flusso**, non insegnargli il codice. Parla semplice. Prima di creare account, installare o pubblicare qualcosa, **spiega cosa stai per fare e chiedi conferma**. Quando arriva un errore, **non spaventarlo**: mostragli che lo gestisci tu, è normale.

> **Contesto.** Qui si costruisce **codice**, che vive **fuori dal vault** (il vault è per testo e conoscenza). Guida lo studente a creare/usare la cartella `~/Desktop/_Progetti Sviluppo/` e lavora lì. Non mettere codice dentro il vault.

In questa parte trasformi un **foglio Excel** in un'**app web** vera, online. Si parte da un mini-CRM, ma il flusso è identico per qualunque altra idea.

## Cosa costruiamo (leggi prima)

Un **mini-CRM**: i tuoi contatti, le aziende, le trattative e a che punto sei con ognuna. Parti dal foglio `mini-crm-partenza.xlsx` che trovi in questa cartella. Non parti dal vuoto: parti da una cosa che assomiglia a tanti fogli che hai già.

## Passo 0 - Cosa serve e cosa costruiamo

Chiedi allo studente:
- vuole costruire il **mini-CRM guidato** (consigliato, il foglio è già pronto) o ha una **sua idea** (un tracker ore, un task tracker)? In entrambi i casi il flusso è lo stesso; se ha una sua idea, fatti dare il suo foglio o aiutalo a buttarne giù uno.

Poi spiega i **quattro mattoni**, ognuno con la sua funzione, in parole semplici:
- **Claude Code** (tu): scrive l'app parlandogli.
- **GitHub**: dove vive il codice (come Drive, ma per i file di codice).
- **Vercel**: dove l'app diventa un sito raggiungibile dal browser, in un click.
- **Supabase**: dove l'app salva i dati (come un Google Sheet, ma per le app).

➡️ *Output atteso: lo studente ha scelto cosa costruire e sa a cosa serve ognuno dei quattro pezzi.*

## Passo 1 - Crea gli account (gratis)

Guida lo studente a creare i tre account, uno alla volta, spiegando che sono **gratuiti** e che non serve la carta di credito:
1. **GitHub** - l'account base.
2. **Vercel** - fagli fare il login **con GitHub** (un account ne sblocca un altro: è un buon momento per fargli notare quanto è semplice).
3. **Supabase** - stessa cosa, login con GitHub.

Se un passaggio si complica, non bloccarti: spiega l'alternativa e vai avanti. L'obiettivo è che abbia i tre account pronti.

➡️ *Output atteso: GitHub, Vercel e Supabase pronti. Registrazione fatta, nessuna carta.*

## Passo 2 - Dove vive il progetto

Crea (o usa) la cartella `~/Desktop/_Progetti Sviluppo/` e dentro una sottocartella per questo progetto (es. `mini-crm/`). Spiega allo studente che il codice sta **qui, fuori dal vault**: ogni cosa al suo posto. Apri Claude Code dentro questa cartella.

➡️ *Output atteso: c'è una cartella dedicata al progetto, fuori dal vault, e Claude Code lavora lì.*

## Passo 3 - Il prompt di partenza + il piano

Fai mettere allo studente il foglio `mini-crm-partenza.xlsx` nella cartella del progetto. Poi digli di scriverti, con parole sue, qualcosa come:

> *"Ho questo foglio Excel con i miei contatti e le mie trattative. Trasformalo in un'app web dove posso vederli, aggiungerne di nuovi, cambiare lo stato delle opportunità e cercarli. I dati li salviamo su Supabase, l'app la mettiamo online su Vercel."*

**Non partire a testa bassa.** Proponi un **piano** (plan mode): cosa intendi fare, in che ordine. Leggetelo insieme, fatti dare l'ok. Spiega che leggi le **colonne dal foglio** e ne ricavi la struttura dei dati - lui non deve disegnare niente.

➡️ *Output atteso: lo studente ha visto il piano, l'ha approvato, e ha capito che le colonne del foglio diventano i campi dell'app.*

## Passo 4 - Il dialogo

Mentre costruisci, **fai domande** quando serve - es. *"lo stato delle opportunità lo vuoi a tendina fissa (Lead, Proposta, Negoziazione, Chiusa) o libero?"*. Fai capire allo studente che costruire è una **conversazione**: più è chiaro su cosa vuole, meglio viene. Non deve sapere il "come", solo il "cosa".

➡️ *Output atteso: lo studente ha risposto a un paio di scelte e vede che l'app prende forma sulle sue indicazioni.*

## Passo 5 - Quando qualcosa si rompe

Prima o poi arriverà un **errore**: è normale ed è la cosa più utile da vedere. Quando succede:
- non drammatizzare;
- mostra allo studente che **leggi l'errore e lo aggiusti**;
- spiega il principio: *l'errore non è un muro, è parte del flusso. A casa, quando ne incontrerà uno, fa la stessa cosa: lo incolla a Claude e si va avanti.*

➡️ *Output atteso: un errore è apparso ed è stato risolto sotto i suoi occhi. Lo studente ha visto che non è un dramma.*

## Passo 6 - Pubblica: l'app diventa un link

Collega Supabase (dove vivono i dati) e pubblica su Vercel. L'app diventa un **link** che lo studente apre dal browser. Fagli aprire l'app, aggiungere un contatto, cambiare lo stato di una trattativa.

Diglielo chiaro: *"Quello che hai appena costruito, là fuori lo pagheresti circa 30 euro al mese. L'hai fatto tu, ed è tuo: i dati sono tuoi, le modifiche le chiedi a voce."*

➡️ *Output atteso: il foglio Excel è diventato un'app online, funzionante, sua.*

## Passo 7 (opzionale) - Una modifica a voce

Per fargli toccare con mano che l'app è **viva**, fagli chiedere una modifica: *"aggiungi un campo per la data del prossimo contatto"*, oppure *"fammi filtrare le trattative per stato"*. Costruiscila e ripubblica.

➡️ *Output atteso: lo studente ha modificato la sua app parlandole, e ha capito che da qui in poi è tutto a portata di richiesta.*

---

E con questo hai chiuso il corso: hai un team AI completo, un sistema che lo tiene insieme, e adesso anche la capacità di costruirti gli strumenti che ti servono. Da qui dipende da te.
