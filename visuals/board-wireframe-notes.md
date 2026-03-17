# board-wireframe-notes.md

# Crown of Sovereigns v2.7 — Board Wireframe Notes / Bilješke za wireframe glavne table

## Status dokumenta

* **Dokument:** `visuals/board-wireframe-notes.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati funkcionalne i vizuelne principe za wireframe, raspored i ranu maketu glavne **Board/Table** komponente
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Board/Tabla**, **Provinces/Provincije**, **Event/Događaj**, **Treaty/Sporazum**
* **Povezani dokumenti:** `components/board-spec.md`, `components/terminology-and-labels.md`, `components/iconography-spec.md`, `ux/information-hierarchy.md`, `systems/province-map-system.md`, `systems/event-and-crisis-system.md`, `systems/coronation-system.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* pretvori funkcionalnu specifikaciju table u praktične wireframe smjernice
* odredi kako glavna tabla treba biti raspoređena prije finalnog grafičkog dizajna
* spriječi da ilustracija, heraldika i rubni sistemi pojedu mapu
* pomogne da layout ostane igriv u stvarnoj partiji, a ne samo u lijepom mockupu
* smanji broj skupih iteracija u kasnijoj grafičkoj fazi

Ovo nije finalni art direction dokument.
Ovo je funkcionalna osnova za raspored glavne table.

---

## 2. Zašto je wireframe glavne table kritičan

Glavna tabla je centralna površina cijele igre.
Ako wireframe table radi loše:

* mapa djeluje manja i slabija nego što sistem traži
* zajednički sistemi djeluju rasuti ili nevažni
* setup i tok runde postaju sporiji
* politički i završni signali se teže čitaju

Ako wireframe radi dobro:

* mapa je odmah dominantna
* zajedničke zone djeluju prirodno
* igrači znaju gdje da gledaju u kom trenutku
* budući grafički rad dobija čistu osnovu

---

## 3. Osnovni princip wireframea table

Glavno pravilo glasi:

> wireframe glavne table mora prije svega organizovati pažnju igrača kroz prostor, a ne kroz dekoraciju.

To znači:

* pogled mora prvo ići na mapu
* zatim na aktivni zajednički pritisak
* pa tek onda na političke i završne pomoćne zone
* rubne zone ne smiju voditi vizuelnu kompoziciju više nego jezgro mape

Ako wireframe odmah vuče oko na rubne module umjesto na teritoriju, hijerarhija je pogrešna.

---

## 4. Šta wireframe glavne table jeste

Wireframe glavne table treba da bude:

* kostur rasporeda
* test prioriteta prostora
* alat za provjeru čitljivosti prije vizuelnog stila
* sredstvo da se vidi kako fizičke komponente zaista sjede na tabli

---

## 5. Šta wireframe glavne table nije

Wireframe glavne table nije:

* polu-gotova ilustracija
* mjesto za rano ubacivanje svih dekorativnih ideja
* precizan finalni art layout
* opravdanje da se ignorše gameplay ergonomija dok se “kasnije ne ispegla”

Ako wireframe prerano postane estetski artefakt, izgubiće funkcionalnu vrijednost.

---

## 6. Glavne funkcije dobrog board wireframea

Dobar wireframe glavne table mora raditi najmanje 6 stvari:

1. dati mapi najveći i najjasniji prostor
2. rasporediti zajedničke sisteme tako da ne guše mapu
3. podržati prirodan tok pogleda tokom runde
4. ostati čitljiv kada su komponente zaista postavljene
5. omogućiti dovoljno prostora za markere i stanje partije
6. ostati kompatibilan sa terminologijom, ikonografijom i aid logikom

Ako radi samo prve tri stvari, može izgledati uredno, ali pasti kad uđe pravi gameplay load.

---

## 7. Osnovne zone wireframea

Wireframe glavne table mora testirati najmanje sljedeće glavne zone:

### 7.1. Map Core / Jezgro mape

Centralna i najveća zona, sa **24 Provinces/24 Provincije**.

### 7.2. Event and Crisis Margin / Rub događaja i kriza

Vidljiv, ali ne dominantan prostor za aktivni zajednički pritisak.

### 7.3. Political/Treaty Margin / Politički i treaty rub

Kontrolisan prostor za javni politički kontekst.

### 7.4. Endgame/Coronation Margin / Rub završnice i krunisanja

Diskretniji prostor koji raste u važnosti kako partija ulazi u završni pritisak.

### 7.5. Optional Setup/Reference Edge / Opcioni setup i referentni rub

Vrlo mali pomoćni prostor ako playtest pokaže da je potreban za setup ili zajedničku orijentaciju.

Kritično pravilo:

> nijedan rubni modul ne smije biti veći ili glasniji od prostorne logike mape.

---

## 8. Map Core / Jezgro mape

Ovo je srce wireframea.

### 8.1. Proporcija

Mapa mora uzeti najveći procenat ukupne površine table.

### 8.2. Praktični cilj

Kad igrač pogleda tablu, prvo mora čitati:

* granice
* susjedstva
* stanje kontrole
* zone konflikta i pritiska

