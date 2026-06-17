---
name: stato-memory
description: >
  Check-up della MEMORIA del tuo vault. Rilegge i file di memoria dei tuoi
  progetti (tipo MEMORY.md) e trova i problemi di contenuto - decisioni che
  si contraddicono, informazioni vecchie mai aggiornate, stato corrente
  finito nella memoria storica, note troppo lunghe - e ti propone come
  riconciliarli, scegliendo tu nei casi ambigui. Funziona su qualunque
  vault: al primo avvio si adatta. Usala quando dici "stato memory",
  "controlliamo le memorie", "puliamo la memoria di [progetto]", o lanci
  /stato-memory. Cadenza tipica: ogni 1-2 mesi.
user-invocable: true
allowed-tools:
  - Read
  - Glob
  - Grep
  - Edit
  - AskUserQuestion
---

# Skill /stato-memory (versione corso) - Check-up della memoria

Manutenzione **del contenuto** delle memorie. È il gemello di `/stato-vault` (che controlla la *struttura*). La struttura può essere a posto - i file nel posto giusto - ma il **contenuto** della memoria essersi sporcato: due appunti che si contraddicono, roba vecchia, lo stato di oggi finito tra le cose storiche.

> **Per Claude.** Chi la lancia non è tecnico. Parla semplice. **Le scelte ambigue le decide lo studente**, non tu: tu trovi e proponi, lui sceglie quale versione vale.

## Primo avvio - adattati al vault (fallo solo la prima volta)

1. **Trova le memorie**: cerca nel vault i file di memoria (tipicamente `MEMORY.md`, uno per progetto/cliente/area). Se ce ne sono molti, chiedi su quale/i lavorare adesso (uno, alcuni, tutti).
2. **Capisci la convenzione**: come tiene le cose lo studente? Di solito una memoria sana contiene **decisioni** (con data), **insight/lezioni** e **numeri/dati consolidati** - tutte cose *evergreen*, che non invecchiano. Lo "stato corrente" (a che punto siamo, cosa resta da fare) **non** è memoria: vive altrove (in un diario/log). Se la convenzione dello studente è diversa, **chiedi** com'è organizzato e adattati.

## Cosa controlla (i problemi tipici)

1. **Decisioni che si contraddicono**: due voci che dicono cose opposte, e una è vecchia mai cancellata.
2. **Informazioni superate**: una decisione/numero che è stato rimpiazzato ma è rimasto lì senza essere segnato come superato.
3. **Stato corrente nel posto sbagliato**: sezioni tipo "stato lavori", "cosa resta da fare", "prossimi passi" dentro la memoria - sono fotografie che invecchiano, vanno spostate nel diario/log, non tra le decisioni.
4. **Note troppo lunghe**: voci di memoria che sono diventate paragrafi - vanno asciugate all'essenziale.
5. **Roba fuori posto**: contenuto che non c'entra con quella memoria.

## Come procede

1. **Rileggi** i file di memoria scelti.
2. **Porta la lista** dei problemi, per tipo. Numeri chiari: "2 decisioni in conflitto, 1 informazione superata, 1 sezione di stato da spostare".
3. **Proponi la riconciliazione una alla volta**, con conferma:
   - conflitto → mostra le due versioni e **chiedi allo studente quale vale** (non decidere tu);
   - superata → proponi di segnarla come superata o di rimuoverla;
   - stato corrente → proponi di spostarlo nel diario/log e toglierlo dalla memoria;
   - voce lunga → proponi la versione asciutta.
4. **Non modificare** niente senza il sì esplicito.

## Output

Un breve riepilogo: cosa è stato riconciliato, cosa è rimasto in sospeso. Il messaggio da lasciare: *"una memoria pulita è la differenza tra risposte affidabili e un Claude che si confonde sui tuoi dati."*
