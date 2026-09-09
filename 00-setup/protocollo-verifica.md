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
2. **Inerenza e competenza** — l'inerenza discende dalla nozione stessa di reddito
   d'impresa e va valutata con giudizio **qualitativo**, distinto dalla congruità
   (Cass., sez. trib., nn. 450/2018, 3170/2018, 13882/2018, 18904/2018). L'art. 109,
   c. 5, TUIR regola altro: la deducibilità pro-rata in presenza di proventi esenti.
   La competenza sta all'art. 109, cc. 1 e 2. Non risulta alcuna pronuncia delle
   Sezioni Unite sull'inerenza: non citarne.
3. **Antieconomicità** — congruità e antieconomicità sono **indici sintomatici** del
   difetto di inerenza, non autonomi motivi di ripresa. Contestarli sposta sull'ufficio
   l'onere di dimostrare la macroscopica irragionevolezza dell'operazione.
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
gruppo prima dell'esecuzione.

Per le operazioni più rilevanti va **valutato** l'interpello ex art. 11 L. 212/2000,
nel testo integralmente sostituito dall'art. 1, c. 1, lett. n), D.Lgs. 219/2023 (in
vigore dal 18 gennaio 2024). Ma va valutato sapendo che cosa fa e che cosa non fa:

- **Riduce il rischio di qualificazione, non quello di ricostruzione dei fatti.** La
  risposta vincola l'amministrazione «limitatamente al richiedente e alla fattispecie
  rappresentata». Il rilievo tipico non è che la norma sia stata letta male: è che i
  fatti sono diversi da come sono stati descritti.
- **È inammissibile quando esiste prassi sulla fattispecie** (art. 11, c. 4). Le leve
  classiche di un gruppo familiare — royalties su marchio, TFM, compensi amministratori,
  società di comodo — sono coperte da prassi: sono proprio i casi in cui non si può
  presentare.
- **L'interpello antiabuso (art. 11, c. 1, lett. c) ha un costo asimmetrico.** Se la
  risposta è negativa l'operazione è bruciata e il contribuente si è auto-segnalato su
  una fattispecie che l'ufficio non aveva individuato.
- **La tutela è più debole di prima:** gli atti difformi dalla risposta oggi sono
  *annullabili* e non più *nulli* (artt. 7-bis e 7-ter dello Statuto), quindi il vizio
  va dedotto a pena di decadenza nel ricorso introduttivo e non è più rilevabile
  d'ufficio.

Non è quindi vero che l'interpello "trasforma un GIALLO in un VERDE": lo attenua su un
solo asse, e su alcune fattispecie lo peggiora.

## Binario rapido per le scadenze con data certa

La sequenza richiesta dati → diagnosi → long list → roadmap è corretta per le leve
ricorrenti, ma perde le finestre normative che scadono nel frattempo. Regola: **le
scadenze con data certa si lavorano in parallelo alla raccolta dati, non a valle.**
L'elenco aggiornato delle finestre aperte sta in `01-diagnosi/` di ciascun incarico e
va verificato sul testo di legge prima di essere comunicato al cliente.

## Due campi obbligatori su ogni VERDE

Il VERDE è la categoria che dà più falsa sicurezza: l'ufficio non contesta il regime
opzionale, contesta l'artificiosità dei presupposti che vi danno accesso; e quasi tutti
i regimi hanno clausole di decadenza che trasformano un VERDE di oggi in un recupero
fra tre o cinque anni. Ogni VERDE porta perciò due campi obbligatori:
**condizioni di mantenimento** e **data di scadenza del vincolo**, con il nome del
soggetto responsabile del monitoraggio.

Analogamente ogni GIALLO porta la **data in cui smette di essere un rischio**, cioè la
fine del termine di accertamento.
