# V02 — Verifica indipendente della diagnosi fiscale as-is (D01)

**Revisore:** R1 — Verificatore.
Ufficiale della Guardia di Finanza, esperienza al Nucleo di Polizia Economico-Finanziaria;
trascorsi in Agenzia delle Entrate. Chiave di lettura: *dove si rompe questo fascicolo in sede di
verifica? quale numero è sbagliato? quale conclusione non regge?*

**Data della verifica:** 9 settembre 2026
**Documento verificato:** `01-diagnosi/D01-diagnosi.md` (versione del 9 settembre 2026)

**Documenti esaminati (fonti primarie, cartella `dati/`):**

- `04534450236-VISUORD-20251110.pdf` — visura ordinaria del 10/11/2025
- `2023 (Bilancio)/04534450236-20231231 PDF.pdf` — bilancio XBRL 2023 (con comparativo 2022)
- `2024 (Bilancio)/04534450236-20241231.pdf` — bilancio XBRL 2024 (con comparativo 2023)
- `2025 (Bilancio)/BILANCIO CEE PDF.pdf` — bilancio XBRL 2025 (con comparativo 2024)
- verbali di assemblea 29/04/2024, 30/04/2025, 30/04/2026
- `2025 (Bilancio)/Visura evasione bilancio 2025.pdf` — deposito bilancio 2025 prot. 74681/2026 del 18/05/2026
- `2025 (Bilancio)/Executive_Summary_Bilancio_2025_Overall_Group.docx`
- `Atto.pdf` — atto costitutivo e statuto 15/01/2018
- `DALLA PIAZZA_RE 2025.pdf` e `DALLA PIAZZA_CP 2025.pdf` — quadri RE e CP, periodo d'imposta 2024
- `26-06.pdf`, `26-07.pdf`, `26-08.pdf` — cedolini e riepiloghi paghe giugno-agosto 2026
- `DALLA PIAZZA_VOLUME D'AFFARI.pdf` — **non leggibile** (font a codifica simbolica, testo non
  estraibile): vedi rilievo G-11
- `PRADELLA TAZIO.pdf` — **non leggibile** (pagine immagine senza livello testo)

**Documenti di metodo:** `00-setup/protocollo-verifica.md`, `99-verifiche/V01-verifica-setup.md`.

**Metodo.** Gli importi dei bilanci XBRL sono stati ricostruiti **per quadratura**, non per
posizione: l'estrazione testuale disallinea la colonna dei valori rispetto a quella delle voci, e
la corrispondenza è stata riassegnata verificando che ogni totale parziale e ogni totale generale
tornassero (attivo = passivo; A − B = differenza; somma delle sottovoci = totale di voce). Tutte
le quadrature sono riportate nella prima sezione. I riferimenti normativi sono stati riscontrati
su fonte primaria dove possibile; ciò che non ho potuto confermare è marcato **NON VERIFICATO**.

---

## ESITO COMPLESSIVO

**DA RIVEDERE.**

La ricostruzione contabile è, nella quasi totalità, **corretta**: ho riverificato per quadratura
ogni riga della serie storica 2022-2025 e dello stato patrimoniale 2025 e i numeri tornano. Regge
alla prova dei conti anche l'inferenza centrale — la società è quasi certamente in concordato — e
ho verificato che nessuna delle sette spiegazioni alternative (perdite pregresse, IRES premiale,
super-deduzione assunzioni, crediti d'imposta, ACE residua, fiscalità differita, variazioni
ordinarie) la sostituisce: **due di esse sono escluse in modo dimostrabile dai numeri del bilancio**
(G-7). Reggono anche le due quantificazioni principali, con una correzione: il beneficio 2025 è di
**17.300-18.900 euro** e non di 18-20.000 (E-6), e la quota di utile non tassata di 65-70.000 euro
è corretta ma si riferisce a due basi imponibili distinte che il documento tratta come una sola
(G-8). E la ricostruzione del reddito concordato (≈55.000) e del valore della produzione netta
(≈100.000) è **centrata**, sia pure per un ancoraggio che il documento non mostra (G-8).

Il documento non è però consegnabile per cinque ragioni, tutte concentrate nella parte che il
cliente userà per decidere:

1. **Il modello del § 4.3 — che il documento stesso definisce «la conclusione più importante della
   diagnosi» — è costruito su un denominatore incoerente, su un'aliquota IRAP superata e su
   un'affermazione normativa falsa.** Rifatti i conti con una metrica omogenea, *il dividendo batte
   la fattura anche FUORI dal CPB* per un socio nel terzo scaglione IRPEF, e *la fattura batte il
   dividendo DENTRO il CPB* quando anche il socio è in concordato — cioè esattamente nella
   configurazione che il documento ritiene più probabile e che il quadro CP di Dalla Piazza
   documenta. Le due conclusioni del § 4.3 sono entrambe rovesciate. Vedi R-1 e la sezione
   «Verifica del modello § 4.3».
2. **L'affermazione «i contributi previdenziali restano dovuti sul reddito effettivo» (§ 6, punto
   4) è contraria al testo dell'art. 19, comma 1, D.Lgs. 13/2024**, che dispone l'esatto
   contrario. Vedi R-2.
3. **Il documento ripete alla lettera un errore già rilevato e corretto in V01** (l'art. 105,
   c. 4, TUIR e la data certa del TFM: V01, rilievo G-3), e non recepisce almeno altre cinque
   prescrizioni della verifica precedente e del protocollo. Vedi R-3.
4. **Il § 6 raccomanda il rinnovo del concordato senza sapere su quale base si costruisce la
   proposta.** Per chi era in CPB 2024-2025 la proposta 2026-2027 è elaborata, con ogni
   probabilità, sul **reddito effettivo 2025** — cioè sull'anno migliore nella storia della
   società. Con quella base la società si impegnerebbe a pagare circa 36.800 euro l'anno contro i
   17.190 del 2025. La frase «il concordato premia esattamente questo profilo» è vera per il primo
   accesso e falsa per il rinnovo. Vedi R-4.
5. **L'argomento difensivo del § 5.1 sugli ingegneri è rovesciato dalla prassi che lo fonda.** La
   circolare AdE n. 105/E del 12 dicembre 2001 porta come esempio testuale proprio «l'ingegnere …
   membro del consiglio di amministrazione di una società di ingegneria o di una società che opera
   nel settore delle costruzioni», e applica il criterio della **connessione oggettiva**: per una
   società di consulenza tecnica su sicurezza, ambiente e marcatura CE quel criterio opera in
   pieno. Vedi R-5.

Aggiungo che il documento **non nomina mai l'IVA**, in una società iscritta all'Albo Nazionale
Gestori Ambientali per l'intermediazione di rifiuti e che ha nell'oggetto la formazione e
l'autotrasporto: è la stessa lacuna già contestata al setup in V01 (O-5), e qui pesa di più perché
ci sono i numeri.

**Una notazione sull'unico rilievo che non si può correggere scrivendo.** Alla data odierna il
D.Lgs. 19 giugno 2026 n. 117 (T.U. imposte sui redditi) e il D.Lgs. 5 agosto 2026 n. 141 (T.U.
adempimenti e accertamento) hanno **già abrogato**, con applicazione dal 1° gennaio 2027, sia il
TUIR sia gli articoli del D.Lgs. 13/2024 sul concordato. L'adesione del 2 novembre 2026 si
perfeziona sotto le norme citate in D01, ma i suoi effetti arrivano al periodo d'imposta 2027,
quando cessazione, decadenza e accertamento andranno letti in un testo con numerazione diversa.
Va introdotto il campo che V01 (G-13) aveva già prescritto e che D01 non porta.

---

## Parte I — Errori di fatto e di calcolo

### E-1. § 2, tabella — «Compensi amministratori 2024: n.d.». Il dato c'è: **45.652**

La nota in calce allo stato patrimoniale del bilancio 2024 (`04534450236-20241231.pdf`, pag. 3)
riporta testualmente: «Ammontare dei compensi… ad amministratori e sindaci — Amministratori —
Compensi **45.652**». Il documento lo dà per non disponibile pur avendo letto quel bilancio (da
lì trae i 43.882 del 2023, che si trovano nella stessa posizione del bilancio 2023).

*Scrivere «45.652» al posto di «n.d.» nella colonna 2024.* La serie completa è: 2023 = 43.882,
2024 = 45.652, 2025 = 47.893 — crescita regolare del 4,0% e del 4,9%. Il 2022 resta n.d. (il
bilancio 2023 espone la nota solo per l'esercizio corrente).

Non è un dettaglio: con la serie completa si vede che **i compensi di amministratore crescono del
9,1% in due anni mentre i ricavi crescono del 49,6%**, e che nel 2025 valgono il 38,8% dell'utile
ante imposte contro il 96,3% del 2024. È un dato che entra direttamente nel § 5.1 (congruità) e
nel § 4.3 (il terzo canale, che il documento non considera).

### E-2. § 2, stato patrimoniale — la voce «Utili portati a nuovo 144.006» non esiste. È **Altre riserve** (riserva straordinaria)

Ricostruzione per quadratura del passivo al 31/12/2025:

| Voce XBRL | 31/12/2025 | 31/12/2024 |
|---|---:|---:|
| I — Capitale | 10.000 | 10.000 |
| II — Riserva da soprapprezzo | 0 | 0 |
| III — Riserve di rivalutazione | 0 | 0 |
| IV — Riserva legale | 2.000 | 2.000 |
| V — Riserve statutarie | 0 | 0 |
| **VI — Altre riserve** | **144.006** | **113.103** |
| VIII — Utili (perdite) portati a nuovo | **0** | **0** |
| IX — Utile dell'esercizio | 106.107 | 30.905 |
| X — Riserva negativa azioni proprie | 0 | 0 |
| **Totale patrimonio netto** | **262.113** | **156.008** |
| **B — Fondi per rischi e oneri** | **0** | **0** |
| **C — Trattamento di fine rapporto** | **855** | **936** |
| D — Debiti (entro l'esercizio) | 57.023 | 44.455 |
| E — Ratei e risconti | 570 | 333 |
| **Totale passivo** | **320.561** | **201.732** |

Quadrature: 10.000 + 2.000 + 144.006 + 106.107 = **262.113** ✓ ; 262.113 + 0 + 855 + 57.023 + 570
= **320.561** ✓ ; per il 2024: 10.000 + 2.000 + 113.103 + 30.905 = **156.008** ✓ ; 156.008 + 936 +
44.455 + 333 = **201.732** ✓.

La riclassificazione è confermata dai verbali: tutti e tre deliberano «**a riserva
straordinaria**», mai «a nuovo». Lo conferma anche l'Executive Summary interno («in larga parte
composto da "Altre riserve" (144.006 euro)»).

*Effetto sulla conclusione:* nessuno — la riserva straordinaria è una riserva di utili,
disponibile e distribuibile, e i 210.113 restano corretti (vedi E-3). Ma è un errore di lettura
del bilancio in una tabella marcata **[A] accertato**, e il commercialista del cliente lo vede
alla prima riga.

### E-3. § 4.1 — i **210.113 euro di riserve disponibili sono corretti**

Verifica: 144.006 (riserva straordinaria post-approvazione 2025) + 66.107 (quota dell'utile 2025
destinata a riserva straordinaria dal verbale 30/04/2026) = **210.113** ✓.
Controprova patrimoniale: 262.113 − 40.000 di dividendi deliberati = 222.113 = 10.000 di capitale
+ 2.000 di riserva legale + **210.113** ✓.
La riserva legale è a 2.000 = 20% del capitale, cioè al limite dell'art. 2430 c.c.: nessun
ulteriore accantonamento obbligatorio, e i 2.000 sono effettivamente indisponibili. ✓

Corretti anche i derivati: 210.113 × 26% = **54.629** ✓ ; 210.113 − 54.629 = **155.484** ✓ ;
155.484 / 4 = **38.871** ✓.

L'aliquota del 26% è quella giusta e per una ragione che il documento non dice ma che vale la pena
mettere agli atti: **la società è costituita il 15/01/2018**, quindi non esiste alcuna riserva
formata con utili prodotti fino all'esercizio in corso al 31/12/2017, e non si pone alcun problema
di regime transitorio (art. 1, cc. 1005-1006, L. 205/2017). Tutte le riserve scontano il 26% a
titolo d'imposta ex art. 27, c. 1, DPR 600/1973. **Confermare esplicitamente questo passaggio nel
documento**: è l'unico caso in cui una società di famiglia non ha bisogno di stratificare le
riserve.

### E-4. § 3 — «30.793 euro di reddito professionale effettivo non hanno scontato l'IRPEF»: la cifra sottratta a imposizione è **28.962**

I dati del quadro CP di Dalla Piazza sono tutti **corretti** (li ho riscontrati uno per uno):
CP2 col. 1 = 89.149 ; CP2 col. 2 = 87.318 ; CP2 col. 3 = 1.831 ; CP2 col. 4 (aliquota) = 10 ;
CP2 col. 5 (imposta art. 20-bis) = 183 ; CP9 col. 1 e col. 3 = 87.318 ; CP10 col. 3 = 118.111 ;
CP10 col. 6 = 131.816. Corretto anche il quadro RE: RE2 = RE6 = 128.313 ; RE20 = 10.202
(1.314 + 2.560 + 229 + 1.998 + 4.101 = 10.202 ✓) ; RE21 = 128.313 − 10.202 = 118.111 ✓ ;
RE23 = RE25 = 87.318 ; RE26 = 25.663 = esattamente il 20% di 128.313 ✓.

L'errore è nella lettura. Il reddito **assoggettato a imposizione** è quello concordato: 89.149
(di cui 87.318 a IRPEF ordinaria e 1.831 a sostitutiva del 10%). Il reddito effettivo è 118.111.
La differenza **non tassata è 118.111 − 89.149 = 28.962**, non 30.793. I 30.793 si ottengono
sottraendo dall'effettivo il solo imponibile IRPEF (87.318), cioè trattando come non tassati anche
i 1.831 che la riga precedente della stessa tabella dichiara tassati al 10%. Il documento si
contraddice a due righe di distanza.

*Scrivere:* «28.962 euro di reddito professionale effettivo sono rimasti fuori da qualunque
imposizione; ulteriori 1.831 hanno scontato il 10% invece dell'aliquota marginale».

Il risparmio stimato in «13-14.000 euro» **regge comunque**: 28.962 × 45% (43% + addizionali
regionale Veneto e comunale Padova) = 13.033, più il differenziale sui 1.831 (824 − 183 = 641) =
**13.674**. Ma va detto che è un risparmio **di sola IRPEF**: il beneficio previdenziale (vedi R-2
e la sezione § 4.3) è un tema diverso e va sommato, non ignorato.

**Elemento che il documento aveva sotto gli occhi e non ha usato:** CP2 col. 4 riporta l'aliquota
**10**. Ai sensi dell'art. 20-bis D.Lgs. 13/2024 il 10% spetta ai soggetti con punteggio ISA pari
o superiore a 8. **Il quadro CP prova quindi che Dalla Piazza aveva ISA ≥ 8 per il 2023.** Il § 7,
voce 4, chiede i punteggi ISA «degli ultimi tre anni» come se fossero ignoti: per un socio su
quattro uno di essi è già agli atti, e ha effetto diretto sul costo dell'operazione 2026-2027.

### E-5. § 5.3 e § 4.1 — i «132 giorni» di crediti sono un massimo teorico. Il DSO effettivo è **circa 108 giorni**

Due errori sovrapposti, in un passaggio marcato **[A]**:

1. **I crediti verso clienti sono comprensivi di IVA, i ricavi no.** Il rapporto va costruito su
   basi omogenee: 152.349 / (421.299 × 1,22) × 365 = **108,2 giorni** (2024: 86.719 /
   (302.159 × 1,22) × 365 = **85,9 giorni**). Il calcolo del documento (152.349/421.299 × 365 =
   132,0 e 86.719/302.159 × 365 = 104,8) è aritmeticamente esatto ma metodologicamente sbagliato,
   e sovrastima di circa 24 giorni.
2. **La voce «Crediti» del bilancio micro non è «crediti verso clienti».** Lo schema dell'art.
   2435-*ter* non espone il dettaglio: in quei 152.349 stanno anche crediti tributari, verso
   istituti previdenziali e verso altri. Definirli «crediti verso clienti» e marcare
   l'affermazione **[A] accertato** non è sostenibile.

*Effetto sulla conclusione:* il trend resta reale e va segnalato (86 → 108 giorni, +26%), ma
l'affermazione del § 4.1 che «la distribuzione delle riserve accumulate è un problema di incasso
prima che di fiscalità» perde gran parte del suo fondamento. Vedi anche G-1.

### E-6. § 3 e § 4.3 — l'aliquota IRAP usata è sbagliata (**4,08%, non 3,9%**), e la forchetta «18-20.000» va rifatta in **17.300-18.900**

L'art. 2 della **L.R. Veneto 27 dicembre 2024 n. 32** (BUR n. 169 del 27/12/2024) ha disposto, «a
decorrere dal periodo d'imposta successivo a quello in corso al 31 dicembre 2024», una
maggiorazione dell'aliquota IRAP dello **0,18%** per i soggetti diversi da quelli dell'Allegato C
(per i quali la maggiorazione è dello 0,65%). **L'aliquota applicabile a Overall Group dal periodo
d'imposta 2025 è quindi il 4,08%**, non il 3,90% — salvo che il codice ATECO 74.99.21 rientri
nell'Allegato C, nel qual caso sarebbe il 4,55%: va verificato. Il prelievo societario marginale
combinato non è 27,9% ma **28,08%**.

Ho rifatto il conto per intero (dettaglio nella sezione «Verifica del modello § 4.3», punto 0):

- IRAP 2025 in regime ordinario: base 123.297 + 47.893 (compensi di amministratore indeducibili) =
  **171.190** → 4,08% = **6.985**
- IRES 2025 in regime ordinario: 123.297 − 1.954 (deduzione IRAP sul costo del lavoro imponibile)
  = 121.343 → 24% = **29.122**
- **Totale ordinario ≈ 36.107**, contro **17.190** iscritti → differenza **18.917**

Applicando al modello il fattore di calibrazione ricavato dal 2023 (anno in cui la società era
certamente in tassazione ordinaria e in cui l'aliquota IRAP era ancora il 3,90%: il modello dà
16.633 contro 15.903 effettivi, cioè sovrastima del 4,4%), la stima prudenziale scende a **circa
17.330**.

*Scrivere «17.300-18.900» al posto di «18-20.000», e correggere ovunque «IRAP 3,9%» in «IRAP 4,08%
— aliquota Veneto dal periodo d'imposta 2025, L.R. 32/2024».* Sul totale il documento non è
lontano, ma l'aliquota sbagliata si propaga in tutte le tabelle del § 4.3.

### E-7. § 2, stato patrimoniale — la riga «Fondi e TFR 855» va spaccata, e la spaccatura è la prova del § 5.2

Non è una voce unica. **Fondi per rischi e oneri = 0** (in tutti gli esercizi 2022-2025);
**TFR = 855** (2024: 936; 2023: 0; 2022: 2.876 fra fondi e TFR). Il TFR è quello dei lavoratori
subordinati ex art. 2120 c.c.

Il documento usa quel numero al § 5.2 per dire che «tre anni di accantonamenti da 3.500 non hanno
prodotto un fondo». **È vero, ed è molto più forte di così: il fondo non esiste affatto, vale
esattamente zero, e non è mai esistito in nessuno dei quattro esercizi.** Vedi G-3, dove il
rilievo va chiuso invece che lasciato aperto.

### E-8. § 2 — «Immobilizzazioni materiali per 13.788 (attrezzature e ufficio)» e «zero banche» non sono dati accertati

Il bilancio micro non espone né la composizione delle immobilizzazioni materiali né la
composizione dei debiti. «Attrezzature e ufficio» e «zero banche» sono inferenze — quest'ultima
plausibile (oneri finanziari pari a 0 nel 2024 e nel 2025, e pari a 1 euro nel 2022), ma inferenze.
Vanno marcate **[I]**, non **[A]**. Il documento marca **[A]** l'intera tabella.

### E-9. Cifre che ho verificato e che sono **corrette** — non intervenire

Le elenco perché il consulente sappia dove non deve toccare nulla. Tutti i valori seguenti sono
stati riverificati per quadratura sui tre bilanci XBRL:

| Voce | 2022 | 2023 | 2024 | 2025 |
|---|---:|---:|---:|---:|
| Ricavi (A1) | 263.128 ✓ | 281.589 ✓ | 302.159 ✓ | 421.299 ✓ |
| Valore della produzione | 267.641 ✓ | 285.252 ✓ | 302.988 ✓ | 422.114 ✓ |
| Costi per servizi (B7) | 184.304 ✓ | 158.582 ✓ | 176.141 ✓ | 203.509 ✓ |
| Godimento beni di terzi (B8) | 11.665 ✓ | 14.237 ✓ | 14.927 ✓ | 13.032 ✓ |
| Costo del personale (B9) | 43.902 ✓ | 42.751 ✓ | 49.432 ✓ | 65.422 ✓ |
| Totale costi della produzione | 256.814 ✓ | 230.301 ✓ | 255.540 ✓ | 298.817 ✓ |
| Risultato ante imposte | 10.826 ✓ | 54.951 ✓ | 47.448 ✓ | 123.297 ✓ |
| Imposte correnti | 2.579 ✓ | 15.903 ✓ | 16.543 ✓ | 17.190 ✓ |
| Utile netto | 8.247 ✓ | 39.048 ✓ | 30.905 ✓ | 106.107 ✓ |
| Tax rate | 23,8% ✓ | 28,9% ✓ | 34,9% ✓ | 13,9% ✓ |

Ho aggiunto per completezza le voci che il documento non riporta e che servono al § 3 e al § 4.3:
B6 materie prime 6.475 / 6.657 / 5.431 / 8.364 ; B10 ammortamenti 4.404 / 3.881 / 3.321 / 3.322 ;
B14 oneri diversi 6.064 / 4.193 / 6.288 / 5.168 ; **B9-d «trattamento di quiescenza e simili»
768 / 3.500 / 3.500 / 3.495** (il documento cita correttamente gli ultimi tre; il 2022 aggiunge
768 e porta il cumulato a **11.263**).

Sono inoltre corretti e riscontrati sulla visura e sull'atto:
data di costituzione 15/01/2018 ✓ ; capitale 10.000 i.v. ✓ ; REA VR-428451 ✓ ; sede Villafranca di
Verona fraz. Dossobuono, Via A. Volta 36 ✓ ; ATECO 74.99.21 «attività di consulenza in materia di
sicurezza e salute dei posti di lavoro» ✓ (ATECORI 2007 74.90.21) ; CdA di 4 membri nominati il
15/01/2018 a tempo indeterminato ✓ ; nessun sindaco né revisore ✓ ; quattro soci al 25% con
2.500 euro di quota ciascuno, interamente versati ✓ ; nomi, anni di nascita e domicili dei quattro
soci ✓ (Pradella 1985 Verona, Dalla Piazza 04/10/1971 Padova, Maggia 24/05/1964 Villafranca,
Dall'Oca 28/10/1960 Villafranca) ; tre dipendenti nel 2026 (Stelluti Erika, Vedova Martina, Carli
Anna assunta il **06/07/2026** — confermato dal termine per la scelta di destinazione del TFR
fissato al 05/09/2026) più Pradella co.co.co. con mansione «Pres. Consiglio Amministr.» ✓ ;
percentuali +39,4% ricavi, +16,9% costi, ROS 15,7% → 29,3%, PN/attivo 82%, B7/ricavi 48,3% e
58,3% ✓ ; destinazione degli utili 2023, 2024 e 2025 come da verbali ✓ ; delibera del 30/04/2026
con 40.000 di dividendi (10.000 per socio) da pagare entro il 30/06/2026 ✓.

**Nota su un documento incoerente presente nel fascicolo.** L'`Executive_Summary_Bilancio_2025`
espone utile 105.270, imposte 18.027, patrimonio netto 261.276 e debiti 57.860: sono i numeri di
una **bozza precedente** al bilancio poi depositato il 18/05/2026. **D01 usa correttamente i
numeri del bilancio depositato.** Segnalo però che l'Executive Summary è agli atti del CdA con
numeri diversi da quelli approvati e depositati: va ritirato o annotato, perché due documenti
societari con utili diversi per lo stesso esercizio sono, in sede di accesso, esattamente il tipo
di incoerenza da cui parte la ricostruzione.

---

## Parte II — Rilievi bloccanti (ROSSO)

### R-1. § 4.3 — il modello «costo per euro netto» usa due denominatori diversi nelle due colonne. Corretto l'errore, **entrambe le conclusioni si rovesciano**

Questo è il rilievo principale della verifica. Il § 4.3 è dichiarato dal documento stesso «la
conclusione più importante della diagnosi» ed è la base del § 6, punto 3, e del § 8, punto 3.

**Dov'è l'errore.** Nella colonna «fattura» il documento misura il costo **al netto dello scudo
fiscale** (72,1 euro di costo netto per 47 di netto al socio → 1,53). Nella colonna «dividendo» lo
misura **al lordo** (100 euro di utile ante imposte per 53,4 di netto → 1,87). Sono due metriche
diverse applicate alle due alternative dello stesso confronto: il risultato è predeterminato dalla
scelta del denominatore.

**Il secondo errore, che si somma al primo: l'aliquota IRAP.** Il documento usa il 3,9%; per il
Veneto, dal periodo d'imposta 2025, l'aliquota è il **4,08%** (E-6). Il prelievo societario
marginale combinato è quindi **28,08%**, non 27,9%.

**Il confronto corretto.** Partendo da un margine operativo dato M, l'alternativa è: (a) pagare
una fattura F al socio, oppure (b) non pagarla e distribuire l'utile netto che ne deriva. In
entrambi i casi la società trattiene lo stesso importo, 0,7192 × (M − F): la ricchezza che resta in
società è identica. Il confronto è quindi puro e riguarda solo quanto arriva al socio per ogni
euro di reddito ante imposte sacrificato. Con quella metrica, **fuori dal CPB e con marginale del
43% più addizionali, il dividendo batte già la fattura**: 53,22 contro 45,22.

I conti per esteso, con le soglie di inversione, sono nella sezione «Verifica del modello § 4.3».

**Le due conclusioni del documento vanno riscritte così:**

- «Fuori dal CPB **la fattura batte il dividendo**, perché è deducibile» → **falso** per un socio
  nel terzo scaglione IRPEF. Il valore corretto: fuori dal CPB la fattura conviene **solo se
  l'aliquota marginale complessiva del socio è inferiore a circa il 35,3%** (37,8% se si ignora il
  contributo integrativo Inarcassa del 4%, come fa il documento; 28,0% per un professionista in
  gestione separata). Con la struttura IRPEF vigente nel 2026 — 23% fino a 28.000, **33%** da
  28.000 a 50.000, 43% oltre, dopo la modifica dell'art. 1, c. 3, L. 199/2025, che D01 non recepisce
  — la soglia del 35,3% coincide quasi esattamente con il secondo scaglione più le addizionali:
  **sotto i 50.000 euro di reddito complessivo i due canali si equivalgono, sopra vince il
  dividendo.** Dalla Piazza dichiara 131.816 di reddito complessivo effettivo: per lui il dividendo
  vince già oggi, in regime ordinario. *(Unica eccezione, che il § 4.3 deve contenere: superato il
  massimale reddituale Inarcassa di 147.300 euro il contributo soggettivo non è più dovuto e i due
  canali tornano in parità anche al 45% di marginale. Dalla Piazza è 29.189 euro sotto quel
  massimale.)*
