# Pianificazione fiscale — Overall Group

Repository di lavoro dell'incarico di pianificazione e ottimizzazione fiscale.

## Metodo

| Fase | Contenuto | Cartella |
|---|---|---|
| 0 | Setup incarico, protocollo di verifica, richiesta dati | `00-setup/` |
| 1 | Diagnosi as-is: mappa del gruppo, ETR effettivo, aree di rischio | `01-diagnosi/` |
| 2 | Long list delle leve fiscali applicabili | `02-leve/` |
| 3 | Quantificazione del beneficio + stress test antiabuso per ogni leva | `03-quantificazione/` |
| 4 | Roadmap operativa + dossier documentale difensivo | `04-roadmap/` |
| — | Esiti delle verifiche indipendenti su ogni output | `99-verifiche/` |

## Regola permanente

**Nessun output esce da questo repository senza almeno una verifica indipendente**
condotta con la chiave di lettura di un verificatore (Guardia di Finanza / Agenzia
delle Entrate). Vedi `00-setup/protocollo-verifica.md`.

## Materiale di riferimento

`reference/` — due volumi divulgativi italiani sulla pianificazione fiscale
(scansioni senza livello testo; lettura pagina per pagina via rendering).

- `lib1/` (3132_*) — volume sulla pianificazione fiscale per imprenditori, ~186 pagine.
  Introduzione "Crema pasticcera e pianificazione fiscale"; cap. 1 "Le tasse non sono
  uguali per tutti".
- `lib2/` (3133_*, 3134_*, 3138_*) — *Meno soldi al fisco e più nelle tue tasche*,
  Carlo Alberto Micheli, ~pp. 44-455.

**Status dei volumi: fonte di idee, non fonte di diritto.** Sono testi divulgativi.
Il primo controllo a campione ha già trovato un errore normativo rilevante
(vedi `99-verifiche/V00-note-fonti.md`). Ogni spunto tratto da questi libri viene
riverificato sul testo di legge, sulla prassi e sulla giurisprudenza prima di entrare
in un output.
