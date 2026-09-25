# Q02 — Mix di remunerazione di Tazio Pradella (TP)

**Versione 1** del 25 settembre 2026. Analista: consulente del lavoro (INPS, retribuzione degli
amministratori, IRPEF). **Da sottoporre a verifica indipendente.**
**Recepisce la verifica V04** (`99-verifiche/V04-verifica-leve.md`), rilievi R-1, R-2, G-4…G-7 e
N-1…N-4. Sostituisce il § 3 di L01.

> Convenzione: [A] accertato sui documenti · [I] inferito · [V] da verificare prima di eseguire.
> Semafori come da `00-setup/protocollo-verifica.md`. Importi in euro, anno 2026 salvo diversa
> indicazione. Modello di calcolo: `q02.py` nello scratchpad della sessione, con autoverifica sul
> netto del cedolino.

---

## Sintesi e raccomandazione

1. **Il pacchetto più efficiente è il C.** Dal 2027 il compenso scende a ≈ 26.200 euro. Il
   resto arriva a TP da benefit esenti (utenze fino a 2.000, buoni pasto elettronici fino a 2.200)
   e da un dividendo **proporzionale di 18.808 euro l'anno**, il minimale commercianti: dentro
   questa cifra non ci sono contributi aggiuntivi. TP arriva a 35.000; il costo per Overall
   scende da 39.700 a **34.600** l'anno.
2. **Subito, entro il 31/12/2026:** distribuire altri 8.808 euro a ciascun socio (35.232 in
   totale) e controllare la posizione INPS di TP. I 2.000 euro di fringe erano già stati usati nel
   2025 (CU, punto 475: 1.995), quindi non sono una leva nuova.
3. **Da scartare:** il dividendo privilegiato al posto del compenso (ROSSO, perde ≈ 4.800 ogni
   20.000 convertiti), il welfare della lett. f) e f-*bis*) per il solo TP (ROSSO) e l'auto
   termica o ibrida.
4. **Da decidere con i dati:** l'auto elettrica (GIALLO, vale da −500 a +1.500 l'anno) e
   l'indennità di trasferta forfettaria (GIALLO, ≈ 3.300 l'anno ogni 100 giorni di trasferta). Dipendono entrambe dalla
   composizione dei 17.800 euro di rimborsi della voce 0545, che è **oggi il primo rischio del
   fascicolo**.
5. **Dal 2028:** il compenso torna deducibile e il privilegio perde senso. Il TFM vale ≈ 900
   euro l'anno, ma solo con una nuova nomina a termine deliberata prima con data certa (GIALLO).

---

## 0. I dati di partenza, ricalcolati

| Dato | Valore | Fonte |
|---|---:|---|
| Compenso co.co.co. 2026 | 2.710 al mese, **32.520** l'anno | [A] cedolini 06-08/2026 |
| Compenso 2025 | 29.458; gestione separata 7.069,92 (24,0%), di cui 2.356,64 a carico di TP | [A] CU 2026, sez. 3 |
| Reddito assimilato 2025 | 27.101,36; IRPEF netta 4.176,08; detrazione art. 13 2.057,23 | [A] CU |
| **Fringe benefit 2025 «con figli fiscalmente a carico»** | **1.995,00**, non tassato | [A] CU, punto 475. **Nessuno dei documenti precedenti lo rileva** |
| Figli a carico | 2, nati nel 2014 e nel 2019, al 50%; coniuge non a carico | [A] CU |
| Rimborsi a piè di lista (voce 0545) | 4.444,80 nel trimestre 06-08, **≈ 17.800 l'anno** | [A] cedolini |
| Mandato | Presidente CdA dal 16/01/2018, **a tempo indeterminato** | [A] visura; statuto art. 19.6 |
| Clausola compenso e TFM | Art. 24 statuto: emolumento deciso dai soci; TFM «nei limiti di legge», **senza criterio** | [A] Atto |
| Utili | Art. 27.2 statuto: in proporzione, «salvo diversa deliberazione dell'Assemblea nei limiti di legge» | [A] Atto |
| Dividendi 2026 già pagati | 10.000 lordi a TP (40.000 in totale) | [A] verbale del 30/04/2026 |
| Iscrizione IVS commercianti | sì, come socio lavoratore | [A] dato della proprietà (V04) |

**Netto di TP con il solo compenso [I]:**

| | Importo |
|---|---:|
| Compenso | 32.520 |
| − gestione separata 8% | −2.602 |
| − contributi commercianti sul minimale (deducibili) | −4.612 |
| − IRPEF netta (imponibile 25.306; detrazione 1.808) | −4.012 |
| − addizionali (forfait 2,03%) | −514 |
| **Netto dal compenso** | **≈ 20.780** |
| + dividendo 2026 netto (10.000 × 0,74) | 7.400 |
| + fringe (se ripetuto come nel 2025) [V] | ≈ 2.000 |
| **Totale equivalente 2026** | **≈ 30.200** |

