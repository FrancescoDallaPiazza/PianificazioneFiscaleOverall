# V04 — Verifica indipendente di L01 (leve per i soci Dalla Piazza e Pradella)

**Revisori:** R1 (verificatore: ufficiale GdF, funzionario AdE, ispettore INPS) e R2 (tributarista e
consulente del lavoro, per calcoli e norme). La domanda è la stessa di V03: *quale numero è
sbagliato, quale norma è letta male, dove si rompe il fascicolo quando arriva un accesso?*

**Data della verifica:** 25 settembre 2026
**Documento verificato:** `02-leve/L01-leve-soci.md`, **versione 1** del 25/09/2026. Il file non è
ancora versionato.

**Dati nuovi, comunicati dalla proprietà durante la verifica:**

- **Pradella è iscritto alla gestione IVS commercianti INPS** come socio che lavora in Overall.
  L'alternativa 2 del § 1 (aliquota 35,03%, circa 3.600 euro l'anno mancanti) quindi decade.
- **Nota di lavoro dell'utente del 31/08 e dell'01/09/2026** (`handoff_pensione_inarcassa.md`):
  - pensionamento di Dalla Piazza previsto il **04/04/2039**, a 67 anni e 6 mesi;
  - tetto del fondo pensione **5.300 euro**;
  - contributo modulare Inarcassa **dall'1% all'8,5%**;
  - ricongiunzione gestione separata → Inarcassa già decisa sull'**Allegato B**, gratuito.

**Fonti primarie riscontrate:**

- `dati/26-06.pdf`, `26-07.pdf`, `26-08.pdf`, pagina di Pradella:
  - compensi di 2.719, 2.709 e 2.710 euro al mese, progressivo di agosto **21.695**;
  - trattenuta F.A.P. esattamente all'8,00%, cioè un terzo del 24%;
  - voce 0545 «rimborso a piè di lista» **1.439 + 1.623,80** a giugno e **1.382** ad agosto;
  - nessuna detrazione per familiari;
- `dati/PRADELLA TAZIO.pdf`: scansione della **CU 2026 sui redditi 2025**, letta come immagine con
  PyMuPDF a 110 dpi:
  - reddito assimilato **27.101,36**, IRPEF netta 4.176,08;
  - gestione separata: compensi **29.458**, contributi **7.069,92 (24,0%)**, a carico del
    percipiente 2.356,64, tipo rapporto «1E»;
  - **due figli a carico al 50%**, nati nel 2014 e nel 2019; coniuge non a carico;
  - somma e trattamento integrativo del cuneo con codice 2, cioè non spettanti. È corretto per un
    assimilato;
- `C:\Users\Francesco\Downloads\handoff_pensione_inarcassa.md`;
- modello `calc.py` dello scratchpad, rieseguito e integrato. I due script di controllo, `v04.py`
  e `v04b.py`, sono nello scratchpad della sessione.

**Metodo.** Uso lo stesso modello semplificato di L01: IRPEF 2026 al 23/33/43%, addizionali
forfettarie al 2,03%, detrazione per redditi assimilati dell'art. 13. Vi aggiungo ciò che L01
omette:

- i **contributi commercianti** di Pradella, cioè il minimale 2026 di 18.808 euro con 4.611,64 euro
  fissi e il 24,48% sull'eccedenza, deducibili ai sensi dell'art. 10 TUIR;
- l'**incapienza** delle deduzioni quando il compenso scende.

Le norme sono verificate sulle fonti in fondo. Dove non ho potuto leggere il testo di legge l'ho
scritto.

---

## ESITO COMPLESSIVO

**DA RIVEDERE.** Ci sono due ROSSI, e riguardano il cuore della parte su Pradella.

1. **§ 3.4, il dividendo privilegiato.** Il 16 e il 17 settembre 2026 la Cassazione, sezione
   lavoro, con dieci sentenze gemelle (nn. 25377-25383 e 25465-25467), ha stabilito che il socio
   lavoratore di S.r.l. iscritto ai commercianti paga i contributi sugli utili **fiscalmente
   imputati**, cioè distribuiti, e non su quelli accantonati.
   - Il dividendo che sostituisce il compenso è quindi soggetto al **24,48%** di contributi
     commercianti, appena i dividendi di Pradella superano il minimale di 18.808 euro. Li
     supereranno: servono a coprire il suo fabbisogno.
   - Il «risparmio di 5.100 euro ogni 20.000 convertiti» diventa **una perdita di circa 3.650
     euro**.
   - Anche con la vecchia linea INPS il risparmio sarebbe di 2.300-2.500 euro, non 5.100.
2. **§ 0 e § 4: i numeri di partenza di Pradella non contano i contributi commercianti.**
   - Il netto di 24.000 euro è in realtà **≈ 21.100**, e scende a ≈ 18.800 se l'INPS applica la
     sua linea.
   - Il fabbisogno scoperto è di **≈ 13.900 euro** l'anno, non 11.000.
   - Il dividendo lordo necessario è **≈ 18.800**, non 14.900.
   - Il «26% secco» della distribuzione delle riserve è falso per Pradella. Sui suoi 52.500 euro
     di riserve il prelievo è di **circa il 42%**, a meno di distribuire in tranche annuali entro
     il minimale.

**Il resto regge nell'impianto, ma quasi ogni sezione ha una cifra o una norma da correggere:**

| Sezione | Che cosa va corretto |
|---|---|
| § 2.1 | Il modulare arriva all'**8,5%**, non al 10%. Il fondo pensione ha il tetto di **5.300 euro**. Il risparmio è **≈ 7.800 euro**, non 8.700. L'aliquota del fondo pensione non scende sotto il 15% in 13 anni. |
| § 2.2 | La conclusione regge e anzi si rafforza, ma per ragioni diverse da quelle scritte. |
| § 2.3 | Il rinvio al 2028 poggia su una premessa sbagliata: il conferimento delle quote di una S.r.l. non fa cessare il CPB. La PEX richiede **60 mesi** di possesso, non 12. |
| § 3.1 | Il 70% dal 2028 non vale per gli amministratori. Il fringe dell'auto consuma la soglia dei 2.000 euro del § 3.2. |
| § 3.3 | Ai rimborsi pari al 55% del compenso va dato GIALLO, non VERDE. |
| § 3.5 | Il CdA è **a tempo indeterminato**: il «prossimo rinnovo» non esiste. |

