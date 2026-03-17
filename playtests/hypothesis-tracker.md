# hypothesis-tracker.md

# Crown of Sovereigns v2.7 — Hypothesis Tracker / Praćenje hipoteza

## Status dokumenta

* **Dokument:** `playtests/hypothesis-tracker.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati sistem za praćenje, provjeru i ažuriranje glavnih dizajnerskih hipoteza kroz playtest cikluse
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Hypothesis/Hipoteza**, **Evidence/Dokaz**, **Win Path/Put do pobjede**
* **Povezani dokumenti:** `playtests/playtest-plan-v2.7.md`, `docs/version-status.md`, `gdd/canonical-decisions.md`, `systems/win-paths.md`, `systems/scaling-2p-3p-4p.md`, `systems/catch-up-and-runaway-control.md`, `systems/coronation-system.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* svaku važnu pretpostavku o igri pretvori u pratljivu hipotezu
* spriječi da razvoj bude vođen samo utiskom ili memorijom zadnjeg playtesta
* jasno pokaže šta je potvrđeno, šta je klimavo, a šta je opovrgnuto
* poveže playtest nalaze sa konkretnim dizajnerskim odlukama
* omogući da se hipoteze ne miješaju između verzija i patch iteracija

Ovo nije lista opštih želja za igru.
Ovo je operativni dokument za provjeru da li stvarno radi ono što tvrdimo da radi.

---

## 2. Zašto je hypothesis tracker kritičan

Kod igre kao što je **Crown of Sovereigns v2.7** vrlo je lako početi vjerovati da nešto radi zato što:

* jedna grupa nije imala problem
* jedna partija je bila uzbudljiva
* autor zna šta je “trebalo da se desi” pa to vidi i kad se nije jasno desilo
* više različitih problema djeluje kao isti problem

Bez jasnog praćenja hipoteza, razvoj vrlo lako sklizne u:

* selektivno pamćenje
* kontradiktorne zaključke
* patch promjene bez jasnog razloga
* lažnu sigurnost

Hypothesis tracker je alat protiv toga.

---

## 3. Osnovni princip dokumenta

Glavno pravilo glasi:

> nijedna važna tvrdnja o kvalitetu sistema ne smije ostati samo osjećaj ako je moguće pretvoriti je u testabilnu hipotezu.

To znači da tvrdnje kao što su:

* “**Balanced Path/Balansirani put** radi”
* “2P je zdrav”
* “**Coronation Attempt/Pokušaj krunisanja** daje wow bez swinga”

moraju imati:

* jasan oblik hipoteze
* dokaz ili vrstu dokaza
* status
* sljedeći korak provjere

---

## 4. Šta hypothesis tracker jeste

Ovaj dokument treba da bude:

* radna matrica dizajnerskih pretpostavki
* most između playtest plana i razvojnih odluka
* alat za razlikovanje potvrđenog od samo obećavajućeg
* revizijska mapa za buduće verzije

---

## 5. Šta hypothesis tracker nije

Ovaj dokument nije:

* gotov zaključak da je sistem dokazan
* spisak marketinških tvrdnji
* zamjena za playtest bilješke
* mjesto za duge narative o pojedinačnim partijama

On mora ostati:

* kratak
* precizan
* upotrebljiv
* operativan

---

## 6. Osnovne klase hipoteza

Sve hipoteze u **v2.7** treba podijeliti najmanje na ove klase:

### 6.1. Core System Hypotheses / Hipoteze jezgra sistema

Pitanja o tome da li osnovni motori igre rade kako treba.

### 6.2. Balance Hypotheses / Balansne hipoteze

Pitanja o tome da li su putevi do pobjede i player count modovi pošteni i živi.

### 6.3. UX Hypotheses / UX hipoteze

Pitanja o tome da li igrači razumiju tok, aid, terminologiju i komponente.

### 6.4. Endgame Hypotheses / Hipoteze završnice