- Con il solo compenso il fabbisogno scoperto è **≈ 14.200** (V04 lo stima in ≈ 13.900; la
  differenza sta negli arrotondamenti del modello).
- La marginale reale di TP sul compenso è **≈ 34%** del reddito, non il 33% nominale. Si somma il
  23% di IRPEF, con l'imponibile sotto i 28.000 grazie alla deduzione dei commercianti, più l'8,7%
  di detrazione che si perde sopra i 28.000 di reddito, più le addizionali.
- **Ogni 1.000 euro di compenso lasciano a TP ≈ 606 euro e costano a Overall 1.160.**

**Interpretazione del fabbisogno.** Il fabbisogno di 35.000 euro si intende come cassa netta
**più** il valore dei benefit che sostituiscono una spesa che TP oggi sostiene (utenze, pasti,
auto). Un euro di benefit vale un euro di netto solo se la spesa esiste davvero: le utenze sì, i
pasti fuori casa nei giorni di lavoro in sede sì [I], l'auto solo se TP ne vende una.

---

## 1. Contributi: quanto costa davvero ogni canale

### 1.1 IVS commercianti del socio lavoratore di S.r.l.

- **Presupposto.** Il socio che partecipa personalmente al lavoro aziendale con abitualità e
  prevalenza va iscritto ai commercianti (art. 1, c. 203, L. 662/1996). Chi è anche amministratore
  retribuito ha la doppia iscrizione: gestione separata sul compenso, commercianti sull'attività
  operativa (art. 12, c. 11, D.L. 78/2010, di interpretazione autentica). **[A]** Per TP è così,
  ed è per questo che la sua gestione separata è al 24% e non al 33,72%.
- **Aliquote 2026** (circ. INPS 14/2026):
  - minimale di reddito **18.808**, contributo fisso **4.611,64** (compresa la maternità);
  - **24,48%** fino a 56.224 e 25,48% oltre;
  - massimale 122.295 per chi è iscritto dal 1996;
  - rate fisse il 18/05, 20/08 e 16/11/2026 e il 16/02/2027.
  - I contributi sono **deducibili** per TP (art. 10, c. 1, lett. e, TUIR).
- **La base imponibile oltre il minimale: tre letture.**

| Linea | Base per TP | Effetto dei dividendi | Stato |
|---|---|---|---|
| **INPS** (circ. 102/2003, ribadita nella circ. 14/2026 e nelle istruzioni al quadro RR 2026) | quota del reddito d'impresa dichiarato dalla S.r.l., cioè 25% del reddito IRES, **anche se non distribuito**. Sul concordato 2026: 25% × 132.572 = 33.143 | nessuno, perché la base prescinde dalla distribuzione | prassi amministrativa, **smentita** |
| **Cassazione, sez. lavoro, 16-17/09/2026, nn. 25377-25383 e 25465-25467** | reddito **«fiscalmente imputato al socio e denunciato ai fini IRPEF»**, cioè utili distribuiti o in trasparenza (artt. 115-116 TUIR). Gli utili accantonati sono esclusi e **l'onere della prova è dell'INPS** | il dividendo percepito sopra il minimale sconta il **24,48%** | [A] dieci sentenze conformi, udienza del 07/07/2026 (presidente Tricomi) |
| **Letterale** (art. 3-*bis* D.L. 384/1992) | «redditi d'impresa»: il dividendo è reddito di **capitale** (art. 44 TUIR) e, con la ritenuta del 26%, non si dichiara | nessuno | argomento di dottrina, criticato come «forzatura» da entrambi i lati |

**[V]** Le sentenze le ho verificate su fonti secondarie concordi fra loro (Finanza & Fisco,
Informazione Fiscale, Lavorosì), non sul testo integrale. Il sito di Commercialista Telematico
non era accessibile.

**Conseguenza operativa, che vale sotto tutte e tre le linee:** **i dividendi di TP entro 18.808
euro l'anno non costano contributi aggiuntivi.**
- Linea Cassazione: sono coperti dal minimale.
- Linea INPS: la base non dipende dai dividendi.
- Linea letterale: non sono mai base.

È la regola di progetto. Sopra i 18.808 euro, con la linea Cassazione, ogni euro di dividendo
costa a TP il 24,48% (≈ 16% dopo la deduzione, se capiente).

**Un rischio pregresso da chiarire [V].** Se TP ha pagato, o gli è stato chiesto, il contributo
sul 25% del reddito di Overall come vuole la linea INPS:
- l'importo è ≈ 3.000 euro l'anno sul 2025, (30.735 − 18.555) × 24,48%;
- dopo la Cassazione si può chiedere il rimborso, o resistere all'avviso (V04, N-2);
- il rimborso però riduce il montante pensionistico di TP.

