# cards-spec.md

# Crown of Sovereigns v2.7 — Cards Specification / Specifikacija karata

## Status dokumenta

* **Dokument:** `components/cards-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati vrste, funkciju, osnovne zahtjeve i komponentne granice za sve **Cards/Karte** elemente u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Card/Karta**, **Treaty Card/Karta sporazuma**, **Event Card/Karta događaja**
* **Povezani dokumenti:** `visuals/card-wireframe-notes.md`, `components/terminology-and-labels.md`, `components/iconography-spec.md`, `content/treaties-list.md`, `content/events-and-crises.md`, `content/coronation-content.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše koje vrste **Cards/Karte** postoje u CoS v2.7
* objasni čemu svaka vrsta karte služi u sistemu
* spriječi da karte postanu preširoka kategorija u koju se trpa sve što nema drugo mjesto
* uskladi kartični sistem sa sadržajem, wireframe logikom, terminologijom i produkcijskom disciplinom
* pripremi čist osnov za kasniji grafički handoff, prototip izradu i eventualni produkcijski obračun

Ovo nije content dokument sa punim spiskom svih karata.
Ovo je komponentna specifikacija za to kako kartični sistem treba da bude strukturisan.

---

## 2. Zašto je kartični sistem kritičan

Karte su često najbrži način da igra dobije:

* varijabilnost
* jasan sadržajni signal
* proceduralnu pomoć
* političku i situacionu tenziju

Ali karte su i brz put do problema ako nisu disciplinovane.

Loše definisan kartični sistem vodi ka:

* previše različitih tipova karata
* previše teksta po karti
* lošem onboarding-u
* neujednačenom layoutu
* produkcijskom bloatu

Zato CoS mora imati jasan odgovor na pitanje:

> koje karte postoje, zašto postoje i šta nije dovoljno važno da bude karta.

---

## 3. Osnovni princip kartičnog dizajna

Glavno pravilo glasi:

> karta mora postojati samo onda kada je sadržaj, stanje ili procedura dovoljno kompaktna, dovoljno važna i dovoljno promjenjiva da kartični format stvarno donosi vrijednost.

To znači da karta ne smije postojati samo zato što:

* je zgodna za dizajn
* djeluje “bogatije”
* zamjenjuje slab sistemski opis
* nosi nešto što bi bolje stajalo na tabli, aid-u ili track-u

Ako karta ne donosi jasnoću, varijabilnost ili tempo korist, vjerovatno nije pravi alat za taj posao.

---

## 4. Šta kartični sistem jeste

Kartični sistem treba da bude:

* ograničen
* funkcionalan
* lako čitljiv
* tipološki jasan
* kompatibilan sa onboardingom i produkcijskom disciplinom

---

## 5. Šta kartični sistem nije

Kartični sistem nije:

* skladište za sve zanimljive ideje
* način da se pravila sakriju u pojedinačne karte umjesto jasno dokumentuju
* dekorativni dodatak koji nosi više estetike nego mehaničke vrijednosti
* izgovor za povećanje broja komponenti bez dovoljno jakog razloga

Ako karta postoji samo zato da igra izgleda “veća”, to je loš razlog.

---

## 6. Glavne funkcije karata u CoS v2.7

Karte u ovoj verziji treba da služe najmanje ovim funkcijama:

1. formalizacija političkih odnosa kroz **Treaty Cards/Karte sporazuma**
2. javni ritamski i pritisni signal kroz **Event Cards/Karte događaja** i **Crisis Cards/Karte kriza**
3. podrška završnim i coronation referencama gdje kartični format donosi jasnoću
4. podrška sadržajnoj raznolikosti bez širenja osnovnih pravila na previše novih podsistema
5. pomoć čitljivosti i proceduralnoj jasnoći, a ne otežavanje istih

Ako karta radi samo četvrtu stvar bez prve, druge, treće i pete, vjerovatno je suvišna.

---

## 7. Osnovne klase karata

Sve **Cards/Karte** u CoS v2.7 treba podijeliti najmanje na ove glavne klase:

### 7.1. Treaty Cards / Karte sporazuma

Formalni politički odnosi, npr. **Alliance/Savez**, **Truce/Primirje**, **Trade Pact/Trgovački pakt**.

### 7.2. Event Cards / Karte događaja

Karte koje mijenjaju kontekst runde ili prioritete partije.

### 7.3. Crisis Cards / Karte kriza

Karte koje testiraju kraljevstva i pojačavaju pritisak.

### 7.4. Coronation Reference Cards / Referentne karte krunisanja

Karte ili kartične reference vezane za završni **Coronation Attempt/Pokušaj krunisanja** sistem, samo ako kartični format ostaje najsmisleniji.

### 7.5. Optional Special Cards / Opcione posebne karte

Samo ako buduća iteracija pokaže jasan razlog da neka posebna funkcija traži kartični oblik bez otvaranja novog bloata.

Kritično pravilo:

> svaka karta mora imati jednu jasnu primarnu klasu i ne smije se ponašati kao hibrid nekoliko tipova bez vrlo jakog razloga.

---