- «Sotto CPB … ogni euro fatturato dal socio alla società distrugge valore» → **vero solo se il
  socio NON è a sua volta in concordato**. Se lo è — ed è il caso documentato di Dalla Piazza nel
  2024, e sarà il caso di chiunque aderisca al 2026-2027 — il maggior compenso incassato **non
  rileva ai fini IRPEF né dei contributi obbligatori** (art. 19, c. 1, D.Lgs. 13/2024), e il costo
  per euro netto della fattura crolla a **1,04** (1,22 se il socio sceglie di versare comunque il
  contributo soggettivo) contro **1,35** del dividendo. **In quello scenario la fattura non
  distrugge valore: è il canale migliore, e con un margine del 23-30%.**

**Perché è ROSSO e non GIALLO.** Il documento non si limita a sbagliare un numero: costruisce su
quel numero una raccomandazione operativa («si comprime il canale fattura e si apre quello del
dividendo») e la ripete in chiusura come una delle «tre righe che contano». Applicata alla
configurazione reale — società in CPB *e* socio in CPB — quella raccomandazione **riduce** la
cassa netta ai soci, che è l'obiettivo dell'incarico. Aggiungo che il documento avverte
correttamente al § 4.3 che «la riduzione del canale fattura non può essere una scrittura
contabile»: consigliare di smettere di fatturare senza smettere di prestare, per poi scoprire che
la direzione era sbagliata, è il peggiore dei due mondi.

### R-2. § 6, punto 4 — «i contributi previdenziali restano dovuti sul reddito effettivo»: l'art. 19, c. 1, D.Lgs. 13/2024 dispone il contrario

Testo vigente, riscontrato sul testo pubblicato in Gazzetta Ufficiale (D.Lgs. 12 febbraio 2024
n. 13, art. 19, rubricato «Rilevanza delle basi imponibili concordate»), comma 1, **verbatim**:

> «Fermo restando quanto previsto agli articoli 15, 16 e 17 e al successivo comma 2, gli eventuali
> maggiori o minori redditi effettivi, o maggiori o minori valori della produzione netta effettivi,
> nel periodo di vigenza del concordato, **non rilevano ai fini della determinazione delle imposte
> sui redditi e dell'imposta regionale sulle attività produttive, nonché dei contributi
> previdenziali obbligatori**. Resta ferma la **possibilità** per il contribuente di versare i
> contributi sul reddito effettivo se di importo superiore a quello concordato come integrato ai
> sensi degli articoli 15 e 16.»

I contributi previdenziali obbligatori seguono quindi la **base concordata**; il versamento sul
reddito effettivo è una **facoltà** del contribuente, non un obbligo. L'affermazione del § 6,
punto 4, è falsa e va cancellata.

**Non è un dettaglio.** È il parametro che pesa di più nella tabella del § 4.3: 14,5 punti di
contributo soggettivo Inarcassa (26,07 in gestione separata) sul compenso del socio. Con il testo
corretto della norma, il costo per euro netto della fattura sotto CPB scende da 1,22 a **1,04**,
cioè il divario con il dividendo passa da +10% a +30% in favore della fattura. **L'errore
normativo del § 6 e l'errore metodologico del § 4.3 vanno nella stessa direzione e si sommano.**

**E c'è una simmetria che il documento deve conoscere: l'art. 35, c. 2, dello stesso decreto
dispone l'opposto per tutt'altro.** Quando le disposizioni vigenti fanno riferimento a requisiti
reddituali «per il riconoscimento della spettanza o per la determinazione di deduzioni, detrazioni
o benefici di qualsiasi titolo, **anche di natura non tributaria**», e ai fini **ISEE**, si tiene
conto del **reddito effettivo** e non di quello concordato. Contributi sul concordato, ISEE e
detrazioni sull'effettivo: è un'asimmetria che va spiegata ai soci prima e non dopo.

*Scrivere:* «i contributi previdenziali obbligatori sono commisurati al reddito concordato
(art. 19, c. 1, D.Lgs. 13/2024); il contribuente ha la facoltà, e non l'obbligo, di versarli sul
reddito effettivo se superiore. La scelta va fatta consapevolmente: rinunciarvi aumenta la cassa
di oggi e riduce il montante pensionistico».

### R-3. Il documento ripete un errore già rilevato in V01 e non recepisce almeno cinque prescrizioni della verifica precedente e del protocollo

**(a) L'art. 105, c. 4, TUIR — errore identico, parola per parola.** Il § 5.2 scrive: «la
deducibilità per competenza ex art. 105, c. 4, TUIR richiede che il diritto risulti da atto di data
certa anteriore all'inizio del rapporto». V01, rilievo G-3, aveva già contestato esattamente questa
formulazione: **l'art. 105, c. 4, non contiene nulla del genere**; il suo testo si limita a
estendere ai fondi per indennità di fine rapporto degli amministratori le disposizioni dei commi 1
e 2, con rinvio all'art. 17, c. 1, lett. c); il requisito della data certa è ricavato in via
interpretativa da quel rinvio. Un fascicolo in cui il revisore corregge una citazione e il
deliverable successivo la ripropone identica ha un problema di processo, non solo di contenuto.

Mancano inoltre, sempre da V01 G-3: che l'atto deve specificare anche **l'importo** o un criterio
oggettivo (Cass. nn. 26431/2018 e 17367/2020); che in mancanza di data certa **il costo non si
perde, si deduce per cassa** all'erogazione (Cass. n. 15966/2024) — il documento lo definisce
genericamente «un rilievo aperto», portando il cliente a sopravvalutare il danno; e che esiste una
**pronuncia contraria** (Cass., sez. V, ord. n. 3788/2023) più la norma di comportamento AIDC
n. 180/2011, cioè la linea difensiva.

**(b) Il transfer pricing interno.** Il § 5.4 chiude correttamente la porta dell'art. 110, c. 7,
TUIR (norma riservata alle operazioni con società non residenti; art. 5, c. 2, D.Lgs. 147/2015).
Ma V01, rilievo G-10, prescriveva di **aggiungere** il terreno su cui gli scostamenti fra parti
correlate residenti vengono effettivamente contestati: il **valore normale ex art. 9 TUIR**
(Cass. nn. 5858 e 5859 del 5 marzo 2024). Il documento chiude la porta sbagliata e lascia aperta
quella giusta, proprio nel capitolo in cui si discute di fatture fra soci e società.

**(c) L'IVA.** V01, O-5: «L'IVA non compare in nessuno dei dieci punti». **In D01 non compare
nemmeno una volta**, in 386 righe. Vedi G-4, G-5, G-11.

**(d) I due campi obbligatori sui VERDE e la data di scadenza dei GIALLO.** Il protocollo, nella
versione corretta dopo V01, impone che ogni VERDE porti «condizioni di mantenimento» e «data di
scadenza del vincolo» con il responsabile del monitoraggio, e che ogni GIALLO porti «la data in cui
smette di essere un rischio». Il documento spinge il CPB come leva principale **senza alcuna
tabella di condizioni di mantenimento e di decadenza** (artt. 10, 11, 21 e 22 D.Lgs. 13/2024) e
assegna due GIALLO (§ 5.1 e § 5.2) **senza data di scadenza del rischio**.

**(e) Le finestre con data certa.** Il protocollo prevede il «binario rapido» con l'elenco
aggiornato delle finestre aperte. Il § 6 ne tratta una sola (il CPB) e liquida l'assegnazione
agevolata. Manca la **rideterminazione del costo fiscale delle partecipazioni**, che V01 (O-1)
aveva segnalato con scadenza 30 novembre 2026 e aliquota al 21%: quattro soci con costo fiscale di
2.500 euro ciascuno in una società che genera oltre 120.000 euro di utile ante imposte hanno una
plusvalenza latente rilevante, e la finestra va valutata e *chiusa per iscritto* anche se la
conclusione è negativa (l'aliquota al 21% la rende probabilmente antieconomica: va detto, non
taciuto). *Termine e aliquota da riverificare sul testo di legge: vedi «Verifica delle fonti».*

**(f) Il campo sulla vigenza delle norme al 1° gennaio 2027.** V01, rilievo G-13, prescriveva di
«introdurre in ogni deliverable un campo "norma vigente alla data del …, da riverificare al 1°
gennaio 2027 per effetto del D.Lgs. 141/2026"». D01 non lo porta, e nel frattempo il problema si è
allargato: oltre al **D.Lgs. 5 agosto 2026 n. 141** (T.U. adempimenti e accertamento, che abroga
gran parte del DPR 600/1973 **e gli articoli del D.Lgs. 13/2024 sul concordato**), è stato
pubblicato il **D.Lgs. 19 giugno 2026 n. 117** (T.U. imposte sui redditi, G.U. n. 152 del 3 luglio
2026), che **abroga il DPR 917/1986** con applicazione dal 1° gennaio 2027 e rinumerazione
integrale. In D01 le citazioni TUIR sono corrette **fino al 31 dicembre 2026**; per il periodo
d'imposta 2027 — cioè il secondo anno del concordato che si sta per sottoscrivere — saranno
formalmente disallineate. Dettaglio nella sezione «Verifica normativa».

### R-4. § 6 — «Il concordato premia esattamente questo profilo». Nel **rinnovo** è falso: la proposta 2026-2027 si costruisce sul **reddito effettivo 2025**, cioè sull'anno migliore nella storia della società

Questo rilievo, per conseguenze economiche, è più grave del R-1.

Il § 6 costruisce la raccomandazione su due argomenti: che il CPB «fissa l'imponibile su base
storica mentre il reddito effettivo corre» (punto 2) e che vale già oggi 18-20.000 euro (punto 1).
Il secondo è vero per il biennio scaduto. **Il primo è falso per il rinnovo**, ed è il rinnovo
l'oggetto della decisione del 2 novembre.

**Il dato normativo.** Per chi ha già aderito al biennio 2024-2025, la proposta 2026-2027 è
elaborata sul dato del **rigo P04** del modello CPB, che le istruzioni dell'Agenzia definiscono
come il reddito d'impresa determinato «con riferimento all'articolo 56 del TUIR e, per i soggetti
IRES, alle disposizioni della Sezione I del Capo II del Titolo II del TUIR», cioè secondo le
**ordinarie regole di determinazione del reddito**: il reddito **effettivo**, non quello
concordato. La circolare AdE n. 18/E del 2024 lo dice espressamente per il caso di rinnovo dopo il
primo biennio, richiamando il «reddito effettivo d'impresa relativo al periodo d'imposta 2025 (non
quello concordato)». La metodologia è stata approvata con **D.M. MEF 11 maggio 2026** (G.U. Serie
Generale n. 115 del 20 maggio 2026, S.O. n. 20) e non introduce modifiche al percorso di calcolo
rispetto alle annualità precedenti; la rivalutazione avviene sul **PIL nominale** (+2,7% per il
2026, +2,5% per il 2027).

**Che cosa significa per Overall Group.** Il reddito effettivo 2025 ricostruito è di circa
**121.400 euro** (imponibile IRES) e circa **171.200 euro** (valore della produzione netta IRAP).
Applicando la sola rivalutazione:

| | 2026 | 2027 |
|---|---:|---:|
| Reddito concordato stimato (IRES) | ≈ 124.700 | ≈ 127.800 |
| Valore della produzione netta concordato stimato | ≈ 175.800 | ≈ 180.200 |
| **Imposta annua che la società si impegnerebbe a pagare** | **≈ 36.800** | **≈ 37.700** |

