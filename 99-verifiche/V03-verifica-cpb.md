# V03 — Verifica indipendente del § 6 di D01 (decisione CPB 2026-2027)

**Revisori:** R1 (verificatore, ufficiale GdF / funzionario AdE) e R2 (tributarista, per calcoli
e norme). Chiave di lettura: *quale numero è sbagliato, quale norma è letta male, dove si rompe il
fascicolo quando arriva un accesso?*

**Data della verifica:** 25 settembre 2026
**Documento verificato:** `01-diagnosi/D01-diagnosi.md`, **versione 3** del 25/09/2026. Oggetto
principale il § 6 riscritto; esaminati anche header, § 7 e § 8 punto 3 (`git diff` rispetto alla
versione 2), e le parti delle versioni precedenti su cui il § 6 si appoggia (§ 3, § 4.3, § 5.5).

**Fonti primarie riscontrate:**

- `dati/2026 CPB/message.txt`: mail della commercialista del 14/09 e del 18/09/2026 (società);
- `dati/2026 CPB/Esito del calcolo dichiarato OVERALL GROUP SRL.pdf`: ISA EK30U e proposta CPB;
- `dati/2026 CPB/OVERALL GROUP SRL SITUAZIONE CONTABILE PROVVISORIA 31082026.pdf`: senza testo
  estraibile, **letto come immagine** (PyMuPDF, 110 dpi): stato patrimoniale e conto economico;
- `dati/2026 CPB/Dalla Piazza/message.txt`: mail del 14/09 e del 17/09/2026 (socio);
- `dati/2026 CPB/Dalla Piazza/Esito del calcolo dichiarato DALLA PIAZZA FRANCESCO.pdf`: ISA DG15U e
  proposta CPB;
- `dati/2026 CPB/Dalla Piazza/Eps_1756.pdf`: situazione all'11/09/2026 (scansione, letta come immagine);
- `\\server2016\...\fatturalab_backup_20260903.json`, **aperto in sola lettura**: 1.867 fatture
  emesse (6 TD04), 746 fatture passive, 5 mesi di dati di personale;
- `dati/26-08.pdf`: cedolino di agosto 2026 di Pradella;
- `99-verifiche/V02-verifica-diagnosi.md` per i rilievi precedenti e per la verifica normativa
  sul testo multivigente al 9/9/2026.

**Metodo.** Ogni cifra del § 6 è stata ricalcolata dalla fonte. Le fatture FatturaLab sono state
aggregate con il segno: le TD04 hanno l'imponibile negativo nel backup. Proiezioni e pareggi sono
stati rifatti con la stessa formula del documento: IRES 24%, IRAP Veneto 4,08%, VPN ordinario =
reddito + 58.581, cioè lo scarto effettivo 2025 fra 181.521 e 122.940. Le norme sono verificate
sulle fonti indicate in fondo. Dove non ho potuto accedere al testo di legge l'ho scritto.

---

## ESITO COMPLESSIVO

**APPROVATO CON RILIEVI**, a una condizione: **il ROSSO R-1 va risolto prima della consegna.**
Il ROSSO riguarda il § 4.3, che il § 6 richiama. Non riguarda la decisione del § 6.

**La decisione regge.** Ho rifatto i conti dalle fonti:

- per la **società** l'adesione conviene in tutti e tre gli scenari 2026, con un margine sottile in
  quello pessimo;
- per il **socio** la non adesione è coerente con i numeri, ma è un testa o croce da circa 1.000
  euro, non una scelta netta.

Le cifre principali del § 6 sono corrette o differiscono per arrotondamento:

- le due proposte;
- la base 2025;
- il costo del concordato, 38.332 e 38.795;
- i pareggi, 128.000 per il 2026, 129.600 per il 2027 e 143.343 per il socio;
- l'utile di agosto, 169.596,30;
- le fatture del socio, 25.200 nel 2025 e 19.200 nel 2026.

**Le debolezze stanno altrove, e sono quattro.**

1. **Un errore normativo ereditato, e rovesciato.** Il § 4.3 afferma che sotto CPB i contributi del
   socio ingegnere seguono il reddito concordato, e bolla come «falso» il contrario.
   - Per Inarcassa è sbagliato. La Cassa ha dichiarato che l'adesione al CPB «non produce alcun
     effetto» sugli obblighi contributivi: il soggettivo si paga sul reddito effettivo.
   - L'errore nasce da V02 (rilievo R-2), che ha letto l'art. 19, c. 1, senza considerare
     l'autonomia regolamentare delle casse private. **Lo correggo qui.** Vedi R-1.
2. **Il rischio di decadenza è descritto sulla soglia sbagliata.**
   - I dati FatturaLab mostrano che le fatture dei soci alla società valgono **25.200 euro l'anno**.
     Sono il 6% dei ricavi, non «lo stesso ordine di grandezza» della soglia del 30%.
   - La lett. a) dell'art. 22 non è quindi il canale realistico di decadenza.
   - Il canale realistico è quello **senza soglia**: le violazioni di non lieve entità del c. 2,
     compresi i reati del D.Lgs. 74/2000. Il documento non lo nomina. Vedi G-1.
3. **Le fatture del socio sono un canone fisso mensile con descrizione generica.** Lo sono sia
   nel 2025 sia nel 2026: «consulenze eseguite per vs conto nel mese di…». Il canone è salito da
   2.000 a 2.400 euro da ottobre 2025, senza traccia di delibera.
   - Il § 6.4 le dichiara «attività professionale effettiva» come fatto accertato.
   - Un verificatore partirebbe da lì, e sul fronte IVA, che il CPB non copre. Vedi G-2.
