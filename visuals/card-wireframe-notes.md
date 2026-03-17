# card-wireframe-notes.md

# Crown of Sovereigns v2.7 — Card Wireframe Notes / Bilješke za wireframe karata

## Status dokumenta

* **Dokument:** `visuals/card-wireframe-notes.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati funkcionalne i vizuelne principe za wireframe i layout svih tipova karata u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Card/Karta**, **Treaty/Sporazum**, **Event/Događaj**, **Goods/Roba**
* **Povezani dokumenti:** `components/terminology-and-labels.md`, `components/iconography-spec.md`, `ux/information-hierarchy.md`, `content/treaties-list.md`, `content/events-and-crises.md`, `content/coronation-content.md`, `ux/player-aid-system.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše kako karte treba da budu organizovane prije finalnog grafičkog dizajna
* uskladi layout sa stvarnim gameplay potrebama
* spriječi da karte postanu lijepe, ali spore za čitanje
* postavi jasan wireframe standard za sve tipove karti
* smanji broj kasnijih grafičkih i UX iteracija

Ovo nije završni art direction dokument.
Ovo je funkcionalna osnova za raspored informacija na kartama.

---

## 2. Zašto je wireframe karata kritičan

U CoS v2.7 karte nose važan dio sistema i sadržaja:

* **Treaty/Sporazum** odnose
* **Event/Događaj** i **Crisis/Kriza** pritiske
* moguće goods, završne ili posebne reference
* završne coronation sadržaje gdje je primjenjivo

Ako wireframe radi loše:

* karte se sporije čitaju
* onboarding postaje teži
* ikonografija i tekst se počinju sudarati
* playtest feedback je slabiji jer ljudi više komentarišu konfuziju nego samu igru

Zato wireframe mora biti dizajniran iz gameplay logike, ne iz dekorativne logike.

---

## 3. Osnovni princip dizajna karata

Glavno pravilo glasi:

> karta mora prvo biti brzo čitljiva, pa tek onda vizuelno bogata.

To znači:

* igrač mora odmah vidjeti šta gleda
* tip karte mora biti jasan u manje od sekunde
* glavni efekat mora biti čitljiv bez traženja po karti
* sekundarne informacije ne smiju nadjačati primarne

Ako karta izgleda odlično, ali se čita sporo, wireframe nije uspješan.

---

## 4. Šta wireframe bilješke jesu

Ove bilješke treba da služe kao:

* funkcionalni kostur layouta
* kontrolni dokument prije ilustracije i završnog stila
* osnova za provjeru šta ide u koji dio karte
* filter protiv tekstualnog i ikonografskog bloata

---

## 5. Šta wireframe bilješke nisu

Ove bilješke nisu:

* finalni grafički stil
* moodboard za ilustraciju
* poziv da svaka karta ima poseban raspored
* opravdanje za ekstremnu asimetriju layouta između sličnih karti

Ako svaki tip karte dobije previše drugačiji layout bez jakog razloga, igračko čitanje će biti sporije.

---

## 6. Glavne funkcije dobrog wireframe sistema

Wireframe karata mora raditi najmanje 6 stvari:

1. jasno razlikovati tipove karata
2. jasno prikazati naziv i klasu
3. jasno prikazati glavni efekat
4. jasno odvojiti uslov, trajanje i posljedicu ako postoje
5. ostati kompatibilan sa ikonografijom i terminologijom
6. ostati čitljiv u print prototipu i finalnoj verziji

Ako radi samo prve tri stvari, karta će biti čitljiva, ali možda proceduralno slaba.
Ako pokuša raditi sve kroz previše blokova, karta postaje prenatrpana.

---

## 7. Glavni tipovi karata koje wireframe mora pokriti

Wireframe sistem mora podržavati najmanje sljedeće tipove:

### 7.1. Treaty Cards / Karte sporazuma

Za **Alliance/Savez**, **Truce/Primirje**, **Trade Pact/Trgovački pakt** i srodni formalni diplomatski sadržaj.

### 7.2. Event Cards / Karte događaja

Za aktivne ritamske ili kontekstualne promjene partije.

### 7.3. Crisis Cards / Karte kriza

Za ozbiljnije sistemske testove i završnu kompresiju.

### 7.4. Coronation Reference Cards / Referentne karte krunisanja

Ako se fizički koriste kao podsjetnik ili modul završnog sistema.

### 7.5. Goods or Special Reference Cards / Karte robe ili posebne reference

Samo ako se pokaže da je stvarno potreban kartični oblik za neki dio goods ili posebnog sistema.

Kritično pravilo:

> isti tip karte treba da ima isti osnovni wireframe jezik kroz cijelu igru.

---

## 8. Zajednički osnovni blokovi svih karata

Bez obzira na tip, većina karata treba da dijeli ove osnovne zone:

### 8.1. Header / Zaglavlje

Mjesto za naziv i tip karte.

### 8.2. Type Strip / Traka tipa

Mjesto koje odmah signalizira kojoj klasi karta pripada.

