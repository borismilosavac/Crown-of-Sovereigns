# terminology-and-labels.md

# Crown of Sovereigns v2.7 — Terminology and Labels / Terminologija i oznake

## Status dokumenta

* **Dokument:** `components/terminology-and-labels.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati standard za sve nazive, oznake, kratke tekstove i terminološke forme koje će se pojavljivati na komponentama, tabli, aid materijalima i grafičkim fajlovima
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Cleric/Klerik**
* **Povezani dokumenti:** `GLOSSARY.md`, `docs/version-status.md`, `rules/rules-reference-v2.7.md`, `content/court-roles.md`, `content/treaties-list.md`, `content/goods-list.md`, `components/iconography-spec.md`, `ux/player-aid-system.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* zaključa kako se termini pišu na fizičkim i grafičkim komponentama
* spriječi da isti pojam dobije više različitih naziva kroz kartice, tablu, aid i UI elemente
* uskladi kratke label formate sa punim dokumentacionim terminima
* pomogne da grafički handoff ne uvede terminološki haos
* poveže sadržajni i vizuelni sloj sa kanonskom bazom **v2.7**

Ovo nije opšti pojmovnik. To je već definisano u `GLOSSARY.md`.
Ovo je operativni komponentni standard za to kako se termini stvarno prikazuju na komponentama.

---

## 2. Zašto je ovaj dokument kritičan

Najbrži način da igra djeluje nedovršeno jeste da:

* na tabli piše jedno
* na aid-u drugo
* u pravilima treće
* a na kartama četvrto

To pravi četiri vrste problema:

* onboarding konfuziju
* sporiji gameplay
* skuplji grafički handoff
* lošiji playtest feedback jer ljudi ne koriste isti jezik

Zato ovaj dokument nije kozmetika.
On je most između dokumentacije i stvarnih komponenti.

---

## 3. Hijerarhija izvora istine za terminologiju

Ako postoji konflikt u terminologiji, koristi se ovaj redoslijed prioriteta:

1. `GLOSSARY.md`
2. `components/terminology-and-labels.md`
3. glavni systems ili rules dokument za temu
4. player aid i grafički draftovi

To znači:

* dizajn ne smije samostalno izmišljati kraće nazive ako nisu usklađeni sa ovim dokumentom
* content dokumenti ne smiju krišom uvoditi novi label format bez provjere ovdje

---

## 4. Osnovno pravilo pisanja termina

Za sve ključne termine u GitHub dokumentima i master specifikacijama koristi se format:

* **English/Srpski**

Primjeri:

* **Court/Dvor**
* **Goods/Roba**
* **Marshal/Maršal**
* **Diplomat/Diplomata**
* **Cleric/Klerik**
* **Spy/Špijun**
* **Treaty/Sporazum**
* **Stability/Stabilnost**
* **Unrest/Nemiri**
* **Coronation Attempt/Pokušaj krunisanja**

Ovo je osnovni dokumentacioni standard.

---

## 5. Pravilo za komponente

Na samim fizičkim komponentama nije uvijek moguće koristiti puni dvojezični zapis u svakom kontekstu.

Zato se terminološki prikaz dijeli na 3 nivoa:

### 5.1. Full Label / Puna oznaka

Koristi se kada ima dovoljno prostora i kada je termin važan za jasnoću.
Primjer:

* **Goods/Roba**
* **Stability/Stabilnost**
* **Trade Pact/Trgovački pakt**

### 5.2. Compact Label / Skraćena oznaka

Koristi se kada prostor nije dovoljan za pun zapis, ali treba zadržati jasnoću.
Primjer:

* **Marshal/Maršal** može ostati pun, ali na malim referentnim mjestima može biti samo **Marshal** ili samo **Maršal** ako je kontekst već zaključen u layout sistemu

### 5.3. Icon + Aid Reference / Ikona + aid referenca

Koristi se samo kada je termin već naučen, a prostor veoma ograničen.
Ovo nikad ne smije biti prvi ili jedini susret igrača sa terminom.

---

## 6. Opšte pravilo za izbor između punog i skraćenog labela

Ako termin:

* prvi put susrećeš na komponenti
* nosi važnu sistemsku razliku
* lako se može zamijeniti sa drugim pojmom

onda koristi **Full Label / Punu oznaku**.

Ako termin:

* već postoji na istoj komponenti ili u istom bloku više puta
* prostor je ograničen
* vizuelna hijerarhija je već jasna

onda je dozvoljena **Compact Label / Skraćena oznaka**.

Ako je termin prikazan samo ikonom, aid ili referenca moraju odmah pomoći da igrač zna šta gleda.

---

## 7. Zaključani glavni termini za komponente

Ovo su glavni termini koji moraju ostati dosljedni na svim komponentama.