Se invece TP ha dichiarato solo il minimale, l'INPS potrebbe ancora emettere avvisi sulla sua
linea. Oggi la difesa è forte.

### 1.2 Costo per euro netto a TP, per canale

| Canale | Contributi | 2026-2027, Overall in CPB | Dal 2028, ordinario |
|---|---|---:|---:|
| Compenso co.co.co. | GS 24% (16% Overall, 8% TP) | **1,90** | 1,45 (IRES 24%; indeducibile IRAP) |
| Dividendo **proporzionale** entro 18.808 | nessuno | **0** per gli altri soci: è la quota di TP (1,35 lordo su netto) | idem (1,88 ante IRES) |
| Dividendo **privilegiato** entro il minimale / oltre | — / 24,48% commercianti | 1,35 / 1,73 a carico degli altri soci | 1,88 / 2,40 |
| Fringe (utenze, mutuo) entro 2.000, buoni pasto, indennità di trasferta | nessuno | **1,00** | 0,76 |
| TFM (con data certa, tassazione separata ≈ 23%) | GS 24% al pagamento | 1,64, differito | **1,24**, differito |

- Nel concordato 2026-2027 i costi di Overall non riducono né l'IRES né l'IRAP, perché il reddito
  e il valore della produzione sono concordati (D01 § 6).
- **Ogni euro dato in benefit esenti al posto del compenso fa risparmiare circa 0,90 euro.** È la
  leva principale.

---

## 2. I canali uno per uno

### 2.1 Compenso co.co.co.

Resta la base, e ha tre funzioni che non si possono azzerare:
- remunera il lavoro del presidente;
- regge l'inquadramento (D01 § 5.1);
- alimenta la pensione di TP: 24% del compenso nel montante della gestione separata.

Si decide con **decisione dei soci** (statuto, art. 24.1). **Non** va ridotto sotto circa
15.000 euro: sotto quella soglia TP diventa incapiente e perde la deduzione dei commercianti e
parte della detrazione. Ogni 1.000 euro di compenso in meno sotto i 15.000 gli costano ≈ 740-900
euro di netto invece di 606.

**Un effetto collaterale sul concordato [I].** Ridurre il compenso nel 2026-2027 alza il reddito
**effettivo** di Overall, che è la base della proposta CPB 2028-2029 (V03, N-2). Sui valori del
pacchetto C, circa 6.300 euro l'anno, l'effetto è marginale.

### 2.2 Dividendo proporzionale in tranche entro il minimale — **VERDE**

- **Leva:** distribuire ogni anno **75.232** euro complessivi, cioè 18.808 a socio. TP ne ricava
  **13.918 netti** senza contributi aggiuntivi.
- **Sostenibilità:** riserve distribuibili 210.113, liquidità ≈ 225.600, utile netto annuo atteso
  ben superiore a 75.000 (D01).
- **2026:** TP ha già ricevuto 10.000. Restano **8.808** entro il minimale, cioè una
  distribuzione aggiuntiva di **35.232** da pagare **entro il 31/12/2026**, per cassa.
- **Effetto sugli altri soci:** nessun costo. Ricevono la loro quota.
  - Unica interferenza: se FDP intende conferire la partecipazione in una holding (V04, G-3), gli
    conviene farlo **prima** delle distribuzioni. Altrimenti la sua quota paga il 26% invece
    dell'1,2%. È una decisione di calendario, da coordinare con il documento su FDP.
- **Condizioni di mantenimento:**
  - utili o riserve disponibili;
  - pagamento nell'anno solare;
  - somma dei dividendi percepiti da TP nell'anno ≤ 18.808, da aggiornare ogni anno con la
    circolare INPS.
- **Scadenza del vincolo:** annuale. **Responsabile:** l'organo amministrativo, con la
  commercialista.
- **ISEE e assegno unico [V].** Il dividendo entra nell'ISEE familiare, due anni dopo. Se l'ISEE
  è nella fascia decrescente dell'assegno unico, costa ≈ 4-5 centesimi di assegno per euro lordo
  [I]. Serve la DSU 2026.

### 2.3 Dividendo privilegiato (art. 2468, c. 3, c.c.) — **ROSSO, scartato**

Confermo V04 R-1 con il mio modello.
- **Conversione di 20.000 euro di compenso:** TP perde 14.014 netti, perché scendendo a 12.520
  diventa incapiente. Per compensarli serve un dividendo privilegiato di **28.000** lordi, contro
  23.200 di costo del compenso: **−4.800** l'anno.