**Mancano leve concrete per Pradella**, soprattutto:

- i **buoni pasto elettronici**;
- la verifica di un possibile **rimborso dei contributi commercianti** pagati su utili non
  distribuiti;
- la **distribuzione a tranche entro il minimale**.

---

## Parte I — Cifre verificate

### I-A. Cifre errate, con il valore corretto

| # | Dove | L01 scrive | Valore corretto | Perché |
|---|---|---|---|---|
| E-1 | § 0, § 6 | FDP: «10 anni di attività» | **13 anni**: pensione il 04/04/2039, a 67 anni e 6 mesi | Nota dell'utente. Cambia l'orizzonte del § 2.1 (aliquota del fondo pensione), del § 2.2 (uscita) e del § 2.3 (PEX a 60 mesi). |
| E-2 | § 0 | TP netto disponibile **≈ 24.000** | **≈ 21.100** con il solo minimale commercianti; **≈ 18.800-19.200** se l'INPS applica la sua linea (25% del reddito IRES di Overall, 30.735-33.143 di base) | L01 omette i contributi commercianti: 4.611,64 euro fissi, deducibili. Il 24.000 è riproducibile (23.971) solo senza di essi. |
| E-3 | § 0 | TP differenza **−11.000**, dividendo lordo **≈ 14.900** | **−13.900**, dividendo lordo **≈ 18.800**; linea INPS: −16.200 e ≈ 21.900 | Conseguenza di E-2. Entro 18.808 euro di dividendi non ci sono contributi aggiuntivi: vedi R-2. |
| E-4 | § 2.1 | modulare «fino al 10%», versato ≈ 19.300 | modulare **8,5% × 140.890 = 11.976**; fondo pensione **5.300**; versato **≈ 17.276** | Art. 4.2 del Regolamento generale di previdenza Inarcassa: aliquota dall'1% all'8,5%, massimo 2026 12.520 euro, che è l'8,5% del massimale. L. 199/2025, art. 1, c. 201. Il 12.520 è il tetto assoluto: FDP, sotto il massimale, arriva a 11.976. |
| E-5 | § 2.1, § 6 | risparmio **≈ 8.700** | **≈ 7.780**. Con 12.520 + 5.300 sarebbe 8.024, ma 12.520 non è raggiungibile col reddito 2025 | Ricalcolo con aliquota marginale del 45,03% (43% + Veneto 1,23% + Padova 0,80%). Il calcolo dell'utente «≈ 8.000» usa il massimo assoluto. |
| E-6 | § 2.1 | netto spendibile ≈ 63.500 | **≈ 64.600** | Conseguenza di E-4. |
| E-7 | § 2.1 | fondo pensione «in uscita 15%, che scende fino al 9%» | **15%** per FDP | La riduzione di 0,30 punti l'anno scatta solo **oltre il 15° anno** di partecipazione (art. 11, c. 6, D.Lgs. 252/2005). FDP non ha un fondo (nota dell'utente) e ha 13 anni di orizzonte. |
| E-8 | § 2.2 | STP: 73.600 contro 74.100 | Società di ingegneria con compenso di amministratore: **≈ 70.100** contro 74.100, più **20.445** di soggettivo Inarcassa che nella P.IVA va a montante | Il modello applica Inarcassa al compenso dell'amministratore. Il compenso è però reddito **assimilato** (art. 50, c. 1, lett. c-*bis*) e sconta la gestione separata al 24%, di cui 16% a carico della società. Vedi G-2. |
| E-9 | § 2.2 | IRAP al 3,9% | Da allineare a D01 e V03, che per Overall usano il **4,08%** | Incoerenza interna. Non cambia la conclusione: 70.080 al 3,9% e 69.897 al 4,08%. |
| E-10 | § 3.4, § 6 | «Overall risparmia ≈ 5.100 ogni 20.000» | **−3.650** (linea Cassazione, TP già sopra il minimale); **+2.300 / +2.500** (linea INPS); **+3.780** solo se sui dividendi non si pagano contributi | Vedi R-1. Il 5.099 di L01 è riproducibile, ma senza contributi commercianti e senza incapienza. |
| E-11 | § 3.1 | «servirebbero circa 9.500 euro» di costo, risparmio ≈ 3.000 | Sulle premesse di L01: **≈ 12.050** di compenso lordo, **≈ 14.000** di costo | Il 9.500 non è riproducibile. Il risparmio reale però dipende da variabili che L01 non considera: vedi G-4. |
| E-12 | § 3.2 | valore «1.000-1.300» | **≈ 1.900** di minor costo ogni 2.000 erogati, se la soglia è libera. Con l'auto del § 3.1 lo spazio si riduce a **≈ 1.300** | Il compenso equivalente a 2.000 euro netti costa 3.900 euro (modello con commercianti). |
| E-13 | § 3.3 | indennità forfettaria: «le regole sul cumulo riducono la soglia [V]» | **46,48 euro** al giorno; **30,99** se è rimborsato a piè di lista il vitto o l'alloggio; **15,49** se sono rimborsati entrambi | Art. 51, c. 5, TUIR. Il [V] si chiude. |

### I-B. Cifre verificate e corrette: non intervenire

| Dato L01 | Fonte | Esito |
|---|---|---|
| Compenso TP ≈ 32.500 | cedolini: 21.695 progressivi in 8 mesi, 2.710 al mese | corretto per il 2026. Il 2025 era **29.458** (CU). |
| Gestione separata al 24%, 8% a carico di TP | cedolini; CU sez. 3: 7.069,92 / 29.458 = 24,00% | corretto, e coerente con l'iscrizione ai commercianti |
| FDP netto status quo ≈ 74.000 | modello: 74.069 | corretto nel modello |
| Dividendo FDP 52.500 lordi, 38.900 netti | 210.113 × 25% × 0,74 | corretto (52.528 e 38.871) |
| TP con due figli a carico | CU, righi F1/F: 12 mesi, 50% | corretto: è la condizione della soglia dei 2.000 euro |
| Rimborsi 15.000-18.000 l'anno | cedolini giugno-agosto: 4.444,80 in tre mesi | plausibile: ≈ 17.800 annualizzati |

---

## Parte II — Rilievi bloccanti (ROSSO)

### R-1. § 3.4 — «parte del compenso trasformata in dividendo privilegiato: risparmio 5.100 su 20.000». Con la giurisprudenza di settembre 2026 il vantaggio è negativo