### 8.3. Šta wireframe mora testirati

* veličinu pojedinačnih **Provinces/Provincije**
* prostor za jedinice i markere
* prostor za contest stanje
* čitljivost granica i susjedstava
* odnos prazne i ispunjene table

Ako province izgledaju dobro prazne, a loše pune, wireframe nije uspješan.

---

## 9. Province shape / Oblik provincija

Wireframe ne treba finalizovati stil granica, ali mora postaviti jasna pravila:

* provincije moraju biti dovoljno različite da se lako prate
* ali ne toliko nepravilne da postanu teške za marker placement
* granice moraju ostati dovoljno čiste za brzu prostornu orijentaciju

Previše dekorativno lomljene granice često izgledaju dobro u artu, ali rade loše u partiji.

---

## 10. Marker load test / Test opterećenja markerima

Wireframe glavne table mora se zamišljati u tri stanja:

### 10.1. Prazna tabla

Koristi se samo da se vidi osnovna kompozicija.

### 10.2. Srednje opterećena tabla

Tipično stanje sredine partije sa jedinicama, kontrolama i nekoliko aktivnih rubnih markera.

### 10.3. Teško opterećena tabla

Kasna partija sa contest stanjima, završnim pritiskom i punim političkim signalima.

Ako wireframe funkcioniše samo u praznom stanju, nije dovoljno dobar.

---

## 11. Event and Crisis Margin / Rub događaja i kriza

Ovaj rub mora biti lako vidljiv, ali i dalje podređen mapi.

### 11.1. Šta wireframe treba pokazati

* gdje se nalazi aktivni **Event/Događaj**
* gdje se nalazi aktivna **Crisis/Kriza**
* kako se taj sadržaj vidi svim igračima bez gutanja centra table

### 11.2. Layout pravilo

Event i crisis prostor treba biti:

* dovoljno velik za čitljiv prikaz
* dovoljno mali da ne postane glavna vizuelna tačka
* pozicioniran tako da prirodno ulazi u pogled na početku runde

### 11.3. Šta izbjeći

* velike vertikalne tekstualne kolone
* rub koji djeluje kao drugi odvojeni board
* event/crisis blok koji izgleda važnije od same teritorije

---

## 12. Political/Treaty Margin / Politički i treaty rub

Ovaj prostor mora biti strogo kontrolisan.

### 12.1. Funkcija

Treba da omogući javan pregled političkog stanja i aktivnih **Treaty/Sporazum** odnosa kada je to UX opravdano.

### 12.2. Wireframe cilj

Treba testirati:

* koliko političkih slotova ili referentnih mjesta zaista treba
* da li taj pregled pomaže ili usporava
* koliko prostora mu je stvarno potrebno da ostane čitljiv

### 12.3. Šta izbjeći

* previše slots / previše formalne matrice
* mikrotekst koji traži da igrač ustane ili se nagne da bi pročitao
* politički rub koji djeluje kao spreadsheet odnosâ

Politički kontekst mora biti čitljiv, ali ne smije pojesti društvenu dinamiku stola.

---

## 13. Endgame/Coronation Margin / Rub završnice i krunisanja

Ovaj prostor mora biti diskretan u ranoj partiji, ali spreman da postane važan u kasnijoj.

### 13.1. Wireframe cilj

Treba testirati:

* gdje završni signal može stajati a da ne smeta ranoj partiji
* kako **Coronation Attempt/Pokušaj krunisanja** javni kontekst ulazi u pažnju stola
* kako završni rub ostaje prisutan, ali ne teatralan prije vremena

### 13.2. Šta izbjeći

* veliki stalni coronation panel koji dominira tablom od prvog kruga
* završni modul koji izgleda kao zasebna mini-igra
* višak završnih labela i okvira koji guše centralni prostor

---

## 14. Shared margins as one system / Rubovi kao jedan sistem

Iako postoje različite rubne zone, wireframe ih mora tretirati kao jedan usklađen sistem.

To znači:

* rubovi moraju imati isti osnovni vizuelni jezik
* ne smiju izgledati kao tri različite igre zalijepljene oko mape
* razlike u važnosti treba graditi kroz hijerarhiju, ne kroz haotičnu raznolikost stilova

---

## 15. Veza sa turn flow / tokom runde

Wireframe glavne table mora podržavati prirodan tok pogleda tokom runde.

Preporučeni tok pažnje je:

1. aktivni **Event/Događaj** ili **Crisis/Kriza**
2. politički kontekst ako je relevantan
3. povratak pogleda na mapu i akcije
4. završni ili coronation signal samo kada partija uđe u taj režim

Ako pogled skače haotično između udaljenih ili jednako glasnih zona, wireframe treba prepraviti.

---

## 16. Veza sa information hierarchy dokumentom

Wireframe mora striktno pratiti:

* mapa = **Primary Information/Primarna informacija**
* zajednički aktivni pritisak = **Secondary Information/Sekundarna informacija** visoke važnosti
* politički i završni signali = sekundarna ili tercijarna informacija zavisno od trenutka partije
* dekorativni sloj = uvijek podređen