- **Conversione di 5.000 euro:** serve un dividendo di 5.457 contro 5.800 di costo, cioè **+340**
  l'anno. È irrilevante, a fronte di:
  - modifica statutaria con il consenso di tutti i soci;
  - art. 10-*bis*, perché il privilegio replica il compenso;
  - rischio di simulazione.
- **Dal 2028** è peggiore del compenso in ogni caso (1,88-2,40 contro 1,45).
- **Variante «distribuzione asimmetrica temporanea»,** cioè TP incassa la sua quota di riserve
  prima degli altri, con il consenso unanime, ex art. 27.2 dello statuto **[V]** notaio. Non serve
  se si segue il § 2.2.

### 2.4 Fringe benefit fino a 2.000 euro: utenze, mutuo, affitto — **VERDE, già in uso**

- **Norma.** Art. 1, c. 390, L. 207/2024, per il 2025-2027: soglia di 1.000 euro, **2.000 con
  figli fiscalmente a carico**. Comprende le somme per utenze domestiche, affitto e **interessi**
  del mutuo sulla prima casa.
  - Vale per i **redditi assimilati**, amministratori compresi (circ. 35/E/2022, richiamata dalla
    circ. 4/E/2025).
  - Spetta per intero a ciascun genitore anche con i figli al 50% (circ. 4/E/2025).
  - Serve la dichiarazione del lavoratore con i codici fiscali dei figli.
  - Se si supera la soglia, **tutto** diventa imponibile.
- **[A] Nel 2025 TP ne ha già avuti 1.995** (CU, punto 475). **Non è una leva nuova**: nel
  pacchetto A è già dentro (V04 G-5 lo trattava come incrementale, ≈ 1.900).
  - **[V]:** come è stato erogato nel 2025 (utenze? buoni acquisto?) e se è previsto per il 2026,
    dato che i cedolini di giugno-agosto non lo mostrano.
- **Come usarlo:**
  - prima le **utenze**, con bollette intestate a TP o al coniuge. In questo modo gli interessi
    del mutuo restano detraibili al 19% nel 730, circa 250 euro;
  - poi gli interessi del mutuo solo per la parte residua.
- **Unica soglia con l'auto (§ 2.6):** il fringe dell'auto la consuma.
- **Dossier:**
  - delibera o regolamento del CdA, con astensione di TP;
  - dichiarazione dei figli a carico;
  - copia delle bollette e della quietanza;
  - pagamento o rimborso tracciato;
  - esposizione in cedolino e in CU al punto 475.
- **Mantenimento:** soglia ≤ 2.000 comprensiva di **ogni** altro fringe; figli a carico.
  **Scadenza:** 31/12/2027 salvo proroga. **Responsabile:** centro paghe.

### 2.5 Buoni pasto elettronici — **VERDE [V]**

- **Norma.** Art. 51, c. 2, lett. c), TUIR: soglia a **10 euro al giorno** per i buoni
  elettronici dal 2026 (art. 1, c. 14, L. 199/2025, fonti secondarie concordi).
  - La lettera c) **non** richiede la «generalità» dei dipendenti.
  - Si applica agli assimilati per il rinvio dell'art. 52 (ris. 118/E/2006 sui collaboratori).
  - È esente anche dalla gestione separata, perché la base segue quella fiscale.
  - **Non** consuma la soglia dei fringe.
- **Valore:** 220 giornate × 10 = **2.200** netti, con un costo di 2.200 (IVA al 4% detraibile).
  Con il compenso servirebbero ≈ 4.200 di costo.
- **Limite [I]:** niente buono nei giorni di trasferta in cui il vitto è rimborsato o coperto
  dall'indennità. Se le trasferte sono molte, il valore scende; con 100 giorni di trasferta,
  ≈ 1.200.
- **Dossier:**
  - delibera del CdA;
  - contratto con la società emettitrice;
  - registro delle giornate di presenza in sede, riconciliato con le note spese.
- **Mantenimento:** registro delle presenze; niente cumulo con il vitto rimborsato.
  **Scadenza:** nessuna. **Responsabile:** centro paghe.

### 2.6 Auto aziendale in uso promiscuo — **GIALLO**; solo elettrica

- **Fringe dal 2025** (art. 51, c. 4, TUIR, modificato dalla L. 207/2024; circ. 10/E/2025): 15.000
  km × costo chilometrico ACI × **10%** per l'elettrica, 20% per l'ibrida plug-in, 50% per le
  altre.
  - Per un'elettrica media vale ≈ **600-800** euro [I].
  - Con la plug-in il fringe è ≈ 1.500, quasi tutta la soglia dei 2.000. Con la termica è
    ≈ 3.750: **supera la soglia e rende imponibile tutto**. **Solo l'elettrica.**