4. **In contabilità ci sono ~12.000 euro di compensi di amministratore che nessuna fonte
   attribuisce.** Sono i compensi di otto mesi al netto di quelli di Pradella, e non hanno
   contributo INPS a fronte. Inoltre il § 7 della versione 3 definisce Maggia e Dall'Oca «soci
   di solo capitale», ma la visura li dà come consiglieri. Vedi G-3.

Si aggiungono:

- alcune cifre secondarie errate (Parte I);
- una frase del § 8 che presenta come acquisito un risultato che è solo proiettato (G-4);
- i campi obbligatori del protocollo (semaforo, condizioni di mantenimento, scadenza del vincolo,
  responsabile), che il § 6 non porta (G-6).

---

## Parte I — Cifre verificate

### I-A. Cifre errate, con il valore corretto

| # | Dove | D01 v3 scrive | Valore corretto | Perché |
|---|---|---|---|---|
| E-1 | § 6.2, testo e tabella | ricavi FatturaLab gen-ago 2026 **364.623** («364,6», +44,5%) | **362.219** (+43,6%) | 364.623 è la somma dei valori assoluti: le 6 note di credito TD04 del 2026 (1.202 euro) sono state **sommate** invece che sottratte. Senza le TD04 il totale è 363.421. |
| E-2 | § 6.2 | «quadrano con la contabilità: 364.623 contro 364.670» | 362.219 netto FatturaLab contro **364.288,26** di A1 netto in contabilità (364.669,91 − 745 di resi) | Lo scarto è di **2.069 euro (0,6%)**. La quadratura è buona ma non esatta, e il confronto va fatto fra grandezze nette. |
| E-3 | § 6.2 | costi passivi gen-ago 2026 **108.700** | **106.699** | Stesso errore di segno: 999 euro di TD04 passive sommate. Il 2025 (109.638) è corretto. La conclusione «i costi non crescono» regge, anzi si rafforza. |
| E-4 | § 6.2 | «sette voci … per circa 7.800 euro» con "acconto", "canone", "anticipo" | **Non riproducibile** | Sulle righe 2026 quei tre termini danno **zero** occorrenze. Una ricerca più larga (accont, anticip, canon, abbonam, annual, 2027) dà 6 righe per 6.110 euro, tutte ordinarie: RSPP continuativa, diritti Albo. La conclusione regge, ed è meglio sostenuta dall'andamento mensile (39-58k al mese, nessun picco ad agosto). Va riscritta la frase, non la conclusione. |
| E-5 | § 6.5 | soglia di decadenza sui ricavi 2026 «≈ 160.000-185.000» | **≈ 142.000-183.000** | 30% di (362.219 + 111.173) = 142.018 nello scenario pessimo, 160.215 in quello piatto, 183.066 in quello di tendenza. Il limite inferiore ignora lo scenario pessimo. |
| E-6 | § 3 e § 8 punto 2, non aggiornati nella v3 | beneficio CPB 2025 «17.300-18.900» | **≈ 19.700** | Ora il reddito effettivo 2025 (122.940) e il VPN effettivo (181.521) sono agli atti. Il calcolo è 122.940 × 24% + 181.521 × 4,08% = 36.912, contro 17.190 di imposte correnti: **19.722**. La forchetta della v2 si basava su stime (121.400 e 171.200) superate dai documenti ricevuti. |
| E-7 | § 6.2 | «resta conveniente finché il reddito 2027 non scende più del 30% sotto la proiezione piatta» | Sul **solo 2027** il pareggio è 129.600, cioè −34% rispetto ai 197.400 dello scenario piatto. Sul **biennio**, con i 19.500 risparmiati nel 2026 piatto, il pareggio 2027 scende a **≈ 60.000** di reddito. | Il «30%» non corrisponde a nessuno dei due calcoli e si confonde con la soglia dell'art. 19, c. 2, che è un'altra cosa. |
| E-8 | § 6.1 | «come indicava la circ. 18/E/2024» | citazione da togliere | La circolare 18/E del 17/09/2024 non tratta la base della proposta per chi rinnova, e V02 non aveva trovato prassi sul punto. La prova che la base è il reddito effettivo 2025 è **la proposta stessa**: 132.572 / 122.940 = +7,83%. |

### I-B. Cifre verificate e corrette: non intervenire