Pitanja o napetosti kraja partije, wow kvalitetu i coronation logici.

### 6.5. Scaling Hypotheses / Hipoteze skaliranja

Pitanja o 2P, 3P, 4P i solo/automa zdravlju.

Kritično pravilo:

> svaka hipoteza mora imati jednu jasnu primarnu klasu, čak i ako dotiče više sistema.

---

## 7. Obavezna struktura jedne hipoteze

Svaka hipoteza u trackeru mora biti zapisana ovim redom:

1. **ID**
2. **Naziv hipoteze**
3. **Klasa**
4. **Tvrdnja**
5. **Zašto je važna**
6. **Način provjere**
7. **Vrsta dokaza**
8. **Status**
9. **Confidence/Pouzdanost**
10. **Sljedeći korak**

Ova struktura mora ostati ista za sve hipoteze, da bi bile uporedive i lake za pregled.

---

## 8. Standard za ID oznake

Preporučeni format ID-a:

* `CS-01`, `CS-02` za **Core System**
* `BL-01`, `BL-02` za **Balance**
* `UX-01`, `UX-02` za **UX**
* `EG-01`, `EG-02` za **Endgame**
* `SC-01`, `SC-02` za **Scaling**

Ovo pomaže da svaka hipoteza odmah ima:

* klasu
* trag kroz verzije
* lakšu referencu u playtest izvještajima

---

## 9. Standard za formulisanje tvrdnje

Tvrdnja mora biti:

* konkretna
* testabilna
* dovoljno uska da se može potvrditi ili opovrgnuti

### Dobar primjer

**BL-01:** **Balanced Path/Balansirani put** može realno pobijediti u 3P bez oslanjanja prvenstveno na tuđe greške.

### Loš primjer

“Igra djeluje balansirano.”

Loš primjer je preširok i ne daje jasan test.

---

## 10. Standard za “Zašto je važna”

Ovaj dio mora objasniti zašto hipoteza nije sporedna.

Treba povezati hipotezu sa:

* identitetom igre
* balansnim rizikom
* UX rizikom
* tržišnim ili završnim kvalitetom

Ako nije jasno zašto je hipoteza važna, postoji rizik da se testira nešto što nije dovoljno relevantno za razvoj.

---

## 11. Standard za način provjere

Svaka hipoteza mora imati jasan plan provjere.

To može uključivati:

* određeni tip partije
* određeni player count
* namjerno testiranje određenog **Win Path/Put do pobjede**
* posmatranje određenog trenutka, npr. završnice
* upoređivanje više sesija

Bez načina provjere hipoteza ostaje samo ideja, ne alat.

---

## 12. Standard za vrstu dokaza

Vrsta dokaza mora biti označena jasno.

Preporučene oznake su:

* **Observed/Posmatrano** — viđeno direktno u testovima
* **Pattern/Obrazac** — viđeno više puta kroz sesije
* **Tester Feedback/Povrat testera** — iz izjave i reakcije testera
* **Designer Inference/Dizajnerski zaključak** — zaključeno iz više signala, ali još ne sasvim čvrsto
* **Unverified/Nepotvrđeno** — još nema dovoljno dokaza

Ovo pomaže da se ne miješaju jaka i slaba saznanja.

---

## 13. Standard za status hipoteze

Svaka hipoteza mora imati jedan od sljedećih statusa:

### 13.1. **Open/Otvorena**

Još nema dovoljno dokaza.

### 13.2. **Leaning True/Nagovještava se kao tačna**

Postoje pozitivni signali, ali još nema dovoljno potvrde.

### 13.3. **Confirmed/Potvrđena**

Postoji dovoljno konzistentnog dokaza da trenutno tretiramo hipotezu kao potvrđenu za aktivnu verziju.

### 13.4. **Leaning False/Nagovještava se kao netačna**

Postoje zabrinjavajući signali, ali još nije konačno oborena.