- **Deducibilità dal 2028** (circ. 47/E/2008): per l'amministratore **non** vale il 70% dei
  dipendenti. Il costo è deducibile per intero fino al fringe tassato, e per il resto al 20% entro
  i limiti dell'art. 164 (per il noleggio 3.615,20 euro l'anno).
- **IVA:** detraibile al **40%** (art. 19-*bis*1, lett. c, DPR 633/1972). Il CPB non copre l'IVA.
- **Conto [I],** con ipotesi dichiarate: noleggio a lungo termine di un'elettrica a ≈ 550 euro al
  mese più IVA, più energia.

| | CPB 2026-2027 | Dal 2028 |
|---|---:|---:|
| Costo per Overall: canone, IVA indetraibile ed energia | ≈ 8.500 | ≈ 8.150 |
| Spazio fringe perso per le utenze, ≈ 750 da ridare in compenso | ≈ 1.430 | ≈ 1.090 |
| Compenso equivalente a 6.000 euro di costi auto evitati da TP | ≈ 11.460 | ≈ 8.710 |
| **Vantaggio netto** | **≈ +1.500** | **≈ −500** |

- Il risultato si rovescia se:
  - TP non vende davvero un'auto;
  - il debito residuo del finanziamento supera il valore dell'auto;
  - la voce 0545 contiene **rimborsi chilometrici**: con l'auto aziendale cessano, e insieme la
    cassa esente che oggi finanzia la sua auto.
- **Serve:**
  - la composizione della voce 0545;
  - rata, debito residuo e costi dell'auto da dismettere;
  - un preventivo di noleggio.
- **Dossier:**
  - delibera del CdA con astensione di TP (art. 2475-*ter* c.c.);
  - contratto di assegnazione in uso promiscuo, con data e percorrenza;
  - fringe in cedolino;
  - agenda delle trasferte per l'uso aziendale.

### 2.7 Rimborsi di trasferta e indennità forfettaria — **GIALLO**

- **Oggi [A]:** ≈ 17.800 euro l'anno a piè di lista, il **55% del compenso**. È il primo punto
  che apre un verificatore (V04, G-6).
  - Se i rimborsi vengono riqualificati: ≈ **9.500-10.000 euro l'anno** fra IRPEF, gestione
    separata e sanzioni.
  - Anni aperti dal 2021; il 2025 esce dal rischio il **31/12/2031**.