| Dato D01 | Fonte | Esito |
|---|---|---|
| Reddito d'impresa 2025 **122.940**, VPN 2025 **181.521** | ISA EK30U, rigo ICI02601; mail del 14/09 | corretto. Il VPN sta solo nella mail, non nell'ISA. |
| Proposta 2026 **132.572 / 192.735**, 2027 **135.234 / 197.553** | ISA EK30U, righi ICP00101-00401 | corretto |
| ISA società **10**, ISA socio **10** | righi IIISAAFF | corretto |
| +7,8% nel 2026 e +10,0% nel 2027, sotto il tetto del 10% per ISA 10 | art. 9, c. 3-*bis*, lett. a) | corretto. Il 2027 è **esattamente al tetto** (135.234 / 122.940 = 1,1000). |
| Costo del CPB **38.300 / 38.800** | ricalcolo | 38.332 / 38.795 |
| Sostitutiva **963 / 1.229** | 10% × 9.632 e 10% × 12.294 | corretto. Il limite di 85.000 del c. 1-*bis* non è in gioco. |
| IRAP sul concordato **7.864 / 8.060** | 4,08% | corretto |
| Scenari 2026: reddito 137k / 198k / 274k, risparmio 2.600 / 19.700 / 41.000 | ricalcolo: 136.769 / 197.428 / 273.596, e 2.462 / 19.495 / 40.883 | corretto entro l'arrotondamento |
| Pareggio **≈ 128.000** (2026) e **≈ 130.000** (2027) | ricalcolo | 128.000 / 129.648 |
| Utile al 31/08/2026 **169.596** su ricavi **364.670** | conto economico, p. 2: utile 169.596,30; conto 901400: 364.669,91 | corretto. Il netto A1 è 364.288,26. |
| Ricavi set-dic **111,2** (2024) e **171,8** (2025); anno 2025 **424,1** | FatturaLab | corretto |
| Socio: reddito 2025 **140.890**, compensi **146.126**, proposta **151.929 / 154.979** | ISA DG15U, righi ICA02601, ICA00301, ICP | corretto. La mail cita 140.936, che è il rigo ICA02401 prima degli «ulteriori elementi contabili» (46 euro): D01 usa il dato giusto. |
| Socio all'11/09: compensi **94.508**, utile **91.885** | Eps_1756 (immagine): 94.508,50 e 91.884,71 | corretto |
| Pareggio del socio **≈ 143.300**; «≈ 1.100 in più» | 140.890 + 1.104 / 0,45 = 143.343 | corretto |
| Fatture del socio alla società **25.200** (2025) e **19.200** (2026) | FatturaLab, fornitore «FRANCESCO DALLA PIAZZA», TD06, per data documento | corretto. 2025: 9 × 2.000 + 3 × 2.400; 2026: 8 × 2.400. |
| Costo per euro netto: dividendo 1,35, fattura 2,21, compenso di amministratore 2,29 | modello V02 | corretto per il socio **sotto** il massimale Inarcassa di 147.300. Sopra, la fattura costa 1,89. Non cambia la classifica. |
| Termine **31/10/2026 → 2/11/2026**, art. 7-*bis* D.L. 38/2026 conv. L. 88/2026 | fonti in fondo; V02 | corretto. Manca la norma sullo slittamento: art. 7, c. 2, lett. l), D.L. 70/2011 (già prescritto da V02). |
| Riserve disponibili **210.113** | SP al 31/08: riserva straordinaria 210.113,68 | corretto, e conferma che il riparto 2025 è stato contabilizzato |

---

## Parte II — Rilievi bloccanti (ROSSO)

### R-1. § 4.3 (richiamato dal § 6.4) — «sotto CPB i contributi seguono il concordato; la versione 1 affermava il contrario. È falso»: per Inarcassa è vero il contrario

**Norma.** L'art. 19, c. 1, D.Lgs. 13/2024 dice che i maggiori redditi effettivi non rilevano
«nonché dei contributi previdenziali obbligatori». Ma le casse private dei professionisti
(D.Lgs. 509/1994) applicano i propri regolamenti.

**Posizione di Inarcassa** (comunicazione del 28/10/2024, che richiama il D.Lgs. 13/2024 come
modificato dal D.Lgs. 108/2024):

> «L'adesione al concordato preventivo biennale … non produce alcun effetto in ordine agli
> obblighi contributivi cui sono assoggettati gli iscritti a Inarcassa» — «La contribuzione
> soggettiva dovuta per gli anni oggetto di concordato dovrà essere calcolata e versata sul
> reddito effettivamente prodotto».

La dichiarazione annuale a Inarcassa chiede il **reddito IRPEF effettivo**.

**Rilievo.**

- La riga «Società e socio entrambi in CPB → fattura **1,04**» del § 4.3 è sbagliata per Dalla
  Piazza, che è ingegnere iscritto a Inarcassa.
- Sono sbagliati anche il punto 2 («il compenso eccedente non sconta né IRPEF né contributi») e il
  punto 5 («i contributi seguono il concordato»).
- Il costo corretto della fattura con entrambi in CPB è **≈ 1,22**: niente IRPEF sull'eccedenza, ma
  il 14,5% di soggettivo, fino al massimale. È il valore che V02 aveva scartato.
- Il vantaggio sul dividendo (1,35) scende quindi dal 30% a circa il 10%.
- L'errore non cambia la decisione 2026-2027, perché il socio non aderisce. Resta però nel
  deliverable come principio falso, marcato **[A]** e con la parola «falso» rivolta alla versione
  che era nel giusto. **Rovescerebbe la decisione del biennio 2028-2029.**
- **Chi ha sbagliato:** il rilievo R-2 di V02, che ha applicato l'art. 19 alla lettera senza
  verificare la posizione della cassa. Il protocollo prevede la controreplica agli atti: questa è.

**Correzione proposta.** Nel § 4.3:

- riga «entrambi in CPB» a **1,22**;
- punto 2 riscritto;
- punto 5 riscritto così: «Per i professionisti iscritti a casse private la regola dell'art. 19,
  c. 1, cede al regolamento della cassa. Inarcassa ha dichiarato che l'adesione non ha effetti
  contributivi e che il soggettivo si calcola sul reddito effettivo».

Va tolta la frase «È falso». Nel § 6.3 va aggiunta una riga: i contributi Inarcassa sono **neutri**
nel confronto CPB/ordinario, perché sono dovuti sull'effettivo in entrambi i casi. Il pareggio di
143.300, calcolato sulla sola IRPEF, è quindi corretto.

---

## Parte III — Rilievi da correggere (GIALLO)

### G-1. § 5.5, § 6.5, § 8 punto 4 — la decadenza è descritta sulla soglia del 30% e il canale realistico non è nominato

**Norma.** Nel testo applicabile al biennio 2026-2027 l'art. 22 fa decadere il concordato in più
casi.

- **c. 1, lett. a).** Accertamento, «nei periodi d'imposta oggetto del concordato **o in quello
  precedente**», di attività non dichiarate o di passività inesistenti o indeducibili oltre il 30%
  dei ricavi dichiarati.