**Norma.**

- **Base dei contributi commercianti.** L'art. 3-*bis* D.L. 384/1992 la fissa sulla «totalità dei
  redditi d'impresa denunciati ai fini IRPEF».
- **Doppia iscrizione.** L'art. 12, c. 11, D.L. 78/2010, di interpretazione autentica, impone al
  socio-amministratore che lavora in S.r.l. sia la gestione separata sul compenso sia i
  commercianti sull'attività.
- **Linea INPS.** Con le circolari 102/2003 e 84/2021, citate dalle fonti, l'INPS ha preteso i
  contributi sulla quota di reddito IRES della società **anche se non distribuita**.
- **Cassazione, sezione lavoro, 16 e 17 settembre 2026** (nn. 25377-25383 e 25465-25467):
  - la base è il reddito **fiscalmente imputato** al socio, cioè gli utili distribuiti o il reddito
    in trasparenza (artt. 115-116 TUIR);
  - gli utili accantonati a riserva ne sono esclusi;
  - l'onere della prova è dell'INPS.

**Rilievo.** TP è iscritto ai commercianti (dato della proprietà). Paga quindi il minimale, che
copre i primi 18.808 euro di «reddito», e il **24,48%** sulla parte che eccede.

| Scenario per 20.000 euro di compenso convertiti | Dividendo lordo che rende TP indifferente | Costo del compenso (× 1,16) | Effetto per Overall |
|---|---:|---:|---:|
| L01: nessun contributo sui dividendi, niente commercianti | 18.101 | 23.200 | **+5.099** |
| Nessun contributo sui dividendi, minimale commercianti e incapienza considerati | 19.417 | 23.200 | +3.783 |
| **Linea Cassazione 2026**, TP con ≈ 14.900-18.800 di dividendi ordinari già in pagamento | 26.853 | 23.200 | **−3.653** |
| Linea INPS: base = 25% del reddito IRES di Overall, indipendente dai dividendi | 20.682-20.938 | 23.200 | +2.262 / +2.518 |

Perché il vantaggio sparisce:

- **Il costo contributivo non cambia.** Il compenso sconta il 24% di gestione separata. Il dividendo
  sopra il minimale sconta il 24,48% di commercianti, tutto a carico di TP.
- **Resta solo il differenziale fiscale**, 26% contro la marginale. Non basta, perché:
  - con il compenso ridotto a 12.500 euro TP diventa **incapiente**: i contributi commercianti non
    trovano più IRPEF da cui dedursi;
  - scende anche il vantaggio della detrazione per redditi assimilati.

**Contestazione R1, in aggiunta.**

1. Un privilegio sugli utili calibrato 1:1 sulla riduzione del compenso, con l'impegno che gli
   altri soci «non ci perdono», è remunerazione del lavoro in veste di dividendo. Due sono le vie
   di contestazione:
   - l'**art. 10-*bis* L. 212/2000**: il vantaggio IRPEF è l'unica ragione, e la «remunerazione
     del rischio del socio operativo» non regge se il privilegio si azzera quando il compenso
     risale;
   - la **simulazione relativa** della delibera.
2. L'INPS, con la linea della Cassazione, **non ha interesse a contestare**: incassa di più. Il
   «parere INPS» previsto nel dossier è quindi superfluo, e la leva perde valore da sola.
3. **N-2 di V03.** Il compenso ridotto aumenta il reddito **effettivo** 2026-2027 di Overall, che
   è la base della proposta CPB 2028-2029.

**Correzione proposta.**

- Togliere il § 3.4 dalla sintesi del § 6, riga 6.
- Lasciarlo nel § 5, fra le leve «scartate», con la motivazione: *«Cass. 25377/2026 e collegate:
  sopra il minimale il dividendo del socio lavoratore sconta il 24,48% di contributi commercianti;
  il vantaggio è negativo»*.
- Se si vuole tenere aperta l'ipotesi, va riscritta come scommessa sulla linea INPS, con un valore
  di 2.300-2.500 euro. In quel caso il semaforo è ROSSO per il profilo dell'art. 10-*bis*.

### R-2. § 0, § 1 e § 4 — Pradella è trattato come se non pagasse i commercianti; il «26% secco» sulle riserve è falso per lui

**Fatto.** TP è iscritto ai commercianti (dato della proprietà). Nel 2026 paga almeno il minimale:
**4.611,64 euro** fissi (INPS, circ. 14/2026). Se l'INPS ha applicato la sua linea, paga sul 25%
del reddito IRES di Overall:

- ≈ **7.524** sul 2025 (30.735 di base);
- ≈ **8.113** sul reddito concordato 2026 (33.143 di base).

**Rilievo.**

1. **I numeri di partenza.** Il netto, la differenza col fabbisogno e il dividendo necessario del
   § 0 sono sbagliati: vedi E-2 ed E-3. Tutto il § 3 parte da un fabbisogno scoperto di 11.000
   euro che in realtà è **13.900-16.200**.
2. **La riga «Distribuzione delle riserve: 26% secco» del § 4.**
   - Per FDP è vera, perché non è iscritto ai commercianti.
   - Per TP, con la linea della Cassazione, **ogni euro di dividendo oltre 18.808 euro l'anno
     sconta il 24,48% in più**.
   - Su una distribuzione integrale che gli attribuisca 52.500 euro in un solo anno i contributi
     sono **≈ 8.250**, e il prelievo complessivo sale a **≈ 41,7%**, prima della deduzione IRPEF
     dei contributi, che il compenso ridotto rende in parte incapiente.
3. **Il § 1 va riscritto.** L'alternativa 2 decade. La frase «i contributi commercianti … possono
   seguire anche gli utili» va resa precisa, cioè: *utili distribuiti sì, utili accantonati no,
   secondo Cass. 2026; l'INPS però applica ancora la circ. 102/2003*.
   - Per completezza: anche l'alternativa 2 era sbagliata. Gli **amministratori** non hanno la
     DIS-COLL, e l'aliquota sarebbe stata **33,72%**, non 35,03% **[V]**.

**Correzione proposta.**

