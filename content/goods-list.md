# goods-list.md

# Crown of Sovereigns v2.7 — Goods List / Lista robe

## Status dokumenta

* **Dokument:** `content/goods-list.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati sadržajni okvir, tipove, identitet i pravila pisanja za sve **Goods/Roba** elemente u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Goods/Roba**, **Gold/Zlato**, **Merchant/Trgovac**
* **Povezani dokumenti:** `systems/goods-and-development.md`, `rules/scoring-reference.md`, `systems/province-map-system.md`, `systems/court-system.md`, `systems/win-paths.md`, `components/terminology-and-labels.md`, `visuals/card-wireframe-notes.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* pretvori sistem **Goods/Roba** u disciplinovan sadržajni okvir
* jasno razdvoji **Goods/Roba** od opštih resursa
* postavi standard za buduće goods nazive, tipove i tekstove
* spriječi da goods sadržaj sklizne u generičke “resurse sa drugim imenom”
* olakša kasniji card layout, player board logiku i grafički handoff

Ovo nije systems dokument. Sistemska logika je već zatvorena u `systems/goods-and-development.md`.
Ovo je sadržajni dokument koji definiše kako konkretni goods sadržaj treba da izgleda.

---

## 2. Osnovni princip sadržaja

Svaki **Goods/Roba** element mora biti:

* prepoznatljiv
* razvojno smislen
* vezan za kraljevstvo, a ne samo za apstraktni profit
* dovoljno jasan da odmah djeluje drugačije od običnog resursa
* dovoljno disciplinovan da ne stvara bookkeeping umor

Ako goods izgledaju kao još jedan skup tokena bez identiteta, sistem je sadržajno promašio.

---

## 3. Ključna razlika između Goods/Roba i resursa

Ovo je najvažnija sadržajna tačka.

### 3.1. Resursi

Opšti resursi su:

* **Gold/Zlato**
* **Food/Hrana**
* **Faith/Vjera**
* **Influence/Uticaj**

Oni služe za:

* plaćanje
* održavanje
* aktivaciju odluka
* opšti tok partije

### 3.2. Goods/Roba

**Goods/Roba** služe za:

* razvojnu identifikaciju kraljevstva
* ekonomski i politički leverage
* završnu i srednjeročnu vrijednost
* osjećaj da kraljevstvo proizvodi i organizuje višak, ne samo troši osnovna sredstva

### 3.3. Sadržajna posljedica

Goods moraju zvučati, izgledati i djelovati kao nešto što kraljevstvo razvija i koristi strateški, a ne samo troši kao sirovinu.

---

## 4. Šta Goods/Roba nisu

Goods sadržaj ne smije biti:

* samo drugi naziv za resurse
* generička set-collection lista bez državničkog smisla
* čista ekonomija bez veze sa mapom i politikom
* suviše apstraktan da bi igrač osjetio šta kraljevstvo zapravo razvija
* toliko detaljan da svaka vrsta robe traži poseban podsistem

Ako goods skliznu u bilo šta od navedenog, sistem gubi identitet.

---

## 5. Osnovna dizajnerska funkcija goods sadržaja

Sadržaj **Goods/Roba** mora raditi 5 stvari:

1. dati kraljevstvu razvojni karakter
2. podržati **Economic Path/Ekonomski put**
3. podržati **Balanced Path/Balansirani put**
4. ostati povezan sa mapom i politikom
5. biti dovoljno čist za onboarding i grafički rad

Ako radi samo drugu stvar, goods postaju uska ekonomska linija.
Ako radi samo prvu i petu, goods postaju lijep ali mehanički slab sloj.

---

## 6. Glavne sadržajne klase Goods / Roba

U CoS v2.7 goods sadržaj treba biti organizovan kroz nekoliko jasnih klasa. Ovo nisu nužno finalne kartice, nego sadržajni tipovi.

### 6.1. Proizvodna roba

Roba koja signalizira da kraljevstvo ima stabilnu proizvodnju i razvojni kapacitet.

