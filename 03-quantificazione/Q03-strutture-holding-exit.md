# Q03 — Strutture societarie, holding ed exit per Dalla Piazza e Pradella (orizzonte 2027-2039)

**Versione 1** del 25 settembre 2026. **Da sottoporre a verifica indipendente** (R1 e R2).
**Integra la verifica V04** (rilievi G-2, G-3, R-1, N-6), letta prima della stesura.
**Modello:** script `q03.py` nello scratchpad della sessione. Parametri:
- IRPEF 2026 al 23/33/43%, addizionali 2,03%, marginale FDP 45,03%;
- Inarcassa soggettivo 14,5% fino a 147.300, integrativo 4%;
- IRES 24%, IRAP Veneto 4,08%, ritenuta sui dividendi 26%;
- rendimento lordo della liquidità 4% (sensibilità 2-6%), 13 anni (2027-2039).

> Convenzione: [A] accertato su fonte · [I] inferito · [V] da verificare prima di eseguire.
> Semafori come da `00-setup/protocollo-verifica.md`.

---

## Sintesi — sei righe

1. **FDP resta in P.IVA.** STP e società di ingegneria non producono cassa: +2.700 euro in 13 anni la società di ingegneria, −65.000 la STP. Tolgono però circa 116.000 euro di montante Inarcassa. La conclusione «non conviene» di L01 **è confermata**, ma con motivazioni diverse.
2. **Nessuna holding per FDP, se l'obiettivo è la cassa in vita.** L'1,2% rinvia il 26%, non lo toglie. Tolti i costi di struttura, la holding perde **39.000-43.000 euro** in 13 anni. Conviene solo con un obiettivo successorio (≈ +87.000 [V]). Il CPB non è più un ostacolo: la risposta AdE 102/2025, letta nel testo, lo esclude.
3. **Exit di FDP nel 2039: vendere da persona fisica, con la rivalutazione al 21%**, non al 18%: l'aliquota è cambiata dal 2026. Su un prezzo di 250.000 euro gli restano 194.500 euro, contro 183.500 passando dalla holding con PEX.
4. **La struttura che produce valore è una holding di Tazio Pradella che compra le quote dei soci uscenti** (Dall'Oca, Maggia, FDP). Paga il prezzo con dividendi tassati all'1,2% invece che al 26% (più i contributi commercianti): **≈ 85.000 euro risparmiati ogni 250.000 di prezzo**. L'alternativa è il recesso rimborsato con le riserve. Serve **subito un patto parasociale sulle uscite**.
5. **Dividendo privilegiato al posto di compenso o fatture: scartato.** Per TP è ROSSO: con la Cassazione del settembre 2026 i contributi commercianti lo rendono in perdita. Per FDP il guadagno è di circa 2.600 euro l'anno solo nel 2027, ed è assorbito dal montante che perde e dal rischio di riqualificazione.
6. **Ufficio di FDP:** conviene solo se Overall ne ha un bisogno reale, con una locazione a canone di mercato dal 2028. Costa 1,26 euro per euro netto, contro 1,88 del dividendo. Società semplice e altre strutture: nessun valore.

---

## 0. Premesse corrette rispetto alla richiesta e a L01

| # | Premessa | Stato | Fonte |
|---|---|---|---|
| P-1 | Rivalutazione delle quote al **18%** | **Superata: 21%** per le quote possedute al 1/1/2026 e successive (L. 199/2025, art. 1, c. 144, che modifica l'art. 5, c. 2, L. 448/2001). Perizia e versamento entro il **30/11** di ogni anno, anche in tre rate. I terreni restano al 18% | [A] su fonte secondaria che riporta il testo del comma (FISCOeTASSE) |
| P-2 | Il conferimento delle quote in holding è vietato durante il CPB, quindi va rinviato al 2028 | **Falso.** Nella risposta **102 del 15/04/2025** l'AdE esamina il socio unico di una S.r.l. che conferisce l'intera quota in una sua S.r.l. La società in concordato «non si rende né conferente/cedente né conferitaria/cessionaria», e per la S.r.l. il conferimento delle sue quote «non integra la causa di cessazione» dell'art. 21, c. 1, lett. b-*ter*. **Le modifiche della compagine rilevano solo per le società e associazioni dell'art. 5 TUIR** (FAQ 17/10 e 28/10/2024, richiamate nella risposta) | [A] **testo della risposta letto** (PDF AdE) |
| P-3 | V02, tabella dell'art. 11: «un ingresso in compagine nel 2026 esclude l'accesso» | **Da correggere per Overall.** È una S.r.l. (art. 73), quindi l'aumento del numero dei soci non è causa di esclusione né di cessazione. Restano cause solo le operazioni straordinarie di cui la **società stessa** è parte: fusione, scissione, conferimento **fatto o ricevuto da Overall** | [A] risposta 102/2025 |
| P-4 | PEX dopo 12 mesi | **60 mesi** per le partecipazioni conferite ai sensi del c. 2-*bis* (art. 177, c. 2-*quater*, TUIR) | [A] fonti secondarie concordanti (V04, Studio Mastromattei) |
| P-5 | Art. 89 TUIR: dividendi sempre all'1,2% nella holding | **Dal 2026 solo per partecipazioni ≥ 5% o con valore fiscale ≥ 500.000 euro.** Vale sia per i dividendi (delibere dal 1/1/2026) sia per la PEX (plusvalenze dal 1/1/2026): L. 199/2025, art. 1, cc. 51-55. Il 25% di Overall passa la soglia. **Un portafoglio di titoli quotati detenuto dalla holding no**: i suoi dividendi e le sue plusvalenze sono tassati al 24% pieno | [A] FiscoOggi |
| P-6 | Il compenso di amministratore di FDP in una sua società di ingegneria va in gestione separata (V04, E-8) | **Da precisare.** Per la circ. 105/E/2001 un ingegnere amministratore di una società di ingegneria ha una connessione oggettiva con la professione: il compenso è **lavoro autonomo**, con Inarcassa, se FDP resta in P.IVA. Anche Inarcassa lo prevede (la società non può dedurre l'integrativo sulla fattura dell'amministratore). La conclusione **non cambia** in nessuna delle due letture | [A] D01 § 5.1; FAQ Inarcassa società di ingegneria |

---

## 1. P.IVA, STP, società di ingegneria, società con altri soci

### 1.1 Le regole

| | P.IVA (oggi) | S.r.l. società di ingegneria | STP S.r.l. |
|---|---|---|---|
| Imposte sul reddito | IRPEF marginale 45,03% | IRES 24% + IRAP 4,08%, poi 26% all'uscita | come la società di ingegneria |
| IRAP | **esclusa** per le persone fisiche esercenti arti e professioni dal 2022 (L. 234/2021, art. 1, c. 8) [A] | dovuta. Il compenso di lavoro autonomo abituale è deducibile; quello co.co.co. no [I] | dovuta |
| Inarcassa **soggettivo** | 14,5% del reddito, fino al massimale | **nessuno sugli utili**; solo sul compenso del socio che fattura come professionista [A] | **anche sulla quota di reddito della STP** attribuita al socio, distribuita o no [A, Inarcassa] |
| Inarcassa **integrativo** 4% | a carico del cliente | la società lo applica ai clienti e lo versa; non è deducibile quello sulla fattura dell'amministratore [A] | proporzionale alla quota dei soci iscritti [A] |
| Incarichi personali (RT Albo Gestori, consulente ADR per Ecodent) | restano suoi | **restano personali**: nomina e responsabilità in capo alla persona fisica. Fatturarli tramite la società non è pacifico [V] | idem |
| Neutralità del passaggio | — | nessuna norma di neutralità: una S.r.l. ordinaria non è STP [I] | conferimento neutrale dell'attività professionale ai sensi dell'**art. 177-*bis* TUIR** (D.Lgs. 192/2024) [V] sul testo |
| Costi | nessun costo in più | ≈ 4.000 l'anno, più 3.000 per aprire e 3.000 per chiudere [I] | idem |

**[I] Vincolo pratico.** FDP deve comunque tenere la P.IVA, per gli incarichi personali presso Ecodent, il suo cliente principale. La società conterrebbe quindi solo la parte di attività trasferibile. Il modello sotto la trasferisce tutta, ed è l'ipotesi più favorevole alla società.

### 1.2 I numeri: cassa al 2039 con l'utile trattenuto e reinvestito

FDP ha 140.890 euro di reddito e un fabbisogno di 45.000. Nella P.IVA l'eccedenza è investita personalmente, con i rendimenti tassati al 26%. Nella società FDP preleva quanto gli serve per coprire i 45.000 netti, come amministratore con fattura, cioè come lavoro autonomo con Inarcassa. Il resto resta in società: è investito con i rendimenti al 24% e viene liquidato nel 2039 con il 26%.

| Scenario, rendimento lordo 4% | Netto annuo spendibile | Accumulato annuo | **Cassa netta al 2039** | Soggettivo versato in 13 anni | Totale con il montante valutato al 65% (netto della tassazione della pensione) |
|---|---:|---:|---:|---:|---:|
| **A. P.IVA** | 74.017 | 29.017 (investiti in proprio) | **452.060** | 265.578 | **624.686** |
| B. Società di ingegneria, FDP amministratore con fattura | 45.000 | 39.250 (trattenuti) | 454.745 | 149.198 | 551.724 |
| C. STP | 45.000 | 33.365 | 386.565 | 251.477 | 550.025 |
| *B con compenso in gestione separata (lettura V04)* | *≈ 70.100 a regime* | | *peggiore di A* | *nessun montante Inarcassa* | |

**Sensibilità al rendimento** (differenza B − A di cassa, e con il montante):

| Rendimento lordo | B − A di cassa | B − A con il montante |
|---:|---:|---:|
| 2% | +1.400 | −74.200 |
| 4% | +2.700 | −73.000 |
| 6% | +4.300 | −71.400 |

Nessuno dei due scenari comprende i circa 6.000 euro di apertura e chiusura, né il maggior costo annuo della contabilità.

**Perché il conto torna così** (per ogni euro marginale):
- P.IVA: 0,47 netti più 0,145 di montante;
- società: 0,72 trattenuti, che diventano 0,53 all'uscita.

Differire il 26% non vale nulla, perché l'aliquota d'uscita è proporzionale. Il fattore di crescita dei 0,72 trattenuti e dei 0,47 investiti è quasi uguale: rendimenti tassati al 24% contro il 26%. Quello che la società guadagna in cassa (≈ 6 centesimi per euro) lo perde in montante (14,5 centesimi).

**L'ipotesi «l'utile trattenuto finanzia investimenti»** non cambia il segno. Se l'investimento rende il 6% dentro la società (tassato al 24% più IRAP) o fuori (al 26%), lo scarto resta di pochi migliaia di euro in 13 anni. Il vantaggio diventerebbe rilevante solo con un investimento che FDP **non potrebbe fare da persona fisica** (un'azienda, una partecipazione di controllo). Non è il suo caso: ha un fabbisogno stabile e un orizzonte di uscita.

**D. Società fra professionisti con altri soci**, oppure attività di FDP spostata in Overall. Il fisco è quello di B o C. In più una parte del valore va agli altri soci: in Overall il 75% dell'utile incrementale è di Maggia, Dall'Oca e TP, salvo diritti particolari (§ 3, scartati). V02 segnala inoltre lo spostamento di attività dal socio alla società come indicatore di selezione sotto CPB. **Scartata.**

**Verdetto § 1:** **P.IVA confermata.** Nessun semaforo, perché è lo status quo. Le leve di FDP restano quelle previdenziali, fuori perimetro di questo documento (L01 § 2.1 corretto da V04 G-1, riscatto N-5).

---

## 2. Holding personali

### 2.1 Requisiti e compatibilità

- **Art. 177, c. 2-*bis*, TUIR** (testo D.Lgs. 192/2024, conferimenti dal 31/12/2024) [A]:
  - realizzo controllato anche senza controllo, se la partecipazione conferita supera il **20% dei voti o il 25% del capitale**. FDP e TP hanno il 25% dei voti: **requisito soddisfatto**;
  - la conferitaria deve essere partecipata **unicamente dal conferente o**, se è una persona fisica, **da lui e dai suoi familiari** (art. 5, c. 5): coniuge, parenti entro il terzo grado, affini entro il secondo. Quindi anche una holding familiare.
- **Valore di realizzo** = aumento del patrimonio netto della holding. Se la holding iscrive la quota al costo fiscale (**2.500 euro**, un quarto del capitale di 10.000 [I]: va verificato che le quote siano state sottoscritte e non acquistate a prezzo diverso), **nessuna plusvalenza**.
- **Art. 177, c. 2-*quater*:** PEX sulla quota conferita solo dopo **60 mesi**. Con un conferimento nel 2026 la PEX è disponibile dal 2031 [A].
- **CPB di Overall:** **VERDE.** Il conferimento è un'operazione del **socio**, non della società (risposta 102/2025, testo letto). Il numero dei soci resta quattro, e comunque per una S.r.l. non conterebbe (P-3).
  - Controllo residuo: la holding non deve essere già socia di Overall prima dell'operazione. Overall non deve conferire né ricevere nulla.
- **Società di comodo** (art. 30 L. 724/1994) [I]. I ricavi presunti sono il 2% del valore delle partecipazioni e dei titoli, e il test è sempre superato finché arrivano i dividendi di Overall (≈ 34.000 l'anno su una quota iscritta a 2.500). Il rischio compare **dopo l'exit**, con la holding piena di liquidità investita in titoli e senza dividendi. [V] sul testo vigente e sulla riforma delle società di comodo.
- **Abuso (art. 10-*bis*)** [I].
  - La holding in sé è un'opzione legittima (c. 4).
  - Diventa contestabile la «holding cassaforte» che gira la liquidità al socio con finanziamenti, spese personali o acquisti di beni di godimento: è una distribuzione occulta.
  - Vale anche per la rivalutazione seguita dalla cessione alla propria holding: è **ROSSO**, già scartato in L01.

### 2.2 FDP: la holding conviene? Il conto sull'intero ciclo

FDP non ha bisogno dei dividendi di Overall prima del 2039. Confronto fra riceverli personalmente e investirli (26% più rendimenti al 26%) e farli salire in holding (1,2% più rendimenti al 24%, costi di 3.000 l'anno e 3.000 di apertura), con distribuzione al socio nel 2039 al 26%.

| Dividendo annuo a FDP | Rendimento | Persona fisica | Holding, al netto per FDP nel 2039 | **Differenza** |
|---:|---:|---:|---:|---:|
| 25.000 | 3% | 275.293 | 236.865 | **−38.428** |
| 34.000 | 4% | 391.966 | 351.162 | **−40.804** |
| 50.000 | 5% | 603.703 | 560.159 | **−43.543** |

**Le riserve di 210.113 euro** (52.528 a FDP) meritano una riga a parte. V04 G-3 le presenta come «13.657 di imposta contro 630». **È solo un differimento.** Se nel 2039 FDP preleva, i due percorsi si equivalgono: −229 euro al 3%, +29 al 5%. Ai valori attuali il 26% applicato all'uscita si capitalizza esattamente come la somma investita.

**Perché la holding non conviene a FDP:** con un'imposta d'uscita proporzionale e uguale (26%), il differimento vale zero. Resta solo lo scarto di 2 punti fra il 24% e il 26% sui rendimenti. Non basta a pagare i costi di struttura. **Fa eccezione** la holding che investe in partecipazioni oltre il 5% di società commerciali: dividendi all'1,2% e PEX. Ma questa è attività d'impresa, non impiego del risparmio.

**Quando conviene: la successione [V].**
- Se la holding resta ai discendenti, il 26% sui dividendi accumulati **non si paga mai**. Il costo fiscale della quota ereditata è il valore dichiarato in successione (art. 68, c. 6, TUIR [V]).
- Differenza stimata: holding 478.971 contro 391.966 in capo alla persona fisica, cioè **≈ +87.000** su 34.000 euro l'anno per 13 anni al 4%.
- Tre condizioni:
  - l'erede non deve liquidare subito la holding: con l'art. 47, c. 7, TUIR («prezzo pagato per l'acquisto o la sottoscrizione») lo step-up in caso di liquidazione è **controverso** [V];
  - FDP deve rinunciare in vita a quella cassa;
  - l'esenzione dall'imposta di successione sulle partecipazioni di controllo ai discendenti (art. 3, c. 4-*ter*, D.Lgs. 346/1990 [V]) vale per il 100% della holding, non per il 25% di Overall. Con franchigie di 1 milione per figlio è comunque marginale.
- **La composizione familiare di FDP non è nel fascicolo.**

**Verdetto FDP:**
- **nessuna holding** se l'obiettivo è la cassa in vita, che è l'obiettivo dell'incarico;
- **holding familiare ai sensi del c. 2-*bis*: GIALLO**, solo se FDP dichiara un obiettivo successorio e ha discendenti. In quel caso va conferita **prima** di distribuire le riserve e prima della delibera sul bilancio 2026, cioè entro aprile 2027.

### 2.3 Exit di FDP nel 2039: cessione del 25%

Costo fiscale 2.500 euro. Il prezzo dipende da Overall fra 13 anni. Tre ipotesi: 150.000, 250.000 e 400.000 euro per il 25%, pari a 1-2,5 volte l'utile netto normalizzato della quota, più la liquidità [I].

| Prezzo del 25% | Persona fisica, 26% sulla plusvalenza | **Persona fisica con rivalutazione al 21%** (perizia 3.000) | Holding con PEX, cassa nella holding | Holding con PEX, poi distribuita a FDP | Recesso tipico (reddito di capitale al 26%) |
|---:|---:|---:|---:|---:|---:|
| 150.000 | 111.650 | **115.500** | 148.230 | 110.340 | 111.650 |
| 250.000 | 185.650 | **194.500** | 247.030 | 183.452 | 185.650 |
| 400.000 | 296.650 | **313.000** | 395.230 | 293.120 | 296.650 |

- **Se la cassa deve arrivare a FDP, vince la persona fisica con rivalutazione**: +8.900 euro su 250.000.
  - La rivalutazione si fa nell'anno della vendita, sul valore al 1° gennaio.
  - Per un'uscita nel 2039 non serve farla oggi. L'aliquota è cambiata tre volte in cinque anni (14, 16, 18, 21%) [A].
- **La PEX conviene solo se il prezzo resta nella holding** e viene reinvestito in attività d'impresa, o passato agli eredi.
- **Nel recesso tipico la rivalutazione non serve:** l'eccedenza è reddito di capitale ai sensi dell'art. 47, c. 7, e la rideterminazione vale solo per i redditi diversi [A, prassi e dottrina concordi, fonti Ratio e DB].
  - Il recesso costa al venditore 5 punti in più della cessione rivalutata, ma è il canale più economico per chi resta (§ 2.4).
- Le partecipazioni ereditate hanno lo step-up: la «exit per successione» azzera la plusvalenza anche senza holding [V].

### 2.4 TP: la holding come veicolo d'acquisto delle quote dei soci uscenti

**Il fatto che cambia la prospettiva [A, V02]:** i soci hanno 66 (Dall'Oca), 62 (Maggia), 55 (FDP) e 41 anni (TP). Nei prossimi 13 anni **almeno tre quote del 25% cambieranno mano**, e il successore naturale è TP. Oggi però TP ha un fabbisogno scoperto (V04, R-2) e nessun capitale.

**Chi paga il prezzo e con quale imposta.** Dividendi lordi di Overall necessari per pagare il prezzo P:

| Prezzo del 25% | TP persona fisica (26%) | TP persona fisica con commercianti oltre il minimale (Cass. 2026) | **TP Holding (1,2%)** | Risparmio della holding sul 26% |
|---:|---:|---:|---:|---:|
| 150.000 | 202.703 | 302.908 | **151.822** | **50.881** |
| 250.000 | 337.838 | 504.847 | **253.036** | **84.801** |
| 400.000 | 540.541 | 807.754 | **404.858** | **135.682** |

**Carico fiscale totale del passaggio di una quota** (imposte del venditore più quelle sui dividendi che finanziano il compratore):

| Prezzo | Cessione a TP Holding, venditore con rivalutazione | Recesso rimborsato da Overall con le riserve | Cessione a TP persona fisica | Idem, con i commercianti |
|---:|---:|---:|---:|---:|
| 150.000 | **36.322** | 38.350 | 84.203 | 184.408 |
| 250.000 | **58.536** | 64.350 | 140.338 | 307.347 |
| 400.000 | **91.858** | 103.350 | 224.541 | 491.754 |

**La struttura** [I]:

1. **TP Holding S.r.l.**, costituita da TP (eventualmente con la moglie o i figli) **quando un acquisto è concordato**, non prima: una holding vuota costa senza rendere.
   - **Non serve conferire il 25% di TP.** Tenerlo in capo a lui preserva l'iscrizione ai commercianti e il 24% sulla gestione separata.
   - Se TP smettesse di essere socio diretto di Overall, cambierebbe il suo inquadramento INPS. La gestione separata potrebbe salire al 33,72% [V]: va chiesto a un consulente del lavoro prima di qualsiasi conferimento.
2. **Acquisto a valore di perizia**, pagato con un mutuo bancario (pegno sulle quote) o con una **dilazione concessa dal venditore**.
   - La dilazione ha un effetto utile: la plusvalenza del venditore si tassa per cassa, man mano che incassa [I].
3. **Servizio del debito:**
   - P = 250.000 in 8 anni al 4,5% dà una rata di **37.902 euro**, cioè 38.363 di dividendi lordi alla holding;
   - serve una distribuzione di Overall di **≈ 153.000 euro l'anno**, pro quota. È compatibile con un utile netto di 130.000-190.000 euro solo se Overall distribuisce quasi tutto;
   - **effetto collaterale:** TP riceve la stessa cifra sul proprio 25%. Oltre il minimale (18.808 euro) paga il 24,48% di commercianti, ≈ 4.800 euro l'anno. Se ne tiene conto nella politica dei dividendi, oppure si allunga il piano.
4. **Interessi passivi:** la holding non ha un ROL proprio, quindi la deduzione è limitata (art. 96).
   - Con il **consolidato fiscale** (art. 117), dal momento in cui TP Holding supera il 50% di Overall (seconda quota più il conferimento di quella di TP, oppure terza quota), gli interessi usano il ROL di Overall [V].
5. **Compatibilità CPB:** la cessione di quote fra soci e terzi non tocca Overall (risposta 102/2025). **VERDE** anche nel 2026-2027.

**Semaforo: GIALLO leggero.**
- L'acquisto da un terzo, a valore di mercato, con debito servito dai dividendi è fisiologico.
- Le contestazioni possibili sono due:
  - il **prezzo**, cioè il valore normale per il venditore che rivaluta: serve una perizia coerente con il prezzo;
  - la **deducibilità degli interessi**.
- **Nessuna fusione con Overall** (niente *merger leveraged buyout*, art. 2501-*bis* c.c.): è lì che nascono le contestazioni.

**Alternativa: recesso rimborsato con le riserve** (art. 2473, c. 4, c.c.).
- Per chi resta costa zero di imposte personali: non serve distribuire dividendi per pagare il prezzo.
- Al venditore costa il 26% invece del 21% (tabella § 2.3).
- **La quota del receduto si ripartisce pro quota fra tutti i rimasti**, non solo a TP. È adatto se i rimasti vogliono crescere insieme; se si vuole che TP diventi maggioritario, serve la holding.
- Una S.r.l. non può acquistare quote proprie (art. 2474 c.c.) [A]: il recesso è l'unica via «interna».
- Richiede una causa di recesso nello statuto oppure l'accordo di tutti [V sullo statuto vigente].

**La leva immediata, a costo quasi nullo: un patto parasociale sulle uscite** fra i quattro soci. Contenuto:
- opzioni di acquisto (*call*) a favore di TP o della sua holding e di vendita (*put*) per i soci che raggiungono l'età di uscita;
- una **formula di prezzo** (per esempio patrimonio netto rettificato più un multiplo dell'utile medio del triennio);
- prelazione e gradimento coordinati con lo statuto;
- una scelta preventiva fra cessione e recesso.

Non è un'operazione della società: **nessun effetto sul CPB**. La durata dei patti nelle S.r.l. è discussa (si usa il limite di 5 anni rinnovabile) [V].

---

## 3. Diritti particolari sugli utili e dividendo privilegiato

### 3.1 Fattibilità civilistica [A sul codice, I sull'interpretazione]

- L'art. 2468, c. 3, c.c. ammette diritti particolari «riguardanti … la distribuzione degli utili» attribuiti a **singoli soci**. Sono personali: si estinguono con il trasferimento della quota. È un pregio per l'exit.
- Per introdurli serve una **modifica dell'atto costitutivo** con atto notarile.
- Per la prevalenza degli orientamenti notarili serve il **consenso di tutti i soci**, perché altera la parità. Per modificarli dopo, l'art. 2468, c. 4, richiede l'unanimità salvo diversa previsione [V sulle massime notarili].
- Nessun impatto sul CPB: la modifica statutaria non è un'operazione straordinaria [I].

### 3.2 TP: ROSSO (conferma di V04 R-1)

- Le sentenze della **Cassazione, sezione lavoro, n. 25377 del 16/09/2026** e collegate (fino alla 25383, oltre alle 25465-25467 citate in V04) stabiliscono che la base dei contributi commercianti del socio lavoratore è il reddito **fiscalmente imputato**, cioè gli utili distribuiti [A: esistenza e massima confermate su più fonti secondarie; testo integrale non letto].
- Un dividendo privilegiato a TP oltre il minimale sconta quindi 26% più 24,48%: il cambio compenso → dividendo costa **≈ −3.650 euro ogni 20.000** (V04).
- In più c'è il profilo dell'art. 10-*bis*: il privilegio calibrato 1:1 sul compenso tagliato è remunerazione del lavoro.
- **Scartato.**

### 3.3 FDP: fatture a Overall (2.400 al mese) sostituite da un dividendo privilegiato

| Per 28.800 euro l'anno di fatture | CPB 2026-2027 | Ordinario dal 2028 |
|---|---:|---:|
| Netto di FDP dalla fattura | 13.536 (+ 4.176 di montante) | 13.536 (+ 4.176) |
| Dividendo privilegiato che gli dà lo stesso netto | 18.292 | 18.292 |
| Aumento dell'utile netto di Overall senza la fattura | 28.800 (reddito concordato fisso) | 20.713 |
| **Residuo da dividere al 25%** | **10.508 → 2.627 a socio** | 2.421 → **605 a socio** |

**Come renderlo vantaggioso per gli altri due soci:**
- il privilegio va fissato in un **importo pari al solo netto equivalente** (18.292);
- il residuo si ripartisce pro quota;
- così Maggia e Dall'Oca guadagnano 2.627 euro l'anno nel CPB e 605 dopo.

**Perché si scarta comunque:**
1. **FDP perde il montante:** 4.176 euro l'anno, ≈ 2.700 netti di pensione. È più di quanto guadagna.
2. **Si riduce a un anno utile, il 2027.** Tra modifica statutaria e delibera sul bilancio 2026 non si fa prima, e dal 2028 il valore è marginale.
3. **Riqualificazione [R1].** La prestazione tecnica continua e viene pagata con utili. Il verificatore la riqualifica come compenso di lavoro autonomo (IRPEF e Inarcassa) oppure la contesta come abuso: esiste un'alternativa fisiologica, la fattura, scartata solo per l'imposta. **GIALLO tendente al ROSSO.**
4. Il problema delle fatture generiche (D01 § 6.4, punto 2) **si risolve con il dossier**, non spostando il pagamento sugli utili.

---

## 4. Altre strutture

| Struttura | Esito | Numeri e motivazione |
|---|---|---|
| **Ufficio di proprietà di FDP locato a Overall** | **GIALLO, solo se c'è un bisogno reale** (per esempio una sede operativa a Padova). Dal 2028 | Canone tassato a IRPEF sul 95% (art. 37, c. 4-*bis*, TUIR); niente cedolare per il non abitativo. Costo per euro netto a FDP: **1,26** in regime ordinario contro **1,88** del dividendo; **1,75** sotto CPB, contro 1,35 del dividendo. Quindi **non nel 2026-2027**. Dossier: perizia del canone, contratto registrato, uso effettivo documentato, delibera del CdA con l'astensione di FDP (art. 2475-*ter*). [V] **Chi è il locatore della sede di Villafranca** (B8: 13.032 euro) e che uso ha oggi l'ufficio di FDP (V04, N-6) |
| Ufficio in società semplice | **Scartata** | Una società semplice trasparente tassa come FDP. Il conferimento costa registro e ipocatastali. Nessuna cassa in più |
| Holding familiare per il passaggio generazionale | Vedi § 2.2 | Solo se c'è un obiettivo successorio dichiarato |
| Trust | **Scartata** | Il D.Lgs. 139/2024 tassa all'attribuzione; nessun beneficio di cassa |
| Rivalutazione e cessione della quota alla propria holding | **ROSSO** (L01 § 5) | Estrazione di riserve travestita da plusvalenza |
| Spostare l'attività di FDP in Overall | **Scartata** | § 1.2, D |

---

## 5. Semafori e valori

| # | Raccomandazione | Chi | Semaforo | Valore | Quando |
|---|---|---|---|---|---|
| 1 | Restare in P.IVA; niente STP né società di ingegneria | FDP | — (status quo) | evita −73.000 fra cassa e montante in 13 anni | — |
| 2 | Patto parasociale sulle uscite (call/put, formula di prezzo, cessione o recesso) | 4 soci | **VERDE** | presupposto dei risparmi del # 3 | entro il 31/03/2027 |
| 3 | TP Holding come acquirente delle quote uscenti | TP | **GIALLO** leggero | **≈ 51.000-136.000 per quota** (≈ 85.000 su 250.000) | alla prima uscita concordata |
| 4 | Recesso con rimborso dalle riserve, in alternativa al # 3 | soci che restano | GIALLO [V statuto] | −26% per chi resta, −5 punti per chi esce | come sopra |
| 5 | Exit di FDP da persona fisica con rivalutazione | FDP | **VERDE** | +8.900 su 250.000 rispetto alla holding con PEX | 1/1 e 30/11 dell'anno di vendita |
| 6 | Holding di FDP | FDP | **nessuna** per la cassa; **GIALLO** solo per la successione | −40.000 in vita; ≈ +87.000 per gli eredi [V] | se sì, entro aprile 2027 |
| 7 | Dividendo privilegiato | TP / FDP | **ROSSO** / GIALLO-ROSSO | TP −3.650 ogni 20.000; FDP ≈ 0 netto | scartato |
| 8 | Ufficio di FDP locato a Overall | FDP | GIALLO, solo con bisogno reale | 1,26 contro 1,88 per euro netto | dal 2028 |

**Rischio estinto** per le operazioni del 2026-2027 (termine ordinario): il 31/12 del quinto anno successivo alla dichiarazione [I]. Per la dichiarazione 2027 sul 2026, il 31/12/2032.

---

## 6. Dossier difensivi

**TP Holding (# 3):**
- atto costitutivo con oggetto di assunzione di partecipazioni;
- verbale con la **ragione economica**: continuità dell'impresa, ricambio della compagine, governance;
- perizia di stima della quota comprata, coerente con la perizia di rivalutazione del venditore;
- contratto di finanziamento o di dilazione;
- piano di rimborso legato alla politica dei dividendi deliberata da Overall;
- **nessun** finanziamento della holding a TP e nessuna spesa personale;
- nessuna fusione con Overall.

**Patto parasociale (# 2):**
- scrittura con data certa (PEC o registrazione);
- formula di prezzo;
- riferimento allo statuto (prelazione, gradimento, cause di recesso), da verificare sulla copia vigente.

**Holding di FDP, solo nell'ipotesi successoria (# 6):**
- atto di conferimento con richiamo all'art. 177, c. 2-*bis*, e iscrizione della quota al costo fiscale;
- composizione familiare;
- politica d'investimento scritta;
- divieto di finanziamenti al socio e di beni in godimento;
- verbale sulla ragione successoria.

**Ufficio (# 8):**
- perizia del canone;
- contratto registrato;
- evidenza dell'uso da parte di Overall;
- delibera del CdA con l'astensione di FDP.

---

## 7. Calendario

| Data | Azione | Chi |
|---|---|---|
| entro il 02/11/2026 | Adesione di Overall al CPB (D01). **Nessun vincolo** sulle leve di questo documento: le operazioni sulle quote sono dei soci | commercialista |
| entro il 30/11/2026 | Rivalutazione delle quote al 21% (valore al 1/1/2026) **solo se** Dall'Oca o Maggia vendono entro il 2027. Altrimenti si aspetta l'anno della vendita | soci uscenti |
| entro il 31/12/2026 | Raccolta dei dati: statuto vigente (prelazione, gradimento, recesso), orizzonte d'uscita di ciascun socio, famiglia di FDP, uso dell'ufficio, locatore della sede | proprietà |
| entro il 31/03/2027 | Patto parasociale sulle uscite | 4 soci |
| entro aprile 2027 | Solo se FDP sceglie l'obiettivo successorio: holding familiare ai sensi del c. 2-*bis* **prima** della delibera sul bilancio 2026 e prima di distribuire le riserve | FDP |
| alla prima uscita concordata | Costituzione di TP Holding, perizia, finanziamento, acquisto. Parere del consulente del lavoro sull'inquadramento INPS di TP | TP |
| dal 2028 | Ufficio locato a Overall, se c'è un bisogno reale | FDP, CdA |
| 2039 | Exit di FDP: perizia al 1/1, rivalutazione entro il 30/11, cessione a TP Holding | FDP |

---

## 8. Punti [V] che decidono

1. **Statuto vigente:** clausole di prelazione, gradimento e recesso, e diritti particolari eventualmente già previsti.
2. **Orizzonte d'uscita** di Dall'Oca e Maggia, e disponibilità di TP a diventare maggioritario.
3. **Famiglia di FDP** (discendenti) e sua preferenza fra cassa in vita e patrimonio agli eredi.
4. **Costo fiscale effettivo delle quote**: 2.500 se sottoscritte, altrimenti il prezzo d'acquisto.
5. **Inquadramento INPS di TP** se in futuro conferisce la propria quota.
6. **Step-up successorio** in caso di liquidazione della holding (art. 47, c. 7, contro art. 68, c. 6, TUIR).
7. **Testo vigente** di art. 177-*bis*, art. 30 L. 724/1994 e art. 3, c. 4-*ter*, D.Lgs. 346/1990, da rileggere nei testi unici in vigore dal 2027.

---

## Fonti

- [AdE, risposta n. 102 del 15/04/2025 — CPB, cessione o conferimento di partecipazioni](https://www.agenziaentrate.gov.it/portale/documents/20143/8902784/Risposta+n.+102_2025.pdf/032a23cc-b9ac-575a-24c1-3815c48ba922?t=1744708431002) (testo letto)
- [Brocardi — art. 177 TUIR, testo vigente](https://www.brocardi.it/testo-unico-imposte-redditi/titolo-iii/capo-iii/art177.html)
- [Studio Mastromattei — art. 177, c. 2-*bis* e 2-*quater*, holding period di 60 mesi](https://www.studiomastromattei.it/holding-e-conferimento-di-partecipazioni-qualificate-il-realizzo-controllato-dellart-177-comma-2-bis-tuir/)
- [Quotidianopiù — unipersonalità e holding](https://www.quotidianopiu.it/dettaglio/13588222/conferimenti-di-partecipazioni-qualificate-unipersonalita-e-holding)
- [CNDCEC — conferimento di partecipazioni a realizzo controllato dopo la riforma (marzo 2025)](https://commercialisti.it/wp-content/uploads/2025/03/2025_03_31_Il-conferimento-di-partecipazioni-a-realizzo-controllato-dopo-la-riforma_def.pdf)
- [FiscoOggi — plusvalenze e dividendi dopo la legge di bilancio 2026 (L. 199/2025, cc. 51-55)](https://www.fiscooggi.it/portale/-/fiscalit%C3%A0-plusvalenze-e-dividendi-cosa-cambia-dopo-il-bilancio-2026)
- [FISCOeTASSE — rivalutazione delle partecipazioni al 21% (L. 199/2025, c. 144)](https://www.fiscoetasse.com/approfondimenti/16979-rivalutazione-partecipazioni-con-aliquota-al-21-e-terreni-al-18.html)
- [Inarcassa — obblighi della società tra professionisti](https://www.inarcassa.it/per-te/azienda/societa-tra-professionisti/obblighi-della-societa-tra-professionisti)
- [Inarcassa — FAQ società di ingegneria](https://www.inarcassa.it/articoli/faq-societa-di-ingegneria)
- [Sole 24 Ore, Esperto risponde — società di ingegneria e Inarcassa](https://www.espertorisponde.ilsole24ore.com/quesito/societa-di-ingegneria-basta-la-contribuzione-a-inarcassa/627309)
- [Commercialista Telematico — Cass. 25377/2026, contributi e utili non distribuiti](https://www.commercialistatelematico.com/articoli/2026/09/contributi-inps-soci-srl-utili-non-distribuiti.html)
- [Informazione Fiscale — utili di S.r.l. e contributi, la Cassazione ribalta la posizione INPS](https://www.informazionefiscale.it/contributi-inps-utili-srl-cassazione-base-imponibile)
- [Ratio — rivalutazione delle quote e recesso del socio](https://www.ratio.it/rivalutazione-quote-e-recesso-del-socio/)
- [DirittoBancario — costo fiscale della partecipazione in caso di recesso](https://www.dirittobancario.it/art/il-costo-fiscale-della-partecipazione-caso-di-recesso-da-societa-di-capitali/)
- Codice civile: artt. 2468, 2473, 2474, 2475-*ter*, 2501-*bis*. TUIR: artt. 37, 47, 68, 87, 89, 96, 117, 177. L. 234/2021, art. 1, c. 8. Circ. AdE 105/E/2001 (tramite D01 § 5.1).
- Interni: D01 §§ 4.3, 5.5, 6; L01 §§ 2.2, 2.3, 3.4; V02; V04 (R-1, R-2, G-2, G-3, N-6); `spunti-lib1.md` A1, C1, C3, C6.
