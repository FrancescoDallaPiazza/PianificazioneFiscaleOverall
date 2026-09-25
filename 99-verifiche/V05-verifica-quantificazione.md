# V05 — Verifica indipendente delle analisi specialistiche Q01, Q02, Q03

**Revisori:**
- **R1**, il verificatore: ufficiale GdF, funzionario AdE, ispettore INPS;
- **R2**, il supporto tecnico: tributarista e attuario, per calcoli e norme.

La domanda è la stessa di V03 e V04: *quale numero è sbagliato, quale norma è letta male, dove si
rompe il fascicolo quando arriva un accesso?*

**Data della verifica:** 25 settembre 2026.

**Documenti verificati**, tutti in versione 1 del 25/09/2026 e non ancora versionati:
- `03-quantificazione/Q01-previdenza-fdp.md`;
- `03-quantificazione/Q02-remunerazione-tazio.md`;
- `03-quantificazione/Q03-strutture-holding-exit.md`.

**Letti prima:** `00-setup/protocollo-verifica.md`, `00-setup/parametri-incarico.md`,
`03-quantificazione/00-contesto-comune.md`, `99-verifiche/V04-verifica-leve.md`,
`C:\Users\Francesco\Downloads\handoff_pensione_inarcassa.md`.

**Modelli rieseguiti:** `q01/m.py`, `q01/m2.py`, `q02.py` e `q03.py` nello scratchpad di
sessione. Tutti girano e i loro `assert` passano. Tutte le cifre di Q01, Q02 e Q03 sono
riprodotte dai modelli, salvo quelle indicate in Parte I. I controlli aggiuntivi li ho eseguiti a
riga di comando, sugli stessi moduli.

**Legenda delle fonti:**
- **[P]** fonte primaria o istituzionale letta: testo di legge, sito del Ministero, INPS, AdE;
- **[S]** fonte secondaria: stampa professionale, studi, riviste;
- **[N]** non letta.

---

## ESITO COMPLESSIVO