- **c. 1, lett. c) e c. 2.** Violazioni di non lieve entità, **senza soglia**, fra cui:
  - i reati del D.Lgs. 74/2000 nei periodi concordati;
  - la comunicazione inesatta dei dati ISA che riduca il reddito concordato di oltre il 30%.
- **c. 1, lett. e).** Omesso versamento delle somme dovute entro 60 giorni.
- **c. 3-*bis*.** Anche dopo la decadenza restano dovute le imposte sul concordato, se maggiore.

**Rilievo, in due direzioni.**

1. **Sovrastima.** FatturaLab mostra che l'unico socio che fattura è Dalla Piazza: 25.200 euro nel
   2025, cioè il 6% dei ricavi e un quinto della soglia di 126.390. Il § 5.5 («il perimetro delle
   fatture dei soci è dello stesso ordine di grandezza») e il § 8 punto 4 («sopra i 126.390 …»)
   descrivono un rischio che i dati **non sostengono** sul canale della lett. a).
2. **Omissione.** Il verificatore che contesta fatture generiche fra socio-amministratore e società
   non ragiona sull'indeducibilità: ragiona sull'**inesistenza della prestazione**. Questo apre
   l'art. 2 D.Lgs. 74/2000, che non ha soglia di punibilità, e quindi la decadenza per il c. 2
   **a prescindere dal 30%**. È remoto se la prestazione è reale. Ma è l'unico canale per cui 25.000
   euro di fatture possono far cadere un concordato da 38.000 euro l'anno.
3. **Anno precedente.** Il 2025 è «periodo precedente» del biennio 2026-2027 ed è anche periodo
   concordato del 2024-2025 (vedi N-1). Un rilievo sul 2025 colpisce **due** concordati:
   - circa 19.700 euro di beneficio 2025 (E-6);
   - il beneficio 2024;
   - l'intero 2026-2027.

**Correzione proposta.**

- Riscrivere il § 5.5 elencando lett. a), lett. c) con il c. 2, e lett. e).
- Dire con i numeri che la lett. a) è lontana: 25.200 contro 126.390.
- Spostare il presidio sulla **prova dell'effettività delle prestazioni del socio** (G-2).
- Nel § 8 punto 4 sostituire «sopra i 126.390 euro» con «una contestazione di inesistenza delle
  prestazioni fatturate dal socio, a prescindere dall'importo».

**Termine oltre il quale il rischio si estingue [V].**

| Periodo | Termine ordinario (artt. 43 DPR 600 e 57 DPR 633) | Con i benefici premiali, se non si decade |
|---|---|---|
| 2025 | 31/12/2031 | ridotto di un anno |
| 2026 | 31/12/2032 | ridotto di due anni per il rinnovo (art. 14, c. 1-*bis*) |

I termini vanno riletti sul nuovo testo unico dal 2027: vedi G-7.

### G-2. § 6.4, avvertenza 1 — «le fatture del socio remunerano attività professionale effettiva» è marcato come fatto, ma le fatture dicono il contrario

**Fatto [A], da FatturaLab.** Dalla Piazza emette ogni mese una TD06 con un'unica riga:
**«CONSULENZE ESEGUITE PER VS CONTO NEL MESE DI …»**.

| Periodo | Imponibile mensile | Nota |
|---|---:|---|
| gennaio-settembre 2025 | 2.000 | con «+ RIMBORSO SPESE» forfettario nell'importo |
| da ottobre 2025 | 2.400 | +20% |

È un **canone fisso** pagato da una società al proprio vicepresidente e socio al 25%. Non indica
né l'oggetto, né il cliente, né il risultato. Negli atti non c'è traccia di contratto né di
delibera dell'aumento.

**Contestazione concreta.**

1. **Inerenza ed effettività** (art. 109 TUIR; art. 19 DPR 633/1972).
   - Sotto CPB l'indeducibilità IRES del 2026-2027 non costa nulla. Il 2025, invece, è periodo
     concordato del biennio precedente e periodo «precedente» del biennio attuale.
   - Il vero importo in gioco è l'**IVA**, che il CPB non copre (art. 18): 22% di 25.200 = **5.544
     euro nel 2025**, e 4.224 nel 2026 a tutto agosto, di detrazione a rischio. Si aggiunge la
     sanzione per indebita detrazione.
2. **Riqualificazione come compenso di amministratore.** Per la circ. 105/E/2001, già in § 5.1, i
   due compensi hanno la stessa categoria reddituale, quindi la riqualificazione non cambia
   l'IRPEF del socio. Cambia la **deducibilità per cassa** e il presidio documentale: un canone
   fisso senza oggetto «somiglia» a un compenso di carica non deliberato.
3. **Conflitto di interessi** (art. 2475-*ter* c.c.). Il contratto fra la società e un suo
   amministratore, e l'aumento del 20%, vanno deliberati dal CdA con astensione dell'interessato e
   motivazione della convenienza. In mancanza, un verificatore lo userà come indizio di
   antieconomicità: non come motivo autonomo, ma come innesco del controllo.
4. **Il profilo ISA del socio.** L'esito DG15U lo colloca con probabilità 0,999 nel **MoB 3,
   «servizi prevalentemente al committente principale»**. Con 146.126 euro di compensi e 25.200
   fatturati a Overall, il committente principale **non è Overall**.
   - **[V]** Va detto chi è.
   - Se è un cliente di Overall, o un soggetto che opera nello stesso settore, il verificatore
     chiederà perché quella prestazione non passa dalla società. Ci sono anche l'art. 12.1,
     lett. e), dello statuto sull'attività concorrente, e il tema dell'interposizione, anche se
     in senso fiscalmente sfavorevole al socio.

