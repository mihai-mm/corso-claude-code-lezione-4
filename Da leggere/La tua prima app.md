---
tipo: nota
progetto: Mirai Academy - Corso Claude Code
lezione: L4
destinatario: studenti
aggiornato: 2026-06-17
---

# La tua prima app

Lezione 4, seconda parte. Nella prima parte hai imparato a tenere pulito e a far crescere il tuo secondo cervello. Adesso usciamo dal vault e facciamo una cosa che, fino a tre lezioni fa, avresti detto "non fa per me": **costruisci la tua prima applicazione vera**. Online, con i tuoi dati, fatta da te.

Niente più storia, niente più Alberto. Da qui parliamo di te.

## La barriera è nella tua testa, non nel codice

Partiamo dal punto che blocca tutti: *"io non so programmare"*.

Vero. E non serve. Eppure il computer su cui hai lavorato per tre lezioni - quello dove vive il tuo secondo cervello - è **anche** un computer su cui si costruisce software. È la stessa scrivania. Cambia solo cosa ci appoggi sopra.

Il punto è questo: non devi diventare uno sviluppatore. Devi saper **descrivere** cosa vuoi. Lo stesso Claude Code che ti scrive le proposte e ti tiene la memoria dei clienti sa anche scrivere un'app, se glielo chiedi nel modo giusto. La barriera è psicologica, non tecnica.

E non parti dal vuoto. Parti da cose che già hai - un foglio Excel, un'esigenza concreta. Tre idee, tutte nate dal mondo di questo corso:

- un **tracker delle ore liberate** dall'automazione (quanto tempo ti sei ripreso);
- un **mini-CRM personale** (i tuoi contatti e a che punto sei con ognuno);
- un **task tracker** su misura.

In aula ne costruiamo **una** insieme: il mini-CRM, partendo da un foglio Excel. Le altre due te le fai a casa, con lo stesso identico flusso. È l'esercizio del corso.

## I quattro mattoni, in italiano

Per costruire un'app online servono quattro pezzi. Hanno nomi che sembrano difficili, ma ognuno fa una cosa che già conosci.

| Strumento | Cosa fa | A cosa somiglia |
|---|---|---|
| **Claude Code** | scrive l'app, parlandogli | il collaboratore che già usi, qui costruisce invece di scrivere testi |
| **GitHub** | dove vive il codice | come Drive, ma per i file di codice (e tiene la cronologia di ogni modifica) |
| **Vercel** | dove l'app diventa un sito | il "pubblica": da file sul tuo Mac a un link che apri dal browser, in un click |
| **Supabase** | dove l'app salva i dati | come un Google Sheet, ma fatto per le app: i tuoi contatti vivono qui |

Due cose da tenere a mente:

- **Costo zero per iniziare.** Tutti e quattro hanno un piano gratuito che basta e avanza per i tuoi primi progetti.
- **Registrarsi è banale.** In aula creiamo gli account dal vivo: due minuti, nessuna carta di credito. (Vercel fa login *con* GitHub - un account ne sblocca un altro.)

## Dove vivono i progetti di codice

Una regola di ordine, prima di costruire: **il codice non va nel vault.**

Il vault Obsidian è la casa del testo e della conoscenza. Il software è un'altra cosa e va in un'altra casa. La convenzione è semplice:

- una cartella sola per tutto il codice: **`~/Desktop/_Progetti Sviluppo/`** (l'underscore la tiene in cima all'ordine alfabetico, sempre a portata di mano);
- ogni app è una sottocartella lì dentro;
- apri Claude Code dentro la cartella del progetto, e lui sa che lì si lavora a quello.

È la stessa logica del secondo cervello: ogni cosa al suo posto. Il vault resta pulito, il codice ha il suo capannone.

## Da un foglio Excel a un'app online

Ecco il cuore. Si parte da un foglio Excel che assomiglia a tanti che hai già: un piccolo CRM con quattro fogli collegati -

- **Aziende** (ragione sociale, settore, città, dimensione);
- **Persone** (i contatti dentro le aziende: ruolo, email, telefono);
- **Commerciali** (chi segue cosa);
- **Opportunità** (le trattative: valore, **stato** - lead, proposta, negoziazione, chiusa - probabilità, data prevista).

Il prompt che apre tutto è semplice come parlare a un collega:

> *"Ho questo foglio Excel con i miei contatti e le mie trattative. Trasformalo in un'app web dove posso vederli, aggiungerne di nuovi, cambiare lo stato delle opportunità e cercarli. I dati li salviamo su Supabase, l'app la mettiamo online su Vercel."*

Da lì, quello che vedrai non è magia istantanea - è un **dialogo**, ed è meglio così:

1. **Claude propone un piano.** Non parte a testa bassa: ti mostra cosa intende fare, lo leggi insieme, approvi. (È il *plan mode* che hai già visto.)
2. **Claude fa domande.** Tipo: *"lo stato delle opportunità lo vuoi a tendina fissa o libero?"*. Costruire è una conversazione, non un comando secco.
3. **Le colonne diventano i campi.** Claude legge lo schema dal tuo Excel e ne ricava la struttura dei dati, senza che tu disegni niente. Dal foglio alla struttura in un passo.
4. **Qualcosa andrà storto.** È normale, ed è la parte più utile da vedere: un errore appare, glielo dai, lui lo legge e lo aggiusta. **L'errore non è un muro: è parte del flusso.**
5. **Il primo deploy.** L'app diventa un link che apri dal browser. Il tuo foglio Excel è diventato un'applicazione online.

Il punto da portarsi a casa, detto chiaro:

> Quello che hai appena costruito, là fuori lo pagheresti circa 30 euro al mese a un fornitore. L'hai fatto in un paio d'ore, ed è tuo: i dati sono tuoi, le modifiche le chiedi a voce.

## E oltre? (un cenno onesto)

Due cose, per completezza:

- Esiste una skill avanzata chiamata `superpowers` che alza il livello sui progetti complessi. Non ti serve adesso, ma è giusto sapere che c'è: quando i tuoi progetti cresceranno, è una porta.
- E non c'è solo Claude Code: esistono Cursor, Lovable e altri. Sei in Claude Code perché è la scelta consigliata in questo corso, ma sapere che esistono alternative ti rende un cliente più consapevole, non meno.

Niente di tutto questo ti serve adesso. Sapere che esiste basta.

## Cosa ti porti a casa

- **Posso costruire software senza saper programmare.** La barriera è nella mia testa. Lo stesso strumento che mi tiene il sistema sa anche costruire app.
- **Quattro mattoni, quattro funzioni chiare.** Claude Code scrive, GitHub conserva, Vercel pubblica, Supabase salva i dati. Gratis per iniziare.
- **Il codice ha una casa fuori dal vault** (`_Progetti Sviluppo/`). Apro Claude Code nella cartella del progetto e lui lavora lì.
- **Non parto dal vuoto: parto da quello che ho** (un foglio). Il flusso è: descrivere → pianificare → dialogare → gestire l'errore → pubblicare.
- **L'errore è parte del flusso, non un muro.** Lo incollo, Claude lo aggiusta, si va avanti.
- **Esiste altro** (skill avanzate, altri strumenti). Non mi serve ora, ma so dove guardare quando i progetti cresceranno.

E con questo il corso si chiude. Hai un team AI completo, un sistema che lo coordina, e adesso anche la capacità di costruirti gli strumenti che ti servono. Da qui in poi dipende da te.