- **Regole** (art. 51, c. 5, TUIR, applicabile tramite l'art. 52):
  - esente solo la trasferta **fuori dal comune della sede di lavoro**. Il tragitto
    Verona-Villafranca è casa-lavoro, non trasferta;
  - dal 2025 vitto, alloggio, viaggio e taxi/NCC sono esenti **solo se pagati con mezzi
    tracciabili** (L. 207/2024, c. 81);
  - i rimborsi chilometrici ACI richiedono un prospetto per ogni viaggio;
  - **indennità forfettaria esente:** 46,48 euro al giorno; **30,99** se è rimborsato il vitto o
    l'alloggio; **15,49** se sono rimborsati entrambi. Le spese di viaggio si possono rimborsare
    a parte senza ridurla.
- **Leva possibile [I]:** nei giorni di trasferta senza pernottamento, sostituire il rimborso del
  vitto con l'indennità di 46,48 euro, e rimborsare solo il viaggio.
  - **Per 100 giorni** di trasferta: 4.648 esenti, contro i ≈ 1.500-2.000 di vitto rimborsato
    oggi [V], cioè ≈ **2.600-3.100 netti in più** a costo pari.
  - **Solo** con trasferte reali e documentate.
  - Rischio «trasfertista» (art. 51, c. 6, esenzione al 50%) se la trasferta diventa la regola.
- **Dossier:**
  - delibera che fissi la **sede di lavoro** di TP a Villafranca;
  - regolamento trasferte (misto: forfait + viaggio);
  - report mensile con data, luogo, cliente e commessa;
  - pagamenti tracciati;
  - **verifica a campione dei giustificativi 2021-2025 prima** di cambiare lo schema.

### 2.8 Welfare art. 51, c. 2, lett. f) e f-*bis*) — **ROSSO per il solo TP**

- L'AdE (risposta 10/2019) nega l'esenzione all'amministratore per due ragioni:
  - «categoria» costruita attorno al vertice;
  - immedesimazione organica.
- Esempio escluso: rette scolastiche e centri estivi pagati per i figli di TP.
- Resta solo un piano esteso a **tutti** i lavoratori con figli, per categoria oggettiva, con
  costo anche per i tre dipendenti e con l'inclusione di TP comunque contestabile. **Non entra nei
  pacchetti.**

### 2.9 TFM — **GIALLO**, solo dal 2028 con nuova nomina a termine

- **Norma.** Tassazione separata (art. 17, c. 1, lett. c, TUIR) solo se il diritto risulta da
  un **atto di data certa anteriore all'inizio del rapporto**. La giurisprudenza richiede anche
  l'**importo o il criterio** (Cass. 19571/2022 e conformi; D01 § 5.2).
  - Il CdA è in carica **a tempo indeterminato dal 2018**: per il mandato in corso il TFM va a
    tassazione **ordinaria**.
  - La gestione separata è **dovuta** al pagamento, entro il massimale.
- **Percorso:**
  1. entro il **31/12/2027**, decisione dei soci che fissa per **tutti** gli amministratori una
     durata triennale 2028-2030. È la ragione extrafiscale: governance e fine del concordato;
  2. delibera del TFM con criterio, per esempio una percentuale del compenso, e data certa (PEC o
     registrazione), **prima** della nuova nomina;
  3. eventuale polizza, con Overall contraente e beneficiaria.
- **Valore [I]:** convertire 7.000 euro di compenso l'anno in ≈ 6.000 di accantonamento, a parità
  di netto di TP, fa risparmiare **≈ 900 euro l'anno** dal 2028. La cassa arriva ogni tre anni: va
  pianificata.
- **Da chiarire prima [V]:** a chi si riferiscono i 3.500 euro l'anno di «quiescenza» (B9-d)
  dedotti dal 2023. Se sono premi di una polizza TFM per TP, oggi la clausola dell'art. 24 è
  generica e il fondo non c'è: vanno sistemati (D01 § 5.2).
- **Il rischio si estingue** cinque anni dopo la dichiarazione dell'anno di deduzione.

### 2.10 Previdenza complementare con contributo di Overall — non nei pacchetti

- Il contributo del committente è deducibile per TP entro 5.300 euro (L. 199/2025) ed esce
  tassato al 15%-9%.
- Ma è **illiquido** fino alla pensione, per TP circa 25 anni. TP ha bisogno di cassa: la
  previdenza complementare non copre il fabbisogno.
- Va ripresa quando il compenso eccede il fabbisogno. **[V]** Regime contributivo in gestione
  separata del contributo del committente.

---

## 3. I pacchetti

Ipotesi comuni: il compenso cambia dal **1/1/2027**; dividendi proporzionali; rimborsi 0545
invariati e fuori dal netto, perché coprono spese; linea Cassazione per i commercianti.

**Il «costo per Overall»** è la spesa specifica per TP: compenso × 1,16 più i benefit. Il
dividendo proporzionale **non** è un costo: è la quota di TP, mentre gli altri ricevono la loro.
**L'«effetto sugli altri soci»** è il 75% della variazione di costo rispetto ad A.

| | **A. Status quo 2026** | **B. Status quo + tranche + buoni pasto** | **C. Benefit, compenso ricalibrato** ★ | **D. C dal 2028 + TFM** |
|---|---:|---:|---:|---:|
| Compenso annuo | 32.520 | 32.520 | **26.200** (2.184 al mese) | 19.200 + TFM ≈ 6.000 accantonato |
| Dividendo lordo a TP | 10.000 | 18.808 | 18.808 | 18.808 |
| Distribuzione totale | 40.000 | 75.232 | 75.232 | 75.232 |
| Netto cassa: compenso + dividendo | 28.180 | 34.700 | 30.800 | ≈ 26.550 + TFM ≈ 4.250 l'anno, differito |
| Fringe utenze ≤ 2.000 | 2.000 [V 2026] | 2.000 | 2.000 | 2.000 |
| Buoni pasto | — | 2.200 | 2.200 | 2.200 |
| **Netto equivalente a TP** | **≈ 30.200** ✗ | **≈ 38.900** | **≈ 35.000** | **≈ 35.000** |
| Gestione separata a montante di TP | 7.805 | 7.805 | 6.290 | ≈ 6.050 |
| Contributi commercianti | 4.612 | 4.612 | 4.612 | 4.612 |
| **Costo per Overall 2026-2027** | **39.700** | **41.900** | **34.600** | — |
| **Costo per Overall dal 2028**, dopo l'IRES | 30.200 | 31.900 | 26.300 | **≈ 25.400** |
| Effetto sugli altri soci rispetto ad A (CPB) | — | −1.650 | **+3.850** | +3.600 dal 2028 |
| Semaforo | GIALLO (rimborsi; INPS pregresso) | VERDE (+ GIALLO rimborsi) | VERDE (+ GIALLO rimborsi) | GIALLO (TFM) |

**Varianti [I], da decidere con i dati della voce 0545:**
- **C + trasferte:** 100 giorni di trasferta a 46,48, con buoni pasto ridotti a 1.200. Il compenso
  scende a ≈ 20.200 e il costo per Overall a **≈ 31.300**. GIALLO.
- **C + auto elettrica:** da −500 a +1.500 l'anno. Assorbe ≈ 750 della soglia dei fringe. GIALLO.

**Come leggerla:**
- **A non raggiunge il fabbisogno.** Gli mancano ≈ 4.800 anche contando i fringe del 2025.
- **B** è il minimo che serve **subito**: raggiunge l'obiettivo con 2.200 euro di costo in più e
  lascia a TP un margine di ≈ 3.900.
- **C** rende TP indifferente all'obiettivo e fa risparmiare ≈ 5.100 l'anno rispetto ad A e
  7.300 rispetto a B.
  - Il risparmio viene dal fatto che 4.200 di benefit sostituiscono ≈ 6.300 di compenso.
  - Il prezzo lo paga TP: **−1.500 l'anno di montante pensionistico**, compensati in piccola parte
    dal minor ISEE, cioè dall'assegno unico [V].
  - **Una via intermedia equa:** compenso a ≈ 29.000, con risparmio e margine divisi a metà.
- **D** dal 2028 cambia poco. Il compenso torna relativamente efficiente, e il TFM vale ≈ 900
  l'anno in cambio di una ristrutturazione del mandato.
- **Sensibilità.** Con la **linea INPS** i pacchetti B-D non cambiano, perché i dividendi restano
  sotto il minimale. TP però ha un costo di fondo di ≈ 3.500 l'anno (25% di 132.572, meno il
  minimale, al 24,48%) che prescinde da ogni leva e che la Cassazione oggi permette di contestare.