**Correzione proposta.** Nel § 6.4 marcare l'avvertenza come **[V]** e aggiungere il piano
documentale. Va costruito **prima del 2/11/2026**, e in ogni caso prima della prossima fattura:

- contratto scritto con data certa (PEC), con oggetto tecnico determinato;
- delibera del CdA di approvazione e dell'aumento da ottobre 2025, con astensione di Dalla Piazza;
- descrizione in fattura delle attività e delle commesse servite;
- report mensile delle attività, con i riferimenti alle commesse FatturaLab;
- separazione dell'eventuale rimborso spese a piè di lista dal forfait.

**Rischio fino al:** 31/12/2031 per il 2025 **[V]**, con la riduzione premiale se non si decade.

### G-3. § 1, § 7 v3 e § 6.4 — circa 12.000 euro di compensi di amministratore nel 2026 senza beneficiario e senza contributi; e i «soci di solo capitale» sono consiglieri

**Fatto [A].**

- Il conto 804301 «Compensi agli amministratori» vale **33.686,80** al 31/08/2026.
- Il cedolino di agosto dà a Pradella compensi progressivi per **21.695**.
- Il conto 804306 «Contributo INPS L. 335/95» vale **3.471,20**, cioè esattamente il 16% di 21.695:
  è la quota a carico del committente sull'aliquota del 24% di Pradella.
- Restano **11.992 euro** di compensi di amministratore **senza contributo di gestione separata**
  e senza fattura riconducibile in FatturaLab. Le fatture di Dalla Piazza sono solo le
  «consulenze» da 2.400 euro, registrate in altri conti.
- Nel 2025 lo scarto è analogo: 47.893 euro di compensi contro circa 32.500 di Pradella.

**Rilievo.**

- Se sono compensi a Maggia o a Dall'Oca, il § 7 della v3 («soci di solo capitale») è in
  contraddizione con la visura (§ 1: consiglieri). Inoltre manca la gestione separata: al 24% o al
  35,03% sono **circa 2.900-4.200 euro** in otto mesi, più sanzioni civili. Mancano anche ritenute
  e CU.
- Se sono un rateo o un accantonamento, va detto, perché i compensi di amministratore sono
  deducibili **per cassa** (art. 95, c. 5, TUIR).
- Se sono di Dalla Piazza, devono stare in una sua fattura, e allora le fatture del socio non sono
  25.200 euro.
- In nessuno dei tre casi il dato è neutro per il § 6.4, che conta i soci che «non fatturano» e
  ripartisce il dividendo al 25%.
- Aggrava il rilievo V02 G-14/1: non c'è delibera dei soci sui compensi.

**Correzione proposta.**

- Voce nuova nel § 7: «mastrino 804301 del 2025 e del 2026 con il dettaglio per beneficiario;
  delibera dei compensi».
- Nel § 7 v3 sostituire «soci di solo capitale» con «soci che non prestano attività professionale
  per la società (restano consiglieri)».

**Rischio fino al** termine di prescrizione contributiva quinquennale. Per il 2026: 2031.

### G-4. § 8 punto 3 e § 6.2 — «pareggio superato già ad agosto con 169.596 di utile»

**Rilievo.**

- L'utile di agosto non è un minimo garantito. Nello scenario pessimo del documento, i ricavi di
  settembre-dicembre (111k) sono inferiori ai costi stimati (139k + 5k): il quadrimestre è in
  **perdita di 33k**, e il reddito scende a 137k.
- Le rettifiche di fine anno sono sottostimate. Il conto 804304 «tenuta contabilità» è
  **negativo (−2.392)**: uno storno senza la fattura dell'anno. Nel 2025 la commercialista è
  costata 4.600. Il TFR è a 254 contro circa 2.500 maturati. Mancano i ratei di ferie e
  mensilità aggiuntive.
- Con rettifiche realistiche di 9-10k invece di 5k, lo scenario pessimo dà **≈ 132.000**: il
  risparmio scende a **≈ 1.200**, a 4.000 euro dal pareggio.
- Manca del tutto una sensibilità sui **costi**. Con costi di settembre-dicembre +10% (+14k),
  lo scenario pessimo va **sotto** il pareggio.

**Non cambia la decisione.** Lo scenario pessimo presuppone che il quadrimestre torni ai livelli
2024 (−35% sul 2025), mentre gennaio-agosto corre al +43,6%. Ma il testo deve dirlo così.

**Correzione proposta.**

- § 8 punto 3: «Il reddito 2026 proiettato è fra ~132.000 e ~274.000, contro un pareggio di
  ~128.000».
- § 6.2: aggiungere la riga di sensibilità sui costi e le rettifiche di fine anno elencate sopra.

### G-5. § 6.3 — la non adesione del socio è presentata come scelta netta: è un testa o croce, e il documento non mette a bilancio ciò che il socio rinuncia

**Rilievo.**

1. **Margine.** Il margine è di 2.400 euro di reddito: 143.343 di pareggio contro 140.900
   proiettati. Poggia interamente su un'ipotesi del socio: 50.000 euro di ulteriori incassi
   **tutti** entro il 31/12.
   - Basta un incasso in più di quanto previsto perché l'adesione diventi conveniente, e la scelta
     è irrevocabile dal 2/11.
   - Il 2027 non è analizzato. Il pareggio 2027 è **144.021** e i compensi 2025 erano 146.126: con
     un 2027 uguale al 2025 l'adesione avrebbe fatto risparmiare circa 900 euro.
