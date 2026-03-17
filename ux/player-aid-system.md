# player-aid-system.md

# Crown of Sovereigns v2.7 — Player Aid System / Sistem pomoćnog igračkog vodiča

## Status dokumenta

* **Dokument:** `ux/player-aid-system.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati strukturu, sadržaj, UX prioritete i pravila za sve **Player Aid/Pomoćni igrački vodič** materijale u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Player Aid/Pomoćni igrački vodič**, **Court/Dvor**, **Goods/Roba**, **Stability/Stabilnost**
* **Povezani dokumenti:** `rules/turn-structure.md`, `rules/quickstart-first-game.md`, `rules/faq-rules.md`, `components/terminology-and-labels.md`, `components/iconography-spec.md`, `components/player-board-spec.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše čemu **Player Aid/Pomoćni igrački vodič** tačno služi u CoS v2.7
* odredi koje informacije pripadaju aid-u, a koje ne
* postavi standard za strukturu, redoslijed i gustinu informacija
* spriječi da aid postane loša zamjena za pravila ili prenatrpani pregled svega odjednom
* pripremi stabilan osnov za grafički handoff, playtest printove i onboarding

Ovo nije rules reference.
Ovo je UX dokument za jedan od najvažnijih pomoćnih alata tokom stvarne partije.

---

## 2. Zašto je Player Aid / Pomoćni igrački vodič kritičan

U CoS v2.7 pomoćni vodič je ključan jer igra ima više međusobno povezanih sistema:

* **Court/Dvor**
* tok runde
* **Goods/Roba** i razvoj
* **Stability/Stabilnost** i **Unrest/Nemiri**
* **Diplomacy/Diplomatija** i **Treaty/Sporazum** logiku
* **Combat/Borba** proceduru
* završni pritisak i **Coronation Attempt/Pokušaj krunisanja**

Bez dobrog aid sistema, igrači će:

* češće tražiti pravila
* sporije igrati
* teže učiti
* imati više malih proceduralnih grešaka

Dobar aid ne čini igru jednostavnom. On čini složeniju igru podnošljivijom i čišćom za korištenje.

---

## 3. Osnovni princip aid dizajna

Glavno pravilo glasi:

> aid mora ubrzati odluku ili provjeru, ne ponoviti cijeli rules dokument.

To znači:

* aid prikazuje ono što se često provjerava
* aid podsjeća na redoslijed i posljedice
* aid ne smije postati pravni tekst
* aid mora biti skenabilan pogledom, ne čitan red po red kao knjižica

Ako aid moraš čitati kao pravila, aid ne radi svoj posao.

---

## 4. Šta Player Aid / Pomoćni igrački vodič jeste

Aid treba da bude:

* brzi referentni alat
* oslonac za onboarding
* podsjetnik za redoslijed i pragove
* pomoć pri rješavanju najčešćih proceduralnih pitanja
* most između pune dokumentacije i stvarnog toka za stolom

---

## 5. Šta Player Aid / Pomoćni igrački vodič nije

Aid ne smije biti:

* zamjena za `rules/rules-reference-v2.7.md`
* sažetak svake moguće rubne situacije
* vizuelni kolaž pun sitnih ikona i mikroteksta
* mjesto za sav lore i atmosferu igre
* komponenta koja uvodi novi jezik ili nove skraćenice

Ako aid pokuša biti sve, postaće loš u onome što je najvažnije: brzini i jasnoći.

---

## 6. Glavne funkcije aid sistema

Aid sistem mora raditi najmanje 6 stvari:

1. pomoći igraču da prati **Round Spine/Kičmu runde**
2. podsjetiti na glavne dvorske i sistemske prioritete
3. objasniti najvažnije pragove i posljedice
4. smanjiti lookup u pravilima
5. pomoći prvoj partiji bez gušenja informacijama
6. ostati čitljiv tokom cijele partije, ne samo u setupu