### 6.2. Trgovačka roba

Roba koja je posebno pogodna za razmjenu, politički leverage i sporazume.

### 6.3. Prestižna roba

Roba koja nosi veću statusnu, legitimacijsku ili završnu vrijednost.

### 6.4. Strateška roba

Roba koja direktno ili indirektno pojačava mapnu, ekonomsku ili političku otpornost.

Kritično pravilo:

> svaka roba može imati sekundarne efekte, ali mora imati jedan jasan primarni identitet.

---

## 7. Kako goods treba da zvuče

Nazivi i ton goods sadržaja treba da zvuče kao nešto što srednjovjekovno kraljevstvo zaista proizvodi, kontroliše, razmjenjuje ili koristi za prestiž.

To znači da goods treba da djeluju:

* konkretno
* zemaljski
* politički i ekonomski uvjerljivo
* dovoljno široko da ostanu čitljivi bez pretjerane istorijske mikrodokumentarnosti

Drugim riječima:

> goods treba da zvuče kao kraljevstvo, ne kao apstraktna excel ćelija.

---

## 8. Standardna struktura jednog Goods / Roba zapisa

Svaki budući **Goods/Roba** zapis treba koristiti ovaj okvir:

1. **Naziv:** English/Srpski
2. **Klasa:** proizvodna / trgovačka / prestižna / strateška
3. **Jednorečenični identitet**
4. **Primarna funkcija**
5. **Sekundarna veza**
6. **Šta pojačava u kraljevstvu**
7. **Wording napomena**

To pomaže da goods sadržaj ostane disciplinovan i uporediv.

---

## 9. Šta dobar Goods/Roba zapis mora sadržajno raditi

Dobar goods zapis mora igraču odmah sugerisati:

* zašto je ta roba važna
* kojoj vrsti kraljevstva prirodno odgovara
* da li više pomaže razvoju, trgovini, prestižu ili strateškoj otpornosti
* kako se uklapa u ostatak sistema

Ako goods zapis to ne komunicira, vjerovatno je previše generički.

---

## 10. Veza sa mapom

Ovo je jedna od najvažnijih sadržajnih veza.

Goods sadržaj mora imati mapni smisao.
To znači da roba treba sadržajno da djeluje kao nešto što:

* dolazi iz određenih prostora
* zavisi od kontrole ili pristupa tim prostorima
* daje razlog da **Provinces/Provincije** budu važne i mimo samog rata

Ako goods nema prostorni identitet, mapa i razvoj se previše odvajaju.

---

## 11. Veza sa Merchant / Trgovac ulogom

**Merchant/Trgovac** je prirodni glavni kanal za goods sadržaj.

To znači da goods zapisi moraju:

* imati jasan odnos prema trgovini i razvoju
* podržavati ekonomski fokus bez svođenja na “uzmi više tokena”
* biti dovoljno zanimljivi da **Merchant/Trgovac** djeluje kao puna dvorska uloga, a ne samo resursna pomoć

---

## 12. Veza sa Diplomacy / Diplomatija sistemom

Nisu svi goods elementi isti u političkom smislu.

Neki goods zapisi treba da:

* prirodno podrže **Trade Pact/Trgovački pakt** logiku
* daju politički leverage
* učine ekonomske odnose između kraljevstava zanimljivijim

Ali treba paziti:

* goods ne smiju postati toliko diplomatski da izgube razvojni identitet

---

## 13. Veza sa Stability / Stabilnost sistemom

Goods sadržaj mora podržavati ideju da razvoj bez upravljanja nosi rizik.

To ne znači da svaki goods zapis mora direktno kažnjavati igrača.
To znači da goods kao sadržaj treba da djeluju kao:

* snaga koju treba održati
* razvoj koji traži sistemsku disciplinu
* izvor moći koji ima smisla samo u zdravom kraljevstvu

To jača fantaziju vođenja države, a ne samo sticanja profita.

---

