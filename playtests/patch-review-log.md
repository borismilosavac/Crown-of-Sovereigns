# patch-review-log.md

# Crown of Sovereigns v2.7 — Patch Review Log / Dnevnik revizije zakrpa

## Status dokumenta

* **Dokument:** `playtests/patch-review-log.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati standard za praćenje, procjenu i retrospektivu svih patch promjena unutar aktivne verzije i njenih pod-iteracija
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Patch/Zakrpa**, **Review/Provjera**, **Impact/Uticaj**
* **Povezani dokumenti:** `VERSIONING.md`, `CHANGELOG.md`, `docs/revision-workflow.md`, `docs/version-status.md`, `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `playtests/balance-watchlist.md`, `playtests/session-report-template.md`, `playtests/matchup-matrix.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uvede jasan trag za svaku patch promjenu unutar **v2.7** linije
* spriječi da se zakrpe gomilaju bez jasnog sjećanja šta su trebale popraviti
* omogući da se vidi da li je patch stvarno riješio problem ili samo premjestio simptom
* poveže promjene sa playtest dokazima, hipotezama i balansnim rizicima
* olakša odluku da li neku zakrpu zadržati, vratiti, doraditi ili eskalirati u veću verziju

Ovo nije samo spisak promjena.
Ovo je radni dokument za procjenu kvaliteta patch ciklusa.

---

## 2. Zašto je patch review log kritičan

Kod razvoja igre vrlo brzo nastaje opasan obrazac:

* uvede se mala promjena
* djeluje da pomaže
* onda uvedeš još dvije ili tri
* poslije nekoliko sesija više nije jasno koja promjena je šta uradila
* problem se možda smanji na jednom mjestu, ali poraste na drugom

Bez patch dnevnika razvoj lako sklizne u:

* improvizovano “osjećam da je bolje” odlučivanje
* previše zakrpa bez dovoljno potvrde
* zaboravljanje stvarnog razloga za promjenu
* balansne i UX regresije koje se kasno primijete

Dobar patch log čuva uzrok, promjenu i rezultat na jednom mjestu.

---

## 3. Osnovni princip dokumenta

Glavno pravilo glasi:

> svaka zakrpa mora imati jasan problem koji pokušava riješiti i jasan način da se provjeri da li je uspjela.

To znači da patch ne smije biti samo:

* “malo smo pojačali ovo”
* “malo smo smanjili ono”
* “sad djeluje glađe”

Patch mora imati:

* cilj
* opseg
* očekivani efekat
* stvarni signal nakon testiranja

---

## 4. Šta patch review log jeste

Ovaj dokument treba da bude:

* istorija patch odluka unutar aktivne verzije
* most između revizionog workflow-a i playtest nalaza
* kontrolna tabla za patch uspješnost
* alat za prepoznavanje regresija i lažnih poboljšanja

---

## 5. Šta patch review log nije

Ovaj dokument nije:

* zamjena za globalni `CHANGELOG.md`
* zamjena za hypothesis tracker
* zamjena za balansnu watchlistu
* detaljan session report

`CHANGELOG.md` govori šta se promijenilo.
Ovaj dokument govori da li je ta promjena uradila ono što je trebala.

---

## 6. Kada koristiti patch review log

Patch review log treba koristiti kada:

* postoji jasna patch izmjena unutar aktivne verzije
* promjena dotiče sistem, balans, UX ili komponentni prikaz dovoljno da može uticati na igru
* postoji potreba da se kroz više sesija prati efekat te promjene

Ne treba ga koristiti za:

* čiste pravopisne ispravke
* minor formatting izmjene bez stvarnog efekta na igru ili repo disciplinu

---

## 7. Osnovne klase patch promjena

Svaki patch unos treba pripadati jednoj glavnoj klasi:

### 7.1. Balance Patch / Balansna zakrpa

Mijenja odnos snaga između stilova, završnice ili scaling modova.

### 7.2. System Patch / Sistemska zakrpa

Mijenja pravilo ili tok nekog sistema.

### 7.3. UX Patch / UX zakrpa

Mijenja aid, terminologiju, komponentni raspored ili čitljivost bez nužne promjene same mehanike.

### 7.4. Content Patch / Sadržajna zakrpa

Mijenja listu, tekst ili raspored sadržaja koji utiče na upotrebu i čitljivost, ali ne uvodi novi glavni sistem.

### 7.5. Hybrid Patch / Hibridna zakrpa

Dotiče više slojeva odjednom i zato traži pažljiviju provjeru.

Kritično pravilo:

> svaka zakrpa mora imati jednu primarnu klasu čak i ako dotiče više slojeva.

---

## 8. Obavezna struktura jednog patch unosa

Svaki patch unos u dnevniku mora sadržati najmanje:

1. **Patch ID**
2. **Verzija / patch oznaka**
3. **Klasa zakrpe**
4. **Problem koji se rješava**
5. **Šta je promijenjeno**
6. **Očekivani efekat**
7. **Rizik regresije**
8. **Kako se provjerava**
9. **Stvarni rezultat**
10. **Status zakrpe**
11. **Sljedeći korak**

Ova struktura mora ostati ista da bi patch unosi bili uporedivi.

---

## 9. Standard za Patch ID

Preporučeni format:

* `P-2.7-01`
* `P-2.7-02`
* `P-2.7a-01`
* `P-2.7b-01`

ID treba odmah da kaže:

* da je riječ o patch unosu
* kojoj verzionoj liniji pripada
* koji je redni broj u toj liniji

To pomaže da se patch lako poveže sa:

* changelogom
* playtest izvještajima
* hypothesis i watchlist signalima

---

## 10. Standard za “Problem koji se rješava”

Ovaj dio mora biti konkretan i dijagnostički jasan.

Dobar primjer:

* **Aggro/Aggro** u 2P prečesto zatvara partiju prije nego goods i stabilnost dobiju realnu završnu težinu.

Loš primjer:

* 2P djeluje malo off.

Ako problem nije dovoljno jasno definisan, patch će vjerovatno biti neprecizan.

---

## 11. Standard za “Šta je promijenjeno”

Ovaj dio mora navesti:

* tačnu mehaničku ili UX promjenu
* šta je ostalo isto
* koji dokumenti ili komponente su zahvaćeni

Ne smije ostati na nivou:

* “pojačano”
* “smanjeno”
* “pojednostavljeno”

Mora biti jasno šta je konkretno dirnuto.

---

## 12. Standard za “Očekivani efekat”

Ovaj dio mora odgovoriti:

* šta patch treba da popravi
* koji signal bi trebao oslabiti ili nestati
* koji signal bi trebao ojačati

Dobar primjer:

* povećati 2P comeback prozor bez smanjenja vrijednosti ranog mapnog pritiska.

To pomaže da poslije testiranja ne improvizuješ kriterij uspjeha.

---

## 13. Standard za “Rizik regresije”

Svaka patch promjena mora unaprijed priznati gdje bi mogla pokvariti nešto drugo.

Primjeri:

* zakrpa koja pomaže **Balanced Path/Balansirani put** može nehotice ugušiti **Aggro/Aggro** previše
* zakrpa koja pojačava coronation contest može povećati swing ili usporiti završnicu
* zakrpa koja smanjuje 4P pregovaračko usporenje može oslabiti diplomatiju previše

Bez ovog dijela lako se zaboravi da svaka popravka nosi tradeoff.

---

## 14. Standard za “Kako se provjerava”

Patch ne smije ući u sesije bez plana provjere.

Treba zapisati:

* koji player count je najvažniji za provjeru
* koji matchup je najvažniji
* da li treba fokusirani stres test ili normalna sesija
* koje metrike ili signale treba posebno posmatrati

To povezuje patch sa stvarnim test radom, a ne samo sa nadom.

---

## 15. Standard za “Stvarni rezultat”

Ovaj dio se popunjava tek nakon relevantnih sesija.

Treba sadržati:

* kratak sažetak signala
* da li je očekivani efekat ostvaren djelimično, potpuno ili uopšte nije
* da li se pojavio novi neželjeni efekat

Ne treba pisati dugi narativ.
Treba ostati kratak i jasan.

---

## 16. Standard za status zakrpe

Svaka zakrpa mora imati jedan od sljedećih statusa:

### 16.1. **Proposed/Predložena**

Ideja i plan postoje, ali patch još nije ugrađen.

### 16.2. **Implemented/Primijenjena**

Patch je ugrađen u dokumente ili prototip, ali još nije dovoljno provjeren.

### 16.3. **Testing/U testiranju**

Patch se aktivno provjerava kroz ciljane sesije.

### 16.4. **Validated/Potvrđena**

Patch je dao dovoljno jak signal da trenutno djeluje uspješno.

### 16.5. **Partially Effective/Djelimično uspješna**

Patch je nešto popravio, ali nije riješio cijeli problem ili je otvorio novi.

### 16.6. **Rejected/Odbačena**

Patch nije dao dobar rezultat ili je pogoršao sistem.

### 16.7. **Superseded/Zamijenjena**

Patch je kasnije zamijenjen boljom ili širim rješenjem.

Kritično pravilo:

> “Implemented/Primijenjena” nije isto što i “Validated/Potvrđena”.

---

## 17. Početne tipične patch teme za v2.7

Ovaj dokument treba posebno očekivati unose oko tema kao što su:

* 2P **Crown Pressure/Pritisak krune** korekcije
* **Aggro/Aggro** tempo kontrola
* **Balanced Path/Balansirani put** finishing power
* **Diplomatic Path/Diplomatski put** završni leverage
* **Coronation Attempt/Pokušaj krunisanja** contest i wow fino podešavanje
* 4P pregovaračko usporenje i treaty disciplina
* aid i komponentna čitljivost gdje utiču na percepciju sistema

Ovo nisu jedine teme, ali su među najlogičnijim patch rizicima za ovu verziju.

---

## 18. Veza sa session reportovima

Svaki ozbiljan patch unos treba biti povezan sa relevantnim:

* `playtests/session-report-template.md` izvještajima

To znači da patch ne smije živjeti odvojeno od sesija koje su ga inspirisale ili provjerile.

Bez tog mosta patch review log postaje previše apstraktan i slab za stvarni rad.

---

## 19. Veza sa hypothesis tracker dokumentom

Ako je patch direktno vezan za neku hipotezu, to treba zapisati.

Primjeri:

* patch postoji da ojača `BL-01`
* patch postoji da ponovo testira `EG-02`
* patch postoji da smanji signal protiv `SC-01`

Tako se kasnije lakše vidi:

* koje hipoteze su tražile najviše zakrpa
* koje su zakrpe zapravo pomogle da hipoteza pređe u potvrđeno stanje

---

## 20. Veza sa balance watchlist dokumentom

Ako je patch uveden zbog watchlist stavke, to mora biti jasno navedeno.

Primjeri:

* patch je reakcija na `WP-01`
* patch je reakcija na `EG-02`
* patch je reakcija na `SC-02`

Na taj način se može pratiti:

* da li se balansni rizik stabilizuje
* da li patch samo skriva problem u kratkom roku

---

## 21. Pravilo protiv patch stackinga bez provjere

Jedna od najvećih opasnosti je dodavanje više zakrpa na isti problem prije nego što se prva stvarno provjeri.

To nije zdravo, jer poslije više nije jasno:

* koja zakrpa je pomogla
* koja je napravila regresiju
* da li je problem stvarno riješen ili samo zamagljen

Dobro pravilo je:

* ne slagati više velikih patch-eva na istu osovinu bez barem jedne smislene serije provjere između njih

---

## 22. Pravilo protiv “patch placebo” efekta

Nakon što uvedeš zakrpu, lako je vidjeti poboljšanje samo zato što ga očekuješ.

Zato patch review mora tražiti:

* stvarni signal u sesijama
* više od jednog tester konteksta kad je moguće
* zapisane kontra-signale, ne samo pozitivne

Ovo je posebno važno za završnicu i balansne osovine gdje subjektivni utisak može biti vrlo jak.

---

## 23. Najčešće greške u radu sa patch revizijom

* patch nema dovoljno jasan problem
* patch nema jasan test fokus
* status prebrzo prelazi u **Validated/Potvrđena**
* regresija se ne zapisuje jer je patch “uglavnom pomogao”
* više patch-eva se spoji u jednu promjenu bez dovoljno traga
* changelog i patch review log se raziđu

---

## 24. Workflow pravilo za novi patch unos

Kad se otvara novi patch unos, treba provjeriti redom:

1. da li postoji jasan problem
2. da li je promjena dovoljno važna za patch log
3. da li je jasno šta se mijenja
4. da li je jasno šta bi bio uspjeh ili neuspjeh
5. da li postoji plan test provjere
6. koje hipoteze i watchlist stavke su povezane s patch-em

Ako ne prolazi ova pitanja, patch još nije spreman za ozbiljan unos.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li log postaje praktičniji ili birokratskiji?
2. da li bolje prati vezu između problema, promjene i rezultata?
3. da li pomaže otkrivanju regresija?
4. da li ostaje usklađen sa verzionim i playtest dokumentima?
5. da li ostaje dovoljno lagan za stvarnu upotrebu?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `VERSIONING.md`
* `CHANGELOG.md`
* `docs/revision-workflow.md`
* `docs/version-status.md`
* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`
* `playtests/session-report-template.md`
* `playtests/matchup-matrix.md`
* `GLOSSARY.md`

---

## 27. Završna napomena

**Patch Review Log / Dnevnik revizije zakrpa** mora ostati jedan od najvažnijih operativnih alata za razvoj unutar aktivne verzije **v2.7**.

Ako radi dobro:

* svaka zakrpa ima trag
* lakše se vidi šta je stvarno pomoglo
* regresije se brže otkrivaju
* patch odluke postaju manje impulsivne
* a prelazak u narednu verziju je mnogo čišći

Ako radi loše:

* zakrpe se gomilaju bez jasnog sjećanja i dokaza
* problemi se “krpe” bez razumijevanja
* tim počinje vjerovati placebo poboljšanjima
* a razvoj postaje sporiji i manje pouzdan nego što mora biti

Zato ovaj dokument mora ostati strog, konkretan i potpuno usklađen sa logikom **v2.7**.
