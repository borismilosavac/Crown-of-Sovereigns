# Crown of Sovereigns v2.8 — Game Design Document / Dokument dizajna igre

## Status dokumenta

- **Dokument:** `gdd/crown-of-sovereigns-v2.8-gdd.md`
- **Aktivna verzija:** **v2.8**
- **Status:** **Locked Direction / Active Development Base**
- **Svrha:** glavni krovni dizajnerski izvor istine za v2.8
- **Povezani dokumenti:** `docs/version-status.md`, `docs/product-parameters-v2.8.md`, `gdd/canonical-decisions.md`, `systems/court-authority-system.md`, `rules/rules-reference-v2.8.md`

---

## 1. Identitet igre

**Crown of Sovereigns** je kompetitivna strateška igra upravljanja kraljevstvom za 2–4 igrača, smještena u istorijski inspirisanu Evropu oko 1350. godine.

Centralna fantazija:

> Igrač mora imati osjećaj da vodi državu, a ne samo vojsku.

Igra povezuje:

- **Court/Dvor**
- **Provinces/Provincije**
- **Goods/Robu** i razvoj
- **Stability/Stabilnost** i **Unrest/Nemire**
- formalnu **Diplomacy/Diplomatiju**
- kompresovani teritorijalni konflikt
- završni **Coronation Attempt/Pokušaj krunisanja**

## 2. Proizvodni profil

- **Igrači:** 2–4
- **Najbolje iskustvo:** 3–4
- **Trajanje iskusne grupe:** 60–90 minuta
- **Prva partija:** 90–120 minuta
- **Ciljana kompleksnost:** BGG 3.3 ± 0.2
- **Format:** standardna velika euro/strategy igra
- **Ciljani MSRP:** 99,99 €
- **Solo:** buduća mogućnost, ne trenutni prioritet

## 3. Dizajnerski stubovi

### 3.1. Court/Dvor je centralan

Dvor određuje administrativni fokus države i način na koji igrač troši ograničeni akcioni kapacitet.

### 3.2. Mapa je stvarna moć

Provincije daju teritorijalnu, resursnu, goods, odbrambenu i političku vrijednost. Mapa ne smije postati bodovni wallpaper.

### 3.3. Goods/Roba predstavljaju razvoj

Resursi hrane sistem iz runde u rundu. Goods grade dugoročnu kvalitetu, specijalizaciju i kapacitet države.

### 3.4. Stability/Stabilnost je cijena moći

Ekspanzija, rat, izdaja i prenapregnut razvoj moraju nositi unutrašnju cijenu.

### 3.5. Diplomacy/Diplomatija je formalna

Razgovor je slobodan, ali mehaničku težinu imaju samo sistemski priznati sporazumi, obaveze i raskidi.

### 3.6. Rat je neizvjestan, ali ne nasumičan

Borba mora stvarati bluff i procjenu protivnika kroz skrivene simultane odluke. Sreća mora ostati vrlo niska.

### 3.7. Završnica je zaslužena

Coronation je contest koji testira izgrađenu teritoriju, legitimitet, stabilnost, političku mrežu i sposobnost protivnika da ospore krunu.

## 4. Simetrija i asimetrija

Kraljevstva koriste ista osnovna pravila, početni potencijal i dostupne sisteme.

Asimetrija dolazi iz:

- izbora aktivne dvorske uloge
- različitog načina trošenja Authority/AP
- trenutnog mapnog i političkog položaja
- Goods razvoja i Treaty mreže
- odluka igrača, ne zaključanih frakcijskih skripti

Ovo čuva fer osnovu i smanjuje balansni teret u odnosu na snažno asimetrične frakcije.

## 5. Court Authority / Dvorski autoritet

Svaki igrač na početku runde dobija:

- 3 AP na aktivnoj **Court Role/Dvorskoj ulozi**
- 1 univerzalni **Crown AP/Poen autoriteta krune**

Akcije koštaju 1–3 AP.

- 1 AP = osnovna akcija
- 2 AP = glavna strateška akcija
- 3 AP = velika akcija ili kompresija dva povezana koraka

Igrači se smjenjuju poslije svake glavne akcije.

## 6. Pet dvorskih uloga

### Marshal/Maršal

Vlada prostorom, vojnom prijetnjom, mobilizacijom, odbranom i osvajanjem. Dodatna agresija u istoj rundi nosi ratni zamor.

### Diplomat/Diplomata

Vlada sporazumima, priznanjima, političkim leverageom, koalicijama i cijenom izdaje.

### Merchant/Trgovac

Vlada robom, razvojem, trgovinskim vezama i pretvaranjem ekonomskog viška u državnu snagu.

### Cleric/Klerik

Vlada stabilnošću, legitimitetom, kriznim odgovorom i održivošću krune. Može sačuvati ograničenu reakciju za kasniju fazu iste runde.

### Spy/Špijun

