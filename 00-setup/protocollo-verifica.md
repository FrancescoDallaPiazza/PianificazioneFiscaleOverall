# Protocollo di verifica indipendente

## Principio

Ogni deliverable prodotto dal consulente (Claude) viene sottoposto, prima della
consegna, ad almeno un **revisore indipendente** che non ha partecipato alla stesura
e che lavora con la chiave di lettura di chi contesta, non di chi propone.

## Profili dei revisori

| Sigla | Profilo | Che cosa cerca |
|---|---|---|
| **R1 — Verificatore** | Ufficiale GdF / funzionario Agenzia delle Entrate, Ufficio Grandi Contribuenti o Nucleo PT | Come si smonta l'operazione in sede di verifica: abuso del diritto, interposizione, antieconomicità, inerenza, esterovestizione, soglie penali |
| **R2 — Peer review tecnica** | Dottore commercialista / tributarista | Correttezza normativa, aggiornamento alla legge vigente, calcoli, riferimenti di prassi e giurisprudenza |

Per gli output di merito (leve fiscali, quantificazioni, roadmap) è **obbligatorio R1**.
R2 si aggiunge quando l'output contiene calcoli o citazioni normative puntuali.

## Griglia di contestazione R1 (checklist del verificatore)

1. **Abuso del diritto** — art. 10-bis L. 212/2000: l'operazione è priva di sostanza
   economica? Realizza vantaggi fiscali indebiti? Le ragioni extrafiscali sono
   marginali? Esiste un'alternativa "fisiologica" più onerosa che il contribuente ha
   scartato solo per il fisco?
2. **Inerenza e competenza** — artt. 109 e 110 TUIR: il costo è correlato all'attività?
   È documentato? È congruo? (Cass. SS.UU. e giurisprudenza sull'inerenza qualitativa
   vs quantitativa.)
3. **Antieconomicità** — l'operazione ha senso per un imprenditore razionale a
   prescindere dal risparmio d'imposta?
4. **Interposizione / simulazione** — art. 37 c. 3 DPR 600/1973: chi possiede
   davvero il reddito? Il soggetto interposto ha struttura, rischio, personale?
5. **Esterovestizione e residenza** — art. 73 TUIR (sede di direzione effettiva),
   art. 2 TUIR per le persone fisiche; CFC art. 167 TUIR.
6. **Transfer pricing** — art. 110 c. 7 TUIR: valore di libera concorrenza, esistenza
   e qualità della documentazione, penalty protection.
7. **Qualificazione dei redditi** — la riclassificazione proposta (compenso →
   dividendo → royalty → rimborso spese) regge alla luce della norma corretta?
8. **Sostanza documentale** — esistono delibere, contratti con data certa,
   corrispondenza, evidenza dell'effettiva esecuzione? Un'operazione corretta ma non
   documentata è comunque una perdita in contenzioso.
9. **Soglie penali** — D.Lgs. 74/2000: dichiarazione infedele (art. 4), fraudolenta
   (artt. 2-3), omesso versamento (artt. 10-bis/10-ter), sottrazione fraudolenta
   (art. 11). L'operazione avvicina una soglia?
10. **Indicatori di selezione** — l'operazione genera anomalie che finiscono nelle
    liste selettive: ISA, redditometro, scostamenti settoriali, perdite reiterate,
    società di comodo (L. 724/1994), operazioni con paesi a fiscalità privilegiata.

## Formato dell'esito

Ogni raccomandazione riceve un semaforo:

- **VERDE** — regime opzionale espressamente previsto dalla legge, usato per lo scopo
  per cui esiste. Rischio di contestazione basso.
- **GIALLO** — legittima ma contestabile: richiede documentazione difensiva specifica,
  o presenta incertezza interpretativa. Va indicato *che cosa* costruire per difenderla.
- **ROSSO** — non proponibile: abuso del diritto, rischio penale, o fondata su una
  norma inesistente o male interpretata.

Il revisore deve indicare, per ogni GIALLO e ROSSO, **la contestazione concreta**
(quale norma, quale rilievo, quale importo) e non un rischio generico.

## Regola di risoluzione

- Un ROSSO da parte di R1 **elimina** la raccomandazione dall'output, salvo che il
  consulente dimostri per iscritto l'errore del revisore; la controreplica resta
  agli atti in `99-verifiche/`.
- Un GIALLO non elimina la raccomandazione ma **obbliga** ad allegarle il piano di
  documentazione difensiva.
- Nessun deliverable si considera chiuso finché tutti i ROSSI non sono stati risolti.

## Limite dell'incarico

Questo lavoro è consulenza di pianificazione, non certificazione. Le operazioni con
profilo GIALLO devono essere validate dal commercialista/tributarista di fiducia del
gruppo prima dell'esecuzione, e per le più rilevanti va valutato l'**interpello**
(art. 11 L. 212/2000), che è lo strumento con cui si trasforma un GIALLO in un VERDE.