### 8.3. Main Effect Block / Blok glavnog efekta

Najvažniji dio karte. Tu ide ono što igrač mora prvo razumjeti.

### 8.4. Secondary Rules Block / Blok sekundarnih pravila

Mjesto za trajanje, ograničenje, uslov ili posljedicu.

### 8.5. Reminder / Aid Footer / Podsjetnik ili aid podnožje

Mjesto za ultra-kratak podsjetnik ako je stvarno potreban.

Ne moraju sve karte koristiti sve blokove istim intenzitetom, ali wireframe treba da zadrži ovu logiku kao osnovu.

---

## 9. Header / Zaglavlje standard

Zaglavlje mora odmah reći:

* naziv karte
* tip karte
* osnovni identitet

Zaglavlje ne smije:

* biti previše dekorativno
* zauzeti previše prostora u odnosu na glavni efekat
* koristiti ornament koji smanjuje čitljivost naziva

Naziv je važan, ali efekat je važniji od ornamentalnog okvira naslova.

---

## 10. Type Strip / Traka tipa

Ova traka mora pomoći da igrač odmah zna koju vrstu logike očekuje.

Na primjer:

* **Treaty/Sporazum** karta mora odmah izgledati kao treaty karta
* **Event/Događaj** karta mora odmah izgledati kao event karta
* **Crisis/Kriza** karta mora odmah izgledati kao ozbiljniji test, ne isto što i event

Razlika može dolaziti iz:

* pozicije tipa
* tonalne trake
* jasne tekstualne klase
* kontrolisane ikonografije

Ali nikad ne smije zavisiti samo od boje.

---

## 11. Main Effect Block / Blok glavnog efekta

Ovo je najvažnija zona svake karte.

### 11.1. Šta mora raditi

Mora omogućiti da igrač u 1–2 sekunde razumije:

* šta karta radi
* na koga ili šta utiče
* koji je glavni mehanički pomak

### 11.2. Šta ne smije raditi

Ne smije:

* biti zakopan između previše ikona
* biti prelomljen u previše kratkih linija bez logike
* biti sitniji od sporednih blokova

Ako glavni efekat nije vizuelni fokus, karta ne radi.

---

## 12. Secondary Rules Block / Blok sekundarnih pravila

Ova zona služi za:

* uslove
* trajanje
* posljedicu raskida ili neuspjeha
* contest uslove gdje je relevantno

Sekundarni blok mora biti jasno odvojen od glavnog efekta.

To znači:

* druga hijerarhija veličine
* jasna pozicija
* dovoljno razmaka

Igrač mora moći prvo pročitati glavni efekat, pa tek onda dublji kontekst.

---

## 13. Reminder / Aid Footer / Podsjetnik ili aid podnožje

Ovaj blok je opcioni i treba ga koristiti štedljivo.

Koristan je kada:

* karta nosi važan proceduralni podsjetnik
* kratka posljedica ili trajanje treba biti stalno vidljivo
* aid funkcija može ubrzati igru bez dodatnog lookupa

Ne treba ga koristiti kada samo ponavlja ono što karta već jasno kaže.

---

## 14. Wireframe za Treaty Cards / Karte sporazuma

Ove karte moraju naglasiti:

* tip sporazuma
* benefit
* obavezu / ograničenje
* uslov raskida ili **Betrayal/Izdaja** posljedicu

Preporučeni red čitanja je:

1. naziv i treaty klasa
2. glavni benefit
3. glavna obaveza
4. raskid / izdaja posljedica

Ako treaty karta ne komunicira tradeoff u prva dva pogleda, wireframe je slab.

---

## 15. Wireframe za Event Cards / Karte događaja

Ove karte moraju naglasiti:

* da se radi o promjeni okolnosti
* glavni efekat na rundu ili prioritet
* trajanje ili okvir važenja

Preporučeni red čitanja je:

1. naziv i event tip
2. glavni kontekstualni pomak
3. koliko traje ili kada ističe

Event karta ne smije djelovati kao crisis karta ili kao treaty karta.

---

## 16. Wireframe za Crisis Cards / Karte kriza

Ove karte moraju naglasiti:

* da se radi o ozbiljnijem sistemskom testu
* šta tačno testira
* ko je najviše izložen
* kako se pritisak rješava ili trpi

Preporučeni red čitanja je:

1. naziv i crisis tip
2. šta je testirano / pogođeno
3. glavni pritisak ili posljedica
4. upravljanje ili contest logika

Kriza mora odmah djelovati “teže” od eventa, ali bez dužeg ili težeg layouta po svaku cijenu.

---

## 17. Wireframe za Coronation sadržaj

Ako se koristi posebna karta ili referentna komponenta za **Coronation Attempt/Pokušaj krunisanja**, ona mora naglasiti:

* da je ovo završni politički vrhunac
* uslov ili legalni ulaz
* contest prostor
* jasan ishod ili referencu na ishod

Preporučeni red čitanja je:

1. naziv / završni identitet
2. ulaz ili aktivacija
3. contest
4. ishod

