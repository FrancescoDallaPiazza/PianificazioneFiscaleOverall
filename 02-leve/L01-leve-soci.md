# L01 — Leve per i soci Dalla Piazza e Pradella

**Versione 1** del 25 settembre 2026, **da sottoporre a verifica indipendente** (V04).
**Perimetro:** Francesco Dalla Piazza (FDP) e Tazio Pradella (TP). Gli altri due soci non
sono coinvolti: nessuna leva deve danneggiarli, e quelle che toccano la ripartizione
degli utili richiedono il loro consenso.
**Fonti:** diagnosi D01 v3, cedolini giugno-agosto 2026, dati dichiarati dalla proprietà il
25/09/2026, spunti dai due volumi in `spunti-volumi/`, riverificati qui. Il modello di
calcolo è semplificato: IRPEF 2026 23/33/43%, addizionali forfettarie 2,03%, Inarcassa
soggettivo 14,5%.

> **Convenzione:** [A] accertato · [I] inferito · [V] da verificare prima di eseguire.
> Semafori come da `00-setup/protocollo-verifica.md`.

---

## 0. I dati di partenza

| | FDP | TP |
|---|---|---|
| Età / orizzonte | 55 anni, **10 anni di attività** | 41 anni |
| Reddito | professionale ~141.000 (P.IVA, Inarcassa) | compenso co.co.co. Overall ~32.500, **nessun altro reddito** |
| Netto disponibile oggi [I] | **≈ 74.000** | **≈ 24.000** + dividendi |
| Fabbisogno di cassa annuo | **45.000** | **35.000** |
| **Differenza** | **+29.000 l'anno di eccedenza** | **−11.000 l'anno**, da coprire con i dividendi (≈ 14.900 lordi) |
| Famiglia | — | moglie (15.000 di reddito), 2 figli minorenni |
| Patrimonio | ufficio di proprietà, nessuna auto | casa con mutuo, 2 auto a rate |

**I due soci hanno problemi opposti.** FDP guadagna più di quanto spende: per lui il tema
è **dove accumulare l'eccedenza** con il minor prelievo. TP spende più di quanto il
compenso gli lascia: per lui il tema è **aumentare il netto a parità di costo per la
società**.

---

## 1. Una questione da chiarire prima di tutto — Pradella e l'INPS

**[A]** Sul compenso di TP la gestione separata è applicata al **24%**: 16% a carico della
società e 8% a suo carico. È l'aliquota di chi è **già iscritto a un'altra gestione
previdenziale obbligatoria**. **[A]** La proprietà dichiara che TP non ha altro lavoro né
pensione.

**Le possibilità sono due:**
1. **TP è iscritto alla gestione commercianti INPS** come socio che lavora nella società.
   Allora il 24% è corretto, e va tenuto presente in ogni leva sotto: i contributi
   commercianti dei soci di SRL possono seguire anche gli utili, non solo il compenso.
2. **TP non è iscritto altrove.** Allora l'aliquota corretta è **35,03%** e mancano circa
   11 punti sul compenso: **≈ 3.600 euro l'anno**, recuperabili dall'INPS per cinque anni,
   con sanzioni civili.

**Semaforo: da chiarire subito con il centro paghe.** Non è una leva, ma condiziona tutte
quelle del § 3.

---

## 2. Francesco Dalla Piazza

### 2.1 Previdenza: contribuzione Inarcassa facoltativa + fondo pensione — **VERDE**

- **Contribuzione facoltativa modulare Inarcassa [V]:** un versamento aggiuntivo in
  percentuale del reddito professionale (fino al 10%), interamente deducibile (art. 10,
  c. 1, lett. e, TUIR) e destinato al montante pensionistico.
- **Fondo pensione:** deduzione fino a **5.164,57 euro** l'anno (art. 8 D.Lgs. 252/2005).
  In uscita è tassato al 15%, che scende fino al 9%.

| | Status quo | Con modulare 10% + fondo pensione |
|---|---:|---:|
| Versato a previdenza | — | ≈ 19.300 |
| **Risparmio d'imposta** | — | **≈ 8.700 l'anno** |
| Netto spendibile | ≈ 74.000 | ≈ 63.500 (fabbisogno 45.000: coperto) |