2. **Benefici persi.** Il socio era in CPB 2024-2025 (quadro CP agli atti), quindi il 2026-2027
   sarebbe stato un **rinnovo**. Rinuncia a quattro cose:
   - la preclusione degli accertamenti ex art. 39 DPR 600/1973 (art. 34, c. 1);
   - l'anticipazione di **due** anni dei termini di accertamento;
   - l'esonero dal visto fino a 70.000 euro (art. 14, c. 1-*bis*);
   - l'assenza di interessi sulle rate (c. 1-*ter*).

   E si colloca nella platea dell'art. 34, c. 2, cioè quella dei controlli intensificati.
3. **Contrasto con il profilo di rischio.** L'unico rischio documentale concreto di tutto il
   fascicolo, G-2, riguarda proprio le fatture del socio. Il § 6.4 punto 2 lo chiama «rischio
   concreto modesto» perché l'ISA è 10. L'ISA 10 non protegge dal controllo documentale: protegge
   dagli accertamenti presuntivi.

**Correzione proposta.**

- Riscrivere la conclusione così: «Sui numeri la scelta è indifferente, ±1.000-1.500 euro l'anno.
  La proprietà ha scelto di non aderire rinunciando alla preclusione dell'art. 34, c. 1, e alla
  riduzione di due anni dei termini. Il presidio sostitutivo è il dossier G-2».
- Aggiungere la verifica degli incassi effettivi al 31/10, prima della scadenza.

### G-6. § 6 — mancano i campi obbligatori del protocollo su una raccomandazione VERDE

L'adesione della società è un **regime opzionale usato per lo scopo per cui esiste**, quindi
**VERDE**. Il protocollo impone però su ogni VERDE tre campi: condizioni di mantenimento, data di
scadenza del vincolo e responsabile del monitoraggio. Il § 6.5 li sfiora senza intestarli.

**Correzione proposta.** Aggiungere al § 6 un riquadro.

- **Semaforo:** VERDE.
- **Vincolo:** dal 1/1/2026 al 31/12/2027. Gli effetti premiali valgono fino alla scadenza dei
  termini di accertamento ridotti.
- **Condizioni di mantenimento:**
  - nessuna operazione straordinaria (fusione, scissione, conferimento) e nessun aumento del numero
    dei soci nel biennio (art. 21, lett. b-*ter*). **Lega la roadmap:** qualsiasi leva di
    «catena partecipativa» dei parametri d'incarico che coinvolga la società va rinviata al 2028;
  - nessuna modifica dell'attività verso un ISA diverso (art. 21, lett. a);
  - versamento delle somme dovute entro 60 giorni dagli avvisi (art. 22, lett. e);
  - assenza delle violazioni dell'art. 22, c. 2 (G-1);
  - ricavi sotto 7.746.853,50 euro;
  - requisiti dell'art. 10 permanenti: debiti tributari o contributivi definitivi sotto 5.000 euro,
    rilevante per G-3.
- **Responsabile:** da nominare. Suggerisco la commercialista per gli adempimenti e il Presidente
  per le operazioni societarie.

### G-7. Header e § 6 — manca ancora il campo sulla successione normativa dal 2027 (già prescritto da V02)

V02 ha segnalato che dal 1/1/2027 il T.U. imposte sui redditi (D.Lgs. 117/2026) e il T.U.
adempimenti e accertamento (D.Lgs. 141/2026) sostituiscono gli articoli citati. **Non l'ho
riverificato sul testo**: la fonte è V02. Il 2027 del biennio vivrà sotto una numerazione
diversa per cessazione, decadenza e accertamento.

**Correzione proposta.** Una nota nel § 6: «Gli articoli citati sono quelli vigenti all'adesione;
per il 2027 vanno riletti nei testi unici».

### G-8. § 6.5 — benefici e acconti citati in modo impreciso

- **Benefici.** «Riduzione di un anno dei termini di accertamento» e «rimborsi IVA prioritari»
  (art. 19, c. 3) sono i benefici del primo accesso. Per chi **rinnova**, come la società, valgono
  quelli dell'art. 14, c. 1-*bis*: **due anni**, visto fino a 100.000 euro (IVA) e 70.000
  (dirette), rimborsi IVA senza visto né garanzia fino a 100.000. Già detto da V02 (N-3) e non
  recepito.
- **Preclusione.** «Preclusione degli accertamenti dell'art. 34» è una citazione sbagliata. È
  l'art. 34, c. 1, che preclude gli accertamenti **dell'art. 39 DPR 600/1973**. Non copre IVA,
  accessi, ispezioni e controlli 36-*bis*/36-*ter*: va scritto.
- **Acconti.** «Chi aderisce ricalcola gli acconti sul reddito concordato» è impreciso.
  - Il metodo storico resta disponibile. Esclude la quota a sostitutiva.
  - Per il **rinnovo senza interruzione** non si applica la maggiorazione del primo anno (art. 20,
    c. 3-*bis*; FAQ AdE del 3/6/2026 come riportate da Fiscal Focus).
  - **[V]:** la stessa fonte segnala che la maggiorazione torna dovuta in caso di rientro «dopo una
    pausa». Va confermato con la commercialista che la continuità 2024-2025 → 2026-2027 conta come
    rinnovo. Nel caso peggiore la maggiorazione vale 10% × 9.632 + 3% × 11.214 = **≈ 1.300
    euro**, ed è solo di cassa.
  - Dall'SP al 31/08: primo acconto IRES **6.090**, primo acconto IRAP **2.206,50**. Col metodo
    storico il secondo acconto di novembre è dello stesso ordine. Il saldo 2026, ≈ 23.000 di IRES
    più la sostitutiva, cade a giugno 2027 **[I]**.

---

## Parte IV — Rilievi che il documento non ha visto

