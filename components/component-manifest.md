# component-manifest.md

# Crown of Sovereigns v2.7 — Component Manifest / Manifest komponenti

## Status dokumenta

* **Dokument:** `components/component-manifest.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati centralni pregled svih fizičkih i pomoćnih komponenti igre, njihovih klasa, funkcionalne uloge i odnosa prema ostatku repozitorijuma
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Component/Komponenta**, **Board/Tabla**, **Card/Karta**, **Token/Token**
* **Povezani dokumenti:** `components/board-spec.md`, `components/player-board-spec.md`, `components/cards-spec.md`, `components/tokens-spec.md`, `components/units-and-markers-spec.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `components/box-and-insert-notes.md`, `rules/setup-guide.md`, `ux/player-aid-system.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* bude glavni inventarski pregled fizičkog sistema igre
* objedini sve ključne komponente na jednom mjestu bez ulaženja u dubinu svake pojedinačne specifikacije
* omogući da se brzo vidi koje klase komponenti postoje i zašto postoje
* spriječi da se nove komponente uvode bez jasnog mjesta u ukupnoj arhitekturi proizvoda
* pripremi osnov za setup, packaging, vizuelni handoff i produkcijsku procjenu

Ovo nije detaljna tehnička specifikacija svake komponente.
Ovo je krovni manifest koji govori šta postoji, kojoj klasi pripada i koju funkciju nosi.

---

## 2. Zašto je component manifest kritičan

Kod kompleksnijih igara vrlo brzo nastaje problem ako nema jednog centralnog manifesta:

* komponente postoje u više dokumenta, ali bez jedinstvenog pregleda
* novi token, marker ili kartična klasa lako se doda bez pune procjene ukupnog tereta
* packaging i setup logika počinju pratiti različite slike stvarnog sadržaja igre
* vizuelni i produkcijski rad nemaju jedan čist pregled šta sve ulazi u proizvod

Dobar **Component Manifest/Manifest komponenti** ne zamjenjuje ostale dokumente, ali ih povezuje u jednu fizičku sliku igre.

---

## 3. Osnovni princip manifesta

Glavno pravilo glasi:

> manifest mora prikazati kompletan komponentni sistem dovoljno jasno da novi saradnik može razumjeti šta igra fizički jeste, ali ne smije ponavljati dubinske tehničke detalje koji već žive u specifičnim komponentnim dokumentima.

To znači:

* manifest daje pregled
* spec dokumenti daju detalje
* manifest ne smije postati drugi skup istih sadržaja u paraleli

Ako počne da duplira dubinske specifikacije, ubrzo postaje teži za održavanje i manje pouzdan.

---

## 4. Šta component manifest jeste

Ovaj dokument treba da bude:

* krovni pregled svih klasa komponenti
* zajednički inventarski okvir
* most između systems logike i fizičkog proizvoda
* kontrolna tačka prije setup, packaging i graphic handoff rada

---

## 5. Šta component manifest nije

Ovaj dokument nije:

* detaljna lista art asseta
* precizan produkcijski BOM
* finalni manufacturing sheet
* zamjena za pojedinačne specs dokumente

On treba da bude dovoljno jasan za odlučivanje, ali ne toliko dubok da duplira cijeli komponentni sloj.

---

## 6. Glavne komponente proizvoda

CoS v2.7 proizvod, na najvišem nivou, čine sljedeće glavne cjeline:

1. **Board Layer/Sloj table**
2. **Player Layer/Sloj igrača**
3. **Card Layer/Sloj karata**
4. **Token Layer/Sloj tokena**
5. **Units and Markers Layer/Sloj jedinica i markera**
6. **Reference and Aid Layer/Sloj referenci i aid materijala**
7. **Packaging Layer/Sloj pakovanja**

Ove cjeline moraju ostati dovoljno odvojene da fizički sistem bude razumljiv i logistički disciplinovan.

---

## 7. Board Layer / Sloj table

### 7.1. Glavna Board/Tabla

Glavna **Board/Tabla** je centralni zajednički prostor igre.

Njena funkcija je da nosi:

* mapu i **Provinces/Provincije**
* zajedničke zone runde i završnice
* contested i kontrolne prostore gdje je relevantno
* zajednički politički i završni fokus

### 7.2. Dodatne board-adjacent reference zone

Ako postoje rubne ili pomoćne zajedničke zone, one pripadaju ovom sloju samo ako su sastavni dio glavnog board iskustva, a ne zasebni aid materijal.

### 7.3. Ključni guardrail

Tabla ne smije biti pretrpana informacijom koju bi bolje nosili kartice, aid ili table igrača.

---

## 8. Player Layer / Sloj igrača

### 8.1. Player Boards / Table igrača

Svaki igrač ima svoju **Player Board/Tablu igrača**.

Njena funkcija je da nosi:

* lično stanje kraljevstva
* **Court/Dvor** fokus i povezane prostore
* **Stability/Stabilnost** i **Unrest/Nemiri** signal gdje je relevantno
* goods, razvoj i druge lične track-ove ili zone

### 8.2. Individual player areas / Lični prostor igrača

Pored same table igrača, svaki igrač treba jasan fizički prostor za lične karte, markere, jedinice i druge komponente povezane s njegovom državom.

### 8.3. Ključni guardrail

Player layer ne smije postati mini-spreadsheet koji gubi vezu sa glavnom tablom i zajedničkim stanjem partije.

---

## 9. Card Layer / Sloj karata

CoS v2.7 koristi kartični sistem kao disciplinovan sadržajni i proceduralni alat, ne kao bloat platformu.

Glavne kartične klase su:

* **Treaty Cards/Karte sporazuma**
* **Event Cards/Karte događaja**
* **Crisis Cards/Karte kriza**
* **Coronation Reference Cards/Referentne karte krunisanja**, gdje su opravdane

### Ključna funkcija kartičnog sloja

* formalizacija političkih odnosa
* zajednički ritamski pritisak
* završna referenca gdje je kartični format najjasniji

### Ključni guardrail

Ne uvoditi nove kartične klase bez jasnog razloga, jer kartični sistem vrlo brzo povećava onboarding i produkcijski teret.

---

## 10. Token Layer / Sloj tokena

**Tokens/Tokeni** služe da označe važna, česta i jasno izdvojena stanja ili vrijednosti koje imaju smisla kao zaseban fizički signal.

Glavne token kategorije uključuju:

* mapne tokene
* tokene ličnog stanja
* diplomatske tokene gdje su opravdani
* završne tokene gdje završni signal traži poseban marker

### Ključna funkcija token sloja

* čitljivost zajedničkog i ličnog stanja
* podrška stabilnosti, contested statusu, treaty i završnim signalima

### Ključni guardrail

Tokeni ne smiju preuzeti ulogu i jedinica i markera i track markera istovremeno.

---

## 11. Units and Markers Layer / Sloj jedinica i markera

Ovaj sloj nosi razliku između:

* prostorne prisutnosti
* kontrole
* statusa
* pozicijskog praćenja

Glavne klase uključuju:

* **Units/Jedinice**
* **Control Markers/Markeri kontrole**
* **Contested Markers/Markeri osporavanja**
* **Progress Markers/Markeri napretka**
* **Stability Markers/Markeri stabilnosti**
* **Unrest Markers/Markeri nemira**
* završne i treaty pomoćne markere gdje su opravdani

### Ključna funkcija ovog sloja

* učiniti da mapa i lični status budu čitljivi bez miješanja fizičke prisutnosti i apstraktnih stanja

### Ključni guardrail

Svaki novi marker mora opravdati zašto nije token, zašto nije track i zašto nije suvišan.

---

## 12. Reference and Aid Layer / Sloj referenci i aid materijala

Ovaj sloj je ključan za onboarding i kontrolu proceduralne magle.

U njega spadaju:

* **Player Aid/Pomoćni igrački vodič**
* quick reference elementi gdje su potrebni
* **Quickstart/Brzi vodič** podrška za prvu partiju
* rules reference dokumentacija u fizičkom ili štampanom obliku, ako se koristi u prototipu

### Ključna funkcija

* smanjenje lookup tereta
* podrška setupu, toku runde i završnom obračunu

### Ključni guardrail

Aid sloj ne smije biti zakrpa za loš sistem; mora biti podrška dobrom sistemu.

---

## 13. Packaging Layer / Sloj pakovanja

Packaging sloj obuhvata:

* **Box/Kutiju**
* **Insert/Insert** logiku
* raspored komponenti radi zaštite, setupa i teardowna

### Ključna funkcija

* zaštita komponenti
* logična grupacija sadržaja
* ubrzavanje setup i teardown toka

### Ključni guardrail

Pakovanje ne smije biti luksuzni višak koji usporava stvarnu upotrebu ili povećava proizvodni rizik bez jasnog povrata.

---

## 14. Glavni pregled komponentnih klasa

Na jednom mjestu, CoS v2.7 komponentni sistem čine najmanje:

* 1 glavna **Board/Tabla**
* više **Player Boards/Tabli igrača**
* više kartičnih klasa sa jasnim funkcijama
* više token klasa sa strogo opravdanim signalima
* jedinice i markeri koji razlikuju prisutnost, kontrolu i status
* aid i onboarding materijali
* packaging sistem koji podržava logistiku proizvoda

Ovaj pregled namjerno ostaje na nivou klasa, ne numeričkog counta, dok se count ne zaključa dovoljno sigurno kroz produkcijski sloj.

---

## 15. Odnos manifesta prema spec dokumentima

Manifest i spec dokumenti rade različite poslove:

* **Component Manifest/Manifest komponenti** odgovara na pitanje:
  **šta fizički postoji i čemu služi?**

* pojedinačni spec dokumenti odgovaraju na pitanje:
  **kako ta komponenta tačno izgleda, radi i gdje pripada?**

To znači da manifest mora stalno ostati kraći i širi od pojedinačnih spec dokumenata.

---

## 16. Odnos manifesta prema setupu

Manifest mora biti usklađen sa:

* `rules/setup-guide.md`

Zašto?
Zato što setup koristi komponentne grupe kako bi partiju postavio logično.
Ako setup i manifest ne govore istim jezikom, logistički sloj igre postaje nečist.

---

## 17. Odnos manifesta prema packagingu

Manifest mora biti usklađen sa:

* `components/box-and-insert-notes.md`

Zašto?
Zato što packaging organizacija ima smisla samo ako prati stvarne komponente i njihove funkcionalne grupe.

---

## 18. Odnos manifesta prema GDD-u

Manifest mora biti usklađen sa:

* `gdd/crown-of-sovereigns-v2.7-gdd.md`

Zašto?
Zato što fizički proizvod mora pratiti identitet igre.
Ako komponentni sistem ne podržava državni, politički i završni identitet CoS-a, GDD i proizvod govore različitim jezikom.

---

## 19. Komponentni guardrail-i

Pri svakoj novoj komponenti treba provjeriti najmanje:

* da li ta komponenta nosi stvarnu funkciju
* da li se njena funkcija ne duplira postojećim elementom
* da li povećava ili smanjuje čitljivost
* da li povećava onboarding i produkcijski teret
* da li ima jasno mjesto u manifestu

Ako nova komponenta ne prolazi ovaj filter, ne treba je dodavati.

---

## 20. Najčešće greške koje manifest pomaže spriječiti

* dodavanje novih komponenti bez pregleda ukupnog sistema
* miješanje tokena, markera i jedinica
* previše kartičnih klasa bez potrebe
* pomoćni materijali koji dupliraju osnovni layout umjesto da ga podrže
* packaging koji prati zamišljene, a ne stvarne komponente

---

## 21. Workflow pravilo za novu komponentu

Kad se predlaže nova komponenta, treba provjeriti redom:

1. kojoj klasi pripada
2. koju funkciju nosi
3. da li tu funkciju već nosi nešto drugo
4. gdje fizički živi
5. da li je povezana sa setup, aid i packaging logikom
6. da li treba novu spec dokumentaciju ili samo ažuriranje postojeće

Ako ne prolazi ova pitanja, komponenta još nije spremna za uvođenje.

---

## 22. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li manifest ostaje pregledan?
2. da li ostaje krovni dokument, a ne duplikat detaljnih specova?
3. da li bolje povezuje fizički sistem igre?
4. da li smanjuje ili povećava komponentni bloat?
5. da li ostaje usklađen sa GDD, setup i packaging logikom?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 23. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/cards-spec.md`
* `components/tokens-spec.md`
* `components/units-and-markers-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `components/box-and-insert-notes.md`
* `rules/setup-guide.md`
* `ux/player-aid-system.md`
* `GLOSSARY.md`

---

## 24. Završna napomena

**Component Manifest / Manifest komponenti** mora ostati glavni inventarski i kontrolni dokument fizičkog sistema igre u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* komponente su lakše razumljive kao sistem
* setup, packaging i graphic handoff imaju jači zajednički temelj
* novi dokumenti i nove komponente lakše nalaze svoje mjesto
* a produkcijski razgovori postaju mnogo čistiji

Ako radi loše:

* komponentni sloj se širi bez kontrole
* spec dokumenti počinju živjeti kao odvojeni svjetovi
* setup i packaging logika se razilaze
* a fizički proizvod djeluje manje koherentan nego što dizajn zaslužuje

Zato ovaj dokument mora ostati jasan, pregledan i potpuno usklađen sa logikom **v2.7**.