Contro **17.190 euro pagati nel 2025**. La società, aderendo, si impegnerebbe a pagare **più del
doppio** — e a pagarlo **anche se il 2026 tornasse ai livelli del 2024**, quando l'utile ante
imposte era 47.448 e l'imposta ordinaria sarebbe stata di circa 14.600. In quello scenario il CPB
costerebbe **oltre 22.000 euro l'anno di imposte non dovute**.

**Il punto di pareggio è che il 2026 e il 2027 battano il 2025.** E il documento più recente agli
atti della società — l'Executive Summary predisposto per il CdA sul bilancio 2025 — afferma
testualmente: «L'incremento dell'utile del 240% è **straordinario e non si replica per inerzia**».
D01 non cita quel documento e non pone la domanda.

**Effetto sul § 4.3.** Se il concordato 2026 è ancorato al 2025, la **capienza** dello scenario C
(il canale fattura tax-free sull'eccedenza) si riduce alla differenza fra reddito effettivo 2026 e
≈124.700: potrebbe essere prossima a zero, o negativa. Il vantaggio di 1,04 per euro netto esiste
solo sull'eccedenza, e l'eccedenza va stimata prima, non dopo.

*Il § 6 va riscritto per intero.* La conclusione «Perché per Overall Group questa è la decisione
dell'anno» resta valida — ma la decisione può benissimo essere **di non aderire**, e il documento
non presenta quel ramo dell'alternativa. Ciò che serve per decidere non è la proposta CPB
contrapposta al passato: è la **proiezione 2026-2027 costruita sui dati gestionali del 2026 in
corso** (§ 7, voce 3), confrontata con la proposta. D01 lo dice in una riga (§ 6, punto 4) e poi
scrive nelle conclusioni che il CPB «è già la leva che vale di più» e che «l'obiettivo dell'incarico
e questa scadenza sono lo stesso problema». Le due cose non stanno insieme.

**LA DOMANDA DA 38.000 EURO, che nessuno dei due documenti pone.** L'art. 9, c. 3-*bis*, D.Lgs.
13/2024 stabilisce che «la proposta di reddito concordato … **non può eccedere il corrispondente
reddito dichiarato nel periodo d'imposta antecedente** a quelli cui si riferisce la proposta,
rettificato secondo quanto disposto dagli articoli 15 e 16», di una misura graduata sul punteggio
ISA: **10%** se ISA = 10; **15%** se ISA ≥ 9 e < 10; **25%** se ISA ≥ 8 e < 9; **30%** se ISA ≥ 6 e
< 8; **35%** se ISA ≥ 1 e < 6 (le ultime due lettere introdotte dall'art. 7-*bis*, c. 1, del D.L.
38/2026: sono i «tetti agli incrementi» che D01 cita correttamente al § 6). Il limite si disapplica
verso il basso quando la proposta risulti già inferiore ai valori di riferimento settoriali (art.
9, c. 3-*ter*) e si applica anche alla proposta IRAP (c. 3-*quater*).

Per un soggetto che era in concordato nel 2025, «**reddito dichiarato**» può significare due cose,
e la differenza vale l'intera operazione:

| Se «reddito dichiarato 2025» significa… | Proposta 2026 (cap con ISA ≥ 8) | Imposta annua concordata | Confronto con il 2025 |
|---|---:|---:|---:|
| il reddito **effettivo** (≈ 121.400) | fino a ≈ 151.800; proposta stimata ≈ 124.700 | **≈ 36.800** | più del doppio |
| il reddito **concordato** (≈ 55.000) | non oltre ≈ 68.750 | **≈ 19.700** | in linea |

**NON VERIFICATO, ed è il punto su cui l'intera raccomandazione si decide.** Gli elementi
disponibili puntano verso il reddito **effettivo**: il rigo P04 del modello CPB, che è l'input
della metodologia, è definito dalle istruzioni dell'Agenzia come il reddito determinato «con
riferimento all'articolo 56 del TUIR» e, per i soggetti IRES, alle disposizioni ordinarie del Capo
II del Titolo II; e la circolare 18/E del 2024, trattando il rinnovo, parla di «reddito effettivo
d'impresa relativo al periodo d'imposta 2025 (**non quello concordato**)». Ma il D.M. 11 maggio
2026 e la sua Nota tecnica usano la formula ambigua «reddito **dichiarato** per il periodo
d'imposta in corso al 31 dicembre 2025», e l'art. 20-*bis*, c. 2, quando vuole dire «effettivo» lo
scrive («il reddito **effettivo** dichiarato nel periodo d'imposta antecedente») mentre l'art. 9,
c. 3-*bis*, non lo scrive. **Non risulta alcuna circolare o FAQ dell'Agenzia del 2026 dedicata al
punto**: l'ultima prassi in materia elencata dal portale è la circolare n. 9/E del 24 giugno 2025.

*Questa domanda va messa in cima al § 7, prima di ogni altra voce.* Si chiude in un modo solo:
facendo elaborare la proposta dal software dichiarativo (voce 2 del § 7) **e leggendo il numero**.
Finché non c'è quel numero, il § 6 non può concludere né a favore né contro l'adesione.

**Conseguenza collegata: l'imposta sostitutiva sull'incremento.** L'art. 20-*bis*, c. 1, consente
di assoggettare a imposta sostitutiva la parte di reddito concordato eccedente il dichiarato
rettificato, con aliquota del **10%** (ISA ≥ 8), **12%** (ISA ≥ 6 e < 8) o **15%** (ISA < 6). Il
comma 1-*bis*, introdotto dal D.Lgs. 81/2025 e applicabile **dalle adesioni al biennio 2025-2026**,
limita però le aliquote agevolate a un'eccedenza **non superiore a 85.000 euro**: oltre quella
soglia si applicano l'IRPEF al 43% o l'**IRES al 24%**. Nel primo scenario della tabella
l'incremento è quasi nullo e la sostitutiva è irrilevante; nel secondo vale circa 13.750 euro
tassati al 10% invece che al 24%, cioè **1.925 euro di risparmio annuo aggiuntivo**. Anche questo
dipende dalla risposta alla domanda di cui sopra. **D01 non nomina né l'art. 20-*bis* né il tetto
di 85.000 euro**, pur avendo agli atti un quadro CP che ne è un'applicazione.

**Un beneficio del rinnovo che D01 non conosce e che gioca in senso favorevole.** L'art. 14, c.
1-*bis*, D.Lgs. 13/2024 potenzia i benefici premiali per chi **rinnova**: esonero dal visto di
conformità per compensazioni fino a 100.000 euro annui per l'IVA e 70.000 per le imposte dirette
(contro 70.000 e 50.000 del regime base), rimborsi IVA senza visto né garanzia fino a 100.000 euro,
e **anticipazione di due anni** — non di uno — dei termini di decadenza per l'accertamento sul
reddito d'impresa e di lavoro autonomo. Il c. 1-*ter* aggiunge che, per il rinnovo relativo al
biennio 2026-2027, **sui versamenti rateali non sono dovuti interessi**; e l'art. 20, c. 3-*bis*,
esclude in caso di rinnovo la maggiorazione d'acconto del primo anno. Sono benefici reali e vanno
messi sul piatto insieme al costo.

**Una leva compensativa che D01 non vede.** L'art. 7, c. 3-*bis*, del D.L. 38/2026 ha inserito
nell'art. 16 D.Lgs. 13/2024 la lett. b-*ter*), che include fra le variazioni rilevanti «la
maggiorazione delle quote di ammortamento e dei canoni di locazione finanziaria spettanti ai sensi
dell'articolo 1, commi da 427 a 436, della legge 30 dicembre 2025, n. 199»: **l'iperammortamento
resta quindi deducibile anche in costanza di concordato**, come variazione in diminuzione del
reddito concordato. È l'unico modo per abbassare un concordato già accettato, e per una società
con 150.925 euro di liquidità e zero investimenti immateriali è una leva concreta. **Attenzione:
la modifica è stata inserita solo nell'art. 16 (reddito d'impresa) e non nell'art. 15 (lavoro
autonomo)**, quindi non vale per i soci professionisti.

---

### R-5. § 5.1 — l'argomento «per gli ingegneri l'incarico di amministratore non rientra nell'oggetto della professione» **non vale per questa società**, e la prassi che lo fonda porta l'esempio contrario

D01 presenta come «elemento favorevole [I]» il fatto che «per gli ingegneri l'incarico di
amministratore **non** rientra nell'oggetto della professione, quindi la separazione tra i due
redditi è corretta in partenza. Per i commercialisti sarebbe il contrario». La verifica sulla
prassi rovescia l'affermazione proprio nel caso di Overall Group.

**La norma.** Art. 50, c. 1, lett. c-*bis*), TUIR, nel testo vigente: sono assimilate al lavoro
dipendente le somme percepite «in relazione agli uffici di amministratore, sindaco o revisore …
**sempreché gli uffici o le collaborazioni non rientrino nei compiti istituzionali compresi
nell'attività di lavoro dipendente** … **o nell'oggetto dell'arte o professione** … esercitate dal
contribuente». *(Il testo conserva i rinvii alla vecchia numerazione — artt. 46 e 49 anziché 49 e
53: chi cita «art. 53» come se fosse nel testo si qualifica.)*

**La prassi. Il documento pertinente è la circolare dell'Agenzia delle Entrate n. 105/E del 12
dicembre 2001**, che ha espressamente superato la precedente n. 67/E del 6 luglio 2001 («devono
intendersi superate le interpretazioni fornite da questa Agenzia con le precedenti circolari»). La
105/E fissa **due criteri alternativi**, e D01 ne conosce solo il primo:

> «Qualora gli **ordinamenti professionali** ricomprendano espressamente nel novero delle mansioni
> tipiche … l'amministrazione o la gestione di aziende, appare ragionevole ritenere che i compensi
> … vadano ricondotti nella disciplina applicabile ai redditi di lavoro autonomo. L'attrazione …
> opera, inoltre, nella diversa ipotesi in cui, **anche in assenza di una previsione espressa** …,
> il professionista svolga l'incarico di amministratore di una società o di un ente che esercita
> una attività **oggettivamente connessa** alle mansioni tipiche della propria professione abituale
> … **È il caso ad esempio dell'ingegnere edile che sia membro del consiglio di amministrazione di
> una società di ingegneria o di una società che opera nel settore delle costruzioni.**»

**L'esempio testuale dell'Agenzia è l'ingegnere.** E Overall Group è una società che esercita
consulenza tecnica su sicurezza sul lavoro, ambiente, antincendio, direttiva macchine e marcatura
CE: un'attività **oggettivamente connessa** alle mansioni tipiche dell'ingegnere, come definite
dagli artt. 51 e 52 del R.D. 2537/1925 («il progetto, la condotta e la stima dei lavori … alle
macchine ed agli impianti industriali, nonché in generale alle applicazioni della fisica»). Il
criterio della connessione oggettiva **si applica in pieno**.

*(Per completezza: il riferimento per i commercialisti non è l'art. 1, c. 3, lett. c), ma l'**art.
1, comma 2, lettera a), del D.Lgs. 139/2005**, che include fra gli oggetti della professione
«l'amministrazione e la liquidazione di aziende, di patrimoni e di singoli beni».)*

**Le tre conseguenze, tutte contrarie a quanto scrive D01:**

1. **Lo scudo non c'è.** L'affermazione «la separazione tra i due redditi è corretta in partenza»
   va cancellata. Per gli amministratori-ingegneri di questa società i compensi di amministratore
   sono, secondo la prassi, **attratti al reddito di lavoro autonomo**. Il che significa che il
   compenso di amministratore e la fattura tecnica appartengono alla **stessa categoria reddituale
   e alla stessa causa** — cioè che la distinzione che il § 5.1 vuole difendere è, sul piano
   fiscale, molto più debole di quanto il documento lascia intendere.
2. **L'inquadramento di Pradella va verificato in senso opposto.** Se anche Pradella è ingegnere o
   professionista con attività connessa, il cedolino co.co.co. **non** è l'inquadramento corretto:
   i suoi compensi dovrebbero essere reddito di lavoro autonomo con fattura, IVA e cassa
   professionale. D01 tratta l'asimmetria come un dato di fatto da spiegare; è invece una
   questione di qualificazione da risolvere, e la soluzione dipende da un dato — le qualifiche
   professionali dei quattro — che **non è agli atti per tre di essi su quattro** (l'unico
   documentato è Dalla Piazza, dal domicilio digitale `francesco.dallapiazza@ingpec.eu`, dominio
   PEC dell'Ordine degli Ingegneri).
3. **Il codice attività dichiarato da Dalla Piazza spinge nella stessa direzione, e D01 lo riporta
   senza accorgersene.** Il rigo RE1 espone il codice **702002**, che D01 stesso descrive come
   «consulenza gestionale». Un professionista che dichiara al fisco un codice della famiglia della
   **consulenza imprenditoriale e amministrativo-gestionale** — non un codice degli studi di
   ingegneria — è, davanti a un verificatore, il primo a non poter sostenere che l'amministrazione
   di una società sia estranea al suo oggetto professionale.

**Effetto sull'impostazione del § 5.1.** L'argomento va sostituito, non corretto. La difesa reale
non è la separazione delle categorie reddituali, ma la **separazione delle prestazioni**: contratti
scritti che descrivano una prestazione tecnica determinata, evidenza della sua esecuzione,
corrispettivo ancorato a tariffe di mercato. Che è esattamente ciò che D01 raccomanda al paragrafo
successivo — ma senza sapere che quella è l'unica difesa disponibile, e non un rafforzativo di una
difesa già solida.

**Effetto sui conti.** La qualificazione incide anche sulla base IRAP: se i compensi dei tre
amministratori diversi da Pradella fossero reddito di lavoro autonomo, sarebbero **deducibili** ai
fini IRAP e la base 2025 scenderebbe da ≈171.190 a ≈153.300. Ho verificato che la conclusione del
§ 3 **regge in entrambe le ipotesi**: il carico ordinario 2025 passa da 36.107 a 35.553 euro, e lo
scostamento rispetto ai 17.190 iscritti resta fra 18.400 e 18.900 euro.

---

## Parte III — Rilievi da correggere (GIALLO)

### G-1. § 4.1 — «la cassa non c'è» è un'affermazione statica che ignora il flusso di cassa dell'esercizio

Il documento confronta la liquidità di fine 2025 al netto dei dividendi (circa 111.000) con lo
stock di riserve (210.113) e conclude che «la distribuzione delle riserve accumulate è un problema
di incasso prima che di fiscalità». È un confronto fra uno stock istantaneo e uno stock cumulato
di otto esercizi.

Ho ricostruito il flusso di cassa 2025 dai due stati patrimoniali:

| | euro |
|---|---:|
| Utile d'esercizio | 106.107 |
| + ammortamenti | 3.322 |
| − incremento crediti (152.349 − 86.719) | −65.630 |
| − incremento ratei e risconti attivi (3.499 − 3.185) | −314 |
| + incremento debiti (57.023 − 44.455) | +12.568 |
| + incremento ratei e risconti passivi (570 − 333) | +237 |
| − variazione TFR (855 − 936) | −81 |
| − investimenti in immobilizzazioni (13.788 − 11.086 + 3.322) | −6.024 |
| **= flusso di cassa** | **+50.185** |

Variazione effettiva delle disponibilità liquide: 150.925 − 100.742 = **+50.183**. La quadratura
torna a 2 euro. **La società autofinanzia circa 50.000 euro l'anno di cassa netta pur assorbendo
65.630 euro di crescita dei crediti.** La distribuzione integrale delle riserve è quindi un
problema di *fasatura su tre esercizi*, non un vincolo strutturale — e diventa ancora meno
vincolante se si interviene sul circolante.

*Riscrivere* la frase come: «la distribuzione integrale in un solo esercizio non è finanziabile:
va pianificata su tre esercizi, o accompagnata da un'azione sul circolante che liberi 40-60.000
euro».

### G-2. § 4.2 e § 4.3 — «i soci fatturano per il 48% dei ricavi» non è dimostrato, e i numeri disponibili vanno nella direzione opposta

Il § 4.3 afferma, nel riquadro conclusivo, che «il gruppo … fattura per il 48% dei ricavi». Quel
48,3% è il rapporto **B7 costi per servizi / ricavi**, che comprende tutto: medici competenti per
la sorveglianza sanitaria, docenti dei corsi, consulenti esterni, utenze, assicurazioni,
manutenzioni, compenso del commercialista e — molto probabilmente — parte dei compensi di
amministratore. Attribuirlo ai soci è un salto logico non dichiarato.

Tre elementi lo contraddicono:

1. **B7 al netto dei compensi di amministratore** vale 203.509 − 47.893 = **155.616**, cioè il
   36,9% dei ricavi. È il tetto massimo, non la stima.
2. **Il solo Dalla Piazza ha fatturato 128.313 nel 2024** (quadro RE) su un B7 2024 di 176.141. Se
   davvero fatturasse tutto alla società, resterebbero **47.828 euro** per gli altri tre soci *e*
   per ogni altro servizio acquistato dall'azienda: impossibile per una società che vende
   sorveglianza sanitaria e formazione. La lettura più probabile è che **la quota prevalente dei
   suoi compensi provenga da committenti terzi**, il che cambia il § 4.2 e cambia soprattutto il
   § 4.3 (le sue aliquote marginali si formano su un reddito che la società non controlla).
3. **La dinamica 2024-2025 va nella direzione opposta.** Ricavi +39,4% (+119.140), B7 +15,5%
   (+27.368). Se i soci fatturassero una quota strutturale del fatturato, B7 crescerebbe in modo
   proporzionale. Non lo fa. **Nel 2025 la società ha assorbito ricavi senza aumentare in misura
   corrispondente il costo esterno.** Da dove vengono quei 119.140 euro è la prima domanda di
   qualunque verifica, e il documento non se la pone. Vedi G-6.

*Riscrivere il § 4.2 e il riquadro del § 4.3 marcando esplicitamente [V] l'entità del canale
fattura-socio, e sostituendo «il 48% dei ricavi» con «una quota non ancora quantificata, comunque
non superiore al 36,9% dei ricavi».*

### G-3. § 5.2 — il rilievo sul «trattamento di quiescenza» va chiuso, non lasciato aperto: gli elementi per chiuderlo sono già nel fascicolo

Il documento chiede la delibera istitutiva del TFM. Ma tre elementi decisivi sono già agli atti e
non vengono usati:

1. **L'atto costitutivo contiene la clausola, ed è insufficiente.** L'art. 24 dello statuto
   (`Atto.pdf`) dispone: «Agli Amministratori *può* spettare, oltre al rimborso delle spese …, un
   emolumento annuo nella misura stabilita da decisione dei soci …; a favore degli stessi
   *potranno altresì essere accantonate* somme a titolo di trattamento di fine mandato … A fronte
   di tale onere la società *potrà* stipulare polizze assicurative». È una **facoltà**, priva di
   importo e di criterio oggettivo di determinazione. Secondo l'orientamento dominante (Cass.
   nn. 26431/2018 e 17367/2020) **non basta**: serve un atto di data certa che specifichi anche
   l'ammontare. Il documento deve dirlo — l'atto di data certa esiste già, ed è quello che non
   funziona.
2. **Nessuna attività a fronte dei premi.** Se si trattasse di polizza con la società contraente e
   beneficiaria, il diritto al riscatto sarebbe un'attività da iscrivere. Le **immobilizzazioni
   finanziarie sono pari a zero in tutti e quattro gli esercizi** e i «Crediti» non sono
   dettagliati. Delle due l'una: o la polizza è intestata all'amministratore — e allora il premio è
   una **liberalità in natura / fringe benefit** da assoggettare a ritenuta e contributi, con
   riflesso su CU e 770 — oppure il costo è dedotto senza alcuna rappresentazione patrimoniale.