## 8. Obavezna struktura jedne kartične specifikacije

Svaka kartična klasa treba biti dokumentovana ovim redom:

1. **Naziv klase:** English/Srpski
2. **Primarna funkcija**
3. **Ko je koristi ili čita**
4. **Kada ulazi u partiju**
5. **Koliko mora biti čitljiva na prvi pogled**
6. **Koji je minimalni sadržaj karte**
7. **Šta ne smije da zbuni**
8. **Wireframe i ikonografska napomena**

Ovo pomaže da svi tipovi karata ostanu produkcijski i UX dosljedni.

---

## 9. Treaty Cards / Karte sporazuma

### 9.1. Primarna funkcija

Formalizuju političke odnose tako da diplomatija bude javna, mjerljiva i dovoljno ozbiljna da utiče na tok partije.

### 9.2. Ko ih koristi ili čita

Prvenstveno svi igrači za stolom, jer treaty stanje treba biti javno čitljivo.

### 9.3. Kada ulaze u partiju

Tokom **Diplomatic Window/Diplomatski prozor** ili drugih formalnih političkih trenutaka koje sistem dopušta.

### 9.4. Minimalni sadržaj

* naziv sporazuma
* klasa sporazuma
* benefit
* obaveza / ograničenje
* uslov raskida ili posljedica **Betrayal/Izdaja**

### 9.5. Glavna opasnost

Ako treaty karta postane preduga ili pravnički teška, diplomatija usporava i gubi eleganciju.

---

## 10. Event Cards / Karte događaja

### 10.1. Primarna funkcija

Uvode promjenu okolnosti i fokusiraju rundu na određeni politički, ekonomski, teritorijalni ili stabilnost pritisak.

### 10.2. Ko ih koristi ili čita

Svi igrači, jer su dio zajedničkog ritma partije.

### 10.3. Kada ulaze u partiju

Na početku runde ili u jasno definisanom zajedničkom proceduralnom trenutku.

### 10.4. Minimalni sadržaj

* naziv događaja
* tip događaja
* glavni efekat
* trajanje ili okvir važenja

### 10.5. Glavna opasnost

Ako event karta postane previše duga ili previše granularna, prestaje biti ritamski signal i postaje pravilo u mini-knjižici.

---

## 11. Crisis Cards / Karte kriza

### 11.1. Primarna funkcija

Uvode ozbiljniji test za kraljevstva i pojačavaju važnost unutrašnje i spoljne otpornosti.

### 11.2. Ko ih koristi ili čita

Svi igrači, jer kriza treba da bude javno razumljiv sistemski pritisak.

### 11.3. Kada ulaze u partiju

U kriznim ili kasnim segmentima runde i partije kada sistem traži pojačani test.

### 11.4. Minimalni sadržaj

* naziv krize
* tip krize
* šta testira
* glavni pritisak / posljedica
* kako se contestuje ili trpi

### 11.5. Glavna opasnost

Ako krizna karta izgleda samo kao “teži event”, bez jasnog identiteta, igrači slabije čitaju njenu ozbiljnost.

---

## 12. Coronation Reference Cards / Referentne karte krunisanja

### 12.1. Primarna funkcija

Podržavaju završni **Coronation Attempt/Pokušaj krunisanja** kroz jasan referentni ili proceduralni prikaz ako kartični format donosi stvarnu korist.

### 12.2. Ko ih koristi ili čita

Svi igrači u završnom segmentu partije.

### 12.3. Kada ulaze u partiju

Samo kada završni sistem postane relevantan.

### 12.4. Minimalni sadržaj

* coronation identitet
* ulazni uslov ili aktivacija
* contest prostor
* ishod ili jasan referentni podsjetnik

### 12.5. Glavna opasnost

Ako ova karta izgleda kao još jedan event ili obična scoring karta, završni signal slabi.

---

## 13. Optional Special Cards / Opcione posebne karte

Ova grupa ne smije postati kanta za “sve ostalo”.

Opciona posebna karta smije se uvesti samo ako:

* ima jasnu funkciju koju drugi alat ne pokriva bolje
* ne otvara novi sistemski bloat
* ne slabi preglednost postojećih kartičnih klasa

Ako novi sadržaj samo traži “možda posebnu kartu”, to nije dovoljno dobar razlog.

---

## 14. Card count discipline / Disciplina broja karata

CoS v2.7 mora imati strogu disciplinu u broju karata.

To znači:

* svaka nova kartična klasa mora opravdati svoje postojanje
* broj karata po klasi treba biti vođen sistemskom potrebom, ne željom za većim box utiskom
* treba izbjegavati kartični višak koji otežava teach, setup, sortiranje i balansnu provjeru

Pravilo:

> više karata nije automatski više dubine.

---

## 15. Card size and format / Veličina i format karata

Veličina i format karata moraju služiti čitljivosti i produkcijskoj disciplini.

To znači:

* ne koristiti više različitih formata bez jakog razloga
* glavni kartični format treba pokrivati većinu klasa ako je moguće
* manji ili posebni format smije postojati samo ako ima jasan UX razlog

Previše različitih formata povećava:

* proizvodni rizik
* logistiku prototipa
* složenost zaštite, sortiranja i grafičkog rada

---

## 16. Card and wireframe relation / Odnos karata i wireframea

Sve kartične klase moraju biti kompatibilne sa:

* `visuals/card-wireframe-notes.md`

To znači:

* specifikacija karte definiše funkciju i sadržajni minimum
* wireframe dokument definiše raspored i hijerarhiju tih informacija

Ne smije se desiti da komponentna specifikacija traži nešto što wireframe realno ne može nositi bez prenatrpavanja.

---

## 17. Card and terminology relation / Odnos karata i terminologije

Sve karte moraju slijediti:

* `components/terminology-and-labels.md`

To znači:

* dosljedan **English/Srpski** standard tamo gdje je potreban
* bez paralelnih naziva za iste kartične klase
* bez “grafički zgodnijih” preimenovanja koja kvare dosljednost sa pravilima i sadržajnim dokumentima

---

## 18. Card and iconography relation / Odnos karata i ikonografije

Karte treba da koriste ikonografiju kao podršku, ne kao zamjenu za čitljiv tekst.

To znači:

* najvažniji tip, resurs ili sistemski signal može imati ikonu
* glavni efekat ne smije biti pojeden ikonama
* ikone ne smiju stvoriti osjećaj da karta ima više pod-sistema nego što stvarno ima

Kartični UX treba ostati tekstualno jasan i skenabilan.

---

## 19. Card and information hierarchy relation / Odnos karata i hijerarhije informacija

Svaka kartična klasa mora pratiti logiku:

* naziv i tip = brzo prepoznavanje
* glavni efekat = primarna informacija
* trajanje / uslov / posljedica = sekundarna informacija
* atmosferični ili dekorativni sloj = tercijarni sloj

Ako karta ovu hijerarhiju izgubi, čitanje se usporava bez obzira na kvalitet sadržaja.

---

## 20. Card and onboarding relation / Odnos karata i onboardinga

Kartični sistem mora ostati dovoljno čist za prvu partiju.

To znači:

* glavni tipovi karata moraju se lako razlikovati
* tekst na kartama mora biti dovoljno jasan da ne traži stalno dodatno tumačenje
* broj izuzetaka i rubnih formulacija mora ostati pod kontrolom

Ako karte djeluju kao najveći izvor zbunjenosti u ranoj partiji, sistem je previše gust ili slabo organizovan.

---

## 21. Card setup and teardown discipline / Disciplina setupa i raspremanja karata

Treba procijeniti i:

* koliko različitih špilova ili paketa karata postoji
* koliko je sortiranje intuitivno
* da li se karte lako vraćaju u pravilan poredak ili grupu
* da li broj kartičnih grupa otežava pripremu partije bez dovoljno razloga

Kartični sistem ne smije biti logistički teži nego što njegov gameplay dobitak opravdava.

---

## 22. Najčešće greške u kartičnom sistemu

* previše različitih tipova karata
* treaty karte koje zvuče kao pravni dokumenti
* event i crisis karte koje izgledaju ili se čitaju previše slično
* coronation reference koje ne djeluju završno i posebno
* posebne karte koje postoje bez jasnog razloga
* kartični count koji raste brže od stvarnog kvaliteta igre

---

## 23. Workflow pravilo za novu kartičnu klasu

Ako se predlaže nova kartična klasa, treba provjeriti redom:

1. koju funkciju karta rješava
2. da li je kartični format zaista najbolji alat za tu funkciju
3. da li već postojeća klasa može nositi taj sadržaj
4. da li nova klasa povećava onboarding i produkcijski teret
5. da li wireframe i komponentni sistem mogu zdravo podržati novu klasu
6. da li njen benefit opravdava novi špil, novu logiku i novi set revizija

Ako ne prolazi ova pitanja, nova kartična klasa se ne uvodi.

---

## 24. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li kartični sistem ostaje ograničen i jasan?
2. da li nova karta ili klasa donosi stvarni gameplay benefit?
3. da li ostaje usklađena sa content i wireframe dokumentima?
4. da li ostaje kompatibilna sa terminologijom i ikonografijom?
5. da li smanjuje ili povećava produkcijski i onboarding teret?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `visuals/card-wireframe-notes.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `content/treaties-list.md`
* `content/events-and-crises.md`
* `content/coronation-content.md`
* `ux/information-hierarchy.md`
* `GLOSSARY.md`

---

## 26. Završna napomena

**Cards Specification / Specifikacija karata** mora ostati jedan od glavnih filtera protiv kartičnog bloata i nečistog sadržajnog širenja u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* tipovi karata su jasni
* onboarding ostaje zdrav
* sadržaj dobija pravi kartični dom samo kada to ima smisla
* grafički handoff je stabilniji
* a produkcijski okvir ostaje disciplinovan

Ako radi loše:

* karte se množe bez potrebe
* layout postaje teži
* teach i setup postaju sporiji
* a igra djeluje šira i mutnija nego što treba

Zato ovaj dokument mora ostati strog, funkcionalan i potpuno usklađen sa logikom **v2.7**.