Ako radi samo prvu stvar, previše je plitak.
Ako pokuša raditi sve kroz previše teksta, postaje pretežak.

---

## 7. Osnovni model aid sistema u CoS v2.7

Aid sistem treba biti podijeljen u više slojeva, a ne u jedan prenatrpani karton.

Preporučeni slojevi su:

### 7.1. Core Player Aid / Glavni pomoćni vodič

Glavni aid koji svaki igrač ima ispred sebe.

### 7.2. First Game Overlay / Preklop za prvu partiju

Pojednostavljen ili dodatni onboarding sloj za **First Game Mode/Mod prve partije**.

### 7.3. System Reference Micro-Aids / Mikro-aidovi za sisteme

Vrlo kratke reference za specifične stvari koje se često gledaju, ako test pokaže da su potrebne.

Kritično pravilo:

> prvo aid mora riješiti najviše sa najmanje fizičkih komada. Dodatni aidovi dolaze samo ako test pokaže stvarnu potrebu.

---

## 8. Core Player Aid / Glavni pomoćni vodič

Ovo je najvažniji aid materijal.

### 8.1. Šta mora sadržavati

Mora sadržavati najmanje:

* **Round Spine/Kičma runde**
* osnovni pregled **Court/Dvor** logike
* najvažnije **Stability/Stabilnost** i **Unrest/Nemiri** posljedice
* kratki podsjetnik na **Combat/Borba** redoslijed
* kratki podsjetnik na **Treaty/Sporazum** logiku ili diplomatski prozor
* završni podsjetnik kada partija ulazi u završni pritisak

### 8.2. Šta ne smije sadržavati

Ne smije sadržavati:

* sve detaljne exceptions
* puni spisak svih mogućih treaty sadržaja
* previše kartičnog teksta eventova ili kriza
* previše sitnih numeričkih tabela ako se rijetko koriste

---

## 9. Round Spine / Kičma runde

Ovo mora biti najvažniji blok na aid-u.

### 9.1. Zašto

Tok runde je najčešće provjeravana stvar, posebno u prvim partijama.

### 9.2. Kako treba izgledati

Treba biti:

* linearan
* skenabilan
* dovoljno kratak da stane u jedan dominantan blok
* vizuelno razdvojen po fazama

### 9.3. Obavezni sadržaj

Treba podsjetiti na redoslijed:

* **Event/Crisis Phase/Faza događaja i krize**
* **Diplomatic Window/Diplomatski prozor**
* **Court Reveal and Order/Otkrivanje dvora i redoslijed**
* **Action Phase/Faza akcija**
* **Conflict Resolution/Rješavanje sukoba**
* **Income and Development/Prihod i razvoj**
* **Stability and Unrest Update/Ažuriranje stabilnosti i nemira**
* **Round End Check/Završna provjera runde**

---

## 10. Court Aid / Dvorski podsjetnik

Aid mora pomoći da igrač ne zaboravi šta koje uloge znače.

To ne znači pun opis svake moguće kartice ili efekta.
To znači kratki funkcionalni podsjetnik:

* **Marshal/Maršal** = rat i pritisak
* **Diplomat/Diplomata** = sporazumi i politika
* **Merchant/Trgovac** = roba i razvoj
* **Cleric/Klerik** = stabilnost i legitimitet
* **Spy/Špijun** = contest i podrivanje

Ovo je posebno važno za onboarding i rane partije.

---

## 11. Stability Aid / Podsjetnik za stabilnost

Ovo je drugi najvažniji blok poslije toka runde.

### 11.1. Zašto

**Stability/Stabilnost** je jedan od najlakše zaboravljenih, a najvažnijih sistema tokom stvarne partije.

### 11.2. Šta mora sadržavati

Aid treba da podsjeti:

* šta znači da je kraljevstvo zdravo
* šta znači da je pod pritiskom
* šta znači da je blizu loma ili u opasnoj zoni
* najvažnije izvore gubitka stabilnosti
* najvažnije izvore oporavka ili održavanja