## 14. Veza sa Win Paths / Putanje do pobjede

Goods sadržaj mora najprirodnije podržavati:

* **Economic Path/Ekonomski put**
* **Balanced Path/Balansirani put**

Ali takođe treba da indirektno pomogne:

* **Diplomatic Path/Diplomatski put** kroz trgovačku i političku vrijednost
* čak i **Aggro/Aggro** ako teritorijalna kontrola goods prostora daje strateški razlog za sukob

Ako goods sadržaj radi samo za jednu putanju, sistem postaje uži nego što treba.

---

## 15. Goods i scoring

Sadržaj goods liste mora biti kompatibilan sa time da goods imaju stvarnu završnu vrijednost.

To znači da goods zapisi sadržajno treba da djeluju kao nešto što:

* se razvija tokom partije
* može imati srednjeročnu i završnu težinu
* ima razlog da ostane važan do kraja, a ne samo u prvim rundama

Ako goods djeluju kao rana pomoć koja kasnije ništa ne znači, njihov identitet je slab.

---

## 16. Onboarding filter

Za **First Game Mode/Mod prve partije**, goods sadržaj mora proći dodatni filter:

* nazivi moraju biti lako razumljivi
* funkcije moraju biti kratke
* roba ne smije djelovati kao još jedan apstraktni mini-sistem

Nova grupa nakon prve partije mora razumjeti:

* da **Goods/Roba** nisu isto što i resursi
* da goods znače razvoj
* da goods mogu pomoći da se pobijedi, ali ne sami i izolovano

---

## 17. Wording standard

Wording za goods sadržaj mora biti:

* kratak
* konkretan
* razvojno orijentisan
* bez nepotrebnog istorijskog objašnjavanja u samom efektu
* bez skrivanja mehaničke funkcije iza atmosferskog teksta

Dobar goods tekst treba čitati brzo i odmah signalizirati šta ta roba znači za kraljevstvo.

---

## 18. Najčešće greške pri pisanju goods sadržaja

* praviti goods koji zvuče isto kao resursi
* davati previše sitnih funkcija jednoj robi
* potpuno odvojiti goods od mape
* tretirati goods kao pasivni spreadsheet plus
* učiniti goods toliko apstraktnim da igrač ne osjeti šta razvija
* učiniti goods toliko specifičnim da svaki traži posebno pravilo

---

## 19. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li goods i dalje zvuče i djeluju drugačije od resursa?
2. da li goods ostaju povezani sa mapom i razvojem?
3. da li sadržaj pomaže više putanja do pobjede?
4. da li wording ostaje kratak i čist?
5. da li onboarding ostaje izvediv?
6. da li grafički handoff ostaje realan?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 20. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `components/player-board-spec.md`
* `visuals/card-wireframe-notes.md`
* `ux/player-aid-system.md`

Ako goods sadržaj nije sadržajno čist prije grafičke faze, tokeni, ikonografija i board UI vrlo brzo postaju konfuzni.

---

## 21. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `systems/goods-and-development.md`
* `systems/province-map-system.md`
* `systems/court-system.md`
* `systems/win-paths.md`
* `rules/scoring-reference.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `components/player-board-spec.md`

---

## 22. Završna napomena

**Goods List / Lista robe** mora ostati jedan od ključnih sadržajnih temelja ekonomske i razvojne strane CoS v2.7.

Ako radi dobro:

* goods imaju karakter
* razvoj djeluje stvarno
* mapa i ekonomija ostaju povezane
* **Economic Path/Ekonomski put** i **Balanced Path/Balansirani put** ostaju živi
* a igra djeluje bogatije i ozbiljnije

Ako radi loše:

* goods se utope u resurse
* razvoj izgubi identitet
* ekonomija djeluje generički
* a sadržaj postaje teži za onboarding i grafički handoff

Zato ovaj dokument mora ostati strogi filter prije pisanja bilo kakvih konkretnih goods elemenata, kartica ili oznaka.