Ova karta ne smije izgledati kao event niti kao obični scoring podsjetnik.

---

## 18. Veza sa terminology-and-labels standardom

Sve karte moraju koristiti terminologiju iz:

* `components/terminology-and-labels.md`

To znači:

* isti termini kao u pravilima i aids
* isti dvojezični redoslijed gdje je potreban
* bez improvizovanih skraćenica
* bez “grafički zgodnijih” paralelnih naziva

Ako wireframe traži da termin bude promijenjen, prvo se preispituje layout, ne termin.

---

## 19. Veza sa ikonografijom

Karte treba da koriste ikonografiju štedljivo i u službi čitanja.

To znači:

* ikona pojačava tip, resurs ili važan signal
* ne zatrpava tekst
* ne pravi lažni osjećaj da karta ima više sistema nego što stvarno ima

Ikona ne smije pojesti prostor glavnog efekta.

---

## 20. Veza sa information-hierarchy dokumentom

Wireframe mora slijediti logiku:

* naziv i tip = brzo prepoznavanje
* glavni efekat = primarna informacija
* uslov / trajanje / posljedica = sekundarna informacija
* ukrasni ton = tercijarni ili dekorativni sloj

Ako karta nema jasnu hijerarhiju informacija, izgleda “bogato”, ali radi sporo.

---

## 21. Veza sa onboardingom

Za **First Game Mode/Mod prve partije**, karte moraju ostati posebno čitljive.

To znači:

* manje tekstualnog zbijanja
* manje nepotrebnih blokova
* jasnije razlikovanje tipova
* dovoljno prostora da novi igrač ne osjeti da mora “dešifrovati” karticu

Ako je kartični UX loš, nova grupa će pomisliti da su pravila komplikovanija nego što jesu.

---

## 22. Fizička čitljivost karata

Wireframe mora biti testiran mentalno za stvarne uslove:

* mali format karte
* sto pod normalnim svjetlom
* brzi pogled iz ruke ili sa stola
* print prototip bez savršenih boja i oštrine

To znači da layout ne smije zavisiti od:

* sitnog teksta
* delikatnih finih linija
* previše tankih razmaka
* boje kao jedinog razlikovnog sredstva

---

## 23. Najčešće greške u wireframe dizajnu karata

* previše ukrasnog zaglavlja
* glavni efekat nije najveći ili najčitljiviji blok
* previše ikona u odnosu na tekst
* sekundarna pravila izgledaju važnije od glavnog efekta
* isti tip karte ima različit layout bez jakog razloga
* event, crisis i treaty karte djeluju previše slično na prvi pogled
* karta izgleda dobro na ekranu, ali loše u stvarnom printu

---

## 24. Workflow pravilo za novi kartični blok

Ako se predlaže novi blok na karti, mora se provjeriti redom:

1. da li igrač to mora vidjeti na prvi pogled ili tek kasnije
2. da li informacija već ima mjesto u postojećem wireframeu
3. da li blok ubrzava ili usporava čitanje
4. da li pripada karti ili aid-u
5. da li se isti problem može riješiti boljim wordingom umjesto novim blokom
6. da li blok povećava vizuelni šum

Ako ne prolazi ova pitanja, novi blok se ne uvodi.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li čitanje karte postaje brže ili sporije?
2. da li se tip karte lakše ili teže prepoznaje?
3. da li glavni efekat ostaje glavni fokus?
4. da li ikonografija i terminologija ostaju usklađene?
5. da li prototip i konačna štampa ostaju realni?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 26. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `ux/information-hierarchy.md`
* `ux/player-aid-system.md`
* `visuals/board-wireframe-notes.md`
* sve buduće kartične template fajlove

Ako wireframe karata nije dovoljno čist prije završnog grafičkog rada, gotovo sigurno dolazi do:

* previše revizija kartičnih layouta
* slabijeg onboarding efekta
* sporijeg gameplay čitanja
* većeg rizika da sadržaj i vizuelni stil počnu raditi jedan protiv drugog

---

## 27. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `ux/information-hierarchy.md`
* `content/treaties-list.md`
* `content/events-and-crises.md`
* `content/coronation-content.md`
* `ux/player-aid-system.md`
* `GLOSSARY.md`

---

## 28. Završna napomena

**Card Wireframe Notes / Bilješke za wireframe karata** moraju ostati jedan od glavnih funkcionalnih filtera prije završnog grafičkog dizajna.

Ako rade dobro:

* karte se brzo čitaju
* onboarding je lakši
* različiti tipovi karata se odmah prepoznaju
* grafički handoff je sigurniji
* a sadržaj i vizuelni sloj počinju raditi zajedno

Ako rade loše:

* karte izgledaju ljepše nego što rade
* gameplay se usporava
* lookup raste
* a svaki kasniji grafički krug postaje skuplji i sporiji

Zato ovaj dokument mora ostati strogo funkcionalan, čitljiv i potpuno usklađen sa jezgrom **v2.7**.