### 11.3. Šta ne smije sadržavati

Ne smije sadržavati kompletnu teoriju sistema. Samo ono što igrača najčešće spašava od greške ili zaborava.

---

## 12. Combat Aid / Podsjetnik za borbu

Pošto je borba kratka, aid za nju mora biti još kraći.

Treba sadržavati samo:

* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

Po potrebi može dodati jednu kratku rečenicu o tome šta svaki korak znači, ali ne smije postati mini combat pravilnik.

---

## 13. Diplomacy Aid / Podsjetnik za diplomatiju

Aid treba podsjetiti na:

* da formalna diplomatija ide u **Diplomatic Window/Diplomatski prozor**
* koje su glavne klase **Treaty/Sporazum** odnosa
* da svaki treaty ima benefit i obavezu
* da raskid i **Betrayal/Izdaja** imaju posljedice

Ovo mora biti dovoljno da igrač ne zaboravi logiku, ali ne toliko detaljno da ponavlja cijeli treaty content dokument.

---

## 14. Endgame Aid / Podsjetnik za završnicu

Pošto v2.7 snažno oslanja završnicu na politički i legitimacijski pritisak, aid mora imati mali završni blok koji podsjeća na:

* završni pritisak
* contest vrijednost kraja partije
* **Coronation Attempt/Pokušaj krunisanja** kao završni politički test

Ovaj blok mora biti diskretan u ranoj partiji, ali dovoljno jasan da kraj ne djeluje kao iznenadna promjena žanra.

---

## 15. First Game Overlay / Preklop za prvu partiju

Za **First Game Mode/Mod prve partije** aid sistem treba imati poseban onboarding sloj.

On treba da:

* skrati odluke na razumljivije blokove
* pojača objašnjenje toka runde
* pojača objašnjenje dvorskih uloga
* pojednostavi fokus na nekoliko najvažnijih stvari koje nova grupa mora razumjeti

Ovaj sloj ne smije zamijeniti normalni aid, nego ga učiniti pristupačnijim prvoj partiji.

---

## 16. Mikro-aidovi

Mikro-aidovi su dozvoljeni samo ako playtest pokaže stvarnu potrebu.

To mogu biti kratki pomoćni elementi za:

* 2P **Crown Pressure/Pritisak krune**
* solo **Automa/Automa**
* završni coronation podsjetnik

Ali pravilo je strogo:

> ne praviti mikro-aid za svaki mali problem koji bi bolje riješio bolji glavni aid ili jasniji sistem.

---

## 17. Odnos teksta i ikona na aid-u

Aid ne smije biti ni:

* čisti tekst bez skenabilnosti
* ni čista ikonografija bez sigurnog značenja

Najzdraviji format je:

* kratki label
* po potrebi ikona
* vrlo kratka pomoćna riječ ili linija ispod

Cilj je da aid bude čitljiv za 1–2 sekunde po bloku, ne za 20 sekundi tumačenja.

---

## 18. Veza sa terminology-and-labels standardom

Aid mora strogo slijediti:

* `components/terminology-and-labels.md`

To znači:

* isti termini kao u pravilima i content dokumentima
* isti dvojezični redoslijed
* bez improvizovanih skraćenica
* bez “friendly rewrites” koji mijenjaju značenje sistema

Aid ne smije uvoditi paralelni jezik igre.

---

## 19. Veza sa iconography standardom

Aid treba koristiti ikonografiju, ali štedljivo i namjenski.

To znači:

* najčešće ikone za najčešće pojmove
* bez prenatrpavanja aid površine ikonama za rijetke slučajeve
* ikona mora pomagati skeniranju, ne otežavati ga

Ako aid izgleda kao poster legende ikona, prešao je granicu korisnosti.

---

## 20. Veza sa player-board i board spec dokumentima

Aid ne smije ponavljati ono što je već jasno i stalno vidljivo na:

* **Player Board/Tabli igrača**
* glavnoj **Board/Tabli**

Aid treba podsjećati na:

* redoslijed
* pragove
* proceduralne korake
* ključne posljedice

Ako aid previše duplicira komponente, povećava šum umjesto da pomaže.

---

## 21. Vizuelna hijerarhija aid-a

Preporučena hijerarhija na glavnom aid-u je:

1. **Round Spine/Kičma runde**
2. **Stability/Stabilnost** pragovi i posljedice
3. **Court/Dvor** podsjetnik
4. **Combat/Borba** i **Diplomacy/Diplomatija** mikro-podsjetnici
5. završni / coronation podsjetnik

Ako se ova hijerarhija poremeti, aid će slabije odgovarati stvarnim potrebama partije.

---

## 22. Fizička upotrebljivost aid-a

Aid mora biti upotrebljiv u stvarnim uslovima:

* na stolu sa više komponenti
* pod različitim uglovima gledanja
* u print prototipu i finalnoj verziji
* bez stalnog okretanja ili premeštanja ako to nije nužno

Dizajn koji je lijep, ali traži previše rukovanja, nije dobar aid dizajn.

---

## 23. Najčešće greške u aid dizajnu

* previše teksta u svakom bloku
* premalo teksta pa igrač ne zna šta ikone znače
* isti aid pokušava riješiti i onboarding i sve rubne situacije
* loša hijerarhija gdje su manje bitne stvari veće od toka runde
* dupliciranje pola rulebooka na jednoj karti
* previše različitih aid komada bez stvarnog razloga

---

## 24. Workflow pravilo za novi aid blok

Ako se predlaže novi blok na aid-u, mora se provjeriti redom:

1. da li se ta informacija često traži tokom partije
2. da li se može riješiti boljim postojećim blokom
3. da li blok ubrzava lookup ili samo dodaje još sadržaja
4. da li će nova grupa bolje ili lošije učiti uz njega
5. da li blok može ostati kratak i skenabilan
6. da li pripada aid-u ili rules dokumentu

Ako ne prolazi ova pitanja, novi blok se ne uvodi.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li aid postaje brži za korištenje ili sporiji?
2. da li onboarding postaje lakši ili teži?
3. da li se lookup smanjuje ili povećava?
4. da li se poštuje terminološki i ikonografski standard?
5. da li aid ostaje aid, a ne mini rulebook?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 26. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/player-board-spec.md`
* `components/board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `visuals/card-wireframe-notes.md`
* `ux/information-hierarchy.md`

Ako aid sistem nije dovoljno čist prije grafičke faze, gotovo sigurno dolazi do:

* prenatrpanih aid karti
* slabije čitljivosti prototipa
* više lookup trenutaka nego što sistem zaslužuje
* skupljih iteracija na layoutu

---

## 27. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `rules/turn-structure.md`
* `rules/quickstart-first-game.md`
* `rules/faq-rules.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `components/player-board-spec.md`
* `ux/information-hierarchy.md`
* `visuals/card-wireframe-notes.md`

---

## 28. Završna napomena

**Player Aid System / Sistem pomoćnog igračkog vodiča** mora ostati jedan od najpraktičnijih i najstrože disciplinovanih UX slojeva u CoS v2.7.

Ako radi dobro:

* partije teku brže
* nova grupa lakše uči
* lookup u pravilima se smanjuje
* sistemi izgledaju čišće nego što bi bez aid-a djelovali
* a grafički handoff dobija jasan prioritet sadržaja

Ako radi loše:

* igra djeluje težom nego što jeste
* pomoćni materijal postaje novi izvor konfuzije
* onboarding pati
* a partija dobija više sitnih zastoja nego što sistem zaslužuje

Zato ovaj dokument mora ostati strogo fokusiran na funkciju, brzinu i čitljivost kroz cijeli dalji razvoj **v2.7**.
