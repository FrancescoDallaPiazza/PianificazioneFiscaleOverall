# Parametri dell'incarico

Definiti dalla proprietà il 9 settembre 2026. Sono i vincoli entro cui ogni
raccomandazione deve stare.

| Parametro | Scelta |
|---|---|
| **Obiettivo prevalente** | Massimizzare la cassa netta ai soci |
| **Propensione al rischio** | VERDE + GIALLO documentato |
| **Approccio** | Diagnosi completa sui dati |
| **Consegna dati** | File depositati in `dati/` |

## Cosa comportano operativamente

### Obiettivo: massimizzare la cassa ai soci

La funzione obiettivo non è minimizzare l'IRES: è **massimizzare l'euro netto che
arriva sul conto personale del socio, a parità di costo per il gruppo**. Sono due cose
diverse e a volte confliggenti — un'operazione che riduce l'imponibile della società
ma genera reddito pesantemente tassato in capo alla persona fisica peggiora
l'obiettivo pur migliorando l'IRES.

Il numero da ottimizzare è quindi il **cuneo complessivo di estrazione**:

```
cuneo = (costo per la società − netto incassato dal socio) / costo per la società
```

calcolato su ogni canale di uscita e sommato lungo tutta la catena
società → socio, includendo IRES, IRAP, contributi previdenziali, ritenute e IRPEF.
Le aree di lavoro che ne discendono, in ordine di rilevanza attesa:

1. **Mix di remunerazione** — compenso amministratore, dividendo, TFM, welfare,
   rimborsi, canoni: ciascun canale ha un cuneo diverso e una capienza diversa.
   L'ottimo è quasi sempre una combinazione, non un canale unico.
2. **Struttura della catena partecipativa** — se e quanto conviene interporre una
   holding tra le operative e le persone fisiche, considerando che la holding sposta
   il momento della tassazione ma non lo elimina se la cassa deve comunque arrivare
   alla persona fisica.
3. **Beni e patrimonio** — chi deve possedere cosa perché il flusso verso il socio sia
   il meno tassato possibile (immobili, marchi, veicoli).
4. **Base imponibile a monte** — agevolazioni e regimi che riducono l'imposta
   societaria e quindi aumentano l'utile distribuibile.

⚠️ Vincolo di coerenza: l'obiettivo "estrarre cassa" e i regimi premiali sugli utili
**non distribuiti** sono in conflitto diretto. Se il gruppo sta beneficiando di
un'agevolazione condizionata alla patrimonializzazione, il costo del recapture va
messo a bilancio della decisione, non ignorato.

### Rischio: VERDE + GIALLO documentato

- Le operazioni GIALLE sono ammesse **solo se il dossier difensivo è costruito prima
  dell'esecuzione**, non dopo. Ogni raccomandazione GIALLA arriverà con l'elenco
  puntuale dei documenti da produrre e delle date entro cui devono esistere.
- Le operazioni ROSSE non vengono proposte.
- Per le GIALLE ad alto valore si valuta l'interpello, che è lo strumento con cui un
  GIALLO diventa un VERDE.

### Approccio: diagnosi sui dati

Il lavoro è fermo in attesa dei documenti di `00-setup/richiesta-dati.md`, blocchi
A, B, D, G, H. In particolare, per l'obiettivo scelto, sono indispensabili:

- il dettaglio **D** (compensi, delibere, dividendi, riserve, prelievi) — è l'area su
  cui si gioca la partita;
- il **fabbisogno di cassa personale annuo di ciascun socio** — senza questo numero
  non si può dimensionare il mix ottimale;
- la **stratificazione delle riserve** — determina il costo fiscale della
  distribuzione di ciò che è già stato accantonato negli anni passati.