### 13.5. **Rejected/Odbačena**

Dokaz jasno pokazuje da hipoteza za ovu verziju ne stoji.

Kritično pravilo:

> “Leaning True” nije isto što i “Confirmed”.

---

## 14. Standard za confidence / pouzdanost

Pouzdanost mora biti označena kao:

* **Low/Niska**
* **Medium/Srednja**
* **High/Visoka**

### Kako koristiti

* **Low/Niska** kada je malo sesija ili je dokaz fragmentaran
* **Medium/Srednja** kada postoji više dobrih signala, ali i dalje postoje rupe
* **High/Visoka** tek kada postoji više konzistentnih partija i malo kontradiktornih nalaza

Pouzdanost se odnosi na snagu dokaza, ne na želju autora da hipoteza bude tačna.

---

## 15. Obavezni početni skup hipoteza za v2.7

Tracker mora najmanje sadržati ove početne hipoteze.

### Core System

* **CS-01:** Igra zaista djeluje kao **kingdom-management** iskustvo, a ne kao samo multi-system competition.
* **CS-02:** **Court/Dvor** je glavni motor odluka kroz cijelu partiju.
* **CS-03:** **Stability/Stabilnost** djeluje kao stvarna cijena moći, ne kao sporedni broj.

### Balance

* **BL-01:** **Balanced Path/Balansirani put** je stvarna i pobjednička putanja.
* **BL-02:** **Diplomatic Path/Diplomatski put** može realno zatvoriti partiju.
* **BL-03:** **Aggro/Aggro** je snažan, ali ne dominantan autopilot.
* **BL-04:** **Economic Path/Ekonomski put** ostaje stvaran i ne djeluje odvojen od mape.

### UX

* **UX-01:** **Round Spine/Kičma runde** je razumljiva nakon prve ili druge runde.
* **UX-02:** **Player Aid/Pomoćni igrački vodič** realno smanjuje lookup.
* **UX-03:** Terminologija i ikonografija ne stvaraju značajnu konfuziju.

### Endgame

* **EG-01:** Završnica češće ostaje otvorena nego zatvorena.
* **EG-02:** **Coronation Attempt/Pokušaj krunisanja** daje wow bez reset osjećaja.
* **EG-03:** Kasne **Crises/Krize** pojačavaju tenziju bez lažnog swinga.

### Scaling

* **SC-01:** 2P ostaje fer i napet kroz **Crown Pressure/Pritisak krune**.
* **SC-02:** 3P je politički najčitljiviji mod.
* **SC-03:** 4P ostaje bogat, ali ne previše spor.
* **SC-04:** **Automa/Automa** je koristan za solo i trening, bez prenapuhanosti.

---

## 16. Kako se hipoteze ažuriraju poslije sesije

Poslije svake relevantne sesije treba uraditi:

1. označiti koje hipoteze je sesija zapravo dodirnula
2. dodati novi dokaz ili kontradokaz
3. po potrebi promijeniti status
4. po potrebi promijeniti confidence
5. zapisati sljedeći korak provjere

Ne treba ažurirati sve hipoteze poslije svake partije. Samo one koje je partija stvarno testirala.

---

## 17. Pravilo protiv prebrze potvrde

Hipoteza ne smije postati **Confirmed/Potvrđena** samo zato što:

* jedna partija nije pokazala problem
* testeri nisu komentarisali problem
* autor misli da je najnoviji patch “sigurno to popravio”

Potvrda traži:

* više signala
* konzistentnost
* odsustvo ozbiljnih kontra-primjera

Ovo je posebno važno za balansne i završne hipoteze.

---

## 18. Pravilo protiv prebrzog odbacivanja

Isto tako, hipoteza ne smije biti **Rejected/Odbačena** samo zato što:

* jedna grupa nije razumjela sistem
* jedna partija otišla u čudan ekstrem
* jedan tester nije volio određeni stil igre

