---
name: youtube-notes
description: >
  Trasforma un video YouTube in una nota ordinata dentro il tuo vault.
  Estrae i punti chiave, gli esempi e le citazioni utili, e li salva tra
  le Risorse, collegati alle cose a cui si legano. Funziona su qualunque
  vault: al primo avvio trova (o chiede) dove tieni le Risorse. Usala
  quando condividi un link YouTube e vuoi prendere appunti, dici "riassumi
  questo video", "salva le note di questo video", o lanci /youtube-notes.
  Salva nel vault SOLO dopo la tua conferma.
user-invocable: true
allowed-tools:
  - Read
  - Glob
  - Grep
  - Write
  - Edit
  - WebFetch
  - AskUserQuestion
---

# Skill /youtube-notes (versione corso) - Nutrire il vault da fuori

Il tuo secondo cervello non vive solo di quello che ci metti lavorando: lo **nutri dall'esterno**. Questa skill prende un video YouTube e ne fa una nota ordinata, dentro le tue Risorse, collegata al resto.

> **Per Claude.** Chi la lancia non è tecnico. Genera **sempre** prima il riassunto in chat; salva nel vault **solo dopo conferma esplicita**.

## Procurarsi la trascrizione (senza dipendere da programmi esterni)

1. Chiedi (o prendi) il **link** del video.
2. Prova a recuperarne il contenuto con gli strumenti che hai (es. WebFetch sul link). Se ottieni titolo, autore e una trascrizione utile, usali.
3. **Se non riesci** (YouTube spesso blocca l'accesso automatico), non bloccarti: chiedi allo studente di incollarti la trascrizione, spiegandogli come si fa in 10 secondi -
   > *"Apri il video su YouTube. Sotto il video clicca i tre puntini '...' (o 'Mostra altro') e scegli **Mostra trascrizione**. Si apre la lista del parlato a destra: selezionala tutta, copiala e incollala qui."*
   Poi lavora sul testo che ti incolla. Funziona sempre, su qualunque computer.

## Genera la nota (in chat, prima di salvare)

Struttura semplice e leggibile:
- **Titolo** del video + autore/canale + link.
- **In una riga**: di cosa parla.
- **Punti chiave**: gli spunti che contano, in elenco, con parole tue (non la trascrizione grezza).
- **Esempi / dati / citazioni** utili, se ce ne sono.
- **Perché ti serve**: una riga su come si lega al tuo lavoro.

## Primo avvio - dove vivono le Risorse (adattati al vault)

Prima di salvare, capisci **dove** lo studente tiene il materiale di riferimento (corsi, libri, note esterne). Tipicamente una cartella tipo `3-Resources/` o `Risorse/`. Se non la trovi con sicurezza, **chiedi**: *"Dove vuoi che salvi le note dei video? Hai una cartella per le risorse esterne?"*. Ricordala per le volte successive.

## Collegamenti motivati

Quando salvi, collega la nota alle cose del vault a cui si lega - ma **spiega sempre perché** il collegamento esiste: la nota *conferma*, *espande* o *contraddice* qualcosa che già hai. Un collegamento senza motivo non aiuta a ritrovare il pensiero.

## Salva (solo dopo conferma)

Mostra la nota finita, chiedi *"la salvo nelle Risorse?"*, e solo dopo il sì scrivi il file. Il messaggio da lasciare: *"più nutri il sistema da fuori, più diventa tuo."*

> Se la trascrizione incollata è lunghissima, lavora sui punti che contano: non serve riportarla tutta nella nota, serve la sostanza. E non sovrascrivere una nota già esistente senza chiedere.

## Nota - oltre YouTube

Lo stesso principio vale per un **PDF** o un documento: se lo studente ne ha uno, puoi estrarne il testo pulito (apri il file, leggine il contenuto) e portarlo dentro le Risorse con la stessa struttura. Non serve un programma speciale per i casi semplici.