3. **L'importo esatto della posta in gioco.** Cumulato 2022-2025: 768 + 3.500 + 3.500 + 3.495 =
   **11.263 euro** di costi dedotti. Trattandosi di costo per soggetto assimilato a lavoro
   dipendente, **non è deducibile ai fini IRAP** in nessuna ipotesi, quindi il recupero massimo è
   di sola IRES: 11.263 × 24% = **2.703 euro**, oltre sanzioni e interessi, sui soli periodi ancora
   accertabili. Dare il numero cambia la percezione del rischio: è un rilievo da chiudere con una
   delibera, non un problema da 20.000 euro.

*Aggiungere al § 5.2 i tre punti sopra, la quantificazione di 2.703 euro e la data di scadenza del
rischio (art. 43 DPR 600/1973), come impone il protocollo.*

### G-4. § 5.4 — «Beni ai soci in godimento: non emergono dal bilancio». Emergono: la voce si chiama B8 e vale 13.032

La voce «costi per godimento di beni di terzi» — 11.665 / 14.237 / 14.927 / 13.032 nei quattro
esercizi — è **esattamente** la posta in cui si collocano sia la locazione della sede sia i noleggi
e i leasing delle autovetture. Scrivere che i beni ai soci «non emergono dal bilancio» quando c'è
una voce dedicata da 13.032 euro non è sostenibile.

Le domande concrete, che il § 7 non pone:

- **Chi è il locatore della sede di Via A. Volta 36, Dossobuono?** Se è un socio, una loro società
  o un familiare, si applicano il valore normale ex art. 9 TUIR e l'imposta di registro sul
  contratto; il canone è reddito fondiario in capo al percettore. È una delle prime cose che si
  verificano in accesso, perché la sede si vede.
- **Se i 13.032 sono noleggi auto**, si aprono l'art. 164 TUIR (deducibilità limitata) e il fringe
  benefit per uso promiscuo degli amministratori, con riflesso su CU e 770 e — se non tassato — la
  fattispecie dell'art. 67, c. 1, lett. h-*ter*, TUIR con la corrispondente indeducibilità in capo
  alla società prevista **non dal TUIR ma dall'art. 2, c. 36-*quaterdecies*, D.L. 138/2011**
  (V01, G-4: il documento non cita né l'una né l'altra).
- **Perché B8 scende del 12,7% nel 2025 mentre i ricavi salgono del 39,4%?** Un canone di
  locazione della sede sarebbe stabile. Il profilo suggerisce contratti di noleggio in scadenza.

*Sostituire «non emergono dal bilancio» con «la voce B8 vale 13.032 euro: va acquisito il dettaglio
(contratto di locazione della sede con indicazione del locatore; contratti di noleggio/leasing auto
con assegnatari e valori convenzionali di fringe benefit)».*

### G-5. § 5.4 — «Società di comodo: non applicabile perché la società è operativa, in utile e in crescita» non è il test di legge

L'art. 30 L. 724/1994 non chiede se la società sia «operativa»: chiede di confrontare i ricavi
effettivi medi del triennio con i ricavi presunti calcolati applicando i coefficienti al valore
degli asset. La conclusione del documento è giusta, il percorso no. Rifatto il test con i
coefficienti dimezzati dal D.Lgs. 192/2024 (V01, G-6):

- ricavi presunti: 15% sulla media triennale delle «altre immobilizzazioni» (5.107 + 11.086 +
  13.788) / 3 = 9.994 → **1.499 euro**; nessun immobile, nessun titolo, nessuna partecipazione
- ricavi effettivi medi (A1 + A5): (285.252 + 302.988 + 422.114) / 3 = **336.785 euro**

**Test superato di 225 volte.** Scriverlo così: due righe, un numero, la porta è chiusa in modo
verificabile invece che per impressione. Va aggiunto, come prescriveva V01 G-6, che la
disciplina delle società in perdita sistematica è **abrogata** e che la conseguenza più pesante
della non operatività non è la maggiorazione IRES ma il **blocco del credito IVA** (art. 30, c. 4,
L. 724/1994) — se il documento cita l'istituto, deve citarne l'effetto.

### G-6. § 2 e § 3 — il salto del fatturato 2025 non è spiegato, ed è il fatto che genera tutto il resto

Il documento definisce il 2025 «un anno di rottura» e lo attribuisce alla leva operativa. La leva
operativa spiega perché il margine cresce più dei ricavi; **non spiega da dove vengono 119.140
euro di ricavi in più** in una struttura che nello stesso anno aggiunge, al massimo, un dipendente.

Le ipotesi che un verificatore mette sul tavolo, in ordine di interesse:

1. **Spostamento di attività dai soci alla società.** Se i soci professionisti hanno smesso di
   fatturare in proprio parte del lavoro e lo hanno fatto fatturare dalla società, il ricavo si
   sposta su un soggetto che (per ipotesi) è in concordato e non lo tassa. È la manovra tipica del
   primo anno di CPB e produce esattamente questo profilo: ricavi +39%, costi esterni +15%, utile
   +160%. Il dato del quadro RE 2024 di Dalla Piazza (128.313 di compensi propri) e il quadro RE
   2025, quando arriverà, permettono di verificarlo in dieci minuti.
2. **Commessa una tantum o cliente nuovo di grande dimensione**, con conseguente concentrazione
   del credito (che infatti cresce del 76%).
3. **Anticipo di fatturazione a fine esercizio** per saturare la capienza del concordato prima
   della scadenza del biennio.

La prima ipotesi non è teorica ed è quella con le conseguenze più serie: se il maggior reddito
2025 della società deriva dallo spostamento di ricavi personali dei soci in un anno coperto da
concordato, si è dentro l'art. 10-*bis* L. 212/2000 (operazione priva di sostanza economica
diretta a realizzare un vantaggio fiscale indebito) e, sul piano del CPB, potenzialmente dentro
l'art. 22, c. 1, lett. a).

*Aggiungere al § 7 una voce: «riconciliazione dei ricavi 2024 → 2025 per cliente e per linea di
servizio, con indicazione dei clienti nuovi e delle commesse non ricorrenti».* Senza quella, la
proiezione 2026-2027 su cui si decide il CPB non è costruibile.

### G-7. § 3 — le spiegazioni alternative al crollo del tax rate non sono state esaminate. Le ho esaminate io: **il CPB regge, ma il documento deve dimostrarlo**

Il documento definisce l'inferenza «quasi certa» senza escludere nulla. Un fascicolo che spinge
verso una decisione da 18.000 euro l'anno non può fondarsi su un'inferenza non falsificata, tanto
più che l'**Executive Summary interno al CdA** aveva già messo per iscritto le ipotesi alternative
(«eventuali crediti d'imposta utilizzati, agevolazione ACE, sopravvenienze attive non tassabili»)
e D01 non risponde a nessuna. Ho fatto io il lavoro; l'esito è favorevole al consulente, ma va
messo nel documento:

| Ipotesi alternativa | Esito | Prova |
|---|---|---|
| **Perdite pregresse riportate** (art. 84 TUIR) | **Esclusa** | La società non ha mai chiuso in perdita: il patrimonio netto mostra riserve di utili positive e crescenti in tutti gli esercizi 2018-2025 (65.808 di riserve già al 31/12/2022, tutte da utili). |
| **IRES premiale al 20%** (art. 1, cc. 436-444, L. 207/2024) | **Esclusa: fallisce due condizioni su quattro** | (i) Richiede investimenti in beni 4.0/5.0 (allegati A e B L. 232/2016 e art. 38 D.L. 19/2024) per almeno 20.000 euro: gli acquisti di immobilizzazioni 2025 valgono 13.788 − 11.086 + 3.322 = **6.024 euro**. (ii) Richiede nuove assunzioni a tempo indeterminato pari almeno all'1% e comunque non inferiori a un lavoratore (art. 1, c. 437, lett. a), n. 2): nel 2025 non risultano assunzioni (la visura certifica 2 dipendenti al 30/06/2025; Carli Anna è del 06/07/2026). E comunque varrebbe 4 punti di IRES, cioè circa 4.900 euro: insufficiente. **Non è stata prorogata al 2026.** |
| **Super-deduzione nuove assunzioni** (art. 4 D.Lgs. 216/2023, prorogata dalla L. 207/2024) | **Insufficiente** | Anche ammettendo un'assunzione a tempo indeterminato nel secondo semestre 2025 (la visura certifica 2 dipendenti al 30/06/2025; Carli Anna è del 06/07/2026) e un incremento del costo del personale pari all'intero +11.965 di B9-a, la maggiorazione del 20% vale **2.393 di variazione in diminuzione = 574 euro di IRES**. Spiega il 3% dello scostamento. |
| **Crediti d'imposta** | **Esclusa** | I crediti d'imposta non riducono la voce «imposte correnti» del conto economico: transitano da A5 o dalla compensazione in F24. A5 vale **815 euro** nel 2025 e i contributi in conto esercizio sono **zero** nel 2024 e nel 2025. |
| **ACE residua** (eccedenze ante 2024) | **Irrilevante** | Base ACE massima teorica ≈ capitale 10.000 + utili accantonati 2018-2023: rendimento nozionale nell'ordine di 1.000-1.500 euro l'anno, cioè 250-350 euro di IRES. |
| **Imposte anticipate/differite** | **Esclusa dal bilancio** | La riga «Totale delle imposte sul reddito dell'esercizio, correnti, differite e anticipate» vale 17.190, **interamente** «imposte correnti»: non c'è alcuna fiscalità differita. |
| **Errore di stanziamento / IRAP omessa** | **Non escludibile senza le dichiarazioni** | 17.190 / 0,24 = 71.625: sarebbe compatibile con un'IRES ordinaria su un imponibile di 71.625 **senza alcuno stanziamento IRAP**. È l'unica alternativa che regge, e si chiude in un minuto guardando la dichiarazione IRAP. |
| **Variazioni in diminuzione ordinarie** | **Insufficienti** | Per portare il carico da 36.100 a 17.190 servirebbero circa 78.800 euro di variazioni in diminuzione: non esistono poste di quella dimensione in questo conto economico. |

**Verifica indipendente dell'ipotesi CPB, e un risultato che il documento non ha visto.** Ho
ricostruito il carico ordinario di ciascun esercizio con lo stesso metodo (dettaglio nella sezione
§ 4.3, punto 0):

| | 2023 | 2024 | 2025 |
|---|---:|---:|---:|
| IRES + IRAP ricostruite in regime ordinario | 16.633 | 14.591 | 36.107 |
| Imposte correnti effettivamente iscritte | 15.903 | 16.543 | 17.190 |
| Scostamento | −730 (−4,4%) | **+1.952 (+13,4%)** | **−18.917 (−52,4%)** |

*(IRAP al 3,90% per il 2023 e il 2024, al 4,08% dal 2025: vedi E-6.)*

Il 2023 quadra entro il 4,4%: è un anno di tassazione ordinaria, e serve da taratura del modello.
Il **2024 paga 1.952 euro in più dell'ordinario** e il 2025 ne paga 18.917 in meno. Un carico
d'imposta che *supera* quello ordinario in un anno e crolla nell'anno successivo è il profilo
tipico di una **base imponibile fissa concordata**: nel primo anno il concordato eccede
l'effettivo, nel secondo l'effettivo esplode e l'imposta resta ancorata.

**C'è di più, ed è dirimente.** Le imposte correnti passano da 16.543 a 17.190: **+3,91% esatto**.
Se le due basi (IRES e IRAP) fossero cresciute della stessa percentuale — che è precisamente il
modo in cui la proposta CPB costruisce il secondo anno del biennio a partire dal primo — si
otterrebbe questo identico risultato. Una crescita del 3,9% del carico d'imposta a fronte di un
utile che cresce del 160% non è spiegabile con la tassazione ordinaria.

*Il § 3 va quindi riscritto così:* l'ipotesi «biennio 2024-2025» **non è equivalente** all'ipotesi
«biennio 2025-2026», come invece afferma il documento («il pattern dei tax rate è compatibile con
entrambe le ipotesi»). Se il biennio fosse 2025-2026 il 2024 sarebbe stato in tassazione
ordinaria, e in tassazione ordinaria il 2024 avrebbe dovuto pagare circa 14.600 euro, non 16.543.
**L'ipotesi 2024-2025 è nettamente la più probabile — e questa è la peggiore delle due per il
cliente, perché significa che il concordato è già scaduto, che il 2026 è tornato in tassazione
ordinaria su un utile che corre, e che la finestra di novembre è l'unica.** Il documento
attenua un allarme che avrebbe dovuto alzare.

### G-8. § 3 — la stima «reddito concordato ~55.000 e VPN ~100.000» è indeterminata come è scritta, ma **il numero è giusto**: va ancorata

Come è formulata, la ricostruzione è un'equazione con due incognite: qualunque coppia che
soddisfi 0,24·X + 0,0408·Y = 17.190 funziona (55.000/100.000, ma anche 60.000/68.400 o
50.000/126.700). Il lettore non ha modo di sapere perché quella coppia e non un'altra.

L'ancoraggio esiste e va scritto. La proposta CPB per il biennio 2024-2025 è costruita sui dati
2023, e nel 2023 il rapporto fra valore della produzione netta e reddito d'impresa era:

- VPN IRAP 2023 effettivo = 54.951 (A − B) + 43.882 (compensi di amministratore indeducibili) =
  **98.833**
- reddito IRES 2023 effettivo ≈ 54.951 − 1.711 (deduzione IRAP sul lavoro) = **53.240**
- rapporto VPN / reddito = **1,86**

Imponendo lo stesso rapporto: 0,24·X + 0,0408·(1,86·X) = 17.190 → 0,3159·X = 17.190 →
**X ≈ 54.400 e Y ≈ 101.200**. La stima del documento è centrata. *Aggiungere le tre righe di
derivazione*, altrimenti il numero non è difendibile davanti al commercialista del cliente.

Conseguenza da esplicitare, che il documento non trae: il **valore della produzione netta effettivo
2025 è circa 171.190** contro un concordato di circa 101.200. La quota non tassata è quindi
**66.900 di reddito IRES** *e* **70.000 di valore della produzione netta IRAP**: la forchetta
«65-70.000» del documento è corretta ma si riferisce a due basi diverse che il documento tratta
come una sola.

### G-9. *(rilievo promosso: vedi R-5)*

Il contenuto di questo rilievo è confluito nel rilievo bloccante **R-5** della Parte II, perché la
verifica sulla prassi ha rovesciato il segno dell'argomento.

### G-10. § 4.3 — mancano il terzo canale (compenso di amministratore) e la sua deducibilità per cassa

Il modello confronta due canali su quattro soci che sono anche i quattro amministratori e che nel
2025 hanno percepito **47.893 euro** proprio a quel titolo. Il canale va aggiunto, perché è il
peggiore in assoluto e dirlo con i numeri serve: il costo per euro netto è **2,29-2,51** in ogni
scenario (calcolo nella sezione dedicata), contro 1,04-2,21 della fattura e 1,35-1,87 del
dividendo, e **non beneficia mai del concordato del socio**, essendo reddito assimilato e non
reddito di lavoro autonomo.

Va inoltre citato l'**art. 95, c. 5, TUIR**, che il documento non nomina mai, nel testo verificato:

> «I compensi spettanti agli amministratori delle società ed enti di cui all'articolo 73, comma 1,
> sono deducibili **nell'esercizio in cui sono corrisposti**; quelli erogati sotto forma di
> partecipazione agli utili, anche spettanti ai promotori e soci fondatori, sono deducibili anche
> se non imputati al conto economico.»

Due conseguenze operative:

- **La quota di compenso imputata a conto economico e non pagata entro l'esercizio è una variazione
  in aumento.** È una delle spiegazioni possibili dello scostamento 2024 (+1.952 rispetto
  all'ordinario) e va verificata prima di attribuire tutto al concordato.
- **In presenza di CPB il criterio di cassa non fa differenza per la società** (la base è fissa),
  ma torna a farla dal primo anno fuori dal concordato: se si progetta una manovra sui compensi,
  il timing dei pagamenti conta.

**Trade-off che il documento non vede.** Comprimere il canale fattura e aprire il dividendo
(raccomandazione del § 4.3) lascia in piedi compensi di amministratore per 47.893 su quattro
persone che, per ipotesi, non fatturano più la prestazione tecnica. A quel punto l'ufficio ha
davanti quattro amministratori che percepiscono 12.000 euro l'anno ciascuno per gestire una società
da 421.299 euro di ricavi e ne incassano 38.871 di dividendi: **la compressione del canale fattura
rafforza, non indebolisce, il rilievo di riqualificazione del § 5.1**. Le due raccomandazioni sono
in tensione e il documento le presenta come indipendenti.

### G-11. § 7 — la lista dei documenti mancanti omette quattro voci che decidono, e ne chiede una che è già nel fascicolo

**Già nel fascicolo e non usato:** `DALLA PIAZZA_VOLUME D'AFFARI.pdf`. Il documento non lo cita
nella base documentale e non lo usa. Il volume d'affari IVA del socio è il riscontro diretto sulla
consistenza del canale fattura del § 4.2 e sulla riconciliazione fra compensi per cassa (RE) e
operazioni per competenza IVA. *Ho tentato di estrarlo senza riuscirci* (font a codifica
simbolica, nessun livello testo recuperabile): va riaperto con il software che lo ha generato.
Segnalo anche che `PRADELLA TAZIO.pdf` è composto da pagine immagine prive di livello testo.

**Da aggiungere al § 7:**

1. **Dichiarazioni IVA e LIPE 2023-2025, con riconciliazione volume d'affari / ricavi di bilancio,
   e verifica del pro-rata.** L'IVA non compare in D01. In questa società ci sono almeno tre
   fattispecie IVA aperte e nessuna è nominata: (a) la **formazione**, che è nell'oggetto sociale
   e che, se resa da organismo riconosciuto, è **esente ex art. 10, n. 20, DPR 633/1972**, con
   conseguente **pro-rata di detraibilità** ex artt. 19, c. 5, e 19-*bis*; (b) l'**intermediazione
   e commercio di rifiuti** (vedi punto 2), con i regimi di reverse charge dell'art. 74, cc. 7 e 8,
   DPR 633/1972; (c) l'**autotrasporto di cose per conto terzi**, presente nell'oggetto sociale,
   con il reverse charge dell'art. 17, c. 6, lett. a-*quinquies*. Un pro-rata non applicato opera
   su tutte le annualità aperte ed è la ripresa più meccanica che esista.
2. **Iscrizione all'Albo Nazionale Gestori Ambientali n. VE/026421, sezione di Venezia, categoria
   8 classe f, dal 08/08/2019 al 09/08/2029** (risulta dalla visura, pagina 9, e **D01 non la
   nomina**). Significa che la società esercita **intermediazione e commercio di rifiuti senza
   detenzione**, attività autorizzata, soggetta a garanzie finanziarie, RENTRI e MUD, e con un
   regime IVA proprio. È anche un'attività **secondaria dichiarata al Registro Imprese dal
   08/08/2019** (ATECO secondario 74.99.99 / ATECORI 74.90.93 e 74.90.99). Ha due effetti diretti
   sul § 6: incide sul modello ISA applicabile e, in caso di modifica dell'attività, sulla
   **cessazione del concordato ex art. 21, c. 1, lett. a), D.Lgs. 13/2024**.
3. **Ritenute e 770.** La società è sostituto d'imposta su tre fronti simultanei: ritenute del 20%
   sulle fatture dei professionisti (art. 25 DPR 600/1973), ritenute sui cedolini di tre dipendenti
   e di un co.co.co., e la **ritenuta del 26% sui 40.000 euro di dividendi deliberati il
   30/04/2026 e pagati entro il 30/06/2026: 10.400 euro, da versare con il codice tributo previsto
   entro il 16 del mese successivo al pagamento e da esporre nel 770/2027**. Va verificato che sia
   stata operata e versata: è la verifica più rapida che esista e il documento, che tratta i
   dividendi come la leva principale, non la menziona.
4. **Posizioni personali dei quattro soci al Registro Imprese (visura persona: cariche e
   partecipazioni).** Vedi G-12.

**Voce da correggere nel § 7.** Il n. 9 dice: «il debito tributario oltre 5.000 euro è causa di
esclusione dal CPB». È impreciso in un modo che può far scartare l'operazione senza motivo. L'art.
10, c. 2, D.Lgs. 13/2024, nel testo vigente, dispone tre cose che il documento non distingue:
(i) rilevano **solo i debiti definitivamente accertati** con sentenza irrevocabile o con atti
impositivi non più impugnabili; (ii) è comunque ammesso chi li ha estinti entro il termine di
adesione se il debito residuo, compresi interessi e sanzioni, è **inferiore alla soglia di 5.000
euro** (a 5.000,00 esatti il requisito **non** è soddisfatto); (iii) «**non concorrono al predetto
limite i debiti oggetto di provvedimenti di sospensione o di rateazione**, sino a decadenza dei
relativi benefici». *Scrivere così*: la rateazione in corso non pregiudica l'accesso; la decadenza
dalla rateazione sì; e un avviso bonario non definitivo non conta. Il nuovo c. 2-*bis* aggiunge che
l'adesione in assenza dei requisiti «è priva di effetti».

### G-12. § 1 — «[A] Non è un gruppo … nessuna partecipazione»: la visura dice questo della società, non dei soci. E nel fascicolo ci sono già due indizi contrari

Il riquadro «Partecipazioni» della visura riporta, in nota, che l'informazione «indica se
**l'impresa** detiene partecipazioni in altre società». **Non dice nulla su ciò che detengono i
quattro soci**, che è il perimetro rilevante per un incarico di pianificazione su un gruppo
familiare. Marcare **[A] accertato** l'affermazione «non è un gruppo» sulla base di quella riga non
è corretto.

Due indizi contrari sono già nei documenti che il consulente ha letto:

1. **Dall'Oca Marco** ha come domicilio digitale iscritto al Registro Imprese
   `dallocamarcoaziendaagricola@pec.it`. Un socio con un'**azienda agricola** ha altri redditi che
   ne determinano l'aliquota marginale — cioè uno dei tre parametri che il § 4.3 dichiara di non
   conoscere — e potenzialmente un'altra posizione CPB.
2. **Pradella Tazio** subisce sul cedolino di luglio 2026 un contributo di **216,72 euro su 2.709,00
   di compenso, pari all'8,00% esatto**: è **un terzo dell'aliquota del 24%**, cioè l'aliquota
   della gestione separata riservata ai soggetti **già iscritti ad altra forma pensionistica
   obbligatoria o titolari di pensione**. A 41 anni non è pensionato: **ha un'altra posizione
   previdenziale obbligatoria**, quindi un altro rapporto di lavoro o un'altra attività. Il § 5.1
   lo descrive come colui che «fa eccezione» perché è a cedolino: la sua posizione è più articolata
   di così, e si legge sul cedolino che il consulente ha in mano.

*Aggiungere al § 7 la voce: «visure persona al Registro Imprese dei quattro soci (cariche e
partecipazioni) ed estratto delle rispettive posizioni contributive».* Finché non ci sono, l'intero
§ 1 va marcato **[V]**, non **[A]**. E si tenga presente l'art. 12.1, lett. e), dello statuto, che
prevede l'esclusione del socio che eserciti «attività concorrente con quella della società».

### G-13. § 5.4 — «Collegio sindacale / revisore: non obbligatori, soglie art. 2477 c.c. lontane». Corretto, ma va quantificato

La conclusione è giusta. Va scritta con i numeri, perché è una delle poche affermazioni del
documento che il cliente può verificare da solo e la verifica lo rassicura:

| Parametro art. 2477, c. 3, c.c. | Soglia | Overall 2025 | Overall 2024 |
|---|---:|---:|---:|
| Totale attivo dello stato patrimoniale | 4.000.000 | 320.561 (8,0%) | 201.732 (5,0%) |
| Ricavi delle vendite e delle prestazioni | 4.000.000 | 421.299 (10,5%) | 302.159 (7,6%) |
| Dipendenti occupati in media nell'esercizio | 20 | 2-3 | 2 |

L'obbligo scatta al superamento di **almeno uno** dei tre limiti **per due esercizi consecutivi**,
e cessa «quando, per tre esercizi consecutivi, non è superato alcuno dei predetti limiti». Anche
proiettando la crescita del 39% annuo, la soglia dei ricavi non è raggiungibile prima del 2033.
*Soglie verificate sul testo vigente: 4.000.000 / 4.000.000 / 20 dipendenti, invariate, nel testo
introdotto dall'art. 2-bis del D.L. 32/2019 conv. L. 55/2019. Nessuna modifica nel 2025 né nel
2026.*

Va invece aggiunto ciò che il documento non dice: l'art. 2477, c. 2, prevede l'obbligo **anche**
se la società è tenuta alla redazione del bilancio consolidato o controlla una società obbligata
alla revisione legale. Se in futuro si costituisse una holding — ipotesi non remota in un gruppo
familiare — l'obbligo può scattare da lì, non dalle soglie dimensionali.

### G-14. § 5.1 — mancano tre elementi di sostanza documentale che il verificatore chiede per primi

Il documento chiede correttamente contratti con data certa, evidenza dell'esecuzione e criterio di
determinazione del corrispettivo. Aggiungerei, per esperienza diretta:

1. **La delibera dei soci che determina i compensi degli amministratori.** L'art. 24 dello statuto
   rinvia a «decisione dei soci all'atto della nomina o successivamente». Nei tre verbali agli atti
   (2024, 2025, 2026) **non c'è traccia di alcuna delibera sui compensi**: l'ordine del giorno è
   solo l'approvazione del bilancio. Un compenso di amministratore erogato per 47.893 euro senza
   delibera assembleare è, prima ancora che un tema fiscale, un tema di **art. 2389 c.c.** e di
   ripetibilità, ed è il primo documento che viene chiesto (Cass. SS.UU. n. 1545/2017 sul rapporto
   amministratore-società resta il riferimento sul piano civilistico).
2. **Le fatture dei soci con la descrizione della prestazione.** Una fattura che recita «consulenza
   tecnica» non distingue nulla dall'attività gestoria. La difesa si costruisce sul contenuto della
   descrizione, non sul contratto.
3. **La riconciliazione fra B9-a «salari e stipendi» e i cedolini.** Nel 2025 B9-a vale 49.408
   contro oneri sociali per 9.193, cioè il **18,6%**: un rapporto troppo basso per tre lavoratori
   subordinati (dove si sta sopra il 28-30%) e compatibile con la presenza, dentro quella voce, di
   un compenso di co.co.co. al 16% a carico committente e/o con esoneri contributivi. La
   collocazione contabile dei compensi di amministratore (B7 o B9) **non cambia la base IRAP** —
   sono indeducibili in ogni caso — ma cambia la lettura del costo del lavoro, che è uno degli
   indicatori elementari ISA. *Chiedere il dettaglio del costo del personale e il LUL.*

### G-15. § 6 — «La revoca ha lo stesso termine»: affermazione non riscontrata

Il documento afferma che la revoca dell'adesione al CPB ha lo stesso termine dell'adesione. **NON
VERIFICATO**: non ho trovato conferma su fonte primaria della disciplina della revoca per il
biennio 2026-2027. Va confermata o eliminata prima della consegna: è il tipo di affermazione che
il cliente usa per rinviare la decisione («tanto posso revocare»).

---

## Parte IV — Rilievi che il documento non ha visto

### N-1. Il CPB come leva principale espone la società a una decadenza retroattiva innescata proprio dal rilievo del § 5.1

È il rilievo di impostazione più serio, e nasce dall'incrocio di due capitoli che il documento
tiene separati.

L'art. 22, c. 1, lett. a), D.Lgs. 13/2024 dispone che il concordato **cessa di produrre effetto
per entrambi i periodi d'imposta** quando, a seguito di accertamento relativo ai periodi oggetto
di concordato **o a quello precedente**, «risulta l'esistenza di attività non dichiarate o
**l'inesistenza o l'indeducibilità di passività dichiarate**, per un importo superiore al 30 per
cento dei ricavi dichiarati», ovvero risultano commesse «altre violazioni di non lieve entità»
fra cui, ai sensi del c. 2, lett. a), le fattispecie del D.Lgs. 74/2000 «relativamente ai periodi
di imposta oggetto del concordato **e ai tre precedenti**».