**Perché è la leva migliore per FDP:** usa due terzi dell'eccedenza, ha un'aliquota
implicita del 45% di sconto all'ingresso, e l'orizzonte di 10 anni coincide con l'età
della pensione. Il costo è la minore liquidità: il capitale diventa pensione.
**[V]** Da verificare sul regolamento Inarcassa vigente: le percentuali ammesse, il limite
del massimale e la rivalutazione del montante.

### 2.2 Studio in forma societaria (STP o società di ingegneria) — **NON CONVIENE**, sui dati

I due volumi lo propongono come leva principale. Rifatto il conto su FDP, **non lo è**.

| | P.IVA (oggi) | STP che paga a FDP 45.000 netti |
|---|---:|---:|
| Compenso a FDP | — | ≈ 79.200 |
| Utile trattenuto in società, dopo IRES 24% e IRAP 3,9% | — | ≈ 38.600 |
| **Netto totale se l'utile esce come dividendo (26%)** | **≈ 74.100** | **≈ 73.600** |

**Perché:**
- IRES più IRAP, poi il 26% sul dividendo, pesano quanto l'IRPEF marginale. Il vantaggio è
  **solo di differimento**, finché l'utile resta in società.
- La società paga l'**IRAP**, che FDP come professionista senza organizzazione non paga.
- Ci sono costi di struttura (qui stimati in 4.000 l'anno).
- **[V]** Se Inarcassa chiede il contributo soggettivo anche sulla quota di utile della
  STP, il saldo diventa negativo.
- Gli incarichi di **responsabile tecnico e consulente ADR** restano personali.
- Il contributo soggettivo scende, e con esso la pensione.

**Quando tornerebbe a convenire:** se l'utile trattenuto finanziasse investimenti che
restano nella società (un immobile, un'attività) invece di essere distribuito. Non è il
caso descritto.

### 2.3 Holding personale sul 25% di Overall — **rinviata al 2028**, GIALLO

- I dividendi di Overall entrano in holding tassati all'1,2% (art. 89 TUIR) e possono
  essere reinvestiti. Il 26% si paga solo quando la cassa arriva a FDP.
- **Per FDP l'utilità è concreta**, perché non ha bisogno dei dividendi di Overall per
  vivere: la holding accumula e investe l'eccedenza al posto suo.
- **Conferimento** a realizzo controllato: art. 177, c. 2-*bis*, TUIR, con partecipazione
  sopra il 20% e holding interamente sua **[V]** sul testo dopo il D.Lgs. 192/2024.
- **Vincolo:** nel biennio 2026-2027 Overall è in concordato. Un cambio nella compagine
  sociale va verificato contro le cause di cessazione dell'art. 21 D.Lgs. 13/2024 **[V]**.
  Prudenzialmente, **conferimento dal 2028**.
- **Rischio:** una holding che si limita a incassare i dividendi di una sola società e
  reinvestirli in liquidità è esposta alla contestazione di abuso (art. 10-*bis* L.
  212/2000). Serve una ragione extrafiscale scritta: investimenti, passaggio generazionale,
  exit.
- **Con l'orizzonte di 10 anni** la holding serve anche per l'uscita: la vendita del 25% da
  parte di una holding può godere della PEX (esenzione al 95%, art. 87 TUIR) se sono
  rispettati i requisiti, fra cui il possesso da almeno 12 mesi e la commercialità di
  Overall.

### 2.4 Dividendi di Overall — VERDE

Le riserve disponibili sono 210.113. **Su una distribuzione integrale, a FDP spettano
52.500 lordi e 38.900 netti.** Per FDP servono a poco oggi: vanno letti insieme al § 2.3,
cioè distribuirli dopo il 2028 alla holding invece che alla persona fisica.

---

## 3. Tazio Pradella

**Il principio, con Overall in concordato fino al 2027:** i costi di Overall non riducono
più l'IRES, perché l'imponibile è fisso. Conta solo come viene tassato TP. Ogni euro di
valore che arriva a TP senza IRPEF e senza contributi costa a Overall meno di un euro di
compenso.

### 3.1 Auto aziendale in uso promiscuo — **VERDE**, con contratto

- Overall prende in noleggio a lungo termine o in leasing un'auto, preferibilmente
  elettrica, e la assegna a TP in uso promiscuo. **TP vende una delle due auto a rate.**
- TP è tassato solo sul **fringe benefit convenzionale**: 15.000 km × costo ACI ×
  **10%** per le elettriche, 20% per le ibride plug-in, 50% per le altre (art. 51, c. 4,
  TUIR come modificato dalla L. 207/2024).
- **[I] Ordine di grandezza:** con un'auto elettrica da circa 6.500 euro l'anno tutto
  compreso, il fringe benefit è di circa 700 euro. Per dare a TP lo stesso valore in
  compenso servirebbero circa 9.500 euro di costo per la società. **Risparmio per Overall
  ≈ 3.000 l'anno, e TP libera la rata dell'auto venduta.**
- **Dal 2028**, finito il concordato, il costo delle auto assegnate in uso promiscuo è
  deducibile al 70%.
- **Dossier:** delibera del CdA, contratto di assegnazione con la quota di uso personale,
  fringe benefit in cedolino.

### 3.2 Fringe benefit fino a 2.000 euro, per chi ha figli a carico — **VERDE** [V]

- Per il 2025-2027 la soglia di esenzione dei fringe benefit è di **2.000 euro** per chi ha
  figli a carico. Include le somme per **utenze domestiche, affitto e interessi del mutuo
  sulla prima casa** (L. 207/2024).
- **TP ha due figli e un mutuo: è il caso tipico.**
- **[V]** Da verificare se l'agevolazione si estende ai titolari di **redditi assimilati**
  (co.co.co. amministratore), e quali adempimenti servono (dichiarazione dei figli a
  carico).
- **Valore:** circa 1.000-1.300 euro l'anno di risparmio combinato fra TP e Overall.

### 3.3 Trasferte e rimborsi — **VERDE** se documentati

- I rimborsi a piè di lista già in essere (circa 15.000-18.000 euro l'anno) sono
  corretti **solo** per le trasferte fuori dal comune della sede, con i giustificativi.
  I rimborsi chilometrici richiedono un prospetto per viaggio con le tariffe ACI.
- In alternativa, o in aggiunta: **indennità di trasferta forfettaria esente** fino a
  **46,48 euro al giorno** in Italia (art. 51, c. 5, TUIR). Le regole sul cumulo con il
  rimborso analitico riducono la soglia **[V]**. Dal 2025 i rimborsi di vitto, alloggio e
  taxi vanno pagati con mezzi tracciabili.
- **Dossier:** regolamento trasferte deliberato dal CdA; report mensile delle trasferte.

### 3.4 Parte del compenso trasformata in dividendo privilegiato — **GIALLO**

- **Nel concordato il dividendo costa meno del compenso.** Togliere 20.000 euro di
  compenso a TP gli fa perdere **≈ 13.400 netti**. Restituirglieli come dividendo richiede
  **≈ 18.100 lordi**, contro **23.200** di costo del compenso con l'INPS. **Overall
  risparmia ≈ 5.100 l'anno.**
- **Il problema:** i dividendi si dividono al 25%. Per indirizzarli a TP servono **diritti
  particolari sugli utili** (art. 2468, c. 3, c.c.), cioè una modifica statutaria con il
  **consenso di tutti i soci**.
- **L'argomento con Maggia e Dall'Oca:** il risparmio va a vantaggio di tutti. Si può
  calibrare il privilegio in modo che il loro dividendo non diminuisca.
- **Rischi:**
  - **INPS:** un socio che lavora nella società e viene remunerato con utili è il caso
    della gestione commercianti (§ 1). Il vantaggio contributivo potrebbe non esistere;
  - **fiscale:** un dividendo che remunera un'attività lavorativa può essere riqualificato
    come compenso;
  - l'utilità si riduce dopo il 2027, anche se resta per TP perché il compenso co.co.co.
    non è deducibile ai fini IRAP.
- **Dossier:** ragione extrafiscale del privilegio (per esempio la remunerazione del
  rischio d'impresa del socio operativo), modifica statutaria con atto notarile, parere
  INPS. **Candidato all'interpello.**

### 3.5 TFM (trattamento di fine mandato) — GIALLO, da costruire per il prossimo mandato

- L'accantonamento annuo è tassato **separatamente** all'uscita, con l'aliquota media degli
  ultimi due anni (circa 23% per TP), invece che con l'aliquota marginale del 33%.
- **Limiti:**
  - la cassa arriva a fine mandato, mentre TP ha un fabbisogno annuo;
  - il contributo di gestione separata è dovuto **[V]**;
  - la delibera deve avere **data certa anteriore** all'inizio del mandato, e il CdA
    attuale è già in carica;
  - con Overall in concordato la deduzione non vale nulla fino al 2027.
- **Utile dal prossimo rinnovo del CdA**, per una quota moderata.

### 3.6 Coniuge — solo se c'è un lavoro reale

L'aliquota della moglie (23%) è più bassa di quella di TP (33%). Un rapporto di lavoro con
Overall ha senso **solo** per una prestazione reale e a prezzo di mercato. È GIALLO, con un
beneficio modesto: 10 punti sulla parte trasferita. Non proposto finché non esiste un ruolo.

---

## 4. Leve comuni

| Leva | Chi | Semaforo | Nota |
|---|---|---|---|
| Distribuzione delle riserve (210.113) | tutti i soci | VERDE | 26% secco; copre il fabbisogno di TP per circa 3 anni |
| Iperammortamento in Overall | società | VERDE [V] | unica leva che riduce il reddito concordato in corso (D01 § 6.5) |
| Welfare aziendale con regolamento per categorie | TP e dipendenti | GIALLO | solo se esteso a una **categoria** di dipendenti, non ai soli soci |

---

## 5. Scartate

| Spunto dei volumi | Perché |
|---|---|
| Royalties del socio su marchio o know-how | Redditi diversi a IRPEF piena, IVA rilevante (V00) |
| "Prestazioni accessorie dei soci tassate al 26%" | Nessuna base normativa: **ROSSO** |
| Crediti d'imposta acquistati a sconto | Cessioni bloccate, responsabilità solidale del cessionario: **ROSSO** |
| Collaborazioni occasionali in luogo di rapporti continuativi | Riqualificazione certa: **ROSSO** |
| Rivalutazione delle quote e cessione alla propria holding | Rischio abuso: **ROSSO** |
| Forfettario | FDP è sopra la soglia di 85.000 |

---

## 6. Sintesi e ordine di esecuzione

| # | Leva | Chi | Valore annuo stimato | Quando |
|---|---|---|---:|---|
| 1 | Chiarire l'INPS di TP (§ 1) | TP | fino a −3.600 se c'è un problema | **subito** |
| 2 | Inarcassa modulare + fondo pensione | FDP | **≈ 8.700** di imposte | entro il 31/12/2026 |
| 3 | Auto aziendale elettrica | TP | ≈ 3.000 per Overall + rata auto di TP | 2026-2027 |
| 4 | Fringe benefit 2.000 (mutuo e utenze) | TP | ≈ 1.000-1.300 | entro il 31/12/2026 [V] |
| 5 | Regolamento trasferte | TP | presidio del rischio | subito |
| 6 | Dividendo privilegiato al posto di parte del compenso | TP (e FDP) | ≈ 5.100 ogni 20.000 convertiti | dopo parere INPS e con consenso dei soci |
| 7 | Holding personale | FDP (TP facoltativo) | differimento del 26% sui dividendi reinvestiti; utile all'exit | dal 2028 |
| 8 | TFM | TP | ≈ 10 punti sull'accantonato | prossimo mandato |

**Conclusione non intuitiva:** per FDP la trasformazione della P.IVA in società **non
produce vantaggio** sui suoi numeri. Il vantaggio concreto è previdenziale (§ 2.1), e poi
patrimoniale con la holding dal 2028. Per TP le leve efficaci sono quelle che
**sostituiscono la spesa personale con benefit esenti** (auto, fringe benefit, trasferte),
più il dividendo privilegiato se gli altri soci ci stanno.
