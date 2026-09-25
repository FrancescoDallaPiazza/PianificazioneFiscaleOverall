# Q01 — Piano previdenziale e impiego dell'eccedenza di Francesco Dalla Piazza

Analista: consulente previdenziale e attuario (casse professionali e D.Lgs. 252/2005).
Data: 25/09/2026. Base: `00-contesto-comune.md`, la nota dell'utente
`handoff_pensione_inarcassa.md` (31/08 e 01/09/2026) e V04 § G-1 (E-4…E-7).
Marcatura: [A] accertato su fonte · [I] inferito · [V] da verificare.
Modello di calcolo: `q01/m.py` e `q01/m2.py` nello scratchpad di sessione, con i controlli
`assert`. Non è nel repository.

---

## 0. Sintesi (5 righe)

1. **Fondo pensione: 5.300 € ogni anno dal 2026, VERDE.** È lo strumento dominante. Per ogni euro
   netto rende un TIR dell'8,7% nominale nello scenario centrale, contro il 3,1% di un PAC in ETF.
   Vince in tutti gli scenari. Va aperto e alimentato **entro il 31/12/2026**.
2. **Il modulare Inarcassa non è una leva fiscale.** Si deduce al 45% e la rendita si tassa di
   nuovo al 38-45%: resta un differimento. Rende il 2,2% nominale nello scenario centrale, contro
   il 3,1% del PAC. Conviene solo con una vita lunga (oltre 90 anni), mercati deboli o una
   marginale in pensione non superiore al 38%. È un'**assicurazione di longevità indicizzata**,
   non un investimento. La nota dell'utente del 01/09 lo metteva al secondo posto, ma con una
   marginale in uscita del 37%. Rettifico qui quella conclusione.
3. **Allocazione raccomandata a regime (2026-2038), piano "cassa":**
   - fondo pensione 5.300 lordi, esborso netto 2.913;
   - modulare **0**, oppure 1-4% se FDP vuole alzare il pavimento indicizzato (§ 4, piano "rendita");
   - il resto, circa **26.000 netti l'anno**, in un portafoglio libero personale: ETF globali più
     BTP indicizzati.
   Netto spendibile **71.087** (≥ 45.000). Con il modulare pieno scenderebbe a 64.503.
4. **La holding (dal 2028) serve ai dividendi Overall, non a questa eccedenza.** La liquidità
   personale versata in holding sconta l'IRES al 24% sui proventi finanziari, e poi il 26%
   quando esce: va tenuta in capo alla persona. L'**Allegato A** e il **riscatto della laurea**
   non battono il PAC, salvo che servano per il requisito dei 35 anni di anzianità [V estratto
   conto].
5. **Dopo il 2039:**
   - tenere aperto il fondo e **continuare a versare 5.300 l'anno**: si deducono al 38-45% e si
     riprendono al 15-13,5%, con un guadagno di circa 1.200-1.600 l'anno;
   - rinviare o frazionare i prelievi oltre il 2041, cioè oltre i 15 anni di partecipazione:
     l'aliquota scende di 0,30 punti l'anno.

---

## 1. Fonti verificate