### 7.1. Jezgro igre

* **Court/Dvor**
* **Provinces/Provincije**
* **Goods/Roba**
* **Stability/Stabilnost**
* **Unrest/Nemiri**
* **Influence/Uticaj**
* **Legitimacy/Legitimnost**
* **Coronation Attempt/Pokušaj krunisanja**

### 7.2. Court Roles / Dvorske uloge

* **Marshal/Maršal**
* **Diplomat/Diplomata**
* **Merchant/Trgovac**
* **Cleric/Klerik**
* **Spy/Špijun**

### 7.3. Diplomacy / Diplomatija

* **Treaty/Sporazum**
* **Alliance/Savez**
* **Truce/Primirje**
* **Trade Pact/Trgovački pakt**
* **Betrayal/Izdaja**
* **Contest/Osporavanje**

### 7.4. Combat / Borba

* **Combat/Borba**
* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

### 7.5. Ekonomija i razvoj

* **Gold/Zlato**
* **Food/Hrana**
* **Faith/Vjera**
* **Influence/Uticaj**
* **Income/Prihod**
* **Development/Razvoj**

---

## 8. Zabranjeni paralelni nazivi

Sljedeće stvari nisu dozvoljene ako se misli na iste pojmove:

* koristiti **Resources/Resursi** kada se misli na **Goods/Roba**
* koristiti “Council” ili “Vijeće” kad se misli na **Court/Dvor**
* koristiti “Chaos” ili druge slobodne riječi kad se misli na **Unrest/Nemiri**
* koristiti proizvoljne prevode za **Court Roles/Dvorske uloge** od komponente do komponente
* koristiti “Coronation” bez provjere da li treba puni oblik **Coronation Attempt/Pokušaj krunisanja**

Ako se koristi drugi naziv, mora biti eksplicitno odobren kroz novu verzionu odluku ili dodat u `GLOSSARY.md`.

---

## 9. Standard za naslove na kartama

Naslovi na kartama i većim komponentama treba da koriste:

* puni naziv kada je to moguće
* jasan i vizuelno čist raspored
* isti terminološki oblik kao i u dokumentaciji

### Primjeri

* **Alliance/Savez**
* **Trade Pact/Trgovački pakt**
* **Coronation Attempt/Pokušaj krunisanja**

Ako je naslov predug za layout, prvo treba riješiti layout, a ne proizvoljno mijenjati termin.

---

## 10. Standard za manje labele na tabli

Na tabli i manjim referentnim poljima prioritet je čitljivost na udaljenosti.

To znači:

* važni sistemski nazivi ostaju puni kad god je moguće
* pomoćni mikro-teksti se skraćuju samo kad je kontekst jasan
* terminološka skraćenja moraju biti unaprijed odobrena, ne improvizovana

Na primjer:

* **Stability/Stabilnost** na player board-u može ostati puna oznaka
* na ultra malom podsjetniku može stajati samo **Stability** ili samo **Stabilnost** ako je isti format svuda dosljedan

---

## 11. Standard za Player Aid / Pomoćni igrački vodič

Na aid materijalu prioritet je maksimalna jasnoća.

To znači da aid po pravilu treba češće koristiti:

* **Full Label / Punu oznaku**
* ili vrlo kontrolisanu **Compact Label / Skraćenu oznaku**

Aid nije mjesto za eksperimentisanje sa neobičnim skraćenicama.

---

## 12. Standard za ikone i tekst zajedno

Kada se koristi ikona uz tekst:

* tekst mora potvrditi značenje ikone barem na važnim ili prvim susretima
* ista ikona ne smije pratiti više sličnih, ali različitih termina bez dodatnog razdvajanja
* ikona nikad ne smije postati zamjena za termin ako termin još nije naučen

Drugim riječima:

> ikona pomaže terminologiji; ikona je ne zamjenjuje prerano.

---

## 13. Standard za dvojezični redoslijed

Uvijek se koristi isti redoslijed:

* prvo **English**
* zatim **Srpski**

Primjeri:

* **Goods/Roba**
* **Court/Dvor**
* **Treaty/Sporazum**

Ne mijenjati redoslijed od slučaja do slučaja.
To bi stvorilo vizuelni i terminološki šum.

---

## 14. Standard za separator

Separator između dva termina uvijek je kosa crta:

* `/`

Dakle:

* **Court/Dvor**
* ne “Court - Dvor”
* ne “Court (Dvor)”
* ne “Court | Dvor”

To je zaključani vizuelni standard za projekat.

---

## 15. Standard za velika i mala slova

Nazivi ključnih sistema, uloga i formalnih klasa pišu se dosljedno velikim početnim slovom kada su naslov ili label.

Primjeri:

* **Court/Dvor**
* **Goods/Roba**
* **Stability/Stabilnost**
* **Trade Pact/Trgovački pakt**

U opisnom tekstu može se po potrebi koristiti gramatički prirodniji oblik, ali na komponentama label forma treba ostati dosljedna.

---

## 16. Standard za množinu i jedninu

Na komponentama treba preferirati oblik koji je najjasniji za funkciju elementa.

### Primjeri

* sistemski naslov: **Goods/Roba**
* teritorijalni naslov: **Provinces/Provincije**
* pojedinačni element: **Province/Provincija**
* pojedinačni politički odnos: **Treaty/Sporazum**

Ne smije se nasumično miješati singular i plural na komponentama bez jasnog razloga.

---

## 17. Standard za action wording na komponentama

Kada komponenta koristi kratke proceduralne riječi, koriste se već zaključani termini.

### Primjeri

* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

Ne koristiti alternativne proceduralne glagole ako se misli na iste korake.

---

## 18. Standard za statusne oznake

Statusne oznake na komponentama moraju biti kratke, ali ne smiju uvoditi novi jezik.

Primjeri statusa koji se mogu pojaviti u sistemskim komponentama:

* **Active/Aktivno**
* **Broken/Prekinuto** ako bude relevantno za treaty stanje
* **Contested/Osporeno** ako se koristi kao formalni mapni ili završni status

Svaki novi status prije upotrebe mora biti usklađen sa:

* `GLOSSARY.md`
* ovim dokumentom
* relevantnim systems dokumentom

---

## 19. Standard za numeričke i tekstualne kombinacije

Kada label sadrži broj i termin, termin mora ostati pun ili jasno skraćen u istom standardu.

Primjeri:

* **2 Influence/2 Uticaj**
* **1 Goods/1 Roba** samo ako je u tom layoutu to smisleno
* **+1 Stability/+1 Stabilnost** ako postoji dovoljno prostora

Ako prostora nema, koristi ikonu + aid referencu, ali ne izmišljati novi termin.

---

## 20. Najčešće terminološke greške koje treba spriječiti

* isti termin napisan na tri različita načina kroz tri komponente
* skraćenice koje nisu dokumentovane
* “prevođenje u hodu” tokom grafičkog rada
* miješanje **Goods/Roba** i resursa
* miješanje **Treaty/Sporazum** klasa
* korištenje novih naziva za postojeće dvorske uloge
* neujednačeno pisanje **Coronation Attempt/Pokušaj krunisanja**

---

## 21. Workflow pravilo za nove labele

Ako se uvodi nova label forma, mora se provjeriti redom:

1. da li termin već postoji u `GLOSSARY.md`
2. da li je komponentni prikaz već definisan ovdje
3. da li nova forma ruši dosljednost drugih komponenti
4. da li je potrebna nova skraćena forma ili se može koristiti postojeća
5. da li grafički problem treba rješavati layoutom, a ne promjenom termina

Ne mijenjati termin samo zato što je layout nezgodan.

---

## 22. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li povećava ili smanjuje terminološku dosljednost?
2. da li je kompatibilna sa `GLOSSARY.md`?
3. da li olakšava onboarding ili ga otežava?
4. da li rješava stvarni komponentni problem ili samo uvodi novi stil?
5. da li se može dosljedno primijeniti na sve relevantne komponente?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 23. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/iconography-spec.md`
* `components/player-board-spec.md`
* `components/board-spec.md`
* `ux/player-aid-system.md`
* `visuals/card-wireframe-notes.md`
* `ux/information-hierarchy.md`

Ako terminologija nije zaključana prije grafičke faze, gotovo sigurno dolazi do:

* nedosljednih labela
* duplih korekcija layouta
* sporijeg handoffa
* skupljeg playtest print ciklusa

---

## 24. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `GLOSSARY.md`
* `rules/rules-reference-v2.7.md`
* `content/court-roles.md`
* `content/treaties-list.md`
* `content/goods-list.md`
* `components/iconography-spec.md`
* `ux/player-aid-system.md`
* `visuals/card-wireframe-notes.md`

---

## 25. Završna napomena

**Terminology and Labels / Terminologija i oznake** su jedan od glavnih infrastrukturnih dokumenata projekta.

Ako ovaj dokument radi dobro:

* svi dijelovi igre govore istim jezikom
* onboarding je lakši
* gameplay je čišći
* grafički handoff je stabilniji
* revizije su brže i jeftinije

Ako radi loše:

* terminologija se raspada
* aid i komponente se sudaraju
* pravila djeluju nejasnije nego što jesu
* a čitav projekat izgleda manje profesionalno

Zato ovaj dokument mora ostati strogo zaključan i dosljedno primjenjivan kroz cijeli dalji razvoj **v2.7**.
