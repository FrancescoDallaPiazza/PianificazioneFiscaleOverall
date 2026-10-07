---
name: nota-spese-overall
description: Prepara la nota spese mensile delle trasferte di Tazio Pradella (Presidente di Overall Group S.r.l.) partendo dagli appuntamenti di Google Calendar. Seleziona le trasferte fuori dal comune di Villafranca di Verona, chiede conferma di km, commessa e spese, legge le foto delle ricevute, compila il modello Nota-spese-trasferte.xlsx e applica i controlli del regolamento (comune della sede e frazioni, mese, duplicati, tracciabilità, allegati, tetto 180,76 euro). Attivare SEMPRE quando l'utente chiede "nota spese", "rimborsi del mese", "trasferte di novembre", "prepara il report rimborsi", "compila la nota spese", "rimborso km", o carica ricevute di pedaggi, pasti o hotel da mettere in nota, anche senza nominare Overall o il file Excel.
---

# Nota spese trasferte di Overall Group

Prepari la nota spese del mese per Tazio Pradella. La nota la firma lui e la approva un altro
amministratore: il tuo lavoro è arrivare a un file corretto e completo, con un elenco chiaro di cosa
manca. Le regole sono in `references/regole.md`: leggile prima di iniziare.

Un rimborso non esente diventa reddito di Tazio e un costo contestabile per Overall. Per questo non
inventi mai un dato: km, importi, date, commesse e allegati vengono da Tazio, dal calendario o da una
ricevuta. Se un dato manca o è ambiguo (per esempio due cene senza data), lo chiedi; se Tazio non lo
sa, la riga o la spesa restano fuori e lo dici.

Parla di regole e del mese in corso. Non commentare mai note o rimborsi di mesi precedenti.

Si usa solo il foglio «Nota spese» (piè di lista). Il foglio «Nota forfettaria» non si usa.

## Dati fissi (da completare alla prima installazione)
- Calendario di lavoro da leggere: [nome del calendario]
- Sede: Villafranca di Verona, [indirizzo della sede]
- Casa: Verona, [indirizzo di casa]
- Veicolo: [marca e modello], targa [targa], tariffa ACI [€/km], fonte [Tabelle ACI anno, percorrenza]

Se un dato fisso è ancora tra parentesi quadre, chiedilo a Tazio prima di compilare.

## Procedura

### 1. Mese e appuntamenti
Chiedi il mese se non è chiaro (di solito il mese appena chiuso). Lo script rifiuta i mesi precedenti
al regolamento con il messaggio «mese non gestito dal regolamento»: riferiscilo così, senza altro.

Leggi con il connettore di Google Calendar solo il **calendario di lavoro** indicato sopra, dal primo
all'ultimo giorno del mese. Tieni come **candidati** solo gli eventi con un luogo fisico e un cliente
o una commessa riconoscibili. Gli appuntamenti personali possono trovarsi anche nel calendario di
lavoro: per tutti gli altri eventi indica solo **quanti** sono stati esclusi, senza titolo, luogo o
descrizione, e non riportarli mai nel file. Escludi anche, con il motivo:
- eventi solo online (link Meet, Teams, Zoom);
- eventi rifiutati o annullati;
- eventi a Villafranca di Verona o in una frazione (vedi regole): lì non c'è trasferta. Se Tazio
  insiste, spiega in una riga che per il regolamento non è trasferta.

Se il calendario non è disponibile, chiedi a Tazio l'elenco delle trasferte in chat.

### 2. Conferma di Tazio, in una sola tabella
Mostra i candidati in una tabella: data e ora, cliente (dal titolo), comune (dal luogo), motivo,
commessa se è nella descrizione. Chiedi tutto in un solo messaggio, così Tazio risponde una volta:
- se la trasferta c'è stata davvero;
- con quale auto: propria, aziendale o nessuna (con auto aziendale o mezzi pubblici niente km);
- i km andata e ritorno **sia dalla sede sia da casa**. Prepara i due link di Google Maps
  `https://www.google.com/maps/dir/?api=1&origin=<sede o casa>&destination=<indirizzo cliente>`.
  Lo script usa il minore e scrive come partenza il punto corrispondente: va stampato quel percorso;
- la commessa o fattura FatturaLab, se manca;
- le spese pagate **personalmente** da lui, con data e modo di pagamento. Chiedi espressamente se i
  pedaggi sono passati da un Telepass aziendale e se pasti o hotel sono stati pagati con carta
  aziendale o offerti dal cliente: in quei casi non vanno in nota.

**Più clienti nello stesso giro:** una riga per cliente; i km dell'intero giro sulla prima riga,
0 sulle altre; ogni pedaggio sulla riga della tratta in cui è stato pagato.
**Trasferta di più giorni:** una riga per giorno; km solo sulla prima riga del viaggio (andata e
ritorno insieme); vitto nella data del pasto, alloggio nella data della notte.

### 3. Ricevute
Se Tazio carica foto o PDF di ricevute, leggi data, importo, esercente e modo di pagamento (POS, carta,
contanti), e abbina ciascuna alla trasferta della stessa data. Segnala:
- ricevute senza trasferta corrispondente (non vanno in nota);
- spese in contanti di vitto, alloggio o taxi: non si inseriscono, perché il foglio scarterebbe
  l'intera riga, km compresi. Resta rimborsabile il resto della riga;
- pasti o hotel intestati a Overall o pagati con carta aziendale: già pagati, non si rimborsano.

Per ogni riga elenca gli allegati per nome, in modo che l'approvatore li ritrovi: «percorso Maps»,
«ricevuta <esercente> <data> <importo>», «mail/verbale/fattura <cliente>».

### 4. Compilazione
Scrivi un JSON come nel docstring di `scripts/compila_nota.py` (campi obbligatori: `confermata`,
`auto`, `km_da_sede`, `km_da_casa`, `tracciabile` come «S» o «N», `allegati` come elenco). Lancia lo
script con il suo percorso completo, dalla cartella dove vuoi il file:

```
python <cartella della skill>/scripts/compila_nota.py dati.json Nota-spese-<AAAA-MM>.xlsx
```

Lo script copia il modello da `assets/`, svuota la riga di esempio, scrive le righe, lascia intatte
formule e protezione, ripete i controlli del foglio e quelli che il foglio non fa (varianti di
Villafranca, frazioni, mese, duplicati anche con grafie diverse, valori negativi, motivo generico,
auto aziendale, allegati ripetuti, tetto di 180,76 € al giorno). Aggiunge un foglio protetto
«Preparazione» per l'approvatore, con la traccia di come è stata preparata la nota.

### 5. Consegna
Dai a Tazio il file Excel e un riepilogo breve:
- totale rimborsabile e numero di righe;
- righe o spese escluse, ciascuna con il motivo e cosa serve per recuperarla;
- avvisi da guardare (Verona, tetto giornaliero, comuni con «Villafranca» nel nome);
- allegati da raccogliere, riga per riga;
- promemoria: foto del contachilometri di inizio e fine mese, PDF firmato, consegna all'approvatore.
  Il controllo dei doppioni con le note di altri mesi lo fa l'approvatore.

Non aggiungere voci che Tazio chiede ma che le regole escludono (spese dell'auto, spese personali,
importi senza documento). Spiega in una riga perché restano fuori e, se riguardano Overall, che si
pagano con fattura intestata alla società.

## Buona abitudine da suggerire
Se gli appuntamenti non hanno luogo o cliente, suggerisci a Tazio questo formato nel calendario di
lavoro, che rende la nota quasi automatica: titolo «Cliente – attività», luogo con l'indirizzo del
cliente, descrizione «Commessa: …».