---

## 4. Dossier e scadenze

### Entro il 31/12/2026

| # | Azione | Per | Chi | Scadenza |
|---|---|---|---|---|
| 1 | Estratto conto INPS di TP, F24 dei commercianti 2021-2026, quadri RR 2024-2025: quale linea ha applicato l'INPS? Eventuale rimborso o contestazione (N-2) | tutti | TP, patronato o consulente | **ottobre 2026** |
| 2 | Composizione della voce 0545 2025-2026, con giustificativi; verifica a campione 2021-2025 | rischio, varianti | commercialista | **ottobre-novembre 2026** |
| 3 | Terza rata del minimale commercianti | — | TP | 16/11/2026 |
| 4 | **Decisione dei soci:** distribuzione di riserve per **35.232** (8.808 a socio), pagata entro il 31/12; ritenuta del 26% versata entro il 16/01/2027. Coordinarla prima con l'eventuale holding di FDP | B, C | assemblea | **pagamento entro il 31/12/2026** |
| 5 | Fringe 2026: bollette, dichiarazione dei figli a carico, delibera; erogazione entro il 12/01/2027 (cassa allargata) e CU al punto 475. Totale ≤ 2.000 con qualsiasi altro fringe | tutti | CdA, centro paghe | 31/12/2026 |
| 6 | **Decisione dei soci** sul compenso 2027 (C: 26.200, o 29.000 nella via intermedia), con astensione di TP dal voto in CdA dove serve | C | assemblea | dicembre 2026, dal 1/1/2027 |
| 7 | Delibera buoni pasto, contratto con l'emettitore, registro presenze | B, C | CdA | avvio 1/1/2027 (possibile da novembre) |
| 8 | Delibera della **sede di lavoro** di TP e **regolamento trasferte** (tracciabilità, forfait, prospetti km) | tutti | CdA | 31/12/2026 |
| 9 | Solo se il punto 2 lo giustifica: preventivo di noleggio elettrico, contratto di assegnazione, vendita dell'auto di TP | variante auto | CdA, TP | ordine entro dicembre 2026 |

### 2027-2028

- **Maggio-aprile 2027:** distribuzione annuale di 75.232 euro dopo l'approvazione del bilancio
  2026. Per TP ≤ 18.808 nell'anno solare, compresi gli eventuali acconti.
- **Entro il 31/12/2027:** durata triennale del CdA 2028-2030 e delibera del TFM con criterio e
  data certa, **prima** della nuova nomina (pacchetto D). Nello stesso momento:
  - sistemazione della «quiescenza» B9-d;
  - riesame del compenso, che dal 2028 torna deducibile.
- **31/12/2027:** fine della soglia fringe dei 2.000 euro, salvo proroga. Rifare il conto dei
  pacchetti.

---

## 5. [V] residui

1. Contributi commercianti effettivamente pagati da TP e linea applicata dall'INPS (azione 1).
   Decide il rischio pregresso e il rimborso.
2. Testo integrale di Cass. 25377/2026 e collegate: le ho verificate su fonti secondarie.
3. Composizione della voce 0545: vitto, alloggio, km, altro; giorni di trasferta fuori comune.
4. Fringe 2026: è già previsto? Natura dei 1.995 euro erogati nel 2025.
5. Testo dell'art. 1, c. 14, L. 199/2025 (buoni pasto a 10 euro), e prassi sui buoni pasto agli
   amministratori soci.