| # | Punto | Esito | Fonte |
|---|---|---|---|
| 1 | **Tetto di deducibilità del fondo pensione** 5.300 € dal 01/01/2026 (prima 5.164,57); comprende contributi dell'aderente e del datore, TFR escluso | **[A]** | Art. 8, c. 4, D.Lgs. 252/2005 come modificato dall'art. 1, c. 201, L. 199/2025 ([GU](https://www.gazzettaufficiale.it/eli/id/2025/12/30/25G00212/SG)); [Mefop](https://www.mefop.it/blog/blog-mefop/deducibilita-extradeducibilita-post-legge-bilancio-2026); [FOPEN](https://www.fondofopen.it/blog/manovra-2026-fondo-pensione/). Circ. Assogestioni 15/2026 citata dall'utente: non letta [V] |
| 2 | **Extradeducibilità art. 8, c. 6** (recupero degli anni non dedotti): 2.650 €/anno in più, fino a 7.950, nei 20 anni successivi ai primi 5 di partecipazione | **Non applicabile a FDP** [I]: vale solo per chi ha avuto la **prima occupazione dopo il 01/01/2007**; FDP, nato nel 1971, lavora e contribuisce da prima (GS INPS ricongiunta e Inarcassa) | [Mefop](https://www.mefop.it/blog/blog-mefop/deducibilita-extradeducibilita-post-legge-bilancio-2026) |
| 3 | **Modulare Inarcassa**: aliquota dall'1% all'8,5% del reddito professionale netto IRPEF dell'anno precedente, **entro il massimale** (147.300 nel 2026); minimo 255 €, massimo assoluto 12.520 € (= 8,5% del massimale). Si versa entro il 31/12, anche in più volte e in anni non consecutivi; non compensabile con debiti contributivi | **[A]**. **Per FDP il massimo 2026 è 8,5% × 140.890 = 11.976 €** (V04 E-4) | RGP Inarcassa art. 4.2 e tab. B ([PDF](https://www.inarcassa.it/sites/default/files/legacy/documents/2024-12/Inarcassa_RGP.pdf)); [Inarcassa, versamenti facoltativi](https://www.inarcassa.it/articoli/versamenti-facoltativi) |
| 4 | **Deducibilità del modulare**: integrale, senza tetto | **[A]** | Art. 10, c. 1, lett. e), TUIR («versati facoltativamente alla gestione della forma pensionistica obbligatoria di appartenenza»); Inarcassa, pagina citata |
| 5 | **Il modulare va solo nel montante contributivo** (art. 26.3, lett. b). Il montante si rivaluta alla **media quinquennale del monte redditi** degli iscritti, **minimo 1,5%**, più un eventuale extra-rendimento deliberato ogni due anni dal CND (art. 26.6). La contribuzione dell'anno si rivaluta dall'anno successivo (art. 26.2) | **[A]** | RGP artt. 26.2, 26.3, 26.6 |
| 6 | **Tassi di capitalizzazione storici**: 1,5% nel 2016-2019; 1,6% nel 2020; 3,7% nel 2021; 2,5% nel 2022; **9,0% nel 2023; 12,3% nel 2024; 13,8% nel 2025** (effetto Superbonus) | **[A]**. Il monte redditi 2024 è cresciuto solo dell'1,3% e nel 2025 il fatturato è calato del 6,6%: la media quinquennale **scenderà** verso il minimo dell'1,5% entro il 2029-2030 [I] | [Inarcassa, tassi art. 26.6](https://www.inarcassa.it/articoli/tassi-annui-di-capitalizzazione-dei-montanti-contributivi-individuali-di-cui-allart-266-di); [Edilportale 09/2026](https://www.edilportale.com/news/2026/09/mercati/servizi-di-ingegneria-mercato-verso-15-miliardi-nel-2026_111996_13.html); [ANSA 29/04/2026](https://www.ansa.it/sito/notizie/economia/pmi/2026/04/29/inarcassa-172.916-ingegneri-e-architetti-iscritti-nel-2025-08_e350fc7e-61c2-41e1-8fc0-f6f6a945fd5b.html) |
| 7 | **Coefficiente di trasformazione**, tabella H(60), generazione 1960: 5,811% a 67 anni, 6,035% a 68 (a 67 anni e 6 mesi, interpolato: 5,923%). Le generazioni successive scendono di circa 0,02 punti per anno di nascita (6,001 → 5,811 fra le classi 1950 e 1960). **Per la classe 1971 a 67 anni e 6 mesi stimo il 5,7%** (intervallo 5,4-5,9%). La nota dell'utente usava il 5,3%, prudente. I coefficienti sono calcolati **senza componente di reversibilità**, ma la pensione **è reversibile** (art. 24) | **[A]** H(60); **[I]** la stima 1971 | [Inarcassa, tabella H(60)](https://www.inarcassa.it/articoli/coefficienti-di-trasformazione-il-calcolo-delle-prestazioni-contributive); RGP artt. 24, 26.1 |
| 8 | **Pensione Inarcassa indicizzata** al 100% dell'indice ISTAT FOI (art. 34.1). Contributo di solidarietà dell'1-2% solo sulla **quota retributiva** e solo se prorogato (art. 7) | **[A]** | RGP artt. 7 e 34 |
| 9 | **Tassazione della pensione Inarcassa**: reddito da pensione (art. 49, c. 2, lett. a, TUIR), IRPEF 23/33/43% (il 33% dall'art. 1, c. 3, L. 199/2025), detrazione dell'art. 13, c. 3, decrescente fino a zero a 50.000, più addizionali 2,03%. **Marginale effettiva sulla quota aggiuntiva:** 38,2% fra 44 e 49 mila (33% + 3,2% di perdita della detrazione + addizionali); **45,0% oltre 50 mila** | **[A]** norma; **[I]** calcolo | TUIR artt. 11, 13, 49 |
| 10 | **Fondo pensione, accumulo**: rendimenti tassati ogni anno al 20%, con i titoli pubblici al 12,5% | **[A]** | Art. 17 D.Lgs. 252/2005 (L. 190/2014, c. 621) |
| 11 | **Fondo pensione, uscita**: 15% sulla parte imponibile, cioè i contributi dedotti (i rendimenti sono già tassati), ridotto di 0,30 punti per ogni anno di partecipazione **oltre il 15°**, fino al 9%. **Per FDP: 15% se esce nel 2039** (13 anni, V04 E-7); **13,5% se preleva dal 2046** (20 anni); il 9% non è raggiungibile in pratica (35 anni) | **[A]** | Art. 11, c. 6, D.Lgs. 252/2005 |
| 12 | **Nuove prestazioni dal 01/07/2026**: rendita a durata definita, prelievi liberamente determinabili ed erogazione frazionata (almeno 5 anni; per un fondo la decorrenza è il 31/10/2026), **tassate come il capitale**. Capitale fino al **60%** secondo EC News; un fondo scrive ancora 50% | **[A]** le forme e la decorrenza; **[V]** 60% o 50%, irrilevante per FDP perché le forme flessibili gli danno comunque accesso a tutto il montante al 15% | Art. 1, c. 201, L. 199/2025; [EC News](https://www.ecnews.it/lavoro/news-del-giorno/legge-bilancio-2026-novita-tema-previdenza-complementare/); [Fondo Pensioni Banco Popolare](https://www.fondopensionibancopopolare.it/news/notizie/nuove-prestazioni-pensionistiche-ex-art-11-lgs-252-2005) |
| 13 | **Anticipazioni**: 75% in ogni momento per spese sanitarie gravi (15-9%); dopo 8 anni, 75% per la prima casa e 30% per ulteriori esigenze (23%). **RITA**: con cessazione dell'attività, a non più di 5 anni dall'età di vecchiaia e con 20 anni di contributi obbligatori, al 15-9%. **Riscatti**: il 50% o il 100% per inoccupazione o invalidità al 15-9%; per altre cause al 23% | **[A]** | Art. 11, cc. 4, 7; art. 14 D.Lgs. 252/2005 |
| 14 | **Morte prima della prestazione**: la posizione va ai beneficiari designati, altrimenti agli eredi, con tassazione al 15-9%. Non entra nell'asse ereditario, perché il beneficiario acquista *iure proprio* | **[A]** art. 14, c. 3; **[I]** esclusione dall'imposta di successione, prassi consolidata | Art. 14 D.Lgs. 252/2005 |
| 15 | **Prosecuzione dopo il pensionamento**: si può continuare a versare oltre l'età pensionabile, se a quella data si ha almeno 1 anno di contribuzione alla forma complementare | **[A]** norma; **[V]** statuto del fondo scelto | Art. 8, c. 11, D.Lgs. 252/2005 |
| 16 | **PAC in ETF**: 26% sulle plusvalenze realizzate (12,5% sulla quota di titoli pubblici), imposta di bollo 0,2% annua | **[A]** | Artt. 44 e 67 TUIR; D.L. 66/2014; art. 13, c. 2-*ter*, tariffa DPR 642/1972 |

---

## 2. Ipotesi del modello

- **Versamenti:** 13, a fine anno dal 2026 al 2038; pensione il 04/04/2039.
- **Deduzione:** al 45,03% (43% + 1,23% + 0,80%) [A]. Il reddito imponibile, circa 120.000 dopo
  il soggettivo obbligatorio, resta sopra i 50.000 anche con 17.276 di deduzioni.
- **Inflazione:** 2%. Sfasamento del rimborso IRPEF di circa 6 mesi ignorato: vale per tutti gli
  strumenti deducibili.
- **Rendimento lordo di mercato (comparto bilanciato-azionario o ETF):** 3% / **5%** / 7%.
  - Fondo pensione: ISC 0,70% (Amundi SecondaPensione o Allianz Insieme, dalla nota dell'utente)
    e 20% sul rendimento. Netto centrale 3,44%.
  - PAC: TER 0,20%, bollo 0,20%, 26% sulla plusvalenza al realizzo.
  - **Rettifica alla nota dell'utente:** il suo "5% netto" per il fondo pensione era in realtà
    un lordo. Il netto è circa 3,4%.
- **Inarcassa:**
  - rivalutazione **1,5% / 2,5% / 4%**, più uno scenario "coda Superbonus" (6% nel 2027, 4% nel
    2028, poi 2,5%);
  - coefficiente 5,4 / **5,7** / 5,9%;
  - rendita indicizzata al 2%;
  - morte a **80 / 86 / 92** anni. La speranza di vita a 67 anni è di circa 18 anni [I].
- **Tassazione della rendita modulare:** **45%** nello scenario centrale. La pensione B sale in
  nominale e gli scaglioni restano fermi (drenaggio fiscale), quindi la quota aggiuntiva cade
  sopra i 50.000. Sensibilità al 38%.
- **Misura di confronto:** TIR nominale sull'esborso **netto**, lungo tutto il ciclo. Per
  confrontare una rendita con un capitale uso il "capitale equivalente al 2039": la rendita
  netta attualizzata al rendimento netto che il PAC avrebbe in decumulo.

---

## 3. Scenari

### 3.1 Fondo pensione contro PAC, a parità di esborso netto (2.913 l'anno = 5.300 lordi)

| Rendimento lordo | FP montante 2039 | FP netto (imposta 15% su 68.900) | **TIR FP** | PAC netto 2039 | **TIR PAC** | FP / PAC |
|---|---:|---:|---:|---:|---:|---:|
| 3% | 78.462 | 68.127 | **7,2%** | 43.546 | 1,7% | +56% |
| **5%** | 88.006 | **77.671** | **8,7%** | 48.790 | 3,1% | **+59%** |
| 7% | 98.862 | 88.527 | **10,3%** | 54.952 | 4,6% | +61% |

Con l'uscita nel 2046 (13,5%) l'imposta scende di **1.034**. Nel frattempo il montante rende
come il PAC (3,4% contro 3,1% netto): il rinvio conviene, ma di poco. **Il fondo pensione
domina in tutti gli scenari.** Il motivo è l'arbitraggio: deduzione al 45%, uscita al 15% sui
soli contributi. **[A]** norma, **[I]** numeri.

### 3.2 Modulare Inarcassa: 11.976 lordi l'anno (esborso netto 6.583)

Montante al 2039: 170.500 (all'1,5%), **181.300** (al 2,5%), 199.100 (al 4%). Rendita lorda
iniziale: 9.700 / **10.335** / 11.350 l'anno, indicizzata. Netta al 45%: **5.684**.

| TIR nominale (coefficiente 5,7%) | morte a 80 | **morte a 86** | morte a 92 |
|---|---:|---:|---:|
| rivalutazione 1,5%, tassa 45% | -1,4% | 1,8% | 3,4% |
| **rivalutazione 2,5%, tassa 45%** | -0,9% | **2,2%** | 3,8% |
| rivalutazione 4%, tassa 45% | -0,2% | 2,8% | 4,3% |
| rivalutazione 2,5%, **tassa 38%** | 0,0% | 3,0% | 4,4% |
| coda Superbonus, poi 2,5% | — | 2,2% | — |

Coefficiente 5,4% o 5,9% (rivalutazione 2,5%, morte a 86): TIR 1,9% o 2,4%.

**Capitale equivalente al 2039 del modulare, contro il PAC con lo stesso esborso netto
(tassa 45%):**

| Mercato (PAC) | PAC netto 2039 | Modulare 1,5% (morte 80/86/92) | **Modulare 2,5%** | Modulare 4% |
|---|---:|---|---|---|
| 3% | 98.400 | 63.500 / 94.700 / 125.500 | 67.500 / **100.700** / 133.500 | 74.100 / 110.600 / 146.600 |
| **5%** | **110.200** | 58.100 / 82.700 / 104.800 | 61.800 / **88.000** / 111.400 | 67.900 / 96.600 / 122.400 |
| 7% | 124.200 | 53.500 / 73.000 / 88.800 | 56.900 / 77.600 / 94.500 | 62.400 / 85.200 / 103.700 |

**Break-even:** con morte a 86 anni e tassa al 45%, il modulare pareggia il PAC se Inarcassa
rivaluta del **4,8% l'anno** con mercati al 5%. Pareggia all'1,3% con mercati al 3%, all'8,2%
con mercati al 7%.

**Lettura.** Il modulare equivale a far crescere l'esborso netto al tasso Inarcassa senza
imposte, perché entrata e uscita sono tassate a un'aliquota simile, e poi a trasformarlo in una
rendita. Nello scenario centrale **perde circa 22.000** di capitale equivalente, il 20%, sul
piano pieno a 13 anni. **Vince** con mercati al 3% e vita lunga, oppure con una marginale in
pensione al 38%, dove è in pareggio. Rispetto a un portafoglio di BTP indicizzati (circa 1,5%
reale lordo, 12,5% di imposta, circa 3,1% nominale netto) il risultato è lo stesso: il modulare
non batte nemmeno l'alternativa senza rischio, salvo la longevità [I].

La nota del 01/09 ("il fondo pensione dà +47% di rendita") è **confermata nel verso**. La
conclusione "il modulare per le somme oltre il tetto" regge però solo con la marginale in uscita
al 37%. Con il drenaggio fiscale e la perdita della detrazione pensionati la marginale sale al
38-45%, e il vantaggio fiscale sparisce.

### 3.3 Allegato A della ricongiunzione (per completezza)

L'Allegato A costa 36 rate da 464,13, cioè 16.708,68, deducibili: netto circa **9.190**. Dà
**1.274,99 lordi l'anno** di pensione in più. La nota dell'utente calcolava 9.524 con il 43%.

| TIR nominale | morte a 80 | morte a 86 | morte a 92 |
|---|---:|---:|---:|
| tassa 40%, aumento fisso in moneta 2039 | 0,6% | 2,9% | 4,1% |
| tassa 45%, aumento **indicizzato** dal 2026 (ipotesi dell'utente) | 1,6% | 3,75% | 4,9% |

Questi numeri confermano il TIR reale di circa 2,2% indicato dall'utente. L'Allegato A **non
batte il PAC** e vale quanto il modulare. **Confermo l'Allegato B**, già scelto. Se la risposta a
Inarcassa è già partita, la scelta è chiusa [V]. Se non lo è, il termine è di 60 giorni dal
ricevimento.

### 3.4 Riscatto della laurea o di periodi Inarcassa (richiesta V04)

- **Fiscale:** l'onere è deducibile per intero, senza tetto (art. 10, c. 1, lett. e, TUIR) [A].
- **Economico:** per i periodi anteriori al 2013 l'onere si calcola con la riserva matematica
  (Regolamento riscatti e ricongiunzioni, richiamato dall'art. 26.1 RGP). Il rendimento atteso
  è quindi del tipo dell'Allegato A, con TIR reale intorno al 2% [I]. **Non conviene come
  impiego.**
- **Unica eccezione:** se al 2039 FDP non arriva ai **35 anni** di iscrizione e contribuzione
  (art. 20.1 e tab. I RGP). Senza i 35 anni anche la quota ante 2013 si calcola col contributivo
  (art. 20.2), e la perdita sarebbe molto più grande del costo del riscatto. **[V] prioritario:**
  anzianità utile al 2039 dall'estratto conto IOL, con la ricongiunzione B inclusa.

### 3.5 Flessibilità e liquidità (FDP ha 55 anni)

| | Fondo pensione | Modulare | Allegato A | PAC |
|---|---|---|---|---|
| Liquidità prima del 2039 | anticipazioni dal 2034: 30% per ulteriori esigenze e 75% per la casa (23%); sanità in ogni momento; RITA dal 2034 se cessa l'attività | **nessuna** | nessuna | **totale** |
| Forma all'uscita | capitale, prelievi, rendita a durata definita o vitalizia (15-13,5%) | solo rendita vitalizia | rendita | libera |
| Longevità e inflazione | no, salvo acquisto di rendita | **sì, indicizzata ISTAT** | sì | no |
| Rischio di mercato | sì | no (minimo 1,5% nominale) | no | sì |
| Rischio di controparte e normativo | basso (patrimonio separato) | Inarcassa può cambiare coefficienti ed extra-rendimento | idem | fiscale |
| Eredi | **beneficiari designati**, fuori successione | solo superstiti con reversibilità o indiretta (art. 24); **senza superstiti si perde** | idem | eredi |

---

## 4. Allocazione proposta

### 4.1 A regime, ogni anno dal 2026 al 2038 (valori 2026, netto disponibile ex ante circa 74.000)

| Voce | **Piano "cassa" (raccomandato)** | Piano "rendita" (alternativa) |
|---|---:|---:|
| Fondo pensione (lordo) | **5.300** | 5.300 |
| Modulare Inarcassa (lordo) | **0** | 11.976 (8,5%) |
| Imposte risparmiate | 2.387 | 7.779 |
| Esborso netto per la previdenza | 2.913 | 9.497 |
| **Netto spendibile** | **71.087** | 64.503 |
| Consumo | 45.000 | 45.000 |
| **Portafoglio libero personale** (ETF più BTP indicizzati) | **≈ 26.100** | ≈ 19.500 |
| Holding (dal 2028) | solo dividendi Overall | idem |

Soluzione intermedia: modulare al 4%, circa 5.640 lordi. Netto spendibile 67.988, portafoglio
libero 23.000. Aggiunge circa 4.860 lordi l'anno di rendita indicizzata, 2.680 netti.

**Proiezione al 2039, scenario centrale al 5%, valori nominali:**

| | Piano "cassa" | Modulare 4% | Piano "rendita" |
|---|---:|---:|---:|
| Fondo pensione netto | 77.700 | 77.700 | 77.700 |
| Portafoglio libero netto | **436.900** | 385.000 | 326.600 |
| Rendita modulare netta aggiuntiva | — | 2.675 | 5.684 |
| Pensione Inarcassa B netta (moneta 2026) | 31.518 | 31.518 | 31.518 (con la rendita modulare, netto complessivo 37.615) |

Il fabbisogno di 45.000 in moneta 2026 è coperto in tutti e tre i piani. La pensione netta B
(31.500) lascia un buco di circa 13.500 l'anno. Il capitale di circa 515.000 nominali, pari a
398.000 in moneta 2026, lo copre per oltre 25 anni anche con un rendimento reale zero [I].

**Perché raccomando il piano "cassa".** L'obiettivo dell'incarico è la cassa netta massima. Il
modulare costa circa il 20% di capitale equivalente nello scenario centrale. FDP ha già un
pavimento indicizzato robusto: la pensione B vale il 70% del fabbisogno. E non ha vincoli di
liquidità.

**Quando scegliere invece il piano "rendita" o quello intermedio:**
- FDP ha coniuge o figli a cui tiene la reversibilità, e non gli interessa lasciare capitale;
- vuole una protezione piena dal rischio di mercato e di longevità;
- prevede in pensione una marginale del 38%, cioè redditi IRPEF complessivi sotto i 50.000,
  senza affitti né compensi.

La scelta si può rivedere ogni anno: il modulare si versa anche in anni non consecutivi.

### 4.2 Calendario

| Anno | Azione |
|---|---|
| 2026 | Adesione al fondo pensione aperto (ottobre-novembre), comparto bilanciato-azionario. **5.300 entro il 31/12/2026.** Modulare 2026 solo se si sceglie il piano "rendita" o intermedio: entro il 31/12/2026, sul reddito 2025, al massimo 11.976 |
| 2027-2038 | 5.300 al fondo entro il 31/12. Modulare eventuale sul reddito dell'anno precedente, fino all'8,5% ed entro il massimale. Il resto nel portafoglio libero |
| 2028 | Holding: solo per i dividendi Overall (vedi L01 e V04 G-3). **Non** versarvi l'eccedenza personale: IRES 24% sui proventi finanziari, poi 26% in uscita, circa il 44% contro il 26% del PAC personale [I] |
| 2034 | Il fondo compie 8 anni: si aprono le anticipazioni del 30% e del 75%. RITA possibile se FDP cessa l'attività, a 5 anni dalla vecchiaia |
| 04/2039 | Pensione Inarcassa. Fondo pensione: **non liquidare tutto**. Prelevare solo ciò che serve e **continuare a versare 5.300 l'anno** finché c'è IRPEF capiente: guadagno di circa 1.590 l'anno al 45%, 1.220 al 38% |
| 2041 | 15 anni di partecipazione: da qui l'aliquota scende di 0,30 punti l'anno |
| 2046 | 20 anni di partecipazione: aliquota al 13,5% |

---

## 5. Interazioni

1. **Contributo integrativo e minimi.** Il modulare **non** incide sul contributo integrativo
   (4% sul volume d'affari, art. 5), né sui minimi, né sull'anzianità. Non entra nella quota
   retributiva. Aumenta solo il montante contributivo (art. 26.3, lett. b) [A]. Non riduce il
   soggettivo obbligatorio, che si calcola sul reddito professionale e non sull'imponibile IRPEF
   [A].
2. **Concordato preventivo biennale.** FDP non aderisce. Se aderisse, il modulare resterebbe
   calcolato sul reddito IRPEF effettivo dichiarato a Inarcassa (V03 R-1) [I].
3. **Holding.** Nessuna interferenza con la deduzione del fondo pensione. I dividendi dalla
   holding alla persona (26%) non entrano nell'IRPEF e non alzano la marginale sulla pensione.
   **Un compenso di amministratore della holding invece sì:** dopo il 2039 alzerebbe la
   marginale sulla pensione e sulla rendita modulare al 45% [I].
4. **Successione.**
   - Fondo pensione: designare **per nome** i beneficiari nel modulo di adesione. La posizione
     esce dall'asse ereditario ed è tassata al 15-9% [A/I].
   - Modulare e Allegato A: vanno solo ai superstiti aventi diritto (art. 24); senza superstiti
     il montante si perde.
   - PAC: entra nell'asse ereditario; con la franchigia di 1 milione per coniuge e figli
     l'imposta è in genere zero [I].
   - **[V]** Stato di famiglia di FDP, non indicato nel contesto.
5. **Rischio normativo.**
   - Inarcassa può rivedere coefficienti, extra-rendimento e contributo di solidarietà; il
     minimo dell'1,5% è regolamentare, non di legge.
   - Fondo pensione: l'aliquota di uscita del 15-9% è stabile dal 2005, e la L. 199/2025 ha
     migliorato il regime.
   - Il 26% sulle rendite finanziarie può salire.
   - Drenaggio fiscale sugli scaglioni al 2039: rafforza la conclusione contro il modulare.
6. **Tetto unico del fondo pensione.** I 5.300 comprendono anche i contributi versati per i
   familiari a carico. Un secondo fondo non raddoppia il tetto [A].

---

## 6. Semafori

| Raccomandazione | Semaforo | Valore annuo | Valore sull'orizzonte | Nota |
|---|---|---:|---|---|
| Fondo pensione 5.300 l'anno dal 2026 | **VERDE** | 2.387 di IRPEF (uscita al 15%: -795 l'anno differiti) | +28.900 netti al 2039 rispetto al PAC (77.700 contro 48.800) | Regime previsto dalla legge e usato per il suo scopo |
| Prosecuzione del fondo dopo il 2039, uscita frazionata oltre il 2041 | **VERDE** | 1.200-1.600 | circa 1.000 di minore imposta sullo stock al 2046 | [V] statuto del fondo |
| Modulare Inarcassa | **VERDE** fiscalmente; **economicamente facoltativo** | 7.779 di IRPEF oggi, riprese al 38-45% in rendita | -22.000 di capitale equivalente (centrale), +2.000 / +12.000 con mercati deboli o vita lunga | Scelta di profilo, non fiscale |
| Portafoglio libero personale | **VERDE** | — | 437.000 al 2039 (piano "cassa", al 5%) | — |
| Eccedenza personale versata in holding | **Sconsigliato** (economico, non di rischio) | — | — | Tassazione peggiore |
| Allegato A | **Sconsigliato** (economico) | — | TIR 2,4-3,75% | B già scelto |
| Riscatto laurea | **VERDE** fiscalmente; solo se serve per i 35 anni | — | — | [V] estratto conto |

Nessuna voce è GIALLA o ROSSA: sono tutti regimi espressamente previsti dalla legge o dal
regolamento della cassa. Il revisore R1 non ha profili di abuso da contestare. Il rischio è
solo documentale: la prova della data del versamento e la corretta indicazione nel quadro RP.

---

## 7. Punti [V] residui

1. **Anzianità contributiva al 2039** (estratto conto IOL, con la ricongiunzione B): decide sul
   riscatto della laurea. **Priorità alta.**
2. **Stato di famiglia di FDP** (coniuge, figli): decide fra il piano "cassa" e il piano
   "rendita", e i beneficiari del fondo.
3. **Coefficiente H per la classe 1971**: simulatore IOL. Stimato 5,7%; con 5,4-5,9% il TIR del
   modulare varia di ±0,3 punti, e la conclusione non cambia.
4. **Capitale al 50% o al 60%** dopo la L. 199/2025 (fonti discordi) e disciplina attuativa
   COVIP delle nuove forme. Irrilevante per la raccomandazione.
5. **Statuto e ISC del fondo scelto** (Amundi SecondaPensione o Allianz Insieme; per la
   convenzione BPER Classe C vale la verifica già aperta dall'utente). Prosecuzione dei
   versamenti dopo il pensionamento.
6. **Risposta sull'Allegato B già inviata** a Inarcassa? Se no, il termine è di 60 giorni.
7. Circ. Assogestioni 15/2026, non letta direttamente. Il tetto di 5.300 è comunque confermato
   da Mefop e dal testo di legge.
8. **Redditi IRPEF attesi dopo il 2039** (affitto dell'ufficio, compensi residui): fissano la
   marginale in uscita.

---

## 8. Dossier e scadenze

| Scadenza | Adempimento | Documento da conservare |
|---|---|---|
| **entro novembre 2026** | Adesione al fondo pensione aperto; designazione nominativa dei beneficiari; scelta del comparto | Modulo di adesione, Nota informativa, scheda ISC |
| **31/12/2026** | Bonifico di **5.300** al fondo (data valuta entro l'anno) | Contabile bancaria, estratto del fondo |
| 31/12/2026 (solo con il piano "rendita" o intermedio) | Modulare 2026 via IOL, fino a 11.976 (8,5% × 140.890) | Ricevuta pagoPA/MAV Inarcassa |
| giugno 2027 | Redditi PF 2027: modulare nel quadro **RP rigo 21**, fondo pensione nel **rigo RP27** (deducibilità ordinaria) [I] | Certificazione dei contributi del fondo, estratto Inarcassa |
| 31/12/2027 | Comunicare al fondo gli eventuali contributi non dedotti (nessuno se si resta a 5.300) | Copia della comunicazione |
| ogni anno, 31/12 | 5.300 al fondo; decidere il modulare sul reddito dell'anno precedente | come sopra |
| 2034 | Verificare RITA o anticipazioni, se servono | — |
| 04/2039 | Domanda di pensione Inarcassa. Fondo: prelievi frazionati e prosecuzione dei versamenti | — |

**Responsabile:** FDP, con la commercialista per il quadro RP. **Revisione:** ogni anno a
novembre, prima del versamento.