Vlada contest prostorom, informacijom, pripremom ranjivosti i preciznim podrivanjem protivničkih planova.

## 7. Struktura runde

Standardna partija ima najviše 6 rundi.

1. **Event/Crisis Phase / Faza događaja i krize**
2. **Diplomatic Window / Diplomatski prozor**
3. **Court Selection and Reveal / Izbor i otkrivanje dvora**
4. **Authority Allocation / Dodjela autoriteta**
5. **Action Phase / Faza akcija**
6. **Conflict Resolution / Rješavanje sukoba**
7. **Income and Development / Prihod i razvoj**
8. **Stability and Unrest Update / Stabilnost i nemiri**
9. **Coronation and Round End Check / Krunisanje i završna provjera**

Runde 1–2 predstavljaju otvaranje, 3–4 srednju igru, a 5–6 završni politički pritisak.

## 8. Akcioni tempo

- cilj: prosječno 3 glavna poteza po igraču i rundi
- dozvoljeni raspon: 2–4
- rutinski potez: 30–45 sekundi
- soft cap: 60 sekundi
- veliki contest potez: do 90 sekundi

Nema:

- refundiranja AP
- beskonačnih combo lanaca
- besplatnih dodatnih glavnih poteza
- prenošenja AP u narednu rundu

## 9. Borbeni pravac

Borba zadržava standard:

1. **Declare/Objavi**
2. **Commit/Obaveži snagu i kartu**
3. **Reveal and Modify/Otkrij i izmijeni**
4. **Resolve/Riješi**

Ovo je namjerna v2.8 evolucija starog 3-step okvira radi integracije skrivenih borbenih karata.

Početni razvojni smjer:

- svi igrači imaju identičnu višekratnu Battle Hand
- karta se bira simultano i skriveno
- nema nasumičnog drawa kao glavnog izvora snage
- iskorištene karte ostaju javno iscrpljene do definisanog refresh prozora
- protivnici mogu računati preostale mogućnosti

Tačan broj, snaga i taktički efekti karata ostaju otvoreni za poseban combat prototip.

## 10. Putevi do pobjede

Pet uloga predstavljaju pet ravnopravnih strateških motora:

- Martial/Territorial
- Diplomatic/Political
- Economic/Development
- Stability/Legitimacy
- Intrigue/Contest

Nijedan motor nije samodovoljan. Svaka pobjednička strategija mora koristiti najmanje jednu dodatnu državnu funkciju.

**Balanced Path/Balansirani put** je hibridna državna doktrina, ne šesti izolovani track.

## 11. Uslov pobjede

Pobjednik je igrač sa najviše **Sovereignty Points/Poena suvereniteta** nakon završnog obračuna.

Sovereignty dolazi iz:

- teritorijalne kontrole i važnih provincija
- Goods razvoja
- Treaty i političke vrijednosti
- stabilnosti i legitimiteta
- ciljanih contest uspjeha
- završnog Coronation rezultata

## 12. Coronation Attempt / Pokušaj krunisanja

- eligibility počinje od 5. runde
- pokušaj mora biti javno najavljen i contestable
- može ubrzati kraj partije ako su ispunjeni zaključani uslovi
- ako se ne desi ranije, završni Coronation contest je obavezan poslije 6. runde
- uspjeh daje značajnu, ali ograničenu SP vrijednost
- Coronation ne smije automatski pretvoriti lošu partiju u pobjedu

Numerički pragovi ostaju za playtest kalibraciju.

## 13. Interakcija

Ciljani nivo je umjeren do visok kroz:

- mapno blokiranje i prijetnje
- korištenje zajedničkog ekonomskog prostora
- formalne sporazume
- contest i Spy pritisak
- borbu
- Coronation osporavanje

Interakcija ne smije postati stalni take-that niti neograničeno pregovaranje.

## 14. Glavni razvojni rizici

- previše faza za ciljanu težinu 3.3
- Marshal tempo koji nadjača ostale uloge
- Diplomat bez dovoljno završne snage
- Cleric kao dosadni safety button
- Spy kao generički take-that
- borbene karte koje uvedu dodatni kartični bloat
- 6 rundi koje ne daju dovoljno vremena ekonomskom razvoju
- coronation koji ili ne znači ništa ili znači previše
- prva partija koja prelazi 120–135 minuta

## 15. Obavezni playtest fokus

1. trajanje 2P, 3P i 4P
2. broj poteza po igraču
3. vrijeme rutinskog poteza
4. izbor i SP doprinos svake uloge
5. monofokus naspram hibridne strategije
6. neizvjesnost i pravičnost borbenih karata
7. diplomatski downtime
8. coronation swing
9. 2P runaway
10. jasnoća player aida

---

## Kanonska definicija

Ovaj GDD je glavni krovni dizajnerski izvor istine za **Crown of Sovereigns v2.8**. Stariji GDD dokumenti služe samo kao istorijska i migraciona referenca.