Treba razlikovati:

* sistemski kvar
* loš onboarding trenutak
* neobičan test scenario
* stvarni pattern problema

---

## 19. Veza sa playtest-plan dokumentom

`playtests/playtest-plan-v2.7.md` govori:

* kako testirati
* koje sesije i fokus koristiti

`playtests/hypothesis-tracker.md` govori:

* šta je tim testovima trebalo potvrditi ili opovrgnuti
* gdje trenutno stojimo po svakoj važnoj tvrdnji

Ova dva dokumenta moraju raditi zajedno.

---

## 20. Veza sa version-status i canonical-decisions dokumentima

Ako je neka hipoteza čvrsto potvrđena ili odbačena, to može voditi ka:

* promjeni `docs/version-status.md`
* novoj odluci u `gdd/canonical-decisions.md`
* zaključavanju ili uklanjanju određenog sistema u narednoj iteraciji

Zato hypothesis tracker nije izolovan dokument. On direktno utiče na ono što postaje kanon.

---

## 21. Najčešće greške u radu sa hipotezama

* hipoteza je preširoka da bi se stvarno testirala
* hipoteza nema jasan status
* status i confidence se koriste kao da su isto
* hipoteza se “potvrdi” iz želje, a ne iz dokaza
* UX problem se pogrešno vodi kao balansna hipoteza
* više verzija se miješa u jednom zaključku

---

## 22. Workflow pravilo za novu hipotezu

Ako se uvodi nova hipoteza, mora se provjeriti redom:

1. da li je dovoljno važna za verziju **v2.7**
2. da li se može testirati u realnim sesijama
3. da li već postoji slična hipoteza koju treba proširiti umjesto duplirati
4. da li pripada pravoj klasi
5. da li je formulacija dovoljno konkretna
6. da li je jasno šta bi bio dokaz “za” i “protiv”

Ako ne prolazi ova pitanja, novu hipotezu ne treba uvoditi još.

---

## 23. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li tracker postaje jasniji ili mutniji?
2. da li razlikuje potvrđeno od obećavajućeg?
3. da li pomaže stvarnoj dizajnerskoj odluci?
4. da li ostaje dovoljno lagan za stvarnu upotrebu?
5. da li čuva disciplinu verzija i statusa?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 24. Veza sa grafičkom i UX pripremom

Iako je ovo playtest dokument, on indirektno utiče i na:

* `ux/player-aid-system.md`
* `components/player-board-spec.md`
* `components/board-spec.md`
* `components/iconography-spec.md`

Zašto?
Zato što će mnoge hipoteze biti upravo o tome da li komponente i aid zaista nose sistem kako treba.

Ako tracker to ne bilježi precizno, grafički i UX problemi lako ostaju zamaskirani kao “game feel” problem.

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `playtests/playtest-plan-v2.7.md`
* `docs/version-status.md`
* `gdd/canonical-decisions.md`
* `systems/win-paths.md`
* `systems/scaling-2p-3p-4p.md`
* `systems/catch-up-and-runaway-control.md`
* `systems/coronation-system.md`
* `GLOSSARY.md`

---

## 26. Završna napomena

**Hypothesis Tracker / Praćenje hipoteza** mora ostati jedan od najvažnijih razvojnih filtera za **Crown of Sovereigns v2.7**.

Ako radi dobro:

* znaš šta je stvarno potvrđeno
* znaš šta je samo obećavajuće
* znaš šta moraš testirati sljedeće
* verzije se manje miješaju
* a razvoj postaje mnogo manje zavisan od pamćenja i utiska

Ako radi loše:

* playtest sesije ostavljaju previše buke
* važne pretpostavke ostaju neprovjerene
* autor lako počne vjerovati stvarima koje još nisu dokazane
* a razvoj postaje sporiji i manje siguran

Zato ovaj dokument mora ostati strog, praktičan i trajno usklađen sa jezgrom **v2.7**.