6. Destinatario e natura dei 3.500 euro l'anno in B9-d (polizza TFM?).
7. ISEE 2026 della famiglia di TP e assegno unico percepito: valore implicito dei canali esenti.
8. Dati dell'auto di TP (rata, debito residuo) e preventivo di noleggio.
9. Contribuzione in gestione separata del contributo del committente alla previdenza
   complementare, se mai attivata.
10. Premio INAIL sui cedolini (21,28 al mese): quota di TP e base, irrilevante sui totali [V].

## 6. Fonti

**Normativa:**
- Art. 51, commi 2, 3, 4, 5 e 6, art. 52 e art. 17, c. 1, lett. c), TUIR
- Art. 1, c. 390 (fringe) e c. 81 (tracciabilità), L. 207/2024
- Art. 1, c. 14, L. 199/2025 (buoni pasto)
- Art. 3-*bis* D.L. 384/1992; art. 1, c. 203, L. 662/1996; art. 12, c. 11, D.L. 78/2010
- Art. 19-*bis*1 DPR 633/1972; art. 164 TUIR
- Artt. 2468 e 2475-*ter* c.c.
- Statuto di Overall, artt. 19, 24 e 27

**Giurisprudenza e prassi:**
- **Cass. 25377-25383/2026 e 25465-25467/2026:**
  - [Finanza & Fisco](https://www.finanzaefisco.com/cambia-il-perimetro-della-contribuzione-inps-sugli-utili-non-distribuiti/)
  - [Informazione Fiscale](https://www.informazionefiscale.it/contributi-inps-utili-srl-cassazione-base-imponibile)
  - [Lavorosì](https://www.lavorosi.it/cassazione-i-soci-lavoratori-di-una-s-r-l-devono-versare-i-contributi-anche-sugli-utili-non-distribuiti/)
  - [Commercialista Telematico](https://www.commercialistatelematico.com/articoli/2026/09/contributi-inps-soci-srl-utili-non-distribuiti.html) (non accessibile)
- **Circ. INPS 14/2026:**
  - [Tutela Previdenziale](https://www.tutelaprevidenziale.it/artigiani-e-commercianti-contributi-inps-2026-aliquote-minimali-scadenze-circolare-n-14-2026/)
  - [INPS](https://www.inps.it/it/it/inps-comunica/notizie/dettaglio-news-page.news.2026.02.gestioni-artigiani-e-commercianti-i-contributi-per-il-2026.html)
- **Fringe benefit per gli amministratori, circ. 35/E/2022 e 4/E/2025:**
  - [GEPS](https://www.geps.it/fringe-benefit-esenti-sino-a-2-000-euro-anche-per-gli-amministratori-10838/)
  - [Fiscomania](https://fiscomania.com/fringe-benefit-guida/)
- **Buoni pasto a 10 euro:**
  - [IPSOA](https://www.ipsoa.it/documents/quotidiano/2025/12/30/buoni-pasto-elettronici-limite-esenzione-fiscale-sale-10-euro)
  - [FISCOeTASSE](https://www.fiscoetasse.com/approfondimenti/17162-buoni-pasto-2026-natura-giuridica-regime-fiscale-e-novita.html)
- **Auto in uso promiscuo:**
  - [circ. AdE 10/E/2025](https://www.agenziaentrate.gov.it/portale/documents/20143/8405056/CIRCOLARE_TASSAZIONE_AUTO_USO_PROMISCUO+n.+10+del+3+luglio+2025.pdf/ccaf6f15-2ab8-add4-2283-04a56070acec)
  - circ. 47/E/2008 per gli amministratori, via [FISCOeTASSE](https://www.fiscoetasse.com/approfondimenti/13553-auto-affidate-a-dipendenti-amministratori-complicazioni-a-raffica.html)
- **Welfare e amministratori:**
  - [AdE, risposta 10/2019](https://www.agenziaentrate.gov.it/portale/documents/20143/307208/Interpello+10+2019_Risposta+n.+10+del+2019.pdf/1b3c806d-1843-e780-85dc-033ebe6a2b9f)
  - [Bollettino ADAPT](https://www.bollettinoadapt.it/welfare-aziendale-e-amministratori-dopo-la-risposta-n-10-2019-dellagenzia-delle-entrate/)
- **TFM e data certa:** rinvio alle fonti di V01 e D01 § 5.2.

**Dati primari:**
- cedolini 06, 07 e 08/2026;
- CU 2026 di TP (scansione, letta come immagine);
- Atto costitutivo e statuto;
- visura del 10/11/2025;
- verbale dell'assemblea del 30/04/2026.