| Documento | Esito | In una riga |
|---|---|---|
| **Q01** Previdenza FDP | **DA CORREGGERE** (nessun ROSSO) | Le conclusioni reggono e si rafforzano: fondo pensione al tetto, modulare facoltativo. Da correggere il regime delle nuove prestazioni (capitale di nuovo al 50%, frazionata al 20%), un errore di calendario nel TIR, la riga sulla holding e l'omissione dei dividendi Overall. |
| **Q02** Remunerazione TP | **DA RIVEDERE** (1 ROSSO) | Il pacchetto C, «il più efficiente», è peggiore di B per la cassa di FDP e TP: trasferisce valore agli altri due soci. In più taglia il compenso *in sostituzione* di benefit esenti, cioè il caso che l'AdE riqualifica. La raccomandazione corretta è B. |
| **Q03** Strutture, holding, exit | **DA CORREGGERE** (1 ROSSO sulla premessa) | La soglia 5%/500.000 per l'art. 89 e la PEX (P-5) è stata **abrogata retroattivamente** dal D.L. 38/2026, convertito dalla L. 88/2026. Le conclusioni però reggono: niente holding per FDP, exit con rivalutazione, TP Holding. Il piano dei dividendi della TP Holding è incompatibile con Q02. |
| **Globale** | **DA RIVEDERE** | I tre documenti usano **tre politiche di distribuzione diverse** (0, 75.232 e 136.000-153.000 euro l'anno) e **due tesi opposte sulla holding di FDP**. Serve un modello di cassa unico di Overall per il 2026-2039, prima della consegna. |

**Il punto che l'utente chiede di dirimere, cioè Q01 contro la nota `handoff` sul modulare, dà
ragione a Q01.** La nota confrontava il modulare con il fondo pensione. Per le somme **oltre** il
tetto dei 5.300 euro, però, l'alternativa corretta è l'investimento libero (PAC).

Deduzione ed uscita avvengono ad aliquote simili: 45% in entrata, 38-45% sulla rendita. Il
modulare equivale quindi a una capitalizzazione esente al tasso Inarcassa, trasformata in
rendita. Nello scenario centrale perde contro un PAC al 5% lordo. Con il calendario corretto del
TIR (E-1) il PAC rende il **3,56%** e non il 3,13%, quindi il distacco cresce.

Il modulare pareggia solo con mercati al 3% e una vita lunga. **Resta una scelta di longevità e di
reversibilità, non una leva fiscale.** La conclusione della nota, «il modulare per le somme oltre
il tetto», valeva solo con una marginale in pensione del 37%.

---

## Parte I — Cifre

### I-A. Cifre errate, con il valore corretto

| # | Dove | Il documento scrive | Valore corretto | Perché |
|---|---|---|---|---|
| E-1 | Q01 § 3.1, § 3.2 | TIR del PAC **3,1%** (scenario centrale), 1,7% e 4,6% negli altri; TIR del fondo pensione 8,7% | PAC **3,56%** (1,97% / 5,19%); fondo pensione **9,85%** (8,1% / 11,6%) | In `m.py`, `pac()` e `fp()` fanno crescere il capitale fino a fine 2039 (t = 13) ma registrano l'incasso a t = 14: c'è un anno di rendimento zero. L'ordine delle alternative non cambia. **Sale** invece il break-even del modulare contro il PAC, oggi calcolato al 4,8%: la conclusione contro il modulare si rafforza. |
| E-2 | Q01 § 1 riga 12; § 3.5 | Nuove prestazioni «tassate come il capitale»; «capitale fino al 60% [V]»; «le forme flessibili gli danno comunque accesso a tutto il montante al 15%» | Capitale **50%**: il 60% della L. 199/2025 è stato riportato al 50% dall'art. 16-*ter*, c. 1, L. 112/2026 [P Ministero del Lavoro]. **Erogazione frazionata al 20%**, che scende di 0,25 punti l'anno dopo il 15° anno fino al 15%. Rendita a durata definita e prelievi liberamente determinabili al 15-9% [S EC News; P Ministero] | Per FDP il 15% sull'intero montante si ottiene con la rendita a durata definita o con i prelievi, **non** con la frazionata. Il § 4.2 («2039: prelievi frazionati») va corretto in «prelievi liberamente determinabili o rendita a durata definita». |
| E-3 | Q03 P-5, § 2.2, § 0 | Art. 89 e art. 87 TUIR solo per partecipazioni ≥ 5% o ≥ 500.000 euro dal 2026; il portafoglio quotato della holding è tassato al 24% pieno | **Soglia abrogata** con effetto dal 1/1/2026: art. 11 del D.L. 27/03/2026 n. 38, convertito dalla L. 22/05/2026 n. 88 [S concordi: Fiscomania, Studio Romano, Finanza & Fisco, Andersen, GM Tax] | Vedi R-2. |
| E-4 | Q03 § 2.2 | Holding di FDP: perde **39.000-43.000** in 13 anni | **−20.000 / −31.000** se la holding investe in azioni dirette (dividendi all'1,2%, prelievo medio sui rendimenti 5-12%); −39.000/−43.000 solo se investe in OICR o in obbligazioni (24%) | Ricalcolo con `q03.py` su D = 34.000, r = 4-5%. La conclusione («nessuna holding per la cassa») **regge**, ma con un margine dimezzato. |
| E-5 | Q02 Sintesi 1, § 3 | «Il costo per Overall scende da 39.700 a 34.600»; «4.200 di benefit sostituiscono ≈ 6.300 di compenso» | I 2.000 di fringe **erano già** nel pacchetto A (CU 2025, 1.995): i benefit nuovi sono solo i 2.200 di buoni pasto. **Rispetto a B**, C toglie a TP 3.899 netti e 1.516 di montante. Agli altri due soci dà +2.711 nel 2027 e +2.061 l'anno dal 2028. **Per la coppia FDP+TP: −1.188 nel 2027, −1.838 l'anno dal 2028** | Vedi R-1. |
| E-6 | Q03 § 2.4 | «Carico fiscale totale» della cessione a TP Holding: 58.536 su 250.000 | 55.536 più 3.000 di perizia. La perizia è sommata nella colonna holding ma **non** in quella della cessione a TP persona fisica (140.338 = 52.500 + 87.838) | Il confronto va fatto a parità di perizia: il vantaggio della holding **non cambia**. |
| E-7 | Q03 § 2.4 punto 2 | Con la dilazione concessa dal venditore «la plusvalenza si tassa per cassa» | Vale solo **senza** rivalutazione. Il venditore che rivaluta paga il 21% sull'intero valore **entro il 30/11** (in tre rate annuali al massimo), qualunque sia il piano d'incasso | Il calendario del § 7 (2039: rivalutazione più cessione a TP Holding con dilazione) crea un fabbisogno di cassa per il venditore. |
| E-8 | Q02 § 0; Q02 § 2.2 | Il dividendo di FDP va in holding «se no paga il 26% invece dell'1,2%» | È solo un **differimento**: Q03 § 2.2 lo dimostra (−229 / +29 sulle riserve) | Incoerenza fra i documenti: vedi G-6. |

### I-B. Cifre verificate: non intervenire

| Dato | Esito |
|---|---|
| Q01: esborso netto 2.913; imposte risparmiate 2.387 / 7.779; netto spendibile 71.087 / 64.503 | riprodotti |
| Q01: montante del modulare 181.322, rendita 10.335, TIR 2,21% (morte a 86 anni, tassa 45%) | riprodotti |
| Q01: marginale in pensione 38,2% (base 43.903 più 5.000) e 45,0% oltre 50.000 | riprodotta con la detrazione dell'art. 13, c. 3 |
| Q01: aliquota di uscita del fondo pensione al 15% per l'uscita nel 2039; 13,5% dal 2046 | corretta (art. 11, c. 6, D.Lgs. 252/2005) |
| Q02: netto di TP dal compenso 20.781; pacchetti A 30.181, B 38.899, C 35.000 con compenso 26.203 | riprodotti |
| Q02: conversione di 20.000 in dividendo privilegiato, −4.800 | riprodotta (28.019 contro 23.200) |
| Q02: dividendo annuo di 18.808 a socio, 75.232 in totale; 2026: 8.808 a socio, 35.232 in totale | aritmetica corretta |
| Q03: P.IVA contro società di ingegneria, B − A = +2.685 di cassa, −72.962 con il montante | riprodotto |
| Q03: exit 2039, 194.500 con rivalutazione contro 183.452 con holding e PEX distribuita | riprodotto |
| Q03: dividendi lordi per un prezzo di 250.000: 337.838 (TP persona fisica) contro 253.036 (TP Holding) | riprodotto |

---

## Parte II — Rilievi bloccanti (ROSSO)

### R-1. Q02, Sintesi 1 e § 3: il pacchetto C non è «il più efficiente», va contro l'obiettivo dell'incarico ed è riqualificabile

**Norma.**
- Parametri dell'incarico: massimizzare la cassa netta di **FDP e TP**, senza danneggiare gli
  altri due soci. Non si minimizza il costo di Overall.
- Art. 51, c. 2, lett. c), e c. 3, TUIR. Ris. AdE 55/E/2020 [P, letta tramite sintesi]: i
  benefit finanziati con somme che costituiscono retribuzione fissa o variabile seguono le regole
  ordinarie. È il **principio di non sostituibilità**. L'unica eccezione è la conversione dei premi
  di risultato (L. 208/2015, cc. 182-189).

**Rilievo economico (R2).**
- **Il compenso di TP è l'unico canale con cui la coppia sposta valore dagli altri due soci a TP.**
  Ogni euro di compenso tagliato resta in Overall, e il 75% di quell'euro appartiene a Maggia,
  Dall'Oca e FDP.
- Rispetto a B, nel pacchetto C:
  - TP perde **3.899 euro netti l'anno** e 1.516 di montante di gestione separata;
  - Overall risparmia 7.328 nel 2027 e 5.569 dal 2028, dopo l'IRES;
  - distribuito al 26%, quel risparmio vale 1.356 netti a socio nel 2027 e 1.030 dal 2028.
- **Saldo della coppia FDP+TP: −1.188 nel 2027, −1.838 l'anno dal 2028.** Il guadagno va a
  Maggia e Dall'Oca: +2.711 nel 2027 e +2.061 dal 2028.
- «TP arriva a 35.000» non è l'obiettivo. Il fabbisogno è una soglia minima, non un tetto.
- La metrica «costo per Overall» di Q02 § 1.2 è corretta per la società ma non per l'incarico. È
  lo stesso errore di metodo segnalato da V04 per L01.

**Contestazione R1.** Il dossier prevede, nella stessa tornata di dicembre 2026:
- la riduzione del compenso da 32.520 a 26.200 (azione 6);
- l'introduzione dei buoni pasto (azione 7);
- e la motivazione scritta del § 1.2: «ogni euro dato in benefit esenti al posto del compenso fa
  risparmiare circa 0,90».

È esattamente la prova documentale della sostituzione. In sede di accesso il verificatore:
- riqualifica i 2.200 euro di buoni pasto come compenso: IRPEF ≈ 800 euro l'anno a carico di TP,
  gestione separata ≈ 530 (352 a carico di Overall);
- applica ad Overall la sanzione del 20% per le ritenute non operate (art. 14 D.Lgs. 471/1997).

L'importo è modesto. Ma **brucia l'esenzione anche per gli anni successivi**, e rende contestabile
per sostituzione anche il fringe dei 2.000 euro, se viene deliberato nella stessa sede.

**Correzione.**
1. **Raccomandare B, non C:** compenso invariato, più la tranche entro il minimale, più i buoni
   pasto **in aggiunta**. Netto di TP ≈ 38.900. Costo aggiuntivo per Overall 2.200, di cui il 75%
   a carico degli altri soci, cioè 1.650: è l'effetto che Q02 già dichiara.
2. Se si vuole comunque offrire agli altri soci una contropartita, va presentata come
   **concessione negoziale**, non come ottimizzazione. Per esempio la «via intermedia» a 29.000,
   con i numeri della coppia (≈ −650 l'anno dal 2028).
3. Buoni pasto e fringe vanno deliberati con **motivazione autonoma** (presenza in sede,
   allineamento al trattamento dei dipendenti), **mai** nello stesso atto che riduce il compenso e
   mai con una motivazione di «risparmio».

**Il rischio si estingue** il 31/12 del quinto anno successivo a quello della dichiarazione
(770 e Redditi): per il 2027, il 31/12/2033.

### R-2. Q03 P-5 (e Q01 § 4.2): norma citata come vigente ma abrogata

**Norma.**
- L. 199/2025, art. 1, cc. 51-55: soglia del 5% o di 500.000 euro per l'esclusione dei dividendi
  (art. 89) e per la PEX (art. 87).
- **Abrogata** dall'art. 11 del D.L. 27/03/2026 n. 38, in vigore dal 28/03/2026, con effetto
  retroattivo dal 1/1/2026. Il D.L. è stato convertito dalla **L. 22/05/2026 n. 88**.
- Fonti [S], concordi fra loro: Fiscomania («Le restrizioni PEX … sono state abrogate dal D.L.
  38/2026»), Studio Romano Associati, Finanza & Fisco, Andersen, GM Tax.
- Il testo in Gazzetta **non** l'ho letto [N].

**Rilievo.**
- Q03 attribuisce l'etichetta [A] a una norma non più in vigore, citando FiscoOggi del
  dicembre 2025.
- Il protocollo classifica come ROSSO le raccomandazioni «fondate su una norma inesistente o male
  interpretata».
- Qui le **conclusioni sopravvivono** (E-4): niente holding per FDP, TP Holding all'1,2% su una
  quota del 25% sotto entrambi i regimi. Ma la motivazione e una cifra vanno rifatte:
  - la frase «un portafoglio di titoli quotati detenuto dalla holding è tassato al 24% pieno» è
    **falsa**;
  - dividendi e plusvalenze PEX su azioni dirette tornano all'1,2%, anche sotto il 5%. Per le
    azioni quotate il requisito della commercialità non si applica; restano l'iscrizione fra le
    immobilizzazioni e i 12 mesi di possesso;
  - restano al 24% i proventi degli OICR e le obbligazioni.
- **Q01 § 4.2** («IRES 24% sui proventi finanziari, poi 26%») eredita lo stesso errore per la
  parte azionaria.

**Correzione.**
- Riscrivere P-5 con il D.L. 38/2026 e la L. 88/2026.
- Ricalcolare la tabella del § 2.2 con due righe: holding investita in azioni dirette e holding
  investita in OICR od obbligazioni. I valori sono in E-4.
- Riallineare la frase di Q01 § 4.2.
- Il verdetto «nessuna holding per la cassa in vita» regge.
- **Da aggiungere:** la holding che investe in azioni dirette per godere dell'1,2% sposta il
  rischio sulla **società di comodo**, cioè sui ricavi presunti sulle partecipazioni (art. 30
  L. 724/1994), e sull'**art. 10-*bis***, per la holding «cassaforte» di risparmio personale.

---

## Parte III — Rilievi da correggere (GIALLO)

### G-1. Q01 § 3.2 e § 4: il modulare va presentato come indifferente, non come «perde il 20%»

- Il –22.000 di capitale equivalente dipende da due ipotesi, entrambe favorevoli al PAC:
  - la tassa del 45% in uscita, che presuppone il **drenaggio fiscale** su scaglioni fermi fino
    al 2039. Dal 2022 gli scaglioni sono stati riformati tre volte;
  - un rendimento lordo di mercato del 5% su un portafoglio che include BTP indicizzati.
- Con una tassa del 38% e mercati al 3-4% il modulare è **in pareggio**.
- In più, i tassi Inarcassa dei prossimi due-tre anni incorporano ancora gli anni 2021-2023
  (media quinquennale del monte redditi). Lo scenario «coda Superbonus», al 6% e al 4%, è
  **prudente** [I].
- **Correzione:** scrivere «indifferente entro l'incertezza del modello; decide la preferenza per
  la rendita indicizzata e reversibile». Il piano «cassa» resta un default ragionevole.
  Semaforo **VERDE** confermato: art. 10, c. 1, lett. e), TUIR; RGP art. 4.2 [S sito Inarcassa;
  RGP letto da Q01].

### G-2. Q01 § 4: FDP senza i dividendi Overall e senza la holding coerente con Q03

- Q01 dimensiona il piano su un netto di 74.000 euro, **senza** dividendi.
- Q02, però, fa distribuire a FDP 8.808 euro nel 2026 e 18.808 ogni anno dal 2027. Q03 usa
  34.000 euro l'anno. L'eccedenza investibile di FDP sale quindi da ≈ 26.100 a **≈ 40.000 euro
  l'anno** (26.100 + 13.918).
- La riga «2028 Holding: solo per i dividendi Overall» contraddice Q03, che esclude la holding.
- **Correzione:**
  - togliere la riga sulla holding;
  - aggiungere i dividendi netti al portafoglio libero;
  - rinviare a un modello di cassa unico (G-7).

### G-3. Q02 § 2.5: buoni pasto a TP, da VERDE a GIALLO finché non si conosce la voce 0545

**Norma.**
- Art. 51, c. 2, lett. c), TUIR: 10 euro al giorno per i buoni elettronici dal 1/1/2026, con
  l'art. 1, c. 14, L. 199/2025 [S concordi: FISCOeTASSE, Commercialista Telematico, Edenred,
  Pluxee]. Il testo in Gazzetta non l'ho letto [N].
