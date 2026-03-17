# player-board-spec.md

# Crown of Sovereigns v2.7 — Player Board Specification / Specifikacija table igrača

## Status dokumenta

* **Dokument:** `components/player-board-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati funkciju, sadržaj, zone i UX pravila za **Player Board/Tablu igrača**
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Player Board/Tabla igrača**, **Court/Dvor**, **Goods/Roba**, **Stability/Stabilnost**
* **Povezani dokumenti:** `components/terminology-and-labels.md`, `components/iconography-spec.md`, `rules/rules-reference-v2.7.md`, `systems/court-system.md`, `systems/goods-and-development.md`, `systems/stability-and-unrest.md`, `ux/player-aid-system.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše šta **Player Board/Tabla igrača** mora sadržavati
* odredi koje informacije pripadaju tabli igrača, a koje ne
* spriječi da tabla igrača postane prenatrpana mini-kontrolna tabla za cijelu igru
* osigura da layout podržava stvarni gameplay, a ne samo vizuelni utisak
* pripremi jasan i stabilan osnov za grafički handoff i prototip printove

Ovo nije ilustrativni moodboard.
Ovo je operativna specifikacija za jednu od najvažnijih fizičkih komponenti igre.

---

## 2. Zašto je Player Board / Tabla igrača kritična

U CoS v2.7 tabla igrača nije samo dekorativna površina.
Ona mora pomoći igraču da:

* razumije stanje svog kraljevstva
* prati glavne unutrašnje sisteme
* brže donosi odluke
* manje luta između glavne table, aid-a i ličnih markera

Ako tabla igrača radi loše:

* gameplay postaje sporiji
* onboarding teži
* više pravila djeluje nejasno nego što zaista jeste
* broj mikro-grešaka tokom partije raste

Zato **Player Board/Tabla igrača** mora biti UX komponenta, ne samo estetska.

---

## 3. Osnovni princip dizajna

Glavno pravilo glasi:

> tabla igrača mora prikazivati stanje kraljevstva, ne cijelu igru u malom.

To znači:

* na tabli trebaju biti lične, stalne i često korištene informacije
* ne treba duplicirati sve što već postoji na glavnoj tabli
* ne treba dodavati zone samo zato što bi “moglo biti korisno jednog dana”

Svaka zona mora opravdati svoje mjesto kroz stvarni gameplay dobitak.

---

## 4. Šta tabla igrača jeste

**Player Board/Tabla igrača** treba da bude:

* lična komandna površina kraljevstva
* pregled glavnih internih stanja i ličnih resursa
* jasno organizovan prostor za najčešće privatne ili polu-javne informacije igrača
* mjesto gdje se lako vide unutrašnja cijena moći, razvoj i dvorski fokus

---

## 5. Šta tabla igrača nije

Tabla igrača ne smije biti:

* minijaturna kopija glavne table
* rules summary poster za sve sisteme odjednom
* površina sa deset različitih mikro-trackera koji se rijetko koriste
* mjesto za dekorativni heraldic višak koji guši funkciju
* prostor gdje su važni podaci sakriveni ispod ukrasa ili previše malih ikona

Ako sklizne u bilo šta od navedenog, tabla gubi UX vrijednost.

---

## 6. Glavne funkcije table igrača

**Player Board/Tabla igrača** mora raditi najmanje 5 stvari:

1. prikazati ključno stanje kraljevstva
2. podržati **Court/Dvor** logiku
3. podržati **Goods/Roba** i razvoj
4. jasno prikazivati **Stability/Stabilnost** i povezane unutrašnje pritiske
5. ostati čitljiva i brza za korištenje tokom cijele partije

Ako radi samo prve tri stvari bez četvrte i pete, igra gubi jedan od najvažnijih UX oslonaca.

---

## 7. Informacije koje pripadaju tabli igrača

Na tabli igrača treba da budu samo informacije koje su:

* lične
* često provjeravane
* važne za donošenje odluke
* praktično korisne za držanje na jednom mjestu

To u v2.7 najprirodnije uključuje:

* **Court/Dvor** povezane informacije ili zone
* **Goods/Roba** i razvojne zone
* **Stability/Stabilnost** i eventualno **Unrest/Nemiri** vezane lične zone
* lične resurse ili njihov pregled, gdje je to UX ispravno
* eventualne **Kingdom Advantages/Prednosti kraljevstva** reference

---

## 8. Informacije koje ne pripadaju tabli igrača

Na tabli igrača ne treba držati stvari koje su prvenstveno:

* zajedničke i javne za cijeli sto
* prostorno vezane za glavnu mapu
* rijetke ili situacione do te mjere da zauzimaju stalni prostor bez potrebe

To tipično znači da tabla igrača ne treba da bude glavno mjesto za:

* mapnu kontrolu provincija
* zajedničke event/crisis informacije
* puni treaty pregled cijelog stola
* kompletan rules reference

---

## 9. Obavezne glavne zone na tabli igrača

U v2.7 tabla igrača treba da sadrži najmanje sljedeće glavne zone:

### 9.1. Kingdom Identity Zone / Zona identiteta kraljevstva

Mjesto za:

* naziv ili oznaku kraljevstva
* osnovnu vizuelnu identifikaciju igrača
* eventualnu kratku **Kingdom Advantage/Prednost kraljevstva** referencu

### 9.2. Court Zone / Zona dvora

Mjesto za:

* pregled ili radni prostor vezan za **Court/Dvor**
* pregled **Court Roles/Dvorske uloge** gdje je relevantno
* jasan osjećaj da je dvor srce table, ne sporedni dodatak

### 9.3. Goods and Development Zone / Zona robe i razvoja

Mjesto za:

* **Goods/Roba**
* razvojni napredak
* ekonomski ili razvojni state koji igrač često gleda

### 9.4. Stability Zone / Zona stabilnosti

Mjesto za:

* **Stability/Stabilnost**
* prateće unutrašnje stanje ili upozorenje na pritisak
* eventualnu vidljivu vezu sa pragovima stabilnosti

### 9.5. Resource Support Zone / Zona podrške resursima

Mjesto za:

* pregled ključnih resursa ili njihove organizacije
* ali samo onoliko koliko pomaže, bez pretvaranja table u skladišni kaos

---

## 10. Kingdom Identity Zone / Zona identiteta kraljevstva

Ova zona mora biti:

* lako uočljiva
* dovoljno čista da odmah kaže čije je to kraljevstvo
* vizuelno stabilna kroz sve varijante dizajna

Ona ne smije biti:

* najveći dekorativni blok na tabli
* prenatrpana heraldikom koja smanjuje prostor za funkcionalne zone

Identitet je važan, ali funkcija ima prioritet.

---

## 11. Court Zone / Zona dvora

Ovo je jedna od najvažnijih zona cijele table.

### 11.1. Zašto

Pošto je **Court/Dvor** glavni motor odluka, tabla igrača mora to jasno pokazati.

### 11.2. Šta zona mora raditi

Mora omogućiti:

* brz pregled dvorskih prioriteta
* čitljiv odnos prema dvorskim ulogama
* dovoljno prostora da igrači ne miješaju dvorske informacije sa goods ili resursnim prostorom

### 11.3. Šta ne smije raditi

Ne smije:

* sakriti dvor u mali ugao table
* koristiti layout koji čini da dvor izgleda kao sekundarna pomoćna funkcija

Ako se to desi, cijeli identitet igre slabi.

---

## 12. Goods and Development Zone / Zona robe i razvoja

Ova zona mora jasno razlikovati **Goods/Roba** od opštih resursa.

### 12.1. Zašto

Goods nisu samo potrošni tokeni. Oni su razvojni identitet kraljevstva.

### 12.2. Šta zona mora raditi

