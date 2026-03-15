# CHANGELOG.md

# Crown of Sovereigns — Changelog

## Status dokumenta

* **Dokument:** CHANGELOG.md
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Locked
* **Svrha:** centralna evidencija svih važnih promjena kroz verzije projekta
* **Pravilo jezika:** svi ključni termini se vode dvojezično, npr. **Goods/Roba**, **Court/Dvor**, **Cleric/Klerik**

---

## 1. Svrha changelog dokumenta

Ovaj dokument postoji da bi svaka važna promjena na projektu ostavila jasan trag.

Changelog nije marketinški pregled.
Nije dnevnik ideja.
Nije mjesto za nejasne bilješke.

On mora jasno pokazati:

* šta je promijenjeno
* u kojoj verziji je promijenjeno
* zašto je promijenjeno
* da li je promjena kanonska
* koji dokumenti i sistemi su pogođeni

Ako promjena nije zabilježena u changelog-u, dugoročno postaje teže dokazati:

* kada je uvedena
* zašto je uvedena
* šta je zamijenila
* da li je ispravno propagirana kroz repozitorijum

---

## 2. Pravila upisa u changelog

### 2.1. Šta se upisuje

Upisuju se:

* nove kanonske verzije
* važni **PATCH** paketi
* sistemske promjene koje utiču na više dokumenata
* promjene u identitetu, pravilima, komponentama ili UX-u
* promjene koje utiču na playtest interpretaciju
* promjene koje utiču na grafički handoff

### 2.2. Šta se ne upisuje kao glavna stavka

Ne upisuje se svaka sitna tipfeler korekcija kao posebna velika promjena.
Takve izmjene se mogu grupisati pod:

* wording cleanup
* clarity cleanup
* formatting update

### 2.3. Svaka stavka mora imati

Svaka važna promjena mora navesti:

* **verziju**
* **status promjene**
* **datum** ako je poznat
* **sažetak promjene**
* **razlog promjene**
* **pogođene dokumente / sisteme**

---

## 3. Format jedne changelog stavke

Preporučeni format:

```md
## vX.X.X — Status
- Sažetak promjene
- Razlog
- Pogođeni sistemi
- Pogođeni dokumenti
```

Ako je promjena velika, dodati podsekcije:

* Added
* Changed
* Removed
* Locked
* Notes

---

## 4. Aktivna verzija

## **v2.7 — Locked Canonical Version**

**Status:** jedina aktivna i relevantna verzija za dalji razvoj
**Napomena:** sve ranije verzije tretiraju se kao arhiva i istorija iteracija, ne kao aktivna baza.

### Sažetak

Verzija **v2.7** zaključava koherentan sistemski repair paket zasnovan na prethodnom dijagnostičkom i tuning radu. Ova verzija zadržava identitetske stubove igre — **Court/Dvor**, **Provinces/Provincije**, **Goods/Roba**, **Stability/Stabilnost**, **Structured Diplomacy/Strukturisana diplomatija**, **Condensed Warfare/Kratak rat** i **Sharp Endgame/Oštra završnica** — ali uvodi čišći tempo, jači 2P, precizniju diplomatiju i sistemski građen wow.

### Added / Added as canonical

* uvedeni strukturisani i vremenski ograničeni diplomatski prozori
* uvedena kompresija toka na princip **jedna glavna dvorska akcija po potezu**
* uveden **Coronation Attempt/Pokušaj krunisanja** kao glavni sistemski wow vrhunac
* uvedena pojačana late-crisis compression logika za završnicu
* uveden jači dvodijelni **player aid/pomoćni igrački vodič** sistem
* uvedena stroža komponentna disciplina kao kanonsko pravilo

### Changed

* **Balanced Path/Balansirani put** dobio je konkretniji midgame tempo benefit
* **Diplomatic Path/Diplomatski put** je pretvoren u puni i realni put do pobjede
* **Crown Pressure/Pritisak krune** u 2P modu je retargetiran na lidera
* **Combat/Borba** je standardizovana u 3 koraka: **Declare/Objavi → Modify/Izmijeni → Resolve/Riješi**
* završnica je kompresovana da češće proizvodi tijesan rezultat i pričljiv kraj partije

### Locked identity

Ostaju netaknuti i zaključani:

* **Court/Dvor** kao glavni motor odluka
* **Provinces/Provincije** kao važna mapa
* **Goods/Roba** kao razvojna osovina
* **Stability/Stabilnost** kao cijena moći
* **Structured Diplomacy/Strukturisana diplomatija** kao mjerljiv sistem
* **Condensed Warfare/Kratak rat** kao važan ali ne dominantan konfliktni sloj

### Reason

v2.7 je otvorena i zaključana da bi se:

* smanjio **downtime/usporenje poteza**
* ojačalo povjerenje u balans
* popravio 2P mod
* učinio **Balanced Path/Balansirani put** stvarnim
* učinio **Diplomatic Path/Diplomatski put** stvarnim
* povećala učestalost i kvalitet zasluženih wow vrhunaca
* stabilizovala baza prije daljeg GitHub documentation i graphic handoff rada

### Affected systems