### N-1. La conferma documentale del CPB 2024-2025 è già nel fascicolo, e il documento non la usa

Lo SP al 31/08/2026 porta «Erario c/acconti IRES» **6.090** ed «Erario c/acconti IRAP**
**2.206,50**. Per un soggetto ISA sono due acconti del 50% sull'imposta 2025.

| Imposta 2025 ricostruita | Importo | Base implicita |
|---|---:|---|
| IRES | ≈ 12.180 | ≈ 50.750 di reddito al 24% |
| IRAP | ≈ 4.413 | ≈ 108.000 di VPN |

La differenza fino alle imposte correnti 2025 di 17.190 (≈ 600) è compatibile con una sostitutiva
10% su circa 6.000 di incremento.

È il profilo di un concordato 2024-2025 con sostitutiva, **non** di un reddito effettivo di
122.940. Il § 6.1 può passare da **[I]** ad **[A] indiziario forte**, fermo restando che la
conferma formale resta la dichiarazione. Ne discendono tre cose:

- è un **rinnovo**, con i benefici di G-8;
- per l'acconto vale G-8;
- il 2025 è esposto a decadenza su due concordati (G-1).

### N-2. Il reddito effettivo 2026 fissa la proposta 2028-2029, e il dividendo non la cambia

Il § 6.5 lo accenna. Va aggiunto che l'unica leva che abbassa legittimamente il concordato in
corso è l'**iperammortamento** (art. 16, lett. b-*ter*, inserita dall'art. 7, c. 3-*bis*, D.L.
38/2026, secondo V02). Per una società con circa 225.000 euro di liquidità al 31/08/2026 è una
leva concreta, e il § 6 non la richiama.

### N-3. La cassa per il dividendo del § 6.4 c'è, ma i tempi no

- Liquidità al 31/08/2026: **≈ 225.600** (227.797 − 2.223 di carta di credito), con 21.964 di IVA
  a debito.
- L'eccedenza 2026 si distribuisce solo **dopo l'approvazione del bilancio 2026**, cioè nel 2027:
  gli acconti sui dividendi (art. 2433-*bis* c.c.) non sono praticabili in una S.r.l. senza
  revisione.
- Nell'immediato distribuibili sono i **210.113 euro di riserve**, e non «l'eccedenza del 2026».

Il § 6.4 va letto così, altrimenti il cliente si aspetta cassa nel 2026.

### N-4. Concentrazione della crescita 2026

Tre clienti assenti in gennaio-agosto 2025 valgono **≈ 49.400 euro** in gennaio-agosto 2026:
Velox Servizi 24.213, Velox Hotellerie 17.062, Seasonal Services 8.136. È il 45% dell'incremento.

Non è un rischio fiscale. È però il parametro che decide il 2027, cioè l'anno che il § 6.2 chiama
«rischio vero». **[V]** Va chiesta la natura dei contratti, pluriennali o una tantum, e il § 7
voce 3 va integrato di conseguenza.

---

## Verifica normativa (sintesi)

| Affermazione di D01 v3 | Esito | Fonte |
|---|---|---|
| Termine 31/10/2026, art. 7-*bis* D.L. 38/2026 conv. L. 88/2026; slittamento al 2/11 | **Confermato** | TeamSystem, Lamiafinanza, Agenda Fiscale; V02 sul testo in G.U. Da aggiungere l'art. 7, c. 2, lett. l), D.L. 70/2011. |
| Tetto art. 9, c. 3-*bis*: 10% con ISA 10 | **Confermato** (10% / 15% / 25% / 30% / 35% per fascia) | TeamSystem; V02 |
| Sostitutiva art. 20-*bis* al 10% con ISA ≥ 8 sull'eccedenza rispetto al **reddito effettivo** 2025 (rinnovo, c. 2) | **Confermato**; limite di 85.000 non in gioco | EC News, Edupass; V02 |
| IRAP sul VPN concordato, senza sostitutiva | **Confermato** | art. 20-*bis* riferito a IRPEF e IRES |
| Acconti: «si ricalcolano sul concordato» | **Impreciso** (G-8) | FAQ AdE 3/6/2026 via Fiscal Focus |
| Art. 22: decadenza oltre il 30% dei ricavi | **Incompleto** (G-1): omessi c. 2, lett. e), «periodo precedente» | EC News; V02 |
| Art. 21: cessazione | **Non trattato** nel § 6 (G-6) | V02 |
| Art. 34, c. 2: controlli intensificati sui non aderenti | **Confermato**; la preclusione è citata male (G-8) | V02 |
| Benefici art. 19, c. 3, «un anno» | **Superato per il rinnovo**: art. 14, c. 1-*bis* (G-8) | V02 |
| Contributi sotto CPB seguono il concordato (§ 4.3) | **Errato per Inarcassa** (R-1) | Inarcassa, 28/10/2024 |
| Marginale del socio ≈ 45% | **Plausibile**: 43% + addizionale regionale Veneto + comunale | non riverificate le aliquote locali 2026 |

**Limite della verifica.** Non ho avuto accesso diretto al testo multivigente del D.Lgs. 13/2024
né ai D.Lgs. 81/2025, 148/2026, 117/2026 e 141/2026. Per l'art. 14, c. 1-*bis*/1-*ter*, l'art. 20,
c. 3-*bis*, l'art. 21 e il testo 2026-2027 dell'art. 22 mi appoggio alla verifica testuale di
V02 e alle fonti secondarie indicate. Il protocollo richiede che le GIALLE siano validate dalla
commercialista prima dell'esecuzione, e questo vale in particolare per G-8 (acconti).

**Fonti consultate:**