Mora omogućiti:

* pregled goods stanja
* osjećaj razvoja i napretka
* jasnu odvojenost od običnog “resource pile” prostora

### 12.3. Šta ne smije raditi

Ne smije:

* miješati goods sa resursima bez jasne vizuelne granice
* biti toliko komplikovana da izgleda kao zasebna ekonomska igra

---

## 13. Stability Zone / Zona stabilnosti

Ovo je druga najvažnija interna zona poslije dvora.

### 13.1. Zašto

**Stability/Stabilnost** je jedan od glavnih identitetskih stubova CoS-a.

### 13.2. Šta zona mora raditi

Mora omogućiti:

* trenutno čitanje unutrašnjeg stanja kraljevstva
* vidljiv pregled stabilnost praga ili njegovog kvalitativnog raspona
* jasan osjećaj kada je kraljevstvo zdravo, pod pritiskom ili u opasnosti

### 13.3. Šta ne smije raditi

Ne smije:

* biti skrivena ili premala
* koristiti nejasne oznake koje igrači stalno moraju provjeravati u pravilima

Ako se stabilnost teško čita, igrač neće osjećati cijenu moći kako treba.

---

## 14. Resource Support Zone / Zona podrške resursima

Ova zona mora biti pažljivo kalibrisana.

### 14.1. Zašto

Resursi su važni, ali tabla igrača ne smije postati samo skladišna površina.

### 14.2. Šta zona treba raditi

Treba omogućiti:

* organizaciju osnovnih resursa
* brže čitanje ekonomskog stanja
* manje fizičkog haosa na stolu

### 14.3. Šta ne smije raditi

Ne smije:

* zauzeti više prostora nego goods i stabilnost zajedno ako to guši identitet table
* tjerati igrača da pomjera previše tokena samo zbog dizajna zone

---

## 15. Veza sa terminology-and-labels standardom

Sve labele na tabli igrača moraju koristiti standard iz:

* `components/terminology-and-labels.md`

To znači:

* puni ili kontrolisano skraćeni dvojezični termini
* dosljedan separator `/`
* bez paralelnih naziva za iste sisteme

Tabla igrača je jedno od mjesta gdje terminološka nedosljednost najbrže pravi gameplay konfuziju.

---

## 16. Veza sa iconography sistemom

Ikone na tabli igrača moraju biti:

* podrška labelima
* dosljedne sa `components/iconography-spec.md`
* dovoljno velike da ostanu čitljive
* ograničene na one koje stvarno ubrzavaju korištenje table

Tabela igrača nije mjesto za demonstraciju svih ikona u igri.
Ona treba da koristi samo one koje pomažu njenoj funkciji.

---

## 17. Vizuelna hijerarhija zone

Raspored mora jasno pokazati šta je najvažnije.

Preporučena hijerarhija je:

1. **Court/Dvor**
2. **Stability/Stabilnost**
3. **Goods/Roba** i razvoj
4. identitet kraljevstva
5. podrška resursima i sekundarne reference

Ako resursi ili dekoracija vizuelno pregaze dvor i stabilnost, tabla šalje pogrešnu poruku o tome šta je srce igre.

---

## 18. Čitljivost na stolu

Tabla igrača mora biti čitljiva:

* direktno ispred vlasnika table
* djelimično i drugim igračima kad je to sistemski važno
* u uslovima normalnog stolnog osvjetljenja
* i kada su tokeni stvarno postavljeni na nju, ne samo u idealnom praznom mockupu

Dizajn koji izgleda dobro samo kao prazan render nije dovoljno dobar.

---

## 19. Odnos javnog i privatnog na tabli

CoS nema potrebu da tabla igrača sakrije previše stvari iza privatnog zida.

Zato player board treba da bude prvenstveno:

* ličan
* ali ne potpuno zatvoren za pogled drugih kada su u pitanju važni javni signali kao što su **Stability/Stabilnost** ili opšti goods razvoj