- Applicazione ai collaboratori tramite l'art. 52: ris. 118/E/2006 [N].

**Contestazione R1.**
- **Sovrapposizione con il vitto dei 17.800 euro di rimborsi.** Ogni giorno con buono pasto e
  vitto rimborsato è un doppio beneficio: il buono diventa imponibile.
- **Organo competente.** Lo statuto (art. 24) riserva ai **soci** l'emolumento dell'amministratore.
  Un benefit per il solo presidente deliberato dal CdA è compenso non deliberato dall'organo
  competente. Dal 2028 è indeducibile, perché manca la delibera dei soci; per l'IRPEF di TP non
  cambia nulla.
- **I tre dipendenti ricevono i buoni pasto?** La lett. c) non richiede la generalità. Ma un
  benefit riservato al vertice è il primo indizio che il verificatore usa per la natura
  retributiva e sostitutiva (R-1).

**Correzione.**
- Semaforo **GIALLO** fino alla ricostruzione della voce 0545.
- Nel dossier, sostituire «delibera del CdA» con **decisione dei soci**, con astensione di TP.
- Registro delle presenze incrociato con le note spese.
- **Il rischio si estingue** il 31/12/2032 per il 2026 e il 31/12/2033 per il 2027.

### G-4. Q02 § 2.4: fringe benefit fino a 2.000 euro, da tenere VERDE ma con il dossier giusto

