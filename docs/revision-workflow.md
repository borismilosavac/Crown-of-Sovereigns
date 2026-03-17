# revision-workflow.md

# Crown of Sovereigns v2.7 — Revision Workflow / Tok revizije

## Status dokumenta

* **Dokument:** `docs/revision-workflow.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati kako se predlažu, procjenjuju, odobravaju i ugrađuju izmjene kroz dokumentaciju i naredne patch iteracije
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Revision/Revizija**, **Patch/Zakrpa**, **Canonical/Kanonsko**
* **Povezani dokumenti:** `VERSIONING.md`, `CHANGELOG.md`, `docs/version-status.md`, `docs/repository-structure.md`, `gdd/canonical-decisions.md`, `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `playtests/balance-watchlist.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uspostavi jasan tok kako promjena ide od ideje do kanonske revizije
* spriječi da se dokumenti mijenjaju stihijski i bez traga
* razdvoji sitne korekcije od stvarnih dizajnerskih promjena
* omogući da svaka važna izmjena ima razlog, dokaz i posledicu
* zaštiti **v2.7** od tihog raspadanja kroz nekontrolisane mikro-izmjene

Ovo nije samo administrativni dokument.
Ovo je zaštitni okvir koji čuva disciplinu razvoja.

---

## 2. Zašto je revision workflow kritičan

Kod projekta kao što je **Crown of Sovereigns v2.7**, problemi vrlo brzo nastaju ako ne postoji jasan tok revizije:

* jedan dokument se promijeni, a zavisni dokumenti ostanu stari
* patch se primijeni djelimično, ali se ponaša kao da je potpuno usvojen
* playtest feedback utiče na sistem bez jasnog zapisa zašto
* isti pojam ili pravilo dobije dvije verzije u dva dokumenta
* ljudi više ne znaju šta je aktivno, a šta samo ideja

Dobar revision workflow ne usporava razvoj. On sprečava skupe greške i lažnu sigurnost.

---

## 3. Osnovni princip revizije

Glavno pravilo glasi:

> nijedna važna izmjena ne smije postati kanonska samo zato što djeluje razumno; mora imati jasan razlog, jasan trag i jasan status.

To znači da svaka ozbiljna promjena mora imati najmanje:

* razlog
* opseg
* dokaz ili testni motiv
* dokumente koje dotiče
* status

Bez toga promjena ostaje samo prijedlog ili improvizacija.

---

## 4. Šta revision workflow jeste

Ovaj workflow treba da bude:

* jasan proces odlučivanja
* most između playtest nalaza i kanonskih izmjena
* sistem za kontrolu zavisnosti između dokumenata
* filter protiv verzionog haosa

---

## 5. Šta revision workflow nije

Ovaj workflow nije:

* birokratska prepreka za svaku sitnicu
* izgovor da se ništa ne mijenja dok sve nije savršeno dokazano
* zamjena za dobru dizajnersku prosudbu
* beskonačni approval proces

Cilj je disciplina, ne paraliza.

---

## 6. Osnovne klase revizija

Sve revizije u projektu treba posmatrati kroz najmanje ove klase:

### 6.1. Editorial Revision / Urednička revizija

Promjene koje ne mijenjaju sistemsko značenje.

Primjeri:

* pravopis
* stil pisanja
* preciznije formulacije bez promjene mehanike
* bolja unutrašnja povezanost dokumenta

### 6.2. Clarification Revision / Pojašnjavajuća revizija

Promjene koje ne mijenjaju sistem, ali pojašnjavaju kako sistem treba razumjeti ili prikazati.

Primjeri:

* jasniji wording pravila
* bolja aid formulacija
* preciznije definisani odnosi između dva postojeća pravila

### 6.3. UX Revision / UX revizija

Promjene koje mijenjaju kako se sistem čita, prikazuje ili koristi, bez nužne promjene mehaničke logike.

Primjeri:

* promjena aid strukture
* promjena label hijerarhije
* promjena board ili player board organizacije

### 6.4. System Revision / Sistemska revizija

Promjene koje mijenjaju mehaničku logiku sistema.

Primjeri:

* nova pravila za treaty raskid
* promjena kako radi stabilnost prag
* promjena combat toka

### 6.5. Canon Revision / Kanonska revizija

Promjene koje mijenjaju zaključane projektne odluke i postaju dio nove radne osnove verzije.

Primjeri:

* promjena aktivne verzije iz **v2.7** u **v2.8**
* zaključavanje novog završnog sistema
* uklanjanje ili zamjena glavnog sistema

Kritično pravilo:

> što je revizija viša po ozbiljnosti, to jači mora biti trag i dokaz za nju.

---

## 7. Osnovni tok revizije

Svaka ozbiljnija promjena treba ići ovim redoslijedom:

1. **Trigger/Okidač**
2. **Diagnosis/Dijagnoza**
3. **Proposal/Prijedlog**
4. **Scope Check/Provjera opsega**
5. **Dependency Check/Provjera zavisnosti**
6. **Status Decision/Odluka o statusu**
7. **Document Update/Ažuriranje dokumenata**
8. **Version/Changelog Update/Ažuriranje verzije i changeloga**
9. **Validation/Test provjera**

Ako se preskoče srednji koraci, najčešće nastaje djelimično ažuriran sistem.

---

## 8. Trigger / Okidač revizije

Revizija obično počinje iz jednog od ovih izvora:

* playtest nalaz
* hypothesis tracker promjena statusa
* balance watchlist eskalacija
* UX konfuzija ponovljena kroz više partija
* nova produkcijska ili komponentna prepreka
* otkrivena kontradikcija između dokumenata

Važno pravilo:

* “imam ideju” nije dovoljan okidač za kanonsku promjenu bez dijagnoze i opsega.

---

## 9. Diagnosis / Dijagnoza

Prije bilo kakve izmjene mora se jasno zapisati:

* šta je tačan problem
* da li je problem sistemski, UX, sadržajni, terminološki ili produkcijski
* koliko je ozbiljan
* da li se ponovio ili je viđen samo jednom

Bez dobre dijagnoze postoji veliki rizik da se liječi simptom umjesto uzroka.

---

## 10. Proposal / Prijedlog

Nakon dijagnoze piše se jasan prijedlog revizije.

Dobar prijedlog mora sadržati:

* šta se tačno mijenja
* šta ostaje isto
* zašto je promjena vjerovatno bolja
* koji je očekivani tradeoff
* koje dokumente i komponente zahvata

Loš prijedlog zvuči kao:

* “treba malo pojačati ovo”
* “možda da pojednostavimo ono”

Takav prijedlog nije dovoljno operativan.

---

## 11. Scope Check / Provjera opsega

Ovaj korak služi da se utvrdi kolika je promjena zapravo.

Treba odgovoriti:

* da li je ovo editorial, clarification, UX, system ili canon revizija
* da li mijenja samo jedan dokument ili više slojeva repozitorijuma
* da li traži playtest prije prihvatanja ili je sigurna kao dokumentacijska korekcija

Mnogo grešaka nastaje kad se sistemska promjena tretira kao “samo wording fix”.

---

## 12. Dependency Check / Provjera zavisnosti

Prije usvajanja promjene mora se pogledati:

* koje dokumente ova promjena direktno dotiče
* koje dokumente indirektno dotiče
* da li su `Povezani dokumenti` i `Dependency notes` dovoljni da ništa ne ostane van revizije

Ovaj korak je posebno važan za:

* `systems/`
* `content/`
* `components/`
* `ux/`
* `playtests/`

Ako jedan od ovih slojeva ostane neusklađen, verziona disciplina puca.

---

## 13. Status Decision / Odluka o statusu

Nakon provjere opsega i zavisnosti, promjena dobija status.

Preporučeni statusi promjene su:

* **Proposed/Predloženo**
* **Under Review/U reviziji**
* **Approved/Odobreno**
* **Implemented/Primijenjeno**
* **Validated/Potvrđeno kroz provjeru**
* **Rejected/Odbijeno**
* **Deferred/Odloženo**

Kritično pravilo:

> “Implemented” nije isto što i “Validated”.

Promjena može biti ugrađena u dokumente, ali još ne potvrđena u praksi.

---

## 14. Kada promjena ide odmah, a kada mora čekati test

### Može ići odmah

* čista editorial korekcija
* terminološko usklađivanje bez promjene značenja
* layout/UX pojašnjenje koje ne dira mehaniku

### Mora čekati test ili jaču provjeru

* sistemska promjena pravila
* balansna korekcija
* promjena završnog pritiska
* promjena 2P / 3P / 4P korektiva
* promjena koja dotiče više **Win Paths/Putanja do pobjede**

Ako se ove dvije grupe miješaju, prebrzo se uvode promjene koje nemaju dovoljno potvrde.

---

## 15. Pravilo jedne aktivne kanonske osnove

U svakom trenutku mora postojati samo jedna aktivna kanonska osnova razvoja.

To znači:

* trenutno je to **v2.7**
* sve radne revizije se odnose na nju dok se ne zaključa nova verzija
* ne smije postojati paralelni “skoro-kanonski” paket promjena bez jasnog statusa

Ako se to pravilo prekrši, vrlo brzo se miješaju:

* aktivna baza
* eksperimentalne izmjene
* i nepotvrđeni patch pokušaji

---

## 16. Pravilo patch revizija

Kad se radi unutar iste glavne verzije, može se koristiti patch logika.

Primjeri:

* **v2.7a**
* **v2.7b**
* **v2.7.1**

Ali samo ako postoji stvarna potreba za preciznijim praćenjem.

Patch revizija treba da znači:

* ograničen skup promjena
* jasan razlog
* jasan playtest fokus

Patch ne smije postati način da se skriva da je u stvari napravljena nova mini-verzija bez priznanja.

---

## 17. Pravilo kanonskog zaključavanja

Kada je promjena dovoljno jaka da postane dio aktivne verzije, mora se ažurirati najmanje:

* relevantni dokument(i)
* `CHANGELOG.md`
* `docs/version-status.md`
* po potrebi `gdd/canonical-decisions.md`

Ako ova 4 mjesta nisu usklađena gdje je relevantno, promjena nije stvarno kanonski zaključana.

---

## 18. Pravilo protiv tihih izmjena

Jedna od najvećih opasnosti je tiha izmjena: dokument se promijeni, ali bez traga.

To nije dozvoljeno za:

* systems logiku
* balance korekcije
* završne i scaling promjene
* terminologiju koja utiče na više slojeva

Sve takve promjene moraju ostaviti trag kroz:

* changelog
* status dokumenta
* ili jasno opisanu revizijsku napomenu

---

## 19. Pravilo revizije po slojevima

Kad promjena dotiče više slojeva, preporučeni redoslijed ažuriranja je:

1. `gdd/` ili `systems/` ako se mijenja jezgro
2. `rules/` ako se mijenja kako igrač to čita ili igra
3. `content/` ako se mijenja sadržajna implementacija
4. `components/` i `ux/` ako se mijenja prikaz i korištenje
5. `visuals/` ako se mijenja wireframe ili layout implikacija
6. `playtests/` ako se mijenja fokus provjere

Ovo pomaže da tok izmjene ide od jezgra ka prikazu, a ne obrnuto.

---

## 20. Pravilo “ne liječiš layout sistemskom promjenom”

Ako problem nastaje zato što komponenta ili aid loše komuniciraju sistem, to se ne smije automatski tretirati kao sistemski kvar.

Prvo treba provjeriti:

* da li je problem u rules logici
* da li je problem u terminologiji
* da li je problem u komponentnom prikazu
* da li je problem u onboarding sekvenci

Mnogi skupi i nepotrebni system patch-evi nastaju kada je pravi problem zapravo UX ili layout.

---

## 21. Najčešće greške u toku revizije

* promjena se uvede prije nego što je problem dovoljno dijagnostikovan
* mijenja se više velikih stvari odjednom bez traga
* zavisni dokumenti se ne ažuriraju
* patch se ponaša kao kanonski iako nije validiran
* changelog zaostaje za stvarnim stanjem
* editorial korekcija se koristi da sakrije stvarnu sistemsku promjenu

---

## 22. Workflow pravilo za novu reviziju

Kad se predlaže nova revizija, treba provjeriti redom:

1. šta je tačan problem
2. kojoj klasi revizije pripada
3. koji je opseg promjene
4. koje dokumente dotiče
5. da li traži playtest provjeru
6. da li mijenja kanonsku osnovu ili samo poboljšava postojeći sloj

Ako ne prolazi ova pitanja, revizija još nije spremna za usvajanje.

---

## 23. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li workflow postaje jasniji ili mutniji?
2. da li pomaže disciplini ili uvodi nepotrebnu birokratiju?
3. da li razlikuje male i velike izmjene dovoljno jasno?
4. da li pomaže da se verzije manje miješaju?
5. da li ostaje praktičan za stvaran rad?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 24. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `VERSIONING.md`
* `CHANGELOG.md`
* `docs/version-status.md`
* `docs/repository-structure.md`
* `gdd/canonical-decisions.md`
* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`
* `GLOSSARY.md`

---

## 25. Završna napomena

**Revision Workflow / Tok revizije** mora ostati jedan od glavnih infrastrukturnih dokumenata projekta.

Ako radi dobro:

* promjene imaju trag
* verzije se manje miješaju
* sistemi i dokumenti ostaju usklađeni
* patch odluke postaju jasnije i sigurnije
* a cijeli projekat djeluje ozbiljnije i mnogo otpornije na haos

Ako radi loše:

* izmjene se uvode prebrzo ili bez traga
* dokumenti se razilaze
* playtest nalazi se gube u priči
* a razvoj postaje sporiji, skuplji i manje pouzdan

Zato ovaj dokument mora ostati strog, jasan i potpuno usklađen sa kanonskom logikom **v2.7**.