Applicato a questa società:

- la soglia del 30% sui ricavi 2025 vale **126.390 euro**;
- il perimetro potenzialmente contestabile del § 5.1 (fatture dei soci per prestazioni che si
  sovrappongono all'attività gestoria, difetto di inerenza, valore normale ex art. 9 TUIR) è
  compreso, secondo la stima corretta di G-2, fra 0 e **155.616 euro**;
- **il rilievo che il documento classifica GIALLO è quindi dimensionalmente idoneo a far decadere
  il concordato**, con recupero dell'imposta su **entrambi** gli anni.

**E la decadenza è asimmetrica a sfavore del contribuente.** L'art. 22, c. 3-*bis*, dispone che
«nel caso di decadenza dal concordato **restano dovute le imposte e i contributi determinati
tenendo conto del reddito e del valore della produzione netta concordati se maggiori di quelli
effettivamente conseguiti**». Applicato al biennio 2024-2025 significa: per il 2025 (effettivo
121.343 contro concordato ≈54.400) si paga sull'effettivo, con un recupero di **18.917 euro**; per
il 2024 (effettivo 45.668 contro concordato ≈54.400) **non si restituisce nulla**, perché resta
dovuta l'imposta sul concordato più alto. **Il conto del danno è quindi 18.917 euro di imposte,
oltre sanzioni e interessi, e non c'è alcuna compensazione con l'anno in cui si era pagato di
più.** Nella tassazione ordinaria lo stesso rilievo costerebbe soltanto la ripresa del costo
disconosciuto, cioè il 28,08% dell'importo contestato.

Va aggiunto che il correttivo **D.Lgs. 7 agosto 2026 n. 148** ha riscritto l'art. 22 con effetto
**dal biennio 2026-2027**, e in senso in parte favorevole: la dichiarazione integrativa che
modifica i dati non è più causa di decadenza ma comporta la **rideterminazione** del concordato
(nuovo art. 19, c. 3-*bis*), la sopravvenienza di una causa di esclusione non produce più decadenza
ma **inefficacia originaria** (artt. 10, c. 2-*bis*, e 11, c. 1-*bis*), e il c. 3 salva le
violazioni **regolarizzate con ravvedimento operoso** purché non già constatate e purché non siano
iniziati accessi, ispezioni o verifiche. Quest'ultima è una leva difensiva concreta e va scritta
nel documento: **finché non arriva l'accesso, un rilievo sulle fatture dei soci è sanabile senza
far decadere il concordato.**

**Il CPB non attenua il rischio del § 5.1: lo moltiplica.** Il documento raccomanda il primo senza
mai collegarlo al secondo. Va aggiunta al § 6 una tabella di **condizioni di mantenimento e cause
di decadenza** — che il protocollo, del resto, rende obbligatoria per ogni VERDE.

### N-2. Sotto CPB la discrasia fra reddito dichiarato e volume d'affari IVA cresce, e l'IVA non è coperta dal concordato

La base normativa è l'**art. 18 D.Lgs. 13/2024**, che D01 non cita: «L'adesione al concordato **non
produce effetti ai fini dell'imposta sul valore aggiunto**, la cui applicazione avviene secondo le
regole ordinarie». La conseguenza operativa, che il documento non dice al cliente:

- nel 2025 la società dichiara (per ipotesi) circa 54.400 euro di reddito e circa 101.200 di valore
  della produzione netta, mentre le fatture emesse e trasmesse allo SdI e le LIPE espongono un
  volume d'affari coerente con **421.299 euro di ricavi**;
- l'incrocio fra fatturazione elettronica, LIPE e dichiarazione dei redditi è **automatico e
  immediato**. La discrasia è legittima, ma è visibile e va saputa spiegare: è esattamente il tipo
  di scostamento che alimenta le liste selettive e le lettere di compliance.

Va aggiunta una riga al § 6: sotto CPB il presidio documentale sull'IVA e sulla riconciliazione
volume d'affari / ricavi **aumenta di importanza**, non diminuisce.

### N-3. Il documento non dice quali sono i benefici premiali del CPB, e uno di essi è la contropartita del rischio N-1

L'art. 19, c. 3, D.Lgs. 13/2024 riconosce a chi aderisce i benefici premiali dell'art. 9-*bis*,
c. 11, D.L. 50/2017, **«compresi quelli relativi all'imposta sul valore aggiunto»**, e li riconosce
**per il solo fatto dell'adesione, a prescindere dal punteggio ISA conseguito**. In concreto:

- esonero dal visto di conformità per la compensazione di crediti fino a **70.000 euro annui per
  l'IVA** e **50.000 euro annui per imposte dirette e IRAP**;
- esonero da visto e garanzia per i **rimborsi IVA fino a 70.000 euro annui**;
- **esclusione dalla disciplina delle società non operative** (art. 30 L. 724/1994);
- **esclusione degli accertamenti fondati su presunzioni semplici** ex art. 39, c. 1, lett. d),
  secondo periodo, DPR 600/1973 e art. 54, c. 2, secondo periodo, DPR 633/1972;
- **anticipazione di almeno un anno** dei termini di decadenza per l'accertamento (artt. 43 DPR
  600/1973 e 57 DPR 633/1972);
- esclusione dalla determinazione sintetica del reddito ex art. 38 DPR 600/1973 se il reddito
  accertabile non eccede di due terzi quello dichiarato.

**In caso di rinnovo i benefici sono maggiori** (art. 14, c. 1-*bis*): visto fino a 100.000 euro
per l'IVA e 70.000 per le dirette, rimborsi IVA fino a 100.000, e anticipazione di **due** anni dei
termini di accertamento. Si aggiungono, per il rinnovo relativo al 2026-2027, l'assenza di
interessi sui versamenti rateali (art. 14, c. 1-*ter*) e l'esclusione della maggiorazione d'acconto
del primo anno (art. 20, c. 3-*bis*).

**Va inoltre citato l'art. 34.** Il c. 1 preclude, per i periodi concordati, gli accertamenti
dell'art. 39 DPR 600/1973 «salvo che … ricorrano le cause di decadenza di cui agli articoli 22 e
33». Il c. 2 stabilisce che l'Agenzia e la Guardia di Finanza programmano maggiore capacità
operativa per **intensificare i controlli su chi non aderisce o decade**. Sono due informazioni che
il cliente ha diritto di avere: la prima è il principale beneficio difensivo dell'adesione, la
seconda è il costo dichiarato del non aderire. I limiti della preclusione vanno però detti: copre
**solo l'art. 39 DPR 600/1973**, quindi restano possibili accessi, ispezioni e verifiche,
accertamenti su altre categorie reddituali, accertamenti IVA e controlli ex artt. 36-*bis* e
36-*ter*.

Nessuno di questi elementi compare in D01, che pure dedica al CPB l'intero § 6.

### N-4. Nessuna immobilizzazione immateriale in una società che vive di know-how: il documento lo usa solo per chiudere una porta

Il § 2 registra il dato per escludere le leve immobiliari. Le due letture che mancano:

- **Il marchio.** «OVERALL GROUP» è un segno usato da otto anni e non iscritto all'attivo. Se è
  registrato a nome di uno o più soci a titolo personale, si apre esattamente lo schema royalties
  già analizzato in `V00` e corretto in V01 (R-2), con tutti i suoi rilievi: qualificazione ex art.
  67, c. 1, lett. l), TUIR, ritenuta del 20% ex art. 25 DPR 600/1973, e soprattutto il **requisito
  soggettivo IVA**, che è il vero punto di rottura di quello schema. Se invece non è registrato da
  nessuno, il valore costruito in otto anni è indifendibile in caso di uscita di un socio. **Va
  verificato al registro marchi UIBM: è una ricerca di cinque minuti e cambia due capitoli.**
- **Il software e le banche dati.** Una società di consulenza sicurezza/ambiente con 421.299 euro
  di ricavi ha procedure, format di DVR, banche dati normative, piattaforme di erogazione della
  formazione. Nulla è capitalizzato. Se esistono sviluppi interni tutelati da copyright, rientrano
  fra i beni agevolabili del **nuovo patent box (art. 6 D.L. 146/2021)**, confermato vigente in
  V01. I marchi no, i software sì: è la distinzione che decide se la leva esiste.

### N-5. Il concordato del socio e il concordato della società vanno decisi insieme, e il documento li tratta separatamente

Dalla Piazza è stato in CPB da lavoratore autonomo per il 2024 (e presumibilmente per il 2025, se
il biennio era 2024-2025). La società, per l'ipotesi del documento, era in CPB per lo stesso
biennio. **Entrambe le finestre 2026-2027 si aprono e si chiudono nello stesso momento**, e le due
decisioni sono interdipendenti nel modo dimostrato dal § 4.3 rifatto: se entrambi aderiscono, il
canale ottimale è la fattura; se aderisce solo la società, è il dividendo; se non aderisce nessuno
dei due, dipende dall'aliquota marginale di ciascun socio.

Il § 6 e il § 7 trattano il CPB della società e la «posizione personale dei quattro soci» come due
voci separate della lista. Sono **una sola decisione a quattro (o cinque) variabili**, e va
impostata come tale nelle sette settimane che restano.

### N-6. Il tema ISA è ridotto a un dato da acquisire, mentre è il parametro di prezzo dell'operazione

Il § 7, voce 4, chiede i punteggi ISA per determinare l'aliquota sostitutiva. Manca il resto:

- **il punteggio ISA della società del 2025 è già determinato dai bilanci agli atti** e sarà
  probabilmente migliore di quello del 2024: ricavi per addetto e valore aggiunto per addetto
  crescono del 39% a organico quasi invariato. Un punteggio più alto abbassa l'aliquota
  sostitutiva sull'incremento;
- **quello che conta non è solo il punteggio ma gli indicatori elementari di anomalia** (V01, O-5).
  Un 8 con un indicatore rosso è più pericoloso di un 6 pulito, e in questa società l'indicatore da
  guardare è il costo del lavoro rispetto ai ricavi, che nel 2025 scende dal 16,3% al 15,5% mentre
  i ricavi esplodono;
- **l'iscrizione all'Albo Gestori Ambientali e l'attività secondaria di intermediazione rifiuti**
  possono incidere sul modello ISA applicabile e, in caso di variazione, sull'art. 21, c. 1, lett.
  a).

### N-7. Il rischio di stallo societario è segnalato correttamente ma non è quantificato, e ha un effetto fiscale che il documento nega

Il § 1 conclude che la parità al 25% «non è un tema fiscale». Lo diventa in due casi concreti:

- **la delibera di distribuzione richiede l'unanimità di fatto.** Il documento raccomanda «una
  politica di distribuzione dichiarata»: con quattro quote paritarie, un socio che voglia
  patrimonializzare blocca ogni distribuzione. La raccomandazione del § 4.1 non è eseguibile senza
  un patto parasociale o una modifica statutaria;
- **l'esclusione e il recesso hanno un costo fiscale.** L'art. 12 dello statuto disciplina
  l'esclusione e rinvia alla procedura di rimborso del recesso: il rimborso della quota al socio
  uscente genera, per la parte eccedente il costo fiscalmente riconosciuto (2.500 euro), materia
  imponibile ex art. 47, c. 7, TUIR. Su un patrimonio netto di 262.113 euro la quota vale almeno
  65.528, con un differenziale imponibile di 63.028 euro per socio. **È esattamente il caso in cui
  la rideterminazione del costo delle partecipazioni (R-3, punto e) va valutata**, e il documento
  non collega le due cose.

---

## Verifica del modello § 4.3 — conti rifatti per esteso

### 0. Base di partenza: la ricostruzione IRES/IRAP che il documento non fa

Il § 4.3 usa «IRES 24% + IRAP 3,9% ≈ 27,9%» senza mai costruire le due basi, e con un'aliquota
IRAP che dal 2025 non è più quella applicabile in Veneto (E-6). Ricostruisco entrambe, perché
servono qui e al § 3 (E-6, G-7, G-8).

**Aliquota IRAP.** 3,90% fino al periodo d'imposta 2024; **4,08% dal periodo d'imposta 2025**
(art. 2 L.R. Veneto 27 dicembre 2024 n. 32, maggiorazione dello 0,18% per i soggetti diversi da
quelli dell'Allegato C).

**Base imponibile IRAP (art. 5 D.Lgs. 446/1997).** Si parte dalla differenza A − B e si
**riaggiungono i costi del personale non deducibili**. Precisazioni tecniche che il documento non
fa e che cambiano il risultato:

- l'art. 5, c. 1, esclude dal computo le voci **B.9, B.10 lett. c) e d), B.12 e B.13** — **non** la
  B.14, che resta deducibile (l'ho trattata come tale);
- l'art. 11, c. 4-*octies*, ammette in deduzione «**il costo complessivo per il personale
  dipendente con contratto a tempo indeterminato**»: la deduzione è integrale;
- l'indeducibilità dei compensi ai collaboratori coordinati e continuativi e agli amministratori
  discende dall'**art. 11, c. 1, lett. b), n. 3) e n. 4)**, D.Lgs. 446/1997 (rinvii alla vecchia
  numerazione TUIR: art. 49, c. 2, lett. a) = oggi art. 50, c. 1, lett. c-*bis*). Poiché quei
  compensi sono classificati in **B.7**, che l'art. 5 non esclude, senza l'art. 11 risulterebbero
  deducibili: **è l'art. 11 e non l'art. 5 la fonte dell'indeducibilità**;
- l'indeducibilità opera **a prescindere dalla voce di conto economico** in cui i compensi sono
  classificati (B.7 o B.9). È il motivo per cui la loro collocazione contabile, che dal bilancio
  micro non si vede, non incide sul risultato.

| | 2023 | 2024 | 2025 |
|---|---:|---:|---:|
| Differenza A − B | 54.951 | 47.448 | 123.297 |
| + compensi ad amministratori/co.co.co. indeducibili (nota al bilancio) | 43.882 | 45.652 | 47.893 |
| **= base imponibile IRAP ricostruita** | **98.833** | **93.100** | **171.190** |
| Aliquota | 3,90% | 3,90% | **4,08%** |
| **IRAP** | **3.855** | **3.631** | **6.985** |

**Base imponibile IRES.** Unica variazione strutturale visibile: la deduzione dall'IRES dell'IRAP
relativa alla quota imponibile delle spese per il personale dipendente e assimilato (art. 2, c. 1,
D.L. 201/2011). Poiché il costo dei dipendenti a tempo indeterminato è già interamente dedotto ai
fini IRAP, la quota imponibile residua coincide con i compensi assimilati. La deduzione forfetaria
del 10% non spetta: gli oneri finanziari sono pari a zero nel 2024 e nel 2025.

| | 2023 | 2024 | 2025 |
|---|---:|---:|---:|
| Risultato ante imposte | 54.951 | 47.448 | 123.297 |
| − deduzione IRAP sul costo del lavoro (compensi × aliquota) | −1.711 | −1.780 | −1.954 |
| **= imponibile IRES ricostruito** | **53.240** | **45.668** | **121.343** |
| IRES al 24% | 12.778 | 10.960 | **29.122** |
| **Totale IRES + IRAP ricostruite** | **16.633** | **14.591** | **36.107** |
| Imposte correnti iscritte a bilancio | 15.903 | 16.543 | 17.190 |
| Scostamento | −730 (−4,4%) | **+1.952 (+13,4%)** | **−18.917 (−52,4%)** |

Il 2023 è l'anno di taratura: il modello sovrastima del 4,4%, scarto attribuibile a variazioni in
diminuzione minori non visibili nel bilancio micro. Correggendo il 2025 per lo stesso fattore, il
carico ordinario atteso scende a **34.520** e lo scostamento a **17.330**. Da qui la forchetta
17.300-18.900 di E-6.

**Prova di robustezza.** Se i compensi dei tre amministratori diversi da Pradella fossero reddito
di lavoro autonomo anziché reddito assimilato (ipotesi resa concreta dalla circolare 105/E/2001 —
vedi R-5), sarebbero deducibili ai fini IRAP: la base 2025 scenderebbe a ≈153.300, l'IRAP a 6.255,
l'IRES a 29.298 e il totale a **35.553**. Lo scostamento resterebbe **18.363**. La conclusione del
§ 3 regge in entrambe le ipotesi.

### 1. La metrica corretta

Il confronto va costruito su un **euro di reddito ante imposte della società**, identico nelle due
colonne. Dimostrazione formale, con M = margine operativo prima di qualunque prelievo verso i soci
e F = importo del canale attivato, e con t = 28,08% (IRES 24% + IRAP 4,08%):

- **canale fattura**: reddito ante imposte = M − F ; utile netto trattenuto = (1 − t) · (M − F) ;
  il socio incassa il netto della fattura
- **canale dividendo**: reddito ante imposte = M ; utile netto = (1 − t) · M ; se ne distribuisce
  la quota eccedente, cioè (1 − t) · F, e resta in società (1 − t) · (M − F)

**In entrambi i casi la società trattiene lo stesso importo.** Il confronto è quindi puro e
riguarda solo quanto arriva al socio. Il documento invece divide 72,1 per 47 nella prima colonna e
100 per 53,4 nella seconda: due metriche, un risultato predeterminato.

### 2. Parametri usati, tutti verificati

| Parametro | Valore | Fonte verificata |
|---|---|---|
| IRES | 24% | art. 77 TUIR |
| IRAP Veneto dal 2025 | **4,08%** | art. 16 D.Lgs. 446/1997 + art. 2 L.R. Veneto 32/2024 (3,90% + 0,18%) |
| Prelievo societario marginale combinato | **28,08%** | somma delle due; sul margine nessuna delle due riduce la base dell'altra |
| Ritenuta a titolo d'imposta sui dividendi | 26% | art. 27, c. 1, DPR 600/1973 (testo L. 205/2017, c. 1003) |
| IRPEF 2026 | 23% fino a 28.000; **33%** da 28.000 a 50.000; 43% oltre | art. 11, c. 1, TUIR come modificato dall'art. 1, c. 3, L. 199/2025 |
| Addizionali regionale + comunale | ≈ 2 punti (stima) | *da verificare per Veneto, Verona, Villafranca e Padova* |
| Inarcassa — contributo soggettivo 2026 | **14,50%**, deducibile ex art. 10, c. 1, lett. e), TUIR | Inarcassa, tabella contributi 2026 |
| Inarcassa — massimale reddituale 2026 | **147.300 euro**; **oltre il massimale il contributo soggettivo NON è più dovuto** (nessuna aliquota ridotta dal 2013) | Regolamento generale previdenza Inarcassa, art. 4.1 |
| Inarcassa — contributo integrativo | **4%** sul volume d'affari, ripetibile verso il committente, **non concorre al reddito** del professionista (art. 54, c. 2, lett. a), TUIR) | R.G.P. Inarcassa, art. 5.6 |
| Gestione separata INPS 2026 — professionista senza altra copertura | **26,07%** | circ. INPS 3 febbraio 2026 n. 8 |
| Gestione separata INPS 2026 — co.co.co. e amministratori senza altra copertura | **35,03%** (33 IVS + 0,50 + 0,22 + 1,31 DIS-COLL: gli amministratori la scontano) | circ. INPS n. 8/2026 |
| Gestione separata INPS 2026 — già iscritti ad altra gestione o pensionati | **24,00%** | art. 1, c. 79, L. 247/2007 |
| Ripartizione co.co.co. | 2/3 committente, 1/3 collaboratore | art. 2, c. 30, L. 335/1995 |
| Massimale gestione separata 2026 | 122.295 euro | circ. INPS n. 8/2026 |

**Dato verificato sul cedolino**: a Pradella è trattenuto sul compenso di luglio 2026 un contributo
di 216,72 euro su 2.709,00, pari all'**8,00% esatto**, cioè un terzo del 24%. **È la prova che
Pradella è già iscritto ad altra forma pensionistica obbligatoria o è titolare di pensione.**

**Correzione a un errore ricorrente che il documento non commette ma che va evitato nella
riscrittura:** non esiste alcuna aliquota ridotta né contributo di solidarietà Inarcassa oltre il
massimale. Il sistema a due aliquote (3% sull'eccedenza) è **abolito dal 1° gennaio 2013**. Oltre
il massimale reddituale il contributo soggettivo semplicemente **non è più dovuto**, e questo
cambia il segno del confronto per i redditi alti.

### 3. Scenario A — tassazione ordinaria (fuori CPB). Per 100 euro di reddito ante imposte

| | Fattura del socio (Inarcassa) | Dividendo |
|---|---:|---:|
| Compenso lordo erogabile (100 = compenso + 4% integrativo) | 96,15 | — |
| Contributo integrativo Inarcassa 4% (a Inarcassa, non al socio) | 3,85 | — |
| Contributo soggettivo 14,5% (deducibile) | −13,94 | — |
| Imponibile IRPEF | 82,21 | — |
| IRES + IRAP 28,08% | — | −28,08 |
| Utile distribuibile | — | 71,92 |
| Ritenuta 26% | — | −18,70 |
| **Netto al socio, m = 25% (primo scaglione + addizionali)** | **61,66** | **53,22** |
| **Netto al socio, m = 35% (secondo scaglione 33% + addizionali)** | **53,44** | **53,22** |
| **Netto al socio, m = 45% (terzo scaglione 43% + addizionali)** | **45,22** | **53,22** |
| **Costo per euro netto, m = 45%** | **2,21** | **1,88** |

Ignorando il contributo integrativo — cioè con i parametri esatti del documento — il netto della
fattura a m = 45% è 100 × 0,855 × 0,55 = **47,03** e il costo per euro netto è **2,13**, non 1,53.

**Soglie di inversione (aliquota marginale complessiva del socio alla quale i due canali si
equivalgono):**

| Configurazione previdenziale del socio | Soglia *m** | Sotto la soglia vince |
|---|---:|---|
| Inarcassa 14,5%, integrativo a carico della società | **35,3%** | la fattura |
| Inarcassa 14,5%, integrativo ignorato (ipotesi del documento) | **37,8%** | la fattura |
| Gestione separata INPS 26,07% | **28,0%** | la fattura |
| **Inarcassa oltre il massimale di 147.300** (soggettivo non più dovuto) | **44,6%** | la fattura |

Con la struttura IRPEF 2026 (23 / **33** / 43) la soglia del 35,3% cade **esattamente sul secondo
scaglione**: 33% di IRPEF più circa 2 punti di addizionali fa 35%, cioè la parità. **Il risultato
netto è che sotto i 50.000 euro di reddito complessivo i due canali si equivalgono, e sopra i
50.000 il dividendo vince nettamente.** La riduzione della seconda aliquota dal 35% al 33%
operata dalla L. 199/2025 ha spostato la soglia di due punti a favore della fattura, ma non basta
a cambiare l'esito per i redditi alti.

**Dalla Piazza dichiara 131.816 euro di reddito complessivo effettivo (CP10 col. 6): per lui il
dividendo vince già oggi, in tassazione ordinaria.** L'ultima riga della tabella è però decisiva e
il § 4.3 non la contiene: il suo reddito professionale effettivo 2024 è 118.111, cioè **29.189 euro
sotto il massimale Inarcassa di 147.300**. Fatturare oltre quella soglia azzera il contributo
marginale e riporta i due canali quasi in parità (52,88 contro 53,22). **Il parametro che decide
non è l'aliquota IRPEF: è la distanza del socio dal massimale contributivo.**

### 4. Scenario B — società in CPB, socio in tassazione ordinaria. Per 100 euro di reddito ante imposte

| | Fattura del socio | Dividendo su utile eccedente |
|---|---:|---:|
| Risparmio d'imposta per la società | zero (base fissa, art. 19, c. 1) | — |
| IRES + IRAP sull'eccedenza | — | **zero** |
| Utile distribuibile | — | 100,00 |
| Ritenuta 26% | — | −26,00 |
| **Netto al socio, m = 45%** | **45,22** | **74,00** |
| **Costo per euro netto** | **2,21** | **1,35** |

Soglia di inversione: 82,21 · (1 − m) = 74,00 → m = **10,0%**, cioè al di sotto della minima
aliquota IRPEF. **Il dividendo vince a qualunque aliquota.** La conclusione del documento è
corretta in questo scenario, e va anzi rafforzata: non è «conviene il dividendo», è «il dividendo
conviene sempre, senza eccezioni».

### 5. Scenario C — società E socio entrambi in CPB. Per 100 euro di reddito ante imposte

È lo scenario reale se entrambi aderiscono al biennio 2026-2027, ed è coerente con quanto è già
accaduto nel 2024 (il quadro CP di Dalla Piazza lo prova per lui; il profilo dei tax rate lo rende
probabile per la società).

Per il socio in concordato, il compenso incassato in eccedenza rispetto al proprio reddito
concordato **non rileva né ai fini IRPEF né ai fini dei contributi previdenziali obbligatori**
(art. 19, c. 1, D.Lgs. 13/2024, testo riportato in R-2).

| | Fattura del socio | Dividendo su utile eccedente |
|---|---:|---:|
| Compenso lordo (netto del 4% integrativo) | 96,15 | — |
| IRPEF sull'eccedenza | **zero** | — |
| Contributi obbligatori sull'eccedenza | **zero** (facoltativi) | — |
| Ritenuta 26% | — | −26,00 |
| **Netto al socio** | **96,15** | **74,00** |
| **Costo per euro netto** | **1,04** | **1,35** |
| Variante: il socio versa comunque il soggettivo 14,5% | 82,21 → **1,22** | **1,35** |

**Con entrambi in concordato la fattura batte il dividendo del 30% (o del 10% se il socio versa
comunque i contributi).** È l'esatto contrario della conclusione del documento, e riguarda proprio
la configurazione che il documento ritiene più probabile.

**Cinque limiti da dichiarare al cliente, che non sono opzionali:**

1. **Capienza.** Il vantaggio esiste solo finché il reddito effettivo della società resta **sopra**
   il concordato e il reddito effettivo del socio resta **sopra** il suo. Se la proposta 2026-2027
   fosse ancorata al reddito effettivo 2025 (R-4), la capienza sul lato società potrebbe essere
   prossima a zero e questo scenario **non si aprirebbe affatto**.
2. **Cessazione per crollo del reddito.** L'art. 19, c. 2, D.Lgs. 13/2024 fa cessare il concordato
   se circostanze eccezionali individuate con decreto MEF determinano minori redditi effettivi
   eccedenti il **30 per cento** (non il 50) rispetto al concordato. Comprimere il reddito con
   fatture non è una circostanza eccezionale: non produce cessazione, produce **perdita secca**,
   perché l'imposta resta dovuta sul concordato.
3. **Effetto sul biennio successivo.** Il maggior reddito effettivo del socio alza la base su cui
   sarà elaborata la proposta 2028-2029 (art. 9, c. 3-*bis*, e art. 20-*bis*, c. 2).
4. **Sostanza.** Il vantaggio si costruisce solo su prestazioni **effettivamente rese e
   documentate**. Aumentare il canale fattura senza aumentare la prestazione ricade nell'art. 22,
   c. 1, lett. a), con la decadenza descritta in N-1: il 30% dei ricavi 2025 vale 126.390 euro.
5. **Contributi.** Rinunciare al versamento sul reddito effettivo aumenta la cassa di oggi e riduce
   il montante pensionistico. Va aggiunto che l'art. 35, c. 2, D.Lgs. 13/2024 fa rilevare il
   reddito **effettivo** «per il riconoscimento della spettanza o per la determinazione di
   deduzioni, detrazioni o benefici di qualsiasi titolo, **anche di natura non tributaria**» e ai
   fini **ISEE**: c'è quindi un'asimmetria — contributi sul concordato, ISEE e detrazioni
   sull'effettivo — che va spiegata a soci con figli a carico o con prestazioni collegate all'ISEE.
   **D01 non nomina l'art. 35.**

### 6. Il terzo canale, assente dal documento: il compenso di amministratore

Per 100 euro di reddito ante imposte, con m = 45%:

| | Gestione separata piena 35,03% | Aliquota ridotta 24% (caso Pradella) |
|---|---:|---:|
| Contributo a carico della società (2/3) | 23,35% | 16,00% |
| Compenso lordo erogabile | 81,07 | 86,21 |
| Contributo a carico del socio (1/3, deducibile) | −9,47 | −6,90 |
| Imponibile IRPEF | 71,60 | 79,31 |
| IRPEF + addizionali 45% | −32,22 | −35,69 |
| **Netto al socio** | **39,38** | **43,62** |
| **Costo per euro netto** | **2,54** | **2,29** |

**È il canale peggiore in ogni scenario**, e resta il peggiore anche sotto CPB, perché il compenso
di amministratore è reddito assimilato a lavoro dipendente e **non rientra nel reddito di lavoro
autonomo concordato del socio**: non gode dell'esenzione dell'art. 19, c. 1. *(Se però opera la
riqualificazione della circolare 105/E — vedi R-5 — il compenso diventa reddito di lavoro autonomo
e rientra nel concordato del socio: un'altra ragione per risolvere quella questione prima di
progettare qualunque manovra.)*

Va inoltre citato l'**art. 95, c. 5, TUIR**, che il documento non nomina mai (testo verbatim in
G-10): deducibilità **per cassa**.

Va infine letto insieme al § 5.1: i compensi di amministratore sono il presidio difensivo che
distingue l'attività gestoria dalla prestazione tecnica. **Comprimerli per ragioni fiscali
indebolisce la difesa; mantenerli costa 2,29-2,54 euro per euro netto.** Il trade-off va scritto,
non risolto d'ufficio in un senso o nell'altro.

### 7. Sintesi del modello rifatto — costo per euro netto in tasca al socio