- [Inarcassa — CPB, effetti previdenziali (28/10/2024)](https://www.inarcassa.it/notizie/concordato-preventivo-biennale-effetti-previdenziali)
- [Inarcassa — CPB, reddito IRPEF di riferimento per la dichiarazione](https://www.inarcassa.it/notizie/concordato-preventivo-biennale-reddito-irpef-di-riferimento-la-dichiarazione-inarcassa)
- [TeamSystem — CPB 2026-2027, calcolo con voto ISA](https://www.teamsystem.com/magazine/gestione-dello-studio/concordato-preventivo-biennale-2026-2027-calcolo-voto-isa/)
- [Lamiafinanza — CPB 2026-2027, nuova scadenza](https://www.lamiafinanza.it/2026/09/concordato-preventivo-biennale-2026-2027-nuova-scadenza-e-come-aderire/)
- [Fiscal Focus — CPB, acconti 2026: maggiorazione solo per il primo accesso](https://www.fiscal-focus.it/news-24/ore-09-04-cpb-acconti-2026-maggiorazione-solo-per-il-primo-accesso,3,185331)
- [EC News — tassazione del reddito proposto dopo il correttivo](https://www.ecnews.it/fiscale/fisco-e-patrimonio/imposte-sul-reddito/concordato-preventivo-biennale-post-decreto-correttivo-la-tassazione-del-reddito-proposto/)
- [EC News — cause di decadenza del CPB](https://www.ecnews.it/fiscale/accertamento-e-contenzioso/riscossione/le-cause-di-decadenza-del-concordato-preventivo-biennale/)
- [Edupass — Quadro CP, sezione I, sostitutiva art. 20-bis](https://www.edupass.it/manuali/manualistica-mexal/manuale-redditi?a=manuale-redditi%2Fredditi%2Fredditi-persone-fisiche---quadri-dimpresa%2Fquadro-cp--concordato-preventivo-biennale%2Fsezione-i--imposta-sostitutiva-art-20-bis-del-decreto-cpb)

---

## Riepilogo dei rilievi

| # | Semaforo | Dove | In una riga |
|---|---|---|---|
| R-1 | **ROSSO** | § 4.3 (richiamato dal § 6.4) | Inarcassa: contributi sull'effettivo anche in CPB; la fattura «entrambi in CPB» costa 1,22, non 1,04. Errore nato in V02, R-2. |
| G-1 | GIALLO | §§ 5.5, 6.5, 8.4 | La decadenza è descritta sul 30%, che i dati rendono lontano; manca il canale senza soglia (art. 22, c. 2). |
| G-2 | GIALLO | § 6.4 | Fatture del socio: canone fisso con descrizione generica, +20% senza delibera, MoB 3; IVA a rischio 5.544 euro l'anno. |
| G-3 | GIALLO | §§ 1, 7, 6.4 | 11.992 euro di compensi di amministratore senza beneficiario né INPS; i «soci di solo capitale» sono consiglieri. |
| G-4 | GIALLO | §§ 8.3, 6.2 | «Pareggio superato ad agosto» è falso come formulato; mancano le rettifiche di fine anno e la sensibilità sui costi. |
| G-5 | GIALLO | § 6.3 | La non adesione del socio è indifferente sui numeri; vanno scritti i benefici a cui rinuncia. |
| G-6 | GIALLO | § 6 | Mancano semaforo, condizioni di mantenimento, scadenza del vincolo e responsabile. |
| G-7 | GIALLO | header, § 6 | Manca la nota sui testi unici dal 2027 (già prescritta da V02). |
| G-8 | GIALLO | § 6.5 | Benefici del rinnovo (art. 14, c. 1-*bis*), preclusione dell'art. 34, c. 1, acconti. |
| E-1…E-8 | correzioni numeriche | §§ 3, 6, 8 | Vedi Parte I-A. |
| N-1…N-4 | integrazioni | §§ 6.1, 6.4, 6.5, 7 | Prova del CPB 2024-2025 dagli acconti; iperammortamento; tempi del dividendo; concentrazione clienti. |

---

## Recepimento (consulente, 25/09/2026)

Tutti i rilievi sono stati recepiti in D01 versione 3; nessuna controreplica.

- **R-1 (ROSSO) chiuso.** Nel § 4.3 la riga «entrambi in CPB» è portata a ≈ 1,22, con il margine
  al 10% circa. I punti 2 e 5 sono riscritti con la posizione Inarcassa del 28/10/2024 ed è tolto
  «È falso». Nel § 6.3 è scritto che i contributi sono neutri nel confronto.
- **G-1:** § 5.5 riscritto (lett. a, c con c. 2, e; il 2025 esposto due volte); § 8 punto 4 corretto.
- **G-2 e G-3:** § 6.4, punti 2 e 3, marcati [V], con il dossier da costruire prima del 2/11; voci
  14-16 aggiunte al § 7; «soci di solo capitale» sostituito.
- **G-4:** rettifiche portate a 9-10k; scenari 132 / 193 / 269k; aggiunta la sensibilità sui
  costi; § 8 punto 3 riscritto.
- **G-5:** § 6.3 riscritto come scelta indifferente sui numeri, con i benefici persi e la verifica
  degli incassi al 31/10 (voce 18 del § 7).
- **G-6 e G-7:** riquadro di protocollo in testa al § 6, con la nota sui testi unici dal 2027.
- **G-8:** acconti, benefici del rinnovo (art. 14, c. 1-*bis*) e art. 34, c. 1, corretti nel § 6.5.
- **Cifre della Parte I-A:** tutte corrette. È stata tolta anche la citazione della circ. 18/E.
- **N-1 … N-4:** recepiti nei §§ 6.1, 6.5, 6.4 e 6.2; voce 17 aggiunta al § 7.