* **Court/Dvor**
* **Diplomacy and Treaties/Diplomatija i sporazumi**
* **Stability and Unrest/Stabilnost i nemiri**
* **Combat/Borba**
* **Scaling 2P/3P/4P/Skaliranje 2P/3P/4P**
* **Coronation/Krunisanje**
* **Endgame/Završnica**
* **Player Aid/Player aid**

### Affected documents

* glavni GDD za v2.7
* rules dokumenti
* systems dokumenti
* UX / onboarding dokumenti
* component i graphic handoff dokumenti

---

## 5. Prethodna verzija

## **v2.6.1 — Diagnostic and Repair Phase**

**Status:** archived as transitional repair layer
**Napomena:** v2.6.1 se ne koristi kao aktivna baza, nego kao istorijski i analitički most između v2.6 i v2.7.

### Sažetak

v2.6.1 je definisala detaljni dijagnostički i repair okvir za igru, uključujući metrike, baseline scoring, proxy simulaciju, konkurentski benchmark i preporučene korektivne pakete.

### Ključni doprinosi

* definisan sistemski problem 2P zdravlja
* potvrđena potreba za jačim **Balanced Path/Balansirani put** i **Diplomatic Path/Diplomatski put** payoffem
* definisan problem **downtime/usporenja poteza** i pregovaračkog drift-a
* potvrđena potreba za boljim wow vrhuncima iz sistema, a ne iz nasumičnog haosa
* otvoren pravac prema **Coronation Attempt/Pokušaj krunisanja**

### Zašto nije ostala kanonska baza

Zato što je bila prijelazni repair sloj, a ne čisto zaključana i integrisana verzija dokumentacije.

---

## 6. Starija kanonska baza

## **v2.6 — Repair-aligned Canonical Base**

**Status:** archived
**Napomena:** v2.6 je bila prva kanonska verzija nakon velikog repair rada, ali je kasnije zamijenjena jasnijom i koherentnijom v2.7 bazom.

### Sažetak

v2.6 je zaključala:

* pojednostavljen onboarding
* zategnutiju diplomatiju
* pojednostavljenu borbu
* jači catch-up
* bolji 2P pravac
* smanjenu komponentnu frikciju
* jači tržišni hook

### Ograničenje

Iako jača od v2.5, još nije bila dovoljno jasno integrisana kao potpuna dokumentaciona i sistemska baza.

---

## 7. Starija razvojna osnova

## **v2.5 — Archived Historical Base**

**Status:** archived
**Napomena:** v2.5 ostaje važna istorijska tačka, ali nije više aktivni source of truth.

### Sažetak

v2.5 je definisala ključni identitet igre i bila dugo glavna kanonska baza. U njoj su već bili jasno prepoznati glavni razvojni rizici:

* zdravlje 2P moda
* **Aggro/Aggro** dominacija
* održivost **Balanced Path/Balansirani put**
* održivost **Diplomatic Path/Diplomatski put**
* jačina **catch-up** mehanizama
* završna napetost

### Istorijski značaj

Bez v2.5 ne bi postojao stabilan identitetski okvir za kasnije repair iteracije.

---

## 8. Pravila za buduće unose

Za svaku narednu verziju:

### Ako je PATCH

Primjer:

* `v2.7.1`

Upis mora navesti:

* šta je tačno fino podešeno
* koji sistem je pogođen
* da li se promjena oslanja na playtest nalaze
* da li mijenja aktivna pravila ili samo wording / clarity

### Ako je MINOR

Primjer:

* `v2.8`

Upis mora navesti:

* koji novi zaključani sistemski paket je uveden
* zašto patch više nije bio dovoljan
* koji dokumenti moraju biti tretirani kao nova kanonska baza

### Ako je MAJOR

Primjer:

* `v3.0`

Upis mora navesti:

* koji je razvojni lom nastao
* zašto više nije pošteno tretirati promjenu kao nastavak iste faze
* koji identitet je ostao, a šta se radikalno promijenilo

---

## 9. Pravilo dvojezičnih termina

Od ove tačke u changelog dokumentaciji važi:

* svi ključni sistemski termini pišu se **engleski / srpski**
* primjer: **Goods/Roba**, **Court/Dvor**, **Cleric/Klerik**, **Marshal/Maršal**, **Spy/Špijun**, **Diplomat/Diplomata**

Razlog:

* lakša saradnja sa budućim međunarodnim saradnicima
* lakši GitHub rad
* jasniji prelaz prema grafičkoj pripremi i eventualnom engleskom izdanju

---

## 10. Brutalno iskrena napomena

Ako changelog nije uredan, projekat gubi pamćenje.

To vodi ka tome da:

* niko više ne zna zašto je nešto promijenjeno
* ista rasprava se vodi više puta
* playtest nalazi postaju nepouzdani
* grafika može krenuti iz pogrešne osnove
* repo djeluje neozbiljno

Zato ovaj dokument nije administrativni višak.
On je dokaz razvoja.

---

## 11. Završna definicija

Od sada važi:

* **v2.7** je aktivna kanonska baza
* sve buduće promjene se upisuju ovdje
* nijedna važna sistemska promjena ne smije biti smatrana završenom dok nije unesena u changelog

Ovaj dokument služi kao centralna istorija odluka i promjena projekta **Crown of Sovereigns**.