| Scenario | Fattura del socio | Dividendo | Compenso amministratore | Vince |
|---|---:|---:|---:|---|
| Ordinario, socio con marginale 25% | 1,62 | 1,88 | 2,29 | **fattura** |
| Ordinario, socio con marginale 35% | 1,87 | 1,88 | ~2,40 | **parità** |
| Ordinario, socio con marginale 45% | 2,21 | 1,88 | 2,29 | **dividendo** |
| Ordinario, socio oltre il massimale Inarcassa, marginale 45% | 1,89 | 1,88 | 2,29 | **parità** |
| Società in CPB, socio ordinario 45% | 2,21 | **1,35** | 2,29 | **dividendo**, sempre |
| **Società e socio in CPB** | **1,04** | 1,35 | 2,29 | **fattura**, con margine del 30% |

Le due righe che il documento sbaglia sono la terza (dice fattura, è dividendo) e l'ultima (dice
dividendo, è fattura).

---

## Verifica normativa

Tutte le norme del D.Lgs. 13/2024 sono state riscontrate sul **testo multivigente al 9 settembre
2026** (versione «in vigore dal 12-8-2026 al 31-12-2026»). Le citazioni di D01 sono confrontate
con quel testo.

### Art. 7-*bis*, c. 3, D.L. 27 marzo 2026 n. 38 (conv. L. 22 maggio 2026 n. 88) — **CONFERMATO**: il § 6 di D01 è corretto

> «Per il biennio 2026-2027 il termine per aderire alla proposta di concordato, di cui all'articolo
> 9, comma 3, del decreto legislativo 12 febbraio 2024, n. 13, è differito al **31 ottobre 2026**
> ovvero all'ultimo giorno del decimo mese successivo a quello di chiusura del periodo d'imposta
> per i soggetti con periodo d'imposta non coincidente con l'anno solare.»

Estremi confermati: D.L. 27 marzo 2026 n. 38, convertito con modificazioni dalla L. 22 maggio 2026
n. 88, in G.U. n. 117 del 22 maggio 2026, in vigore dal 23 maggio 2026. L'art. 7-*bis* è stato
inserito in sede di conversione ed è composto di tre commi. **La data del 31 ottobre 2026 indicata
da D01 è corretta.**

Va aggiunto ciò che D01 non dice: **il termine ordinario dell'art. 9, c. 3, D.Lgs. 13/2024 resta il
30 settembre** e non è stato modificato («Il contribuente può aderire alla proposta di concordato
entro il 30 settembre …»). Il 31 ottobre 2026 è una **deroga speciale al solo biennio 2026-2027**:
non è una regola su cui costruire aspettative per i bienni successivi.

**Sono corrette anche le altre due affermazioni del § 6:**

- i «tetti agli incrementi della proposta per i contribuenti con punteggi ISA più bassi» sono
  stati introdotti dall'**art. 7-*bis*, c. 1**, che aggiunge all'art. 9, c. 3-*bis*, D.Lgs.
  13/2024 le lett. c-*bis*) (30% per ISA ≥ 6 e < 8) e c-*ter*) (35% per ISA ≥ 1 e < 6);
- l'estensione al CPB della deducibilità dell'iperammortamento è nello stesso decreto, ma
  all'**art. 7, comma 3-*bis***, che inserisce la lett. b-*ter*) nell'art. 16 D.Lgs. 13/2024. *La
  precisazione conta: la modifica riguarda solo l'art. 16 (reddito d'impresa) e non l'art. 15
  (lavoro autonomo).*

### Slittamento del termine al 2 novembre 2026 — **CONFERMATO**, con la citazione corretta

Il calendario è verificato: **31 ottobre 2026 sabato**, 1° novembre 2026 domenica e festivo, primo
giorno lavorativo successivo **lunedì 2 novembre 2026**.

La base normativa non è una sola disposizione. L'**art. 7, c. 1, lett. h), del D.L. 70/2011**
(conv. L. 106/2011) è la norma-principio; la norma **operativa** è l'**art. 7, c. 2, lett. l)**,
dello stesso decreto:

> «gli adempimenti ed i versamenti previsti da disposizioni relative a materie amministrate da
> articolazioni del Ministero dell'economia e delle finanze, comprese le Agenzie fiscali,
> **ancorché previsti in via esclusivamente telematica**, ovvero che devono essere effettuati nei
> confronti delle medesime articolazioni o presso i relativi uffici, i cui termini scadono di
> sabato o di giorno festivo, sono prorogati al primo giorno lavorativo successivo»

Entrambe coprono gli **adempimenti** e non solo i versamenti: l'adesione al CPB, che è adempimento
telematico verso l'Agenzia, vi rientra. **D01 non cita alcuna norma a sostegno dello slittamento:
va aggiunta questa**, perché fra il 31 ottobre e il 2 novembre corrono due giorni su un termine
decadenziale. *Non risulta un atto dell'Agenzia che dichiari espressamente il 2 novembre: la data
discende da norma più calendario.*

### Art. 19 D.Lgs. 13/2024 — **CONFERMATO**, e D01 lo cita al contrario

Comma 1, verbatim (testo integrale in R-2): i maggiori o minori redditi effettivi non rilevano
«ai fini della determinazione delle imposte sui redditi e dell'imposta regionale sulle attività
produttive, **nonché dei contributi previdenziali obbligatori**. Resta ferma la **possibilità** per
il contribuente di versare i contributi sul reddito effettivo se di importo superiore a quello
concordato». **L'affermazione del § 6, punto 4, di D01 è falsa.**

**Comma 2 — la soglia vigente è il 30 per cento, non il 50.** Testo vigente: «In presenza di
circostanze eccezionali, individuate con decreto del Ministro dell'economia e delle finanze, che
determinano minori redditi effettivi o minori valori della produzione netta effettivi, eccedenti la
misura del **30 per cento** rispetto a quelli oggetto del concordato, quest'ultimo cessa di
produrre effetti a partire dal periodo di imposta in cui tale differenza si realizza.» Le
circostanze eccezionali per il biennio 2026-2027 sono elencate all'art. 4 del D.M. MEF 11 maggio
2026, che vi ha aggiunto la lett. g) sugli impatti economici dei conflitti armati nell'area
mediorientale.

**Comma 3 — i benefici premiali.** «Per i periodi d'imposta oggetto di concordato, ai contribuenti
che aderiscono alla proposta … sono riconosciuti i benefici, **compresi quelli relativi all'imposta
sul valore aggiunto**, previsti dall'articolo 9-*bis*, comma 11, del decreto-legge 24 aprile 2017,
n. 50». Vedi N-3 per l'elenco.

### Art. 20-*bis* D.Lgs. 13/2024 — **CONFERMATO**, con un tetto che D01 non conosce

Comma 1: imposta sostitutiva sulla parte di reddito concordato eccedente il reddito dichiarato nel
periodo antecedente, rettificato ex artt. 15 e 16, con aliquota **10%** se il punteggio ISA del
periodo antecedente è ≥ 8, **12%** se ≥ 6 e < 8, **15%** se < 6. È la norma che spiega il «10»
riportato in CP2 col. 4 del quadro CP 2024 di Dalla Piazza (E-4).

Comma 1-*bis*, introdotto dal D.Lgs. 81/2025: «Le aliquote dell'imposta sostitutiva di cui al comma
1 si applicano nei limiti di un'**eccedenza non superiore a 85.000 euro**. Nel caso in cui
l'eccedenza sia superiore a 85.000 euro, e limitatamente alla parte che supera tale importo,
l'imposta sostitutiva si applica: a) per i contribuenti assoggettati all'IRPEF, con l'aliquota di
cui all'articolo 11, comma 1, lettera c) [43%]; b) per i contribuenti assoggettati all'IRES, con
l'aliquota di cui all'articolo 77 [24%]». **Decorrenza: dalle adesioni al biennio 2025-2026**,
quindi si applica al 2026-2027. Il tetto opera sulla base imponibile, non sull'imposta.

Comma 2, per il rinnovo: il parametro è «il **reddito effettivo dichiarato** nel periodo d'imposta
antecedente a quelli del biennio di rinnovo del concordato, rettificato secondo quanto disposto
dagli articoli 15 e 16».

**L'art. 31-*bis* e l'intero Capo III (CPB dei forfetari, artt. 23-33) sono ABROGATI** dal D.Lgs.
12 giugno 2025 n. 81: il CPB dei forfetari ha riguardato il solo periodo d'imposta 2024. Irrilevante
per Overall Group, ma rilevante per eventuali soci in regime forfetario.

### Artt. 10, 11, 21 e 22 D.Lgs. 13/2024 — testo vigente e applicazione a Overall Group

**Art. 10, c. 2 (requisito sui debiti — non è causa di esclusione, è requisito di accesso).**
Non possono accedere i contribuenti che hanno debiti per tributi amministrati dall'Agenzia o debiti
contributivi; rilevano solo i debiti «definitivamente accertati con sentenza irrevocabile o con
atti impositivi non più soggetti a impugnazione»; è comunque ammesso chi li ha estinti entro il
termine di adesione se il debito residuo, compresi interessi e sanzioni, è **inferiore alla soglia
di 5.000 euro**; e «**non concorrono al predetto limite i debiti oggetto di provvedimenti di
sospensione o di rateazione** sino a decadenza dei relativi benefici». Il nuovo c. 2-*bis*
(D.Lgs. 148/2026) aggiunge che l'adesione in assenza dei requisiti «è priva di effetti».
*La voce 9 del § 7 di D01 va corretta di conseguenza: vedi G-11.*

**Art. 11 — cause di esclusione, elenco vigente completo.** D01 non ne cita nessuna. Le rilevanti
per questa società:

| Lettera | Contenuto | Rilievo per Overall Group |
|---|---|---|
| a) | mancata presentazione della dichiarazione dei redditi in almeno uno dei tre periodi precedenti | da verificare sul cassetto fiscale |
| b) | condanna per reati D.Lgs. 74/2000, art. 2621 c.c., artt. 648-*bis*, 648-*ter*, 648-*ter*.1 c.p. commessi negli ultimi tre periodi; equiparato il patteggiamento | **va chiesto ai quattro amministratori. D01 non lo chiede** |
| b-*bis*) | redditi esenti, esclusi o non concorrenti alla base imponibile in misura superiore al **40%** del reddito d'impresa | non emerge dal bilancio |
| b-*ter*) | adesione al regime forfetario nel primo periodo del concordato | non applicabile |
| b-*quater*) | fusione, scissione, conferimento nel primo anno, **ovvero modifiche della compagine sociale che aumentano il numero dei soci** (salvo il subentro di due o più eredi) | **direttamente rilevante**: con quattro soci di 66, 62, 55 e 41 anni, un ingresso in compagine nel 2026 esclude l'accesso, e nel biennio ne provoca la cessazione (art. 21, lett. b-*ter*). D01 discute lo stallo societario del § 1 senza collegarlo |
| b-*quinquies*) e b-*sexies*) | partecipazione a associazioni professionali, STP o STA con adesione disallineata | rilevante solo se un socio partecipa a una STP: **da verificare, vedi G-12** |

Il nuovo c. 1-*bis* (D.Lgs. 148/2026) dispone che «l'adesione al concordato in presenza di una
delle cause di esclusione di cui al comma 1 è priva di effetti».

**Art. 21 — cessazione.** Lettere vigenti: a) modifica dell'attività nel biennio, con la
salvaguardia «se per le nuove attività è prevista l'applicazione del **medesimo indice sintetico di
affidabilità fiscale**» (il criterio è l'ISA, non il codice ATECO — rilevante per l'attività
secondaria di intermediazione rifiuti, vedi G-11); b) cessazione dell'attività; b-*bis*) adesione
al forfetario; b-*ter*) operazioni straordinarie o aumento del numero dei soci; b-*quater*) ricavi
superiori alla soglia ISA maggiorata del 50% (**7.746.853,50 euro**: lontanissima);
b-*quinquies*)/b-*sexies*) disallineamento con associazioni, STP e STA.

**Art. 22 — decadenza**, nel testo applicabile **dal biennio 2026-2027**: a) accertamento, nei
periodi concordati o in quello precedente, di attività non dichiarate o passività inesistenti o
indeducibili «per un importo superiore al **30 per cento dei ricavi o compensi dichiarati**»;
b) accertamento nel periodo precedente di errori od omissioni nei dati comunicati tali che il
reddito o il VPN ricalcolati risultino superiori di almeno il 30% al concordato; c) altre
violazioni di non lieve entità di cui al c. 2; **d) LETTERA SOPPRESSA dal D.Lgs. 7 agosto 2026 n.
148**; e) omesso versamento delle somme ex art. 12, c. 2, non pagato entro 60 giorni.
Il c. 2 elenca le violazioni di non lieve entità (fra cui le fattispecie del D.Lgs. 74/2000 nei
periodi concordati e la comunicazione inesatta dei dati ISA oltre il 30%); il **c. 3** salva le
violazioni regolarizzate con ravvedimento operoso purché non già constatate e purché non siano
iniziati accessi, ispezioni o verifiche; il **c. 3-*bis*** stabilisce che «nel caso di decadenza dal
concordato **restano dovute le imposte e i contributi determinati tenendo conto del reddito e del
valore della produzione netta concordati se maggiori di quelli effettivamente conseguiti**».

**Il doppio binario introdotto dal D.Lgs. 7 agosto 2026 n. 148** (art. 28, c. 3: le nuove
disposizioni «si applicano a decorrere dal biennio d'imposta 2026-2027») è la novità più rilevante
per chi decide oggi, e D01 non la conosce:

| Fattispecie | Biennio 2025-2026 | **Biennio 2026-2027** |
|---|---|---|
| Dichiarazione integrativa che modifica i dati | decadenza | **non più decadenza**: rideterminazione del concordato ex art. 19, c. 3-*bis*, con sanzioni ravvedibili |
| Dati in dichiarazione non corrispondenti a quelli comunicati | decadenza | sostituita: servono accertamento e soglia del 30% |
| Sopravvenienza di una causa di esclusione o venir meno dei requisiti | decadenza | **inefficacia originaria** (artt. 10, c. 2-*bis*, e 11, c. 1-*bis*) |
| Maggiori redditi accertati oltre il 30% | decadenza | invariata, ma estesa anche ai «compensi» |

### Art. 14 D.Lgs. 13/2024 — rinnovo: **CONFERMATO**, e i benefici sono maggiori di quelli base

Comma 1: «Decorso il biennio oggetto di concordato, permanendo i requisiti di cui all'articolo 10 e
in assenza delle cause di esclusione di cui all'articolo 11, l'Agenzia delle entrate formula … una
nuova proposta di concordato biennale relativa al biennio successivo, a cui il contribuente può
aderire nei termini di cui all'articolo 9, comma 3.» **Chi ha aderito al 2024-2025 può quindi
aderire al 2026-2027.**
Comma 1-*bis*: benefici premiali potenziati (visto di conformità fino a 100.000 euro IVA e 70.000
imposte dirette; rimborsi IVA fino a 100.000; **anticipazione di due anni** dei termini di
accertamento).
Comma 1-*ter*: per il rinnovo relativo al biennio 2026-2027 **non sono dovuti interessi** sui
versamenti rateali.
Art. 20, c. 3-*bis*: in caso di rinnovo **non si applica la maggiorazione d'acconto** del primo
anno.

### Art. 9, c. 3-*bis*, D.Lgs. 13/2024 — il tetto alla proposta, e la domanda aperta

Testo e tabella delle percentuali in R-4. **La grandezza cui il tetto si àncora per gli ex
aderenti 2024-2025 — reddito effettivo o reddito concordato 2025 — resta NON VERIFICATA**, ed è la
questione che decide l'intera raccomandazione.

### Art. 18 D.Lgs. 13/2024 — il CPB non produce effetti ai fini IVA

Comma unico, verbatim: «L'adesione al concordato **non produce effetti ai fini dell'imposta sul
valore aggiunto**, la cui applicazione avviene secondo le regole ordinarie.» È la base del rilievo
N-2. L'unica rilevanza IVA in senso favorevole è quella dei benefici premiali (art. 19, c. 3).

### Art. 34 D.Lgs. 13/2024 — preclusione degli accertamenti, e l'avvertimento che contiene

Comma 1: «Per i periodi di imposta oggetto del concordato, gli accertamenti di cui all'articolo 39
del decreto del Presidente della Repubblica 29 settembre 1973, n. 600, **non possono essere
effettuati** salvo che in esito all'attività istruttoria dell'Amministrazione finanziaria ricorrano
le cause di decadenza di cui agli articoli 22 e 33.»
Comma 2: l'Agenzia e la Guardia di Finanza programmano maggiore capacità operativa per
**intensificare i controlli nei confronti di chi non aderisce o decade**.

Due letture, entrambe assenti da D01: la preclusione copre **solo l'art. 39 DPR 600/1973** —
restano possibili accessi, ispezioni e verifiche, accertamenti su altre categorie reddituali,
accertamenti IVA e controlli ex artt. 36-*bis* e 36-*ter*; e la norma dichiara espressamente che
**non aderire aumenta la probabilità di controllo**. È un argomento a favore dell'adesione che il
documento non usa, ed è anche un dato che il cliente ha diritto di conoscere.

### Art. 35, c. 2, D.Lgs. 13/2024 — l'asimmetria che D01 non nomina

> «Agli effetti del presente decreto, quando le vigenti disposizioni fanno riferimento, per il
> riconoscimento della spettanza o per la determinazione di deduzioni, detrazioni o benefici di
> qualsiasi titolo, **anche di natura non tributaria**, al possesso di requisiti reddituali, si
> tiene comunque conto del **reddito effettivo** e non di quello concordato. Il reddito effettivo
> rileva anche ai fini dell'indicatore della situazione economica equivalente (I.S.E.E.) …»

Contributi previdenziali sul **concordato**; ISEE, detrazioni, deduzioni e benefici anche non
tributari sull'**effettivo**. Va detto ai soci.

### Art. 95, c. 5, TUIR — **CONFERMATO**

Testo verbatim riportato in G-10. Deducibilità **per cassa** dei compensi agli amministratori.
D01 non lo cita mai.

### Art. 105, c. 4, e art. 17, c. 1, lett. c), TUIR — la citazione di D01 è **ERRATA**

Testo verbatim dell'art. 105, c. 4: «**Le disposizioni dei commi 1 e 2 valgono anche per gli
accantonamenti relativi alle indennità di fine rapporto di cui all'articolo 17, comma 1, lettere
c), d) e f).**» Nient'altro. Il requisito sta nell'**art. 17, c. 1, lett. c)**: «indennità percepite
per la cessazione dei rapporti di collaborazione coordinata e continuativa … **se il diritto
all'indennità risulta da atto di data certa anteriore all'inizio del rapporto**». Il requisito di
deducibilità per competenza discende quindi dal **combinato disposto**, non dall'art. 105, c. 4.

Giurisprudenza confermata: Cass. n. 19571/2022 («purché la previsione di detto trattamento risulti
da un atto scritto avente data certa anteriore all'inizio del rapporto, **che ne specifichi anche
l'importo**»); Cass. ord. n. 19445/2023 (non basta che il TFM sia attribuito nella stessa assemblea
di nomina); Cass. sez. V n. 15966/2024; Cass. n. 4487/2025; Cass. ord. n. 16354/2025; Cass. ord.
n. 18026/2025. **Orientamento contrario confermato ed esistente**: Cass., sez. V, ord. n.
3788/2023, che scinde la deducibilità (art. 105) dalla tassazione separata (art. 17), restando
minoritaria e isolata. Nessuna pronuncia del 2026 reperita.

### Art. 50, c. 1, lett. c-*bis*), TUIR e circolare 105/E/2001 — l'affermazione di D01 è **ERRATA per questa società**

Vedi R-5 per il testo della norma, il passaggio della circolare e le conseguenze.