Ako wireframe ne poštuje ovu hijerarhiju, finalni vizuelni rad će gotovo sigurno otići u pogrešnom pravcu.

---

## 17. Veza sa terminology-and-labels standardom

Wireframe table mora ostaviti realan prostor za:

* pune ili kontrolisano skraćene dvojezične labele
* čitljive nazive najvažnijih zajedničkih zona
* dosljednu primjenu `/` separatora

Wireframe koji traži da se termini nasilno skraćuju samo zato što nema prostora, vjerovatno ima lošu raspodjelu prostora.

---

## 18. Veza sa iconography standardom

Wireframe mora predvidjeti gdje ikonografija stvarno pomaže, a gdje samo guši.

To znači:

* najvažnije sistemske ikone mogu imati rezervisana mjesta
* province ne smiju biti zatrpane sitnim simbolima
* rubni sistemi smiju koristiti ikone, ali uz dovoljno praznog prostora i jasan label

Ikonografija mora biti planirana kao podrška, ne kao popunjavanje praznina.

---

## 19. Veza sa player board odnosom

Glavna tabla ne smije preuzimati ono što je već bolje riješeno na **Player Board/Tabli igrača**.

Wireframe mora zato jasno izbjegavati:

* lične goods mikro-trakove na glavnoj tabli
* lične stabilnost detalje na glavnoj tabli
* dvorski pregled koji je već primarno stvar table igrača

Glavna tabla treba ostati zajednički prostor, ne kolekcija četiri male lične table.

---

## 20. Pristupačnost i fizička upotrebljivost

Wireframe glavne table mora biti zamišljen za stvarne uslove:

* igrači sjede sa više strana stola
* svjetlo nije savršeno
* print nije savršeno oštar
* komponente djelimično prekrivaju dijelove table

To znači:

* veće zone moraju biti jasnije od manjih
* glavni nazivi ne smiju biti sitni
* kontrast između funkcionalnih cjelina mora biti predviđen već u wireframeu

---

## 21. Onboarding uloga wireframea table

Nova grupa treba da može iz prvog pogleda shvatiti:

* gdje je jezgro igre
* gdje se gledaju zajednički pritisci
* gdje se pojavljuju politički i završni signali

Ako rani mockup to ne uspijeva bez dodatnog objašnjavanja, wireframe treba reorganizovati prije nego što se potroši vrijeme na ilustraciju.

---

## 22. Najčešće greške u wireframeu glavne table

* rubne zone su prevelike
* mapa je formalno centralna, ali vizuelno nije dominantna
* province nemaju dovoljno prostora za gameplay opterećenje
* event/crisis prostor djeluje kao drugi board
* politički prostor je ili previše skriven ili previše agresivan
* završni modul je previše prisutan od početka partije
* dekorativni okviri jedu funkcionalni prostor

---

## 23. Workflow pravilo za novu zonu ili promjenu na tabli

Ako se predlaže nova zona ili veća izmjena, mora se provjeriti redom:

1. da li to zaista pripada zajedničkoj tabli
2. da li smanjuje prostor mape
3. da li pomaže brzini partije ili samo dodaje još informacija
4. da li tu funkciju bolje rješava aid ili posebna komponenta
5. da li ostaje čitljivo u opterećenom stanju
6. da li hijerarhija pažnje ostaje ista ili se ruši

Ako ne prolazi ova pitanja, izmjena se ne uvodi.

---

## 24. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li mapa ostaje dominantna?
2. da li rubni moduli ostaju korisni, ali kontrolisani?
3. da li wireframe ostaje kompatibilan sa terminologijom i ikonografijom?
4. da li partija ostaje čitljiva pod stvarnim komponentnim opterećenjem?
5. da li grafički handoff postaje lakši ili teži?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 25. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `ux/information-hierarchy.md`
* `visuals/card-wireframe-notes.md`
* buduće board layout i print template fajlove

Ako wireframe glavne table nije dovoljno čist prije završnog vizuelnog rada, gotovo sigurno dolazi do:

* više layout iteracija
* slabije mapne čitljivosti
* sporijeg onboarding rezultata
* skupljih print test korekcija

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/board-spec.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `ux/information-hierarchy.md`
* `systems/province-map-system.md`
* `systems/event-and-crisis-system.md`
* `systems/coronation-system.md`
* `GLOSSARY.md`

---

## 27. Završna napomena

**Board Wireframe Notes / Bilješke za wireframe glavne table** moraju ostati jedan od glavnih funkcionalnih filtera prije finalnog grafičkog dizajna table.

Ako rade dobro:

* mapa ostaje srce igre
* zajednički sistemi se čitaju prirodno
* onboarding je lakši
* politički i završni pritisak dobijaju pravi prostor
* a grafički handoff postaje mnogo sigurniji

Ako rade loše:

* tabla djeluje veća, glasnija i složenija nego što treba
* mapa gubi identitet
* zajednički sistemi se čitaju sporije
* a svaka kasnija vizuelna iteracija postaje skuplja

Zato ovaj dokument mora ostati strogo funkcionalan, hijerarhijski čist i potpuno usklađen sa jezgrom **v2.7**.