**Norma.**
- Art. 1, c. 390, L. 207/2024, per il 2025-2027.
- Vale per gli assimilati: circ. 35/E/2022 e circ. 4/E/2025 [S GEPS, Edenred; N il testo delle
  circolari].

**Correzione.**
- Come in G-3: **decisione dei soci**, non delibera del CdA.
- Non va deliberato nello stesso atto che riduce il compenso (R-1).
- Resta aperto il [V] di Q02 sulla natura dei 1.995 euro del 2025.
- **Mantenimento:** figli a carico e soglia unica con ogni altro fringe.
- **Scadenza:** 31/12/2027, salvo proroga.

### G-5. Q02 § 2.7: rimborsi di 17.800 euro, GIALLO confermato; l'importo esposto è sottostimato

- Il calcolo di Q02 (9.500-10.000 euro l'anno) regge per l'IRPEF e la gestione separata.
- Mancano però **cinque annualità aperte**, dal 2021 al 2025. Il 2021 decade il 31/12/2027.
- L'esposizione massima è di **≈ 50.000 euro più sanzioni**.
- Le soglie penali non sono vicine: l'art. 10-*bis* D.Lgs. 74/2000 scatta a 150.000 euro di
  ritenute certificate non versate.
- **Correzione:** portare la verifica a campione dei giustificativi 2021-2025 (azione 2) al
  **primo posto** nel calendario, prima di ogni delibera nuova su TP. Le delibere del dicembre
  2026 non devono richiamare lo schema dei rimborsi finché la verifica non è chiusa.

### G-6. Coerenza fra i documenti: la holding di FDP e la distribuzione del 2026

| Punto | Q01 | Q02 | Q03 |
|---|---|---|---|
| Holding di FDP | sì, dal 2028, per i dividendi | «conferire prima delle distribuzioni, altrimenti 26% invece dell'1,2%» | **no** per la cassa; GIALLO solo per la successione, e in quel caso entro aprile 2027 |
| Distribuzione del 2026 | ignorata | 35.232 entro il 31/12/2026 | nessuna indicazione; nell'ipotesi successoria va fatta **dopo** il conferimento |

- Q03 ha ragione (E-8): l'1,2% sulle riserve è un differimento con uscita al 26%.
- **Correzione:**
  - Q01 e Q02 si allineano a Q03;
  - la distribuzione di 35.232 euro nel 2026 resta **VERDE**, senza vincoli di calendario, salvo
    che FDP dichiari prima del pagamento l'obiettivo successorio (Q03 § 8, punto 3).

### G-7. Politica dei dividendi: tre numeri incompatibili con la capacità di Overall e con il vincolo di TP

| Documento | Distribuzione annua di Overall | Dividendi lordi a TP |
|---|---:|---:|
| Q01 | 0 (non considerata) | — |
| Q02 | **75.232** | 18.808, il tetto del VERDE |
| Q03 § 2.2 (holding di FDP) | 136.000 (34.000 × 4) | 34.000 |
| Q03 § 2.4 (TP Holding, 250.000 in 8 anni) | **≈ 153.000** per 8 anni | 38.363 |

**Rilievo.**
- **Capacità.** L'utile netto atteso è di 130.000-190.000 euro (Q03). Una distribuzione di
  153.000 euro è un payout del **80-100%** per otto anni, con 225.600 euro di liquidità oggi e
  nessun autofinanziamento.
- **Vincolo di TP.** Con 38.363 euro di dividendi TP supera il minimale. Sotto la linea della
  Cassazione paga ≈ 4.800 euro l'anno di commercianti: il VERDE di Q02 § 2.2 decade negli anni
  del piano.
- **Altri soci.** Se Maggia o Dall'Oca sono soci lavoratori iscritti ai commercianti, un payout
  alto costa anche a loro il 24,48% sopra i 18.808 euro. Sarebbe un danno per soci che «non
  devono essere danneggiati». Il dato **non è nel fascicolo**.

**Correzione.**
- Un solo modello di cassa di Overall 2026-2039: utile, imposte (CPB fino al 2027), payout,
  liquidità minima, servizio del debito della TP Holding.
- Negli anni del piano della TP Holding, il VERDE della tranche di Q02 diventa «VERDE entro
  18.808 euro, costo dichiarato oltre».
- In alternativa, allungare il piano a 12-15 anni, oppure preferire il **recesso** finanziato
  dalle riserve (Q03 § 2.4), che non richiede alcuna distribuzione.

### G-8. Q03 § 2.4: TP Holding che compra le quote pagandole con i dividendi all'1,2%. GIALLO confermato, con condizioni da scrivere

**Norma.**
- Art. 10-*bis* L. 212/2000.
- Circ. AdE 6/E/2016 sulle operazioni di LBO [N il testo; contenuto noto]:
  - l'acquisizione a debito servita dai flussi della società acquisita è **fisiologica**;
  - è abusivo il ***leveraged cash-out***, in cui il venditore resta, direttamente o
    indirettamente, nella compagine dell'acquirente e monetizza le riserve a titolo di
    plusvalenza.
- Art. 2501-*bis* c.c. per la fusione successiva.
- Artt. 96 e 117 TUIR.

**Contestazione R1, con importo.** Se un venditore (Dall'Oca, Maggia, FDP):
- partecipa alla TP Holding, anche tramite familiari;
- oppure riceve un finanziamento o una garanzia dalla holding o da Overall;
- oppure la TP Holding si fonde con Overall entro pochi anni;

il verificatore riqualifica il prezzo come **distribuzione di riserve**. Il venditore sconta il
26% invece del 21% sulla rivalutazione: ≈ +12.400 euro su 250.000. Per la TP Holding, gli
interessi passivi della fusione sono indeducibili.

**Condizioni da aggiungere al dossier di Q03 § 6:**
1. Nessun venditore e nessun suo familiare nel capitale della TP Holding, né prima né dopo.
2. Prezzo pari alla perizia di rivalutazione del venditore, redatta da un perito diverso da quello
   dell'acquirente, oppure riconciliata con essa.
3. Dilazione del venditore a un tasso di mercato scritto nel contratto. Gli interessi sono reddito
   di capitale del venditore, al 26%.
4. Nessuna fusione fra la TP Holding e Overall.

**Il rischio si estingue** il 31/12 del quinto anno successivo alla dichiarazione dell'anno di
ciascuna cessione.

**Put a prezzo di formula nel patto parasociale.** Non è un patto leonino se è strumentale a un
assetto organizzativo della società (Cass. 17498/2018) [N il testo]. Nel patto va scritta questa
causa.

### G-9. Q03 § 2.2: l'ipotesi successoria (+87.000) è sovrastimata

- Il +87.000 presuppone che il 26% sui dividendi accumulati nella holding **non si paghi mai**.
- Lo *step-up* successorio (art. 68, c. 6, TUIR) protegge solo la **cessione** della quota della
  holding. Se gli eredi estraggono la cassa come dividendi o con la liquidazione (art. 47, c. 7)
  il 26% torna, e lo *step-up* sulla liquidazione è dubbio: Q03 lo marca già come [V].
- In più, anche il ramo «persona fisica» gode dello *step-up* sulle plusvalenze latenti degli ETF
  ereditati. Il modello invece le tassa ogni anno al 26%.
- **Correzione:** presentare il +87.000 come **tetto massimo**, «eredi che non estraggono mai
  cassa». Aggiungere lo scenario «eredi che liquidano», il cui vantaggio è vicino a zero o
  negativo per i costi. Semaforo GIALLO invariato.

### G-10. Q03 P-2 e P-3: CPB e compagine sociale. La conclusione è corretta, ma va chiusa su due punti

- **La risposta AdE 102/2025 è verificata [P]**: è sul sito AdE, e la fonte è coerente con
  Finanza & Fisco, Edotto e Metaping.
  - La modifica della compagine rileva solo per le società e associazioni dell'art. 5 TUIR.
  - La S.r.l. non cessa se il socio cede o conferisce le sue quote.
- **Un limite:** la risposta è del 15/04/2025, **anteriore al correttivo D.Lgs. 81/2025**. Non ho
  trovato notizia di modifiche alle cause di cessazione per le S.r.l. [V]. Va riletto l'art. 21
  D.Lgs. 13/2024 nel testo vigente prima di eseguire.
- La risposta segnala anche che il conferimento fra due società **entrambe** in CPB fa cessare
  entrambe: la TP Holding e la holding di FDP **non devono aderire** al CPB.
- **Il contesto comune** (`00-contesto-comune.md`: «niente aumento dei soci nel biennio») va
  corretto di conseguenza. Per una S.r.l. è falso.

### G-11. Q03 P-6: circ. 105/E/2001. Q03 ha ragione e V04 E-8 va corretto

- La circ. 105/E/2001 cita espressamente l'**ingegnere membro del CdA di una società di
  ingegneria o di una società edile** come caso di compenso attratto al lavoro autonomo [S
  concordi: AteneoWeb, Tutela Fiscale, Il Sole 24 Ore; N il testo della circolare].
- **Correzione:**
  - lo scenario B di Q03 va tenuto come base;
  - la riga in corsivo (gestione separata) diventa la sensibilità «se l'INPS non accetta la
    connessione»;
  - V04 E-8 va annotato come superato.
- La conclusione «resta in P.IVA» non cambia.

### G-12. Q03 § 4: l'ufficio di FDP locato a Overall. Manca il profilo del bene strumentale

- Se l'ufficio è oggi **strumentale all'attività professionale** di FDP (art. 54 TUIR, con i
  commi sulle plusvalenze degli immobili strumentali dal 2007), destinarlo in locazione a Overall
  può far emergere:
  - una **plusvalenza** o un **realizzo per destinazione a finalità estranee**;
  - oppure un canone da trattare come componente del reddito professionale.
- **Correzione:** [V] sul regime fiscale attuale dell'immobile (acquisto, ammortamenti dedotti,
  uso), prima di proporre la locazione.
- Resta inoltre valida l'osservazione di R-1: il costo per euro netto (1,26) è calcolato su
  Overall, ma per la coppia vale di più, perché il 50% del costo grava su Maggia e Dall'Oca. È un
  motivo in più per documentare **il bisogno reale e il canone di mercato**: sono loro i
  controinteressati.

### G-13. Etichette [A] su fonti secondarie

Diversi punti sono marcati [A] ma poggiano su fonti secondarie:
- Q03 P-1: rivalutazione al 21%, art. 1, c. 144, L. 199/2025. **Confermata** su più fonti [S]:
  IPSOA, We Wealth, Assolombarda, FISCOeTASSE.
- Q03 P-4: 60 mesi per la PEX sulle quote conferite, art. 177, c. 2-*quater*.
- Q03 P-5: vedi R-2.
- Q02: sentenze della Cassazione.

**Correzione:** usare [A-S], cioè «accertato su fonte secondaria», e riservare [A] al testo letto.
La L. 199/2025 in Gazzetta non è stata letta da nessuno dei tre analisti.

---

## Parte IV — Che cosa manca

1. **Un modello di cassa unico di Overall 2026-2039** (G-7). Senza, i tre documenti non si possono
   sommare.
2. **La posizione INPS di Maggia e Dall'Oca**: sono iscritti ai commercianti? Decide l'effetto di
   ogni politica di payout su di loro.
3. **La composizione della voce 0545** (G-3, G-5). Decide il semaforo dei buoni pasto, delle
   trasferte e dell'auto.
4. **Lo statuto vigente**: prelazione, gradimento, recesso. È presupposto del patto parasociale e
   del recesso.
5. **La famiglia di FDP**: decide l'ipotesi successoria (G-9) e la scelta fra piano «cassa» e
   piano «rendita» in Q01.
6. **Il regime dell'immobile-ufficio di FDP** (G-12).
7. **Il D.Lgs. 81/2025 sul CPB**: rilettura dell'art. 21 vigente (G-10).
8. **Le nuove prestazioni del fondo pensione**: la disciplina COVIP attuativa e il testo della
   L. 112/2026, art. 16-*ter*, sul capitale al 50% (E-2).
9. **La lettura primaria di almeno:**
   - L. 199/2025, cc. 14, 144 e 201;
   - D.L. 38/2026, art. 11, e L. 88/2026;
   - Cass. 25377/2026;
   - circ. 105/E/2001;
   - ris. 55/E/2020;
   - circ. 6/E/2016.

---

## Verifica normativa (sintesi)

| Affermazione | Esito | Fonte |
|---|---|---|
| Fondo pensione: tetto 5.300 dal 2026, art. 1, c. 201, L. 199/2025 | **Confermato**. La decorrenza dal 1/1/2026, e non dal 1/7/2026, è la lettura di Assogestioni (unità del periodo d'imposta); MySolution parla di «decorrenza incerta» | [S] Assogestioni, MySolution |
| Fondo pensione: capitale al 60% | **Superato: 50%** (L. 112/2026, art. 16-*ter*) | [P] Ministero del Lavoro |
| Erogazione frazionata al 15-9% | **Errato: 20%, fino al 15%** | [P] Ministero del Lavoro; [S] EC News |
| Modulare Inarcassa dall'1% all'8,5%, minimo 255, massimo 12.520 | **Confermato** | [S] money.it, FISCOeTASSE; [P] sito Inarcassa (via Q01) |
| Cass. 25377/2026 e collegate: base commercianti = utili imputati | **Confermato nel contenuto** | [S] Commercialista Telematico, Edotto, Informazione Fiscale; [N] il testo |
| Minimale 18.808, 4.611,64, 24,48% | **Confermato** | [P] circ. INPS 14 del 09/02/2026 (PDF INPS indicizzato); [S] Confesercenti |
| Buoni pasto elettronici a 10 euro, art. 1, c. 14, L. 199/2025 | **Confermato** | [S] più fonti |
| Fringe 2.000 agli assimilati | **Confermato** | [S] GEPS, Edenred |
| Risposta AdE 102/2025 | **Confermata** | [P] AdE; [S] Finanza & Fisco, Edotto |
| Rivalutazione al 21%, art. 1, c. 144, L. 199/2025 | **Confermata**; terreni al 18% | [S] IPSOA, We Wealth, Assolombarda |
| Soglia 5%/500.000 per l'art. 89 e la PEX | **Abrogata** dal 1/1/2026 (D.L. 38/2026, art. 11; L. 88/2026) | [S] più fonti |
| Circ. 105/E/2001: ingegnere amministratore di una società di ingegneria | **Lavoro autonomo** (Q03 corretto, V04 E-8 superato) | [S] più fonti |
| Principio di non sostituibilità dei benefit | **Applicabile** alla riduzione del compenso di Q02 C | [P/S] ris. 55/E/2020 |

**Fonti consultate:**
- [Ministero del Lavoro — previdenza complementare, novità dal 1° luglio 2026](https://www.lavoro.gov.it/notizie/pagine/previdenza-complementare-le-novita-della-legge-di-bilancio-2026-vigore-dal-primo-luglio-2026)
- [EC News — Legge di bilancio 2026 e previdenza complementare](https://www.ecnews.it/lavoro/prestazioni-assistenziali-e-previdenziali/pensioni/legge-bilancio-2026-novita-previdenza-complementare/)
- [Assogestioni — novità fiscali della previdenza complementare](https://www.assogestioni.it/articolo/previdenza-complementare-assogestioni-chiarisce-le-novita-fiscali)
- [MySolution — decorrenza incerta del nuovo limite](https://www.mysolution.it/fisco/informazioni/news/2026/05/06/novita-deducibilita-previdenza-complementare-con-decorrenza-incerta/)
- [Fiscomania — il D.L. 38/2026 ripristina la PEX](https://fiscomania.com/ripristinata-pex/)
- [Studio Romano Associati — il D.L. 38/2026 elimina retroattivamente la soglia](https://www.studioromanoassociati.com/post/dividendi-e-participation-exemption-il-dl-38-2026-elimina-retroattivamente-la-soglia-del-5-e-il-li)
- [GM Tax — L. 22/05/2026 n. 88, conversione del D.L. 38/2026](https://www.gm.tax/news/legge-22-maggio-2026-n-88-di-conversione-del-d-l-27-marzo-2026-n-38-recante-disposizioni-urgenti-in-materia-fiscale-ed-economica)
- [Finanza & Fisco — conversione del decreto fiscale](https://www.finanzaefisco.com/conversione-definitiva-per-il-decreto-fiscale/)
- [IPSOA — rivalutazione delle partecipazioni al 21%](https://www.ipsoa.it/documents/quotidiano/2026/01/03/rivalutazione-partecipazioni-imposta-sostitutiva-21)
- [FISCOeTASSE — rivalutazione delle partecipazioni al 21% e dei terreni al 18%](https://www.fiscoetasse.com/approfondimenti/16979-rivalutazione-partecipazioni-con-aliquota-al-21-e-terreni-al-18.html)
- [FISCOeTASSE — buoni pasto 2026](https://www.fiscoetasse.com/approfondimenti/17162-buoni-pasto-2026-natura-giuridica-regime-fiscale-e-novita.html)
- [Commercialista Telematico — Cass. 25377/2026](https://www.commercialistatelematico.com/articoli/2026/09/contributi-inps-soci-srl-utili-non-distribuiti.html)
- [Edotto — utili non distribuiti di S.r.l. esclusi dalla base INPS](https://www.edotto.com/articolo/utili-non-distribuiti-srl-la-cassazione-consolida-lesclusione-inps)
- [INPS — circ. 14 del 09/02/2026](https://www.inps.it/content/dam/inps-site/it/scorporati/circolari-e-messaggi/2026/02/Circolare_15162/Allegati/16561_Circolare-numero-14-del-09-02-2026.pdf)
- [GEPS — fringe benefit fino a 2.000 euro anche per gli amministratori](https://www.geps.it/fringe-benefit-esenti-sino-a-2-000-euro-anche-per-gli-amministratori-10838/)
- [AdE — risposta 102/2025](https://www.agenziaentrate.gov.it/portale/documents/20143/8902784/Risposta+n.+102_2025.pdf/032a23cc-b9ac-575a-24c1-3815c48ba922?t=1744708431002)
- [Finanza & Fisco — CPB e cessione delle quote di S.r.l.](https://www.finanzaefisco.com/no-cessazione-cpb-trasferimento-quote-srl/)
- [AteneoWeb — il reddito degli amministratori che esercitano anche una professione](https://www.ateneoweb.com/news/il-reddito-degli-amministratori-che-esercitano-anche-una-professione/)
- [AdE — ris. 55/E/2020](https://www.agenziaentrate.gov.it/portale/documents/20143/2665656/Risoluzione+n.+55+del+2020+Trattamento+fiscale+dei+benefit+offerti+a+categorie+di+dipendenti+nellambito+di+un+Piano+welfare+aziendale.pdf/84a47433-3820-47d4-6eb9-c410029d0b66)
- [money.it — Inarcassa 2026, aliquote e contributi](https://www.money.it/inarcassa-2026-aliquote-e-contributi-per-ingegneri-e-architetti)

**Limite della verifica.**
- Non ho letto in Gazzetta Ufficiale né la L. 199/2025, né il D.L. 38/2026, né la L. 88/2026,
  né la L. 112/2026. Non ho letto il testo integrale della Cassazione.
- Le abrogazioni in R-2 ed E-2 poggiano su fonti secondarie concordi e sul sito del Ministero del
  Lavoro. Vanno confermate sul testo prima della consegna.

---

## Riepilogo dei rilievi

| # | Semaforo | Dove | In una riga |
|---|---|---|---|
| R-1 | **ROSSO** | Q02 Sintesi e § 3 | Il pacchetto C costa alla coppia FDP+TP −1.188 nel 2027 e −1.838 l'anno dal 2028, e taglia il compenso *in sostituzione* di benefit (ris. 55/E/2020). Va raccomandato B; i benefit si aggiungono, non sostituiscono. |
| R-2 | **ROSSO** | Q03 P-5, § 2.2; Q01 § 4.2 | La soglia 5%/500.000 è stata abrogata dal 1/1/2026 (D.L. 38/2026, art. 11; L. 88/2026). La holding di FDP perde 20-31 mila, non 39-43 mila; il verdetto regge. |
| G-1 | GIALLO | Q01 § 3.2, § 4 | Modulare: «indifferente entro l'incertezza», non «−20%»; decide la preferenza per la rendita. Q01 prevale sulla nota `handoff`. |
| G-2 | GIALLO | Q01 § 4 | Mancano i dividendi Overall di FDP (+13.918 l'anno); va tolta la riga sulla holding del 2028. |
| G-3 | GIALLO | Q02 § 2.5 | Buoni pasto da VERDE a GIALLO: sovrapposizione con il vitto della voce 0545; decisione dei soci, non del CdA. |
| G-4 | GIALLO | Q02 § 2.4 | Fringe: decisione dei soci; mai nello stesso atto della riduzione del compenso. |
| G-5 | GIALLO | Q02 § 2.7 | Rimborsi: esposizione su cinque anni ≈ 50.000 più sanzioni; la verifica a campione va per prima. |
| G-6 | GIALLO | Q01, Q02 contro Q03 | Tesi opposte sulla holding di FDP: prevale Q03. La distribuzione del 2026 resta VERDE. |
| G-7 | GIALLO | Q02 contro Q03 | Payout 75.232 contro 153.000 l'anno: incompatibili fra loro, con il minimale di TP e forse con gli altri soci. Serve un modello di cassa unico. |
| G-8 | GIALLO | Q03 § 2.4 | TP Holding: GIALLO confermato con quattro condizioni anti-*cash-out* (circ. 6/E/2016); put con causa organizzativa. |
| G-9 | GIALLO | Q03 § 2.2 | Il +87.000 successorio è un tetto massimo; con eredi che liquidano il vantaggio è vicino a zero. |
| G-10 | GIALLO | Q03 P-2/P-3; contesto comune | Risposta 102/2025 confermata [P]. Da rileggere l'art. 21 dopo il D.Lgs. 81/2025; le holding non devono aderire al CPB; da correggere il contesto comune. |
| G-11 | GIALLO | Q03 P-6 | Circ. 105/E/2001: Q03 corretto, V04 E-8 superato. |
| G-12 | GIALLO | Q03 § 4 | Ufficio: manca il profilo dell'immobile strumentale (art. 54 TUIR). |
| G-13 | GIALLO | tutti | Etichette [A] su fonti secondarie: usare [A-S]. |
| E-1…E-8 | correzioni numeriche | Q01, Q02, Q03 | Vedi Parte I-A. |