### Art. 2477 c.c. — soglie **CONFERMATE e invariate**

Testo vigente (introdotto dall'art. 2-*bis* D.L. 32/2019, conv. L. 55/2019): l'obbligo scatta se la
società «ha superato per **due esercizi consecutivi** almeno uno dei seguenti limiti: 1) totale
dell'attivo dello stato patrimoniale: **4 milioni di euro**; 2) ricavi delle vendite e delle
prestazioni: **4 milioni di euro**; 3) dipendenti occupati in media durante l'esercizio: **20
unità**», e cessa «quando, per tre esercizi consecutivi, non è superato alcuno dei predetti
limiti». Nessuna modifica nel 2025 né nel 2026. **La conclusione di D01 è corretta**: vedi G-13 per
la quantificazione.
*Segnalazione da riscontrare: il D.Lgs. 47/2026 avrebbe abrogato l'art. 2409 c.c., cui rinvia il
sesto comma dell'art. 2477 — **NON VERIFICATO**, solo fonte secondaria.*

### Art. 27, c. 1, DPR 600/1973 — ritenuta del **26% CONFERMATA** per il 2026

Testo vigente: le società operano «con obbligo di rivalsa, **una ritenuta del 26 per cento a titolo
d'imposta sugli utili in qualunque forma corrisposti** … a persone fisiche residenti in relazione a
partecipazioni qualificate e non qualificate … non relative all'impresa». Il 26% è scritto
letteralmente nel comma, per effetto della riscrittura operata dall'art. 1, c. 1003, L. 205/2017;
non c'è alcun rinvio all'art. 3 del D.L. 66/2014. **Il regime transitorio del c. 1006 è esaurito**
(riguardava le sole distribuzioni deliberate dal 1° gennaio 2018 al 31 dicembre 2022): nel 2026
tutte le distribuzioni a persone fisiche non imprenditori scontano il 26% secco. La L. 199/2025 non
ha toccato la norma. **Il calcolo del § 4.1 di D01 è corretto** (E-3).

### IRPEF 2026 — la seconda aliquota è scesa al **33%**, e D01 non ne tiene conto

Art. 11, c. 1, TUIR vigente: «a) fino a 28.000 euro, **23 per cento**; b) oltre 28.000 euro e fino a
50.000 euro, **33 per cento**; c) oltre 50.000 euro, **43 per cento**». La modifica è dell'art. 1,
c. 3, L. 30 dicembre 2025 n. 199, che ha sostituito «35 per cento» con «33 per cento». Struttura
ancora a tre scaglioni. Per i redditi complessivi superiori a 200.000 euro il beneficio è
sterilizzato riducendo di 440 euro le detrazioni al 19% (art. 1, c. 4, L. 199/2025, che inserisce
il c. 5-*bis* nell'art. 16-*ter* TUIR): **rilevante per Dalla Piazza solo se il reddito complessivo
supera i 200.000, oggi non è il caso (131.816)**.

Effetto sul § 4.3: la soglia di indifferenza fra fattura e dividendo si è spostata di due punti a
favore della fattura, ma non cambia l'esito per un socio nel terzo scaglione.

### IRAP — **dovuta**, aliquota Veneto **4,08%**

L'IRAP è pienamente dovuta dalle società di capitali nel 2025 e nel 2026: il principio di delega
dell'art. 8 L. 111/2023 sul «graduale superamento dell'imposta» **non è stato attuato**, e il
legislatore l'ha anzi aumentata per banche, assicurazioni e comparto energetico. L'esclusione
riguarda solo le persone fisiche (art. 1, c. 8, L. 234/2021). Aliquota Veneto: vedi E-6.
*La conferma numerica sulle tabelle MEF per il 2026 è **NON VERIFICATA**; la vigenza è dedotta
dalla norma regionale a regime e dall'assenza di leggi regionali successive.*

### IRES premiale 2025 — condizioni **CONFERMATE**, e Overall Group ne fallisce **due**

Art. 1, c. 436, L. 207/2024: aliquota ridotta di 4 punti (24% → 20%) al ricorrere di entrambe le
condizioni: (a) accantonamento a riserva di almeno l'**80% degli utili 2024**; (b) destinazione a
investimenti in beni 4.0/5.0 (allegati A e B L. 232/2016 e art. 38 D.L. 19/2024) di un ammontare
non inferiore al 30% degli utili accantonati e comunque non inferiore al 24% degli utili 2023, con
un minimo assoluto di **20.000 euro**.
Art. 1, c. 437: in aggiunta, (a) le ULA non devono diminuire rispetto alla media del triennio; **si
devono effettuare nuove assunzioni a tempo indeterminato pari almeno all'1% dei dipendenti a tempo
indeterminato e comunque non inferiori a un lavoratore**; (b) **divieto di ricorso alla cassa
integrazione** nel 2024 e nel 2025 (salva la CIG ordinaria per situazioni temporanee di mercato).

**Overall Group fallisce due condizioni su quattro**: gli acquisti di immobilizzazioni 2025 valgono
6.024 euro contro il minimo di 20.000, e non risultano assunzioni a tempo indeterminato nel 2025
(la visura certifica 2 dipendenti al 30/06/2025; Carli Anna è assunta il 06/07/2026). L'esclusione
di G-7 è confermata e rafforzata.

**La misura non è stata prorogata al 2026**: la verifica testuale integrale dell'art. 1 della L.
199/2025 non contiene alcun richiamo ai commi 436-444 né alle formule «riduzione dell'aliquota»,
«apposita riserva» o «unità lavorative per anno». Dal 2026 si torna al 24%.

### Super-deduzione nuove assunzioni — **CONFERMATA**, insufficiente, e con una scadenza anticipata

Art. 4 D.Lgs. 216/2023: maggiorazione del **20%** del costo riferibile all'incremento occupazionale
«**ai fini della determinazione del reddito**», elevabile fino al **30%** per le categorie
dell'Allegato 1. Doppia condizione: incremento del numero di dipendenti a tempo indeterminato a
fine periodo rispetto alla media del periodo precedente **e** costo pari al minor importo fra il
costo effettivo dei nuovi assunti e l'incremento complessivo del costo del personale risultante
dalla voce B.9 del conto economico; nessun costo è agevolabile se il numero complessivo dei
dipendenti, inclusi i tempi determinati, non è cresciuto.
Proroga ai periodi 2025-2027 dall'art. 1, c. 399, L. 207/2024, con base di confronto che si azzera
ogni anno; il c. 400 esclude ogni effetto sugli acconti.
**Vale solo ai fini IRES e IRPEF, non ai fini IRAP** (il testo parla di «determinazione del
reddito»; il DM MEF/Lavoro 25 giugno 2024 richiama solo IRPEF e IRES). *Assenza di prassi AdE
espressa sul punto: **NON VERIFICATO**.*
**Scadenza anticipata:** l'art. 376 del D.Lgs. 19 giugno 2026 n. 117 abroga, con effetto dal 1°
gennaio 2027, sia l'art. 4 e l'Allegato 1 del D.Lgs. 216/2023 sia i commi 399 e 400 della L.
207/2024, senza trasposizione nel nuovo Testo unico: **la terza annualità di proroga (2027) viene
meno**. Rilevante se la roadmap prevede assunzioni nel 2027.

### Le norme citate da D01 hanno una data di scadenza: **1° gennaio 2027**

È il rilievo che V01 aveva già formulato (G-13) per il DPR 600/1973 e che va esteso: alla data
odierna **due testi unici hanno già abrogato le norme su cui poggia l'intera diagnosi**, con
applicazione differita al 1° gennaio 2027.

| Testo unico | Cosa abroga | Effetto su D01 |
|---|---|---|
| **D.Lgs. 19 giugno 2026 n. 117** — T.U. imposte sui redditi (G.U. n. 152 del 3/7/2026, in vigore dal 4/7/2026, disposizioni applicabili dal 1/1/2027, art. 377) | **il DPR 917/1986** nella sua interezza, con rinumerazione integrale (377 articoli) | tutte le citazioni TUIR di D01 — artt. 47, 50, 67, 95, 105, 110, 164 — sono corrette **fino al 31/12/2026** |
| **D.Lgs. 5 agosto 2026 n. 141** — T.U. adempimenti e accertamento (G.U. n. 181 del 6/8/2026, applicazione dal 1/1/2027) | gran parte del DPR 600/1973 **e gli articoli del D.Lgs. 13/2024 sul CPB**, che migrano nel T.U. | il § 6 di D01 cita norme che, per il periodo d'imposta 2027 — cioè il secondo anno del concordato che si sta per sottoscrivere — saranno formalmente abrogate |
| **D.Lgs. 24 marzo 2025 n. 33** (come modificato dal D.L. 200/2025) — T.U. versamenti e riscossione | **l'art. 27 DPR 600/1973** (ritenuta sui dividendi) | la citazione del § 4.1 è corretta fino al 31/12/2026 |

**Conseguenza operativa, che va scritta nel documento.** L'adesione al CPB 2026-2027 si perfeziona
entro il 2 novembre 2026 sotto il D.Lgs. 13/2024: nessun rischio di applicare norme sbagliate al
momento dell'adesione. Ma **gli effetti del concordato si dispiegano anche sul periodo d'imposta
2027**, quando cessazione, decadenza, accertamento e adempimenti andranno letti nel Testo unico.
Ogni parere, prospetto o clausola contrattuale che citi «art. 21/22/34 D.Lgs. 13/2024» per condotte
del 2027 sarà formalmente disallineato. **Va programmata una riverifica delle citazioni prima della
chiusura dell'esercizio 2026**, e va introdotto in ogni deliverable il campo che V01 (G-13) aveva
già prescritto e che D01 non ha: «norma vigente alla data del …, da riverificare al 1° gennaio 2027».
*La numerazione esatta degli articoli del CPB nel D.Lgs. 141/2026 è **NON VERIFICATA**: due
verifiche indipendenti hanno restituito intervalli discordanti (artt. 93-106 e artt. 89-111).*

---

## Verifica delle fonti consultate

### Fonti primarie aperte e utilizzate — CONFERMATO

- **D.Lgs. 12 febbraio 2024 n. 13**, testo pubblicato in G.U. n. 43 del 21 febbraio 2024 (copia sul
  portale dell'Agenzia delle Entrate) e **testo multivigente al 9 settembre 2026** su Normattiva
  (`https://www.normattiva.it/uri-res/N2Ls?urn:nir:stato:decreto.legislativo:2024-02-12;13~artNN!vig=2026-09-09`).
  Articoli letti verbatim: 9, 10, 11, 12, 14, 16, 18, 19, 20, 20-*bis*, 21, 22, 34, 35.
- **D.L. 27 marzo 2026 n. 38**, conv. L. 22 maggio 2026 n. 88, G.U. n. 117 del 22 maggio 2026:
  artt. 7 e 7-*bis*.
- **D.L. 13 maggio 2011 n. 70**, conv. L. 106/2011: art. 7, cc. 1 lett. h) e 2 lett. l).
- **D.M. Vice Ministro dell'Economia e delle Finanze 11 maggio 2026**, «Approvazione della
  metodologia relativa al concordato preventivo biennale per i periodi d'imposta 2026 e 2027»,
  G.U. Serie Generale n. 115 del 20 maggio 2026, S.O. n. 20 (cod. red. 26A02451), con Allegato 1
  (Nota tecnica e metodologica) e Relazione illustrativa, su `finanze.gov.it`.
- **Provvedimento del Direttore dell'Agenzia delle Entrate n. 71684 del 27 febbraio 2026** (modello
  CPB 2026-2027) e relative istruzioni, su `agenziaentrate.gov.it`; **circolare AdE n. 18/E del 17
  settembre 2024**.
- **D.Lgs. 12 giugno 2025 n. 81** (abrogazione del Capo III e introduzione del c. 1-*bis* dell'art.
  20-*bis*) e **D.Lgs. 7 agosto 2026 n. 148** (correttivo, doppio binario sulle cause di decadenza).
- **D.Lgs. 19 giugno 2026 n. 117** (T.U. imposte sui redditi), artt. 376 e 377; **D.Lgs. 5 agosto
  2026 n. 141** (T.U. adempimenti e accertamento), G.U. n. 181 del 6 agosto 2026.
- **TUIR**: artt. 11, c. 1 (testo vigente 2026), 50, c. 1, lett. c-*bis*), 95, c. 5, 105, 17, c. 1,
  lett. c), 10, c. 1, lett. e), 54, c. 2, lett. a).
- **DPR 600/1973**, art. 27, c. 1 (vigenze 15/1/2026 e 9/9/2026 a confronto).
- **D.Lgs. 446/1997**, artt. 5, 11 (cc. 1 lett. b) nn. 3-4 e 4-*octies*) e 16; **L.R. Veneto 27
  dicembre 2024 n. 32**, art. 2 (BUR n. 169 del 27/12/2024).
- **Codice civile**, art. 2477 (testo introdotto dall'art. 2-*bis* D.L. 32/2019).
- **L. 30 dicembre 2025 n. 199** (legge di bilancio 2026), art. 1, cc. 3 e 4; **L. 30 dicembre 2024
  n. 207**, art. 1, cc. 399, 400 e 436-444; **D.Lgs. 216/2023**, art. 4; **DM MEF/Lavoro 25 giugno
  2024**; **DM MEF 8 agosto 2025** (IRES premiale).
- **Circolare INPS 3 febbraio 2026 n. 8** (aliquote e massimali gestione separata 2026);
  **art. 2, c. 30, L. 335/1995**.
- **Inarcassa**, tabella contributi 2026 e Regolamento generale di previdenza (artt. 4.1 e 5.6).
- **Circolare AdE n. 105/E del 12 dicembre 2001** e n. 67/E del 6 luglio 2001 (superata), su
  `def.finanze.it`; **D.Lgs. 139/2005**, art. 1, c. 2, lett. a); **R.D. 2537/1925**, artt. 51-52.
- **Calendario 2026**: 31 ottobre sabato, 1° novembre domenica e festivo, 2 novembre lunedì.
- Tutti i **documenti primari del cliente** elencati in intestazione, con ricostruzione per
  quadratura completa dei tre bilanci XBRL.

### NON VERIFICATO — da chiudere prima della consegna al cliente

1. **La grandezza cui si àncora il tetto dell'art. 9, c. 3-*bis*, per chi era in CPB 2024-2025**:
   reddito effettivo o reddito concordato 2025. Gli indizi (rigo P04 del modello CPB, circolare
   18/E) puntano all'effettivo; il D.M. 11 maggio 2026 e la Nota tecnica usano la formula ambigua
   «reddito dichiarato». Nessuna circolare o FAQ AdE del 2026 sul punto (l'ultima prassi elencata
   dal portale è la circ. n. 9/E del 24 giugno 2025). **È la questione da cui dipende l'intera
   raccomandazione: vale circa 38.000 euro sul biennio.** Vedi R-4.
2. **La numerazione degli articoli sul CPB nel D.Lgs. 141/2026**: due verifiche indipendenti hanno
   restituito intervalli discordanti (artt. 93-106 e artt. 89-111).
3. **La disciplina e il termine della revoca** dell'adesione al CPB (§ 6 di D01: «La revoca ha lo
   stesso termine»). Vedi G-15.
4. **L'aliquota IRAP applicabile in Veneto per il 2026** sulle tabelle MEF, e la verifica che il
   codice ATECO 74.99.21 non rientri nell'Allegato C della L.R. 32/2024 (nel qual caso l'aliquota
   sarebbe 4,55% e non 4,08%).
5. **Le addizionali IRPEF regionale del Veneto e comunali** di Verona, Villafranca di Verona e
   Padova per il 2026: nel § 4.3 sono stimate in 2 punti complessivi. Le soglie di inversione sono
   espresse in termini di aliquota marginale complessiva proprio per essere indipendenti da questa
   verifica, ma la loro traduzione in soglie di reddito va rifatta sui valori esatti.
6. **L'abrogazione dell'art. 2409 c.c. da parte del D.Lgs. 47/2026** e il conseguente rinvio a
   norma abrogata nel sesto comma dell'art. 2477 c.c.: solo fonte secondaria.
7. **La deducibilità per il committente del contributo integrativo Inarcassa del 4%**: nessuna
   prassi dell'Agenzia reperita. Sul piano logico è parte del corrispettivo fatturato e imponibile
   ai fini IVA, quindi costo della prestazione.
8. **L'irrilevanza ai fini IRAP della super-deduzione nuove assunzioni**: conclusione fondata sul
   testo di legge e sul DM, non su prassi espressa.
9. **Il riferimento di prassi Circ. 12/E/2007 e Ris. 56/E/2002** talvolta citati sul tema
   dell'oggetto della professione: non aperti, non citarli.
10. **La qualificazione professionale di Pradella, Maggia e Dall'Oca**: nessun documento del
    fascicolo la attesta. È il presupposto di fatto del rilievo R-5.
11. **Contenuto dei documenti `DALLA PIAZZA_VOLUME D'AFFARI.pdf` e `PRADELLA TAZIO.pdf`**: non
    estraibili con gli strumenti disponibili (font a codifica simbolica il primo, pagine immagine
    prive di livello testo il secondo). Vanno riaperti dal consulente.
12. **Il termine e l'aliquota della rideterminazione del costo delle partecipazioni per il 2026**
    (V01, O-1, indicava 30 novembre 2026 e 21%, su fonti secondarie). Vedi R-3, lettera e).

---

## Riepilogo operativo per il consulente

**Da correggere prima di qualunque consegna (ROSSO):**

1. **R-1** — rifare integralmente il § 4.3 con la metrica omogenea, l'aliquota IRAP corretta e i
   tre scenari. Le conclusioni del § 4.3, del § 6 punto 3 e del § 8 punto 3 vanno riscritte: fuori
   dal CPB il dividendo vince già per un socio nel terzo scaglione; con società e socio entrambi in
   concordato vince la fattura.
2. **R-2** — eliminare «i contributi previdenziali restano dovuti sul reddito effettivo» e
   sostituirla con il testo dell'art. 19, c. 1.
3. **R-3** — correggere la citazione dell'art. 105, c. 4, TUIR e recepire le cinque prescrizioni di
   V01 e del protocollo rimaste inattuate (transfer pricing interno ex art. 9 TUIR; IVA; i due
   campi obbligatori sui VERDE e la data di scadenza dei GIALLO; la finestra della rideterminazione
   del costo delle partecipazioni; il campo sulla vigenza delle norme al 1° gennaio 2027).
4. **R-4** — riscrivere il § 6: la proposta 2026-2027 si costruisce con ogni probabilità sul
   reddito **effettivo** 2025, cioè sull'anno migliore nella storia della società. Il documento
   deve presentare anche il ramo «non aderire», e deve mettere in cima al § 7 la domanda sulla base
   di calcolo.
5. **R-5** — sostituire l'argomento sugli ingegneri: la circolare 105/E/2001 porta come esempio
   proprio l'ingegnere amministratore di società con attività oggettivamente connessa.

**Da correggere (GIALLO):** i quattordici rilievi della Parte III, in particolare le correzioni
numeriche E-1 (45.652), E-2 (Altre riserve, non utili portati a nuovo), E-4 (28.962), E-5 (108
giorni), E-6 (IRAP 4,08% e forchetta 17.300-18.900) ed E-7 (fondi per rischi e oneri = 0).

**Da aggiungere:** i sette rilievi della Parte IV, con priorità a N-1 (la decadenza dal CPB
innescata dal rilievo del § 5.1) e all'intera area IVA, assente dal documento e già contestata al
setup in V01.