Ako tabla previše skriva ključno stanje, politička čitljivost partije pati.

---

## 20. Pristupačnost i upotrebljivost

Tabela igrača mora biti projektovana tako da ostane:

* čitljiva pri slabijem kontrastu okoline
* razumljiva bez oslanjanja samo na boju
* dovoljno jasna za nove igrače
* pogodna za prototip i konačnu štampu

To znači:

* jasan kontrast zona
* dovoljno velik tekst za glavne labele
* oblik i layout kao pomoć, ne samo dekorativni okvir

---

## 21. Onboarding uloga table igrača

Za novu grupu tabla igrača treba da bude jedan od glavnih onboarding alata.

Igrač bi nakon prvih nekoliko minuta trebalo da može intuitivno vidjeti:

* gdje mu je dvor
* gdje mu je stabilnost
* gdje mu je goods razvoj
* gdje mu stoje osnovne resursne informacije

Ako nova grupa ne može to odmah pročitati, tabla nije dobro organizovana.

---

## 22. Najčešće greške u dizajnu table igrača

* previše malih odvojenih zona
* dekorativni višak koji jede funkcionalni prostor
* goods i resursi u istoj vizuelnoj masi
* skrivena ili slaba **Stability/Stabilnost** zona
* **Court/Dvor** gurnut na sekundarno mjesto
* previše ikonografije bez dovoljne tekstualne potvrde
* layout koji izgleda lijepo, ali ne radi kad su tokeni fizički prisutni

---

## 23. Workflow pravilo za novu zonu na tabli

Ako se predlaže nova zona na tabli igrača, mora se provjeriti redom:

1. da li ta informacija zaista pripada ličnoj tabli igrača
2. da li se koristi dovoljno često da opravda stalni prostor
3. da li već postoji postojeća zona koja može primiti tu funkciju
4. da li nova zona povećava ili smanjuje čitljivost
5. da li nova zona povećava ili smanjuje onboarding težinu
6. da li se problem može riješiti aid-om umjesto novom zonom

Ako ne prolazi ova pitanja, nova zona se ne uvodi.

---

## 24. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li jača ili slabi čitljivost table?
2. da li dvor ostaje centralan?
3. da li stabilnost ostaje dovoljno vidljiva?
4. da li goods ostaju jasno odvojeni od resursa?
5. da li promjena uvodi nepotrebni layout bloat?
6. da li ostaje kompatibilna sa ikonografijom i terminologijom?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 25. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `ux/player-aid-system.md`
* `ux/information-hierarchy.md`
* `visuals/card-wireframe-notes.md`

Ako tabla igrača nije dovoljno čista prije grafičke faze, gotovo sigurno će doći do:

* skupljih layout revizija
* slabijeg onboarding rezultata
* neujednačenih prototip printova
* više pravilaških lookup trenutaka tokom partije

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `rules/rules-reference-v2.7.md`
* `systems/court-system.md`
* `systems/goods-and-development.md`
* `systems/stability-and-unrest.md`
* `ux/player-aid-system.md`
* `ux/information-hierarchy.md`
* `components/board-spec.md`

---

## 27. Završna napomena

**Player Board Specification / Specifikacija table igrača** mora ostati jedan od glavnih UX stubova fizičkog proizvoda.

Ako radi dobro:

* kraljevstvo je lakše čitati
* odluke su brže
* onboarding je bolji
* dvor, goods i stabilnost djeluju kao dio jedne cjeline
* a grafički handoff je mnogo sigurniji

Ako radi loše:

* tabla postaje lijep, ali neupotrebljiv komad kartona
* igra djeluje težom nego što jeste
* unutrašnji sistemi se čitaju sporije
* a partije dobijaju više sitnih, ali skupih UX grešaka

Zato ovaj dokument mora ostati strogo funkcionalan i stalno usklađen sa jezgrom **v2.7**.