- § 0 con i valori E-2 ed E-3, mostrando le due linee.
- § 1 riscritto come sopra.
- § 4: riga delle riserve con due colonne, FDP (26%) e TP (26% + 24,48% oltre 18.808 euro l'anno).
- Nuova leva nel § 3: **dividendi a TP in tranche annuali non oltre 18.808 euro**. Serve una
  distribuzione complessiva di circa 75.000 euro l'anno, a parità di quote. È il livello che
  copre quasi esattamente il suo fabbisogno e che, con la linea della Cassazione, **non genera
  contributi aggiuntivi**. Semaforo VERDE: è la semplice applicazione del minimale.

---

## Parte III — Rilievi da correggere (GIALLO)

### G-1. § 2.1 — Previdenza di FDP: VERDE confermato, ma cifre, aliquota di uscita e campi obbligatori sono da rifare

**Verifica normativa.**

- **Modulare.** L'art. 4.2 del Regolamento generale di previdenza Inarcassa prevede un'aliquota
  dall'1% all'8,5% del reddito professionale netto IRPEF dell'anno precedente. Il minimo è 255
  euro, il massimo 12.520. Va versato entro il 31/12 dopo la dichiarazione, anche in più volte,
  ed è interamente deducibile (art. 10, c. 1, lett. e, TUIR) senza tetto. **Confermato** su
  inarcassa.it.
- **Fondo pensione.** Il tetto è di 5.300 euro dal 2026 (art. 8, c. 4, D.Lgs. 252/2005 come
  modificato dall'art. 1, c. 201, L. 199/2025). **Confermato** da più fonti. Una fonte, MySolution,
  titola «decorrenza incerta», ma il contenuto è riservato. La circ. Assogestioni 15/2026 citata
  dall'utente non l'ho letta direttamente.

**Rilievo.**

- Le cifre sono sbagliate: vedi E-4, E-5, E-6 ed E-7.
- L'argomento «aliquota implicita del 45% di sconto all'ingresso» è incompleto. La pensione
  Inarcassa da modulare è tassata a **IRPEF ordinaria** in uscita: il vantaggio è un differimento
  più il differenziale fra la marginale di oggi (45%) e quella del 2039.
- La nota dell'utente del 01/09 conclude che il **fondo pensione batte il modulare** di circa il
  47% di rendita netta nello scenario centrale. Quindi l'ordine va scritto:
  1. prima 5.300 al fondo pensione;
  2. il modulare per l'eccedenza;
  3. l'Allegato B della ricongiunzione, già deciso e gratuito.

**Correzione proposta.**

- Tabella con 11.976 + 5.300 = 17.276, risparmio ≈ 7.780 e netto ≈ 64.600.
- Tolta la frase sul 9%.
- Aggiunti i campi del protocollo:
  - **condizioni di mantenimento:** versamento entro il 31/12 di ogni anno; importo del modulare
    ricalcolato ogni anno sul reddito dell'anno precedente;
  - **vincolo:** il capitale è indisponibile fino al 2039, salvo le anticipazioni del fondo
    pensione;
  - **responsabile:** FDP, con la commercialista per il quadro RP.

### G-2. § 2.2 — P.IVA contro società: la conclusione regge, ma il metodo e due delle ragioni sono sbagliati, e manca lo scenario che interessa davvero

**Verifica normativa.**

1. **Inarcassa sui soci.** Le regole sono diverse per le due forme.
   - Per la **STP** il soggettivo è dovuto sulla quota di reddito della società attribuita al socio
     in base alla partecipazione agli utili, **anche se non distribuita** e qualunque sia la
     qualificazione fiscale. È una regola Inarcassa, riportata dalle fonti in fondo. Il [V] di L01
     si chiude in senso **negativo**: l'utile trattenuto in STP paga comunque il 14,5%.
   - Per la **società di ingegneria** sugli utili non è dovuto soggettivo. La società versa
     l'integrativo del 4%.
2. **Il compenso di amministratore** che la società paga a FDP è reddito assimilato: gestione
   separata INPS al 24%, di cui 16% a carico della società, e **non** Inarcassa. Se chiude la
   P.IVA, FDP perde l'iscrizione a Inarcassa, a 13 anni dalla pensione. Il modello applica invece
   Inarcassa al 14,5% sul compenso (E-8).
3. **IRAP.** FDP non la paga perché dal 2022 le persone fisiche esercenti arti e professioni sono
   escluse (art. 1, c. 8, L. 234/2021), e non perché «senza organizzazione».

**Scenario mancante.** Il § 0 dice che il problema di FDP è **dove accumulare 29.000 euro l'anno**.
Lo scenario rilevante è quindi quello con l'utile trattenuto e la liquidazione o cessione al 2039,
ed è proprio quello che il § 2.2 liquida in una riga. Rifatto:

- per ogni euro marginale la P.IVA lascia **0,47 netti più 0,145 di montante Inarcassa**;
- la società di ingegneria trattiene 0,72, che diventano 0,53 all'uscita, senza montante e con
  la gestione separata sul compenso;
- a regime il netto annuo è **≈ 70.100** contro 74.100, e senza i 20.445 euro di montante
  Inarcassa.

Il differimento su 13 anni non colma la differenza con un rendimento plausibile. **La conclusione
«non conviene» si rafforza.**

**Correzione proposta.**

- Rifare la tabella con E-8 e con lo scenario di accumulo al 2039.
- Chiudere il [V] su Inarcassa: STP negativo; società di ingegneria nessun soggettivo sugli utili,
  ma perdita dell'iscrizione.
- Correggere la motivazione sull'IRAP.

### G-3. § 2.3 — Holding: il rinvio al 2028 poggia su una premessa sbagliata; PEX a 60 mesi, non 12

**Verifica normativa.**

1. **Art. 21, c. 1, lett. b-*ter*, D.Lgs. 13/2024.**
   - La cessazione per «modifiche della compagine sociale» riguarda le società e associazioni
     dell'**art. 5 TUIR**, e solo se **aumenta il numero dei soci**.
   - Fusione, scissione e conferimento contano se ne è parte la società in concordato, non un suo
     socio.
   - L'AdE, con la **risposta n. 102 del 15/04/2025**, ha escluso la cessazione del CPB della S.r.l.
     per il conferimento delle quote da parte del socio. La fonte è Cesystemweb **[V]**: non ho
     letto la risposta nel testo originale.
   - FDP che conferisce il suo 25% in una holding lascia i soci di Overall a quattro: **nessuna
     causa di cessazione**. Resta da rispettare la condizione di V03 G-6, cioè non aumentare il
     numero dei soci.
2. **Art. 177, c. 2-*bis*, TUIR dopo il D.Lgs. 192/2024**, in vigore per i conferimenti dal
   31/12/2024.
   - La partecipazione deve essere **qualificata**: diritti di voto sopra il 20% o capitale sopra
     il 25%. Con il **25% dei voti**, sopra il 20%, **il requisito c'è**.
   - La conferitaria deve essere **unipersonale oppure**, se il conferente è una persona fisica,
     partecipata solo da lui e dai suoi **familiari**. È una possibilità nuova, che L01 non
     menziona ed è utile al passaggio generazionale.
3. **Art. 177, c. 2-*quater*.** Dopo un conferimento ex c. 2-*bis* il possesso richiesto per la
   PEX (art. 87, c. 1, lett. a) sale a **60 mesi**. L01 scrive «almeno 12 mesi»: è **sbagliato**.
   Con il conferimento nel 2026 la PEX è possibile solo sulle cessioni dal 2031.

**Rilievo.**

- **Il rinvio al 2028 costa.** Se le riserve di 210.113 euro si distribuiscono prima del
  conferimento, FDP paga il 26% sui suoi 52.528 euro: **13.657 euro**. Se passano per la holding,
  l'imposta è di **≈ 630** (1,2%), e il 26% scatta solo quando la cassa arriva a lui.
  - Non conta se FDP i dividendi non li usa.
  - La scelta corretta è quindi **conferire prima e distribuire dopo**, oppure non distribuire
    fino al conferimento.
- **Mancano i costi della holding:** bilancio, commercialista, diritto camerale, notaio. Sono circa
  2.500-4.000 euro l'anno **[I]**, e vanno messi contro il differimento.
- **Profilo R1.** La contestazione tipica è la «holding cassaforte» che poi finanzia il socio.
  Nel dossier servono:
  - la politica di investimento scritta;
  - il divieto di finanziamenti al socio e di spese personali;
  - la ragione di passaggio generazionale, se c'è.

  La distribuzione alla holding di riserve formate prima del conferimento non è di per sé
  abusiva. Diventa un indizio se la holding le gira subito a FDP.

**Correzione proposta.**

- Togliere la motivazione «art. 21» e sostituirla con la risposta 102/2025, da leggere nel testo.
- Anticipare la valutazione a **prima di qualunque distribuzione delle riserve**.
- Portare la PEX a 60 mesi.
- Aggiungere la holding familiare e i costi.

**Il rischio si estingue** al 31/12 del quinto anno successivo alla dichiarazione del periodo del
conferimento: per un conferimento nel 2026, il **31/12/2032 [V]**.

### G-4. § 3.1 — Auto in uso promiscuo: il regime è VERDE, ma il conto e la deducibilità dal 2028 sono sbagliati

**Verifica normativa.**

- **Fringe benefit.** Dal 2025 l'art. 51, c. 4, TUIR come modificato dalla L. 207/2024 lo fissa al
  50% di 15.000 km ACI, al **10%** per le elettriche e al 20% per le plug-in. Si applica agli
  assimilati tramite l'art. 52. **Confermato.** Le istruzioni sono nella circ. AdE 10/E del
  03/07/2025.
- **Deducibilità.** Il 70% dell'art. 164, c. 1, lett. b-*bis*, vale per i veicoli assegnati ai
  **dipendenti**. Per l'**amministratore** l'AdE (circ. 47/E/2008) applica il regime ordinario:
  - costo deducibile per intero **fino al fringe tassato**;
  - per il resto al 20%, entro i limiti di costo (per il noleggio 3.615,20 euro l'anno).

  La frase «dal 2028 deducibile al 70%» è quindi **sbagliata**.
- **IVA.** È detraibile al **40%** (art. 19-*bis*1, lett. c, DPR 633/1972), salvo addebito del
  corrispettivo a TP. Il CPB non copre l'IVA.

**Rilievo.**

1. **Il conto.** Il 9.500 non è riproducibile (E-11): sulle premesse di L01 il compenso equivalente
   costa ≈ 14.000. Ma il beneficio vero dipende da tre variabili che L01 ignora:
   - **I rimborsi.** Se i rimborsi voce 0545 comprendono **rimborsi chilometrici** per l'auto
     personale di TP, oggi quella cassa arriva già esente. Con l'auto aziendale si ferma, e il
     guadagno netto si riduce di pari importo **[V]**.
   - **La vendita dell'auto a rate** richiede l'estinzione del finanziamento: il residuo può
     superare il valore dell'auto **[V]**.
   - **L'IVA non detratta**: 60% di 22% su 6.500, pari a ≈ 860 euro l'anno, se il 6.500 è
     imponibile.
2. **Il fringe dell'auto concorre alla soglia unica di 2.000 euro** del § 3.2, che è «tutto o
   niente». Con 700 euro di fringe dell'auto restano ≈ 1.300 euro di spazio per mutuo e utenze. Se
   si sfora, **tutto** diventa imponibile. I §§ 3.1 e 3.2 non si sommano come scritto nel § 6.
3. **Dopo il 2027** il costo dell'auto è quasi tutto indeducibile, mentre il compenso è deducibile
   al 24%. Il vantaggio si riduce: rifatto sul 2028 resta positivo, circa 6.300 euro di costo
   contro 10.600 di compenso equivalente al netto IRES.

**Correzione proposta.**

- Rifare l'ordine di grandezza con i dati reali: canone, composizione dei rimborsi 0545, debito
  residuo dell'auto.
- Correggere la deducibilità: fringe più 20% entro 3.615,20.
- Aggiungere l'IVA al 40%.
- Coordinare con il § 3.2.
- **Dossier:** delibera con astensione di TP (art. 2475-*ter* c.c.) e contratto di assegnazione.
  Se l'uso è effettivamente promiscuo, prova dell'uso aziendale: agenda delle trasferte.

### G-5. § 3.2 — Fringe benefit fino a 2.000 euro: il [V] si chiude in positivo, ma con due condizioni

**Verifica.**

- La soglia di 2.000 euro con figli a carico per il 2025-2027 (art. 1, c. 390, L. 207/2024) vale
  anche per i titolari di **redditi assimilati**, amministratori compresi. È la circ. 35/E/2022,
  ritenuta valida anche per il nuovo triennio (circ. 4/E/2025, secondo le fonti secondarie).
- TP ha **due figli a carico al 50%** (CU): il requisito c'è **[A]**. Serve la sua dichiarazione
  al sostituto.
- Le somme ammesse sono quelle per utenze domestiche (acqua, luce, gas), per l'affitto e per gli
  **interessi** del mutuo sulla prima casa. Non il capitale.

**Rilievo.**

- La soglia è **unica** e comprende l'auto del § 3.1 (G-4, punto 2).
- Gli interessi rimborsati in esenzione **non** sono più detraibili al 19% nel 730 di TP: ≈ 250
  euro su 1.300 **[V]** sulla circ. 4/E/2025.
- Il valore è ≈ 1.900 euro di minor costo ogni 2.000 erogati (E-12), non 1.000-1.300.

**Correzione proposta.** Chiudere il [V] e aggiungere il coordinamento con l'auto e la detrazione.
Il semaforo resta VERDE.

- **Condizioni:** soglia rispettata ogni anno, giustificativi delle utenze intestate a TP o ai
  familiari, dichiarazione dei figli a carico.
- **Vincolo:** fino al 31/12/2027, salvo proroga.

### G-6. § 3.3 — Rimborsi a piè di lista pari al 55% del compenso: non è VERDE, è il primo punto che un verificatore apre

**Fatto [A].** Voce 0545 dei cedolini:

- giugno 3.062,80, luglio 0, agosto 1.382;
- ≈ 17.800 euro l'anno annualizzati, contro 32.500 di compenso.

**Contestazione concreta (R1).**

- Rimborsi di questa entità a un presidente-socio sono il classico **compenso occulto**.
- Se non sono documentati come trasferte fuori dal comune della **sede di lavoro**, si
  riqualificano come reddito di TP: IRPEF a ≈ 31-34% effettivo più gestione separata al 24%, cioè
  **≈ 9.500-10.000 euro l'anno** fra imposte e contributi, più le sanzioni.
- Gli anni aperti vanno dal 2021 in poi.
- **La sede di lavoro va definita.** TP risiede a Verona e Overall ha sede a Villafranca: il
  tragitto casa-sede **non** è trasferta. Per l'amministratore la sede va indicata nella delibera.
- **Tracciabilità.** Dal 2025 (L. 207/2024, c. 81) sono esenti solo i rimborsi di vitto,
  alloggio, viaggio e taxi/NCC pagati con mezzi tracciabili. I rimborsi chilometrici ACI non sono
  toccati, ma richiedono il prospetto per viaggio.
- **Trasfertisti.** Se l'attività di TP è strutturalmente itinerante, il rischio è l'art. 51, c. 6,
  che rende esente solo il 50% delle indennità.

**Correzione proposta.**

- Semaforo **GIALLO**, con verifica **retroattiva** a campione dei giustificativi 2021-2025 prima
  di costruire il regolamento.
- L'indennità forfettaria va affiancata ai rimborsi con le riduzioni E-13, e non sommata a rimborsi
  analitici di vitto e alloggio.

**Il rischio si estingue:**

- per il 2021, il 31/12/2027 per le imposte (art. 43 DPR 600/1973); per i contributi valgono i
  cinque anni dalla scadenza;
- per il 2025, il **31/12/2031**.

### G-7. § 3.5 — TFM: il «prossimo rinnovo del CdA» non esiste

**Fatto [A].** Il CdA è nominato il 15/01/2018 **a tempo indeterminato** (D01 § 1).

**Norma.**

- **Tassazione separata.** Per l'indennità di fine rapporto di co.co.co. l'art. 17, c. 1, lett. c,
  TUIR richiede che il diritto risulti da un **atto di data certa anteriore all'inizio del
  rapporto**. Il rapporto di TP è iniziato nel 2018: un TFM deliberato oggi per il mandato in
  corso va a **tassazione ordinaria**.
- **Aliquota.** È quella corrispondente alla metà del reddito del biennio precedente, senza
  addizionali. Per TP circa il 23% **[I]**: il dato di L01 è plausibile.
- **Contributi.** La gestione separata è dovuta al momento del pagamento, entro il massimale
  annuo (122.295 euro nel 2026): un TFM alto pagato in un anno supera in parte il massimale.

**Rilievo.** Per creare un «nuovo mandato» servono le dimissioni e la rinomina, con la delibera del
TFM **prima**. Il verificatore leggerà la sequenza come creata per accedere alla tassazione
separata: è GIALLO, e deve avere una ragione sociale, per esempio l'introduzione di una durata
triennale del CdA per tutti.

**Correzione proposta.**

- Riscrivere «dal prossimo rinnovo» come: *«richiede una nuova nomina a termine, preceduta da
  delibera con data certa»*.
- Aggiungere la gestione separata, che il testo segna [V]: è **dovuta**.

### G-8. § 6 e VERDI in genere — mancano i campi obbligatori del protocollo

I VERDI del § 2.1, del § 3.1 e del § 3.2 non portano le **condizioni di mantenimento**, la
**scadenza del vincolo** e il **responsabile**. I GIALLI non portano la **data in cui smettono di
essere un rischio**. È lo stesso rilievo di V03 G-6.

**Correzione proposta.** Aggiungere i campi, usando come base quelli indicati sopra in G-1, G-3,
G-5, G-6 e G-7.

---

## Parte IV — Leve che il documento non ha visto

### N-1. Buoni pasto elettronici a TP (VERDE [V])

- Sono esenti da IRPEF e da contributi fino al limite giornaliero dell'art. 51, c. 2, lett. c,
  TUIR: **10 euro** elettronici dal 2026 secondo le fonti secondarie sulla L. 199/2025 **[V]** sul
  testo.
- Sono ammessi anche per i collaboratori (ris. AdE 118/E/2006) e **non** concorrono alla soglia dei
  fringe benefit.
- **Valore:** 220 giorni × 10 = **2.200 euro netti** l'anno. Con il compenso servirebbero circa
  4.300 euro di costo per Overall: il **minor costo è ≈ 2.000 euro l'anno**.
- **Dossier:** delibera e registro delle giornate lavorate.

### N-2. Possibile rimborso dei contributi commercianti pagati su utili non distribuiti (GIALLO [V])

- Dal 2025 le riserve risultano accantonate (V03). Se l'INPS ha chiesto a TP contributi sul 25% del
  reddito IRES di Overall oltre il minimale, dopo Cass. 25377/2026 **si può chiedere il rimborso**.
- **Ordine di grandezza sul solo 2025:** (30.735 − 18.555) × 24,48% ≈ **3.000 euro**. Gli anni
  precedenti vanno ricostruiti.
- **Costo:** il rimborso riduce il montante pensionistico di TP.
- **Primo passo:** l'estratto conto contributivo INPS di TP e gli F24 degli ultimi cinque anni.

### N-3. Dividendi a TP in tranche entro il minimale (VERDE)

È la correzione di R-2. Con la linea della Cassazione, fino a 18.808 euro l'anno di dividendi non
costano contributi aggiuntivi. È la leva che sostituisce il § 3.4.

### N-4. Assegno unico e ISEE di TP ([V])

- Dividendi e compensi entrano nell'ISEE: i dividendi come redditi soggetti a imposta sostitutiva.
- Fringe benefit, buoni pasto e rimborsi esenti **non** vi entrano.
- Con due figli minori e un ISEE famigliare probabilmente nella fascia decrescente
  dell'**assegno unico**, ogni euro di dividendo ha un costo implicito in più.
- Rafforza la preferenza per i canali esenti.
- **[V]:** l'ISEE 2026 e l'importo dell'assegno unico percepito.

### N-5. FDP: riscatto della laurea o di periodi Inarcassa ([V])

- L'onere è deducibile senza tetto (art. 10, c. 1, lett. e, TUIR), come il modulare, e compra
  anzianità.
- La nota dell'utente tratta la ricongiunzione (Allegato B, gratuita) ma non il riscatto.
- Con 45% di marginale e 29.000 euro di eccedenza è da quotare sul simulatore Inarcassa prima di
  scegliere fra riscatto e modulare.

### N-6. FDP: ufficio di proprietà ([V])

Va chiarito se l'ufficio serve lo studio di FDP o è locato, per esempio a Overall (D01 § 5.4:
«canone di godimento beni di terzi, da chiarire»).

- **Se è strumentale allo studio:** l'IMU è deducibile al 100% (art. 1, c. 772, L. 160/2019). Il
  regime dell'ammortamento va riletto sull'art. 54 TUIR riformato dal D.Lgs. 192/2024 **[V]**.
- **Se è locato a Overall:** il canone di mercato è reddito fondiario di FDP a IRPEF piena, senza
  cedolare per il non abitativo. Per Overall, in CPB, è un costo che non vale nulla fino al 2027.

### N-7. Deduzioni e detrazioni ordinarie di TP (verifica, non leva)

- Interessi del mutuo sulla prima casa al 19% su un massimo di 4.000 euro (≈ 760 euro).
- Spese per i figli: istruzione e sport.
- Deduzione dei contributi commercianti.

Vanno verificate nel 730 2026: la CU non riporta oneri gestiti dal sostituto, ed è normale.

---

## Verifica normativa (sintesi)

| Affermazione di L01 | Esito | Fonte |
|---|---|---|
| § 1: gestione separata al 24% se c'è altra copertura | **Confermato**: TP iscritto ai commercianti; CU 2026 al 24,0% | dato della proprietà; CU |
| § 1: alternativa al 35,03% | **Decaduta**, e comunque sarebbe stata al 33,72% per gli amministratori **[V]** | circolari INPS sulla gestione separata |
| § 1 e § 3.4: i contributi commercianti «possono seguire gli utili» | **Da precisare**: solo gli utili distribuiti (Cass. 2026); l'INPS applica ancora la circ. 102/2003 | Cass. 25377/2026 e collegate |
| § 2.1: modulare fino al 10% | **Errato**: dall'1% all'8,5%, massimo 12.520 | Inarcassa, art. 4.2 del Regolamento generale di previdenza |
| § 2.1: fondo pensione 5.164,57 | **Superato**: 5.300 dal 2026 | L. 199/2025, c. 201 |
| § 2.1: aliquota del fondo pensione fino al 9% | **Non per FDP**: la riduzione scatta oltre il 15° anno | D.Lgs. 252/2005, art. 11, c. 6 |
| § 2.2: soggettivo sugli utili di STP [V] | **Sì per la STP, no per la società di ingegneria** | Inarcassa; Sole 24 Ore, Esperto risponde |
| § 2.2: IRAP «senza organizzazione» | **Motivazione errata**: esclusione per le persone fisiche dal 2022 | L. 234/2021, c. 8 |
| § 2.3: art. 177, c. 2-*bis*, partecipazione sopra il 20% e holding interamente sua | **Confermato**, e ampliato alla holding familiare | D.Lgs. 192/2024 |
| § 2.3: PEX con 12 mesi | **Errato**: 60 mesi (c. 2-*quater*) | D.Lgs. 192/2024 |
| § 2.3: cessazione del CPB per conferimento [V] | **Non si applica** al conferimento di quote di S.r.l. da parte di un socio | AdE, risposta 102/2025 (fonte secondaria) |
| § 3.1: fringe 10/20/50% | **Confermato** | L. 207/2024; circ. 10/E/2025 |
| § 3.1: 70% dal 2028 | **Errato per gli amministratori** | circ. 47/E/2008 |
| § 3.2: soglia di 2.000 euro, mutuo e utenze, assimilati [V] | **Confermato**; soglia unica comprensiva dell'auto | L. 207/2024, c. 390; circ. 35/E/2022; circ. 4/E/2025 |
| § 3.3: 46,48 euro, tracciabilità dal 2025 | **Confermato**; riduzioni a 30,99 e 15,49 | art. 51, c. 5, TUIR; L. 207/2024, c. 81 |
| § 3.5: TFM a tassazione separata | **Solo con atto di data certa anteriore all'inizio del rapporto** | art. 17, c. 1, lett. c, TUIR |

**Limite della verifica.**

- Non ho letto nel testo originale la risposta AdE 102/2025, le sentenze della Cassazione del
  settembre 2026, la circ. 4/E/2025 né il testo della L. 199/2025 sui buoni pasto. Mi appoggio
  alle fonti secondarie indicate.
- I contributi effettivamente pagati da TP ai commercianti non sono nel fascicolo: sono la prima
  cosa da chiedere, perché decidono fra le due linee di R-1 e R-2.

**Fonti consultate:**

- [Cassazione 25377/2026 — Commercialista Telematico](https://www.commercialistatelematico.com/articoli/2026/09/contributi-inps-soci-srl-utili-non-distribuiti.html)
- [Finanza & Fisco — dieci sentenze gemelle sui soci lavoratori di S.r.l.](https://www.finanzaefisco.com/cambia-il-perimetro-della-contribuzione-inps-sugli-utili-non-distribuiti/)
- [Informazione Fiscale — utili S.r.l. e contributi, la Cassazione ribalta la posizione INPS](https://www.informazionefiscale.it/contributi-inps-utili-srl-cassazione-base-imponibile)
- [INPS — artigiani e commercianti, contributi 2026](https://www.inps.it/it/it/inps-comunica/notizie/dettaglio-news-page.news.2026.02.gestioni-artigiani-e-commercianti-i-contributi-per-il-2026.html)
- [Tutela Previdenziale — circ. INPS 14/2026](https://www.tutelaprevidenziale.it/artigiani-e-commercianti-contributi-inps-2026-aliquote-minimali-scadenze-circolare-n-14-2026/)
- [Inarcassa — versamenti facoltativi](https://www.inarcassa.it/articoli/versamenti-facoltativi)
- [Fiscomania — previdenza complementare, limite 5.300](https://fiscomania.com/previdenza-complementare-deducibilita/)
- [MySolution — L. di Bilancio 2026, tetto 5.300](https://www.mysolution.it/fisco/informazioni/news/2026/01/05/previdenza-complementare-tetto-di-deducibilita-a-5.300-euro-e-super-deduzione-giovani-aggiornata/)
- [Assogestioni — previdenza complementare, novità fiscali](https://www.assogestioni.it/articolo/previdenza-complementare-assogestioni-chiarisce-le-novita-fiscali)
- [Sole 24 Ore, Esperto risponde — società di ingegneria e Inarcassa](https://www.espertorisponde.ilsole24ore.com/quesito/societa-di-ingegneria-basta-la-contribuzione-a-inarcassa/627309)
- [Inarcassa — obblighi della società tra professionisti](https://www.inarcassa.it/per-te/azienda/societa-tra-professionisti/obblighi-della-societa-tra-professionisti)
- [Cesystemweb — CPB, compagine sociale e cessazione (risposta 102/2025)](https://www.cesystemweb.it/news/le-modifiche-a-compagine-sociale-e-cessazione-nel-cpb-215)
- [Quotidianopiù — art. 177, unipersonalità e holding](https://www.quotidianopiu.it/dettaglio/13588222/conferimenti-di-partecipazioni-qualificate-unipersonalita-e-holding)
- [Tramontelli — conferimento in holding, riforma 2025](https://www.tramontelli.it/conferimento-di-partecipazioni-in-holding-la-riforma-2025/)
- [Fiscomania — conferimento a realizzo controllato (c. 2-*quater*, 60 mesi)](https://fiscomania.com/conferimento-di-partecipazioni-realizzo-controllato/)
- [AdE — circ. 10/E/2025, auto in uso promiscuo](https://www.agenziaentrate.gov.it/portale/documents/20143/8405056/CIRCOLARE_TASSAZIONE_AUTO_USO_PROMISCUO+n.+10+del+3+luglio+2025.pdf/ccaf6f15-2ab8-add4-2283-04a56070acec)
- [GEPS — fringe benefit fino a 2.000 euro anche per gli amministratori](https://www.geps.it/fringe-benefit-esenti-sino-a-2-000-euro-anche-per-gli-amministratori-10838/)
- [Fiscomania — fringe benefit 2026, soglia unica](https://fiscomania.com/fringe-benefit-guida/)
- [FISCOeTASSE — auto affidate a dipendenti e amministratori](https://www.fiscoetasse.com/approfondimenti/13553-auto-affidate-a-dipendenti-amministratori-complicazioni-a-raffica.html)

---

## Riepilogo dei rilievi

| # | Semaforo | Dove | In una riga |
|---|---|---|---|
| R-1 | **ROSSO** | § 3.4, § 6 riga 6 | Dividendo privilegiato: con Cass. 25377/2026 sconta il 24,48% di commercianti sopra il minimale; −3.650 ogni 20.000, non +5.100. Va tolto. |
| R-2 | **ROSSO** | § 0, § 1, § 4 | TP paga i commercianti: netto ≈ 21.100, fabbisogno scoperto ≈ 13.900, dividendo necessario ≈ 18.800; «26% secco» falso per TP (≈ 42% su 52.500 in un anno). Tranche entro 18.808. |
| G-1 | GIALLO | § 2.1 | 8,5% e non 10%; 5.300; risparmio ≈ 7.780; fondo pensione al 15%; ordine: fondo pensione, poi modulare; campi del protocollo. |
| G-2 | GIALLO | § 2.2 | STP con soggettivo sugli utili; il compenso dell'amministratore va in gestione separata; motivazione IRAP; scenario di accumulo al 2039: netto ≈ 70.100 contro 74.100. |
| G-3 | GIALLO | § 2.3 | Nessuna cessazione del CPB per il conferimento (risposta 102/2025); PEX a 60 mesi; conferire prima di distribuire le riserve (13.657 contro 630); costi e dossier anti-cassaforte. |
| G-4 | GIALLO | § 3.1 | Per l'amministratore niente 70%, ma fringe più 20%; IVA al 40%; soglia unica con il § 3.2; interazione con i rimborsi chilometrici; conto da rifare. |
| G-5 | GIALLO | § 3.2 | Vale per gli assimilati; soglia unica con l'auto; niente 19% sugli interessi rimborsati; valore ≈ 1.900. |
| G-6 | GIALLO | § 3.3 | Rimborsi pari al 55% del compenso: da VERDE a GIALLO; esposizione ≈ 10.000 euro l'anno se riqualificati; sede di lavoro; 30,99 e 15,49. |
| G-7 | GIALLO | § 3.5 | CdA a tempo indeterminato: la tassazione separata richiede una nuova nomina con delibera di data certa anteriore; gestione separata dovuta. |
| G-8 | GIALLO | § 6 | Mancano i campi del protocollo su VERDI e GIALLI. |
| E-1…E-13 | correzioni numeriche | §§ 0, 2, 3, 6 | Vedi Parte I-A. |
| N-1…N-7 | integrazioni | § 3, § 2, § 4 | Buoni pasto; rimborso dei contributi commercianti; tranche entro il minimale; assegno unico e ISEE; riscatto Inarcassa; ufficio di FDP; oneri nel 730 di TP. |
