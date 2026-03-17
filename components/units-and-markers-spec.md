# units-and-markers-spec.md

# Crown of Sovereigns v2.7 — Units and Markers Specification / Specifikacija jedinica i markera

## Status dokumenta

* **Dokument:** `components/units-and-markers-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati vrste, funkciju, fizičku ulogu i granice za sve **Units/Jedinice** i **Markers/Markeri** elemente u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Unit/Jedinica**, **Marker/Marker**, **Control Marker/Marker kontrole**
* **Povezani dokumenti:** `components/tokens-spec.md`, `components/board-spec.md`, `components/player-board-spec.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `systems/province-map-system.md`, `systems/combat-system.md`, `systems/stability-and-unrest.md`, `systems/coronation-system.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* jasno razdvoji **Units/Jedinice**, **Markers/Markeri** i **Tokens/Tokeni**
* definiše kada nešto treba biti jedinica, kada marker, a kada token
* spriječi fizičku i vizuelnu konfuziju na tabli i tabli igrača
* uskladi prostorno prisustvo, statusno praćenje i kontrolne signale u jedan disciplinovan komponentni sistem
* pripremi čist osnov za prototip, grafički handoff i buduću produkcijsku odluku

Ovo nije samo popis fizičkih komada.
Ovo je dokument koji čuva razliku između “šta je na mapi”, “šta označava stanje” i “šta prati vrijednost”.

---

## 2. Zašto je ova razlika kritična

Kod board game sistema vrlo brzo nastaje zbrka ako nije jasno šta je:

* fizička prisutnost
* kontrola
* status
* promjenjiva vrijednost

Ako se te stvari miješaju, nastaju problemi:

* igrači ne znaju da li komad znači prisutnost ili samo stanje
* mapa postaje teža za čitanje
* combat i kontrola djeluju mutnije nego što jesu
* setup i teardown postaju sporiji
* markeri i tokeni počnu raditi isti posao na različite načine

Zato CoS mora imati strogu komponentnu logiku.

---

## 3. Osnovni princip razlikovanja

Glavno pravilo glasi:

> **Unit/Jedinica** predstavlja prisutnost ili aktera u prostoru; **Marker/Marker** označava stanje, vlasništvo, status ili podsjetnik; **Token/Token** prati jasno izdvojenu vrijednost ili formalizovan signal kada je takav oblik najprikladniji.

To znači:

* jedinica je “na terenu”
* marker obično kaže “šta ovdje važi”
* token obično kaže “koliko nečega postoji” ili “koji formalni signal je aktivan”

Ako ova logika nije čista, cijela komponentna baza postaje zamućena.

---

## 4. Šta Units/Jedinice jesu

**Units/Jedinice** treba da budu:

* fizički prisutni komadi koji predstavljaju stvarnu operativnu snagu ili prisutnost na mapi
* prostorno relevantni
* direktno povezani sa kretanjem, pritiskom, konfliktom ili teritorijalnim uticajem

Jedinica mora značiti da je neko ili nešto stvarno “tu”.

---

## 5. Šta Units/Jedinice nisu

**Units/Jedinice** ne smiju biti:

* univerzalni marker za sve vrste stanja
* zamjena za kontrolni signal ako prisutnost i kontrola nisu ista stvar
* dekorativni vojni višak koji guši mapu
* komponenta koja nosi previše sekundarnih statusa na sebi

Ako se jedinice koriste za previše stvari odjednom, mapa gubi čitljivost.

---

## 6. Šta Markers/Markeri jesu

**Markers/Markeri** treba da budu:

* jednostavni fizički označivači stanja, statusa, vlasništva, podsjetnika ili proceduralne tačke
* vizuelno jasniji od improvizovanih rješenja
* lakši i skromniji od jedinica

Marker ne predstavlja “aktera”.
On predstavlja “informaciju o stanju”.

---

## 7. Šta Markers/Markeri nisu

**Markers/Markeri** ne smiju biti:

* zamjena za jedinice kada je prostorna prisutnost suština
* duplikat tokena ako isti signal već postoji kroz bolji fizički alat
* toliko brojni i raznoliki da stol izgleda kao statusni spreadsheet

Ako markeri rade previše poslova, igra gubi fizičku eleganciju.

---

## 8. Glavne funkcije jedinica i markera u CoS v2.7

Ovaj komponentni sloj treba da radi najmanje sljedeće:

1. da jasno pokaže prostornu prisutnost i vojni / mapni pritisak
2. da odvoji prisutnost od kontrole kada ta dva nisu isto
3. da označi contested i posebna stanja bez gušenja mape
4. da podrži završne i coronation signale tamo gdje marker ima više smisla od kartice ili tokena
5. da ostane komponentno disciplinovan i čitljiv u stvarnoj partiji

---

## 9. Osnovne klase komponenti u ovom dokumentu

Ovaj dokument pokriva najmanje ove klase:

### 9.1. Map Units / Mapne jedinice

Jedinice koje žive na glavnoj **Board/Tabli** i predstavljaju prisutnost na mapi.

### 9.2. Control Markers / Markeri kontrole

Markeri koji označavaju ko kontroliše prostor ili političku tačku gdje to nije dovoljno jasno samo iz jedinica.

### 9.3. Status Markers / Statusni markeri

Markeri koji označavaju **Contested/Osporeno**, aktivan status, podsjetnik ili drugi važan signal.

### 9.4. Progress or Position Markers / Markeri napretka ili pozicije

Markeri koji se koriste na trackovima ili tablama kada nije potreban pun token sistem.

### 9.5. Endgame Markers / Markeri završnice

Markeri koji podržavaju završni pritisak, coronation ili završni contest signal.

Kritično pravilo:

> svaka klasa mora imati jasan razlog postojanja i ne smije previše preklapati drugu klasu.

---

## 10. Obavezna struktura jedne specifikacije

Svaka vrsta jedinice ili markera treba biti opisana ovim redom:

1. **Naziv:** English/Srpski
2. **Klasa**
3. **Primarna funkcija**
4. **Gdje se koristi**
5. **Šta mora jasno komunicirati**
6. **Šta ne smije zbuniti**
7. **Odnosi sa tokenima i drugim markerima**
8. **Napomena za veličinu, oblik ili vizuelni signal**

Ova struktura pomaže da komponente ostanu uporedive i produkcijski jasne.

---

## 11. Map Unit / Mapna jedinica

### 11.1. Primarna funkcija

Predstavlja stvarnu prisutnost igrača ili njegove operativne sile na mapi.

### 11.2. Gdje se koristi

Na glavnoj **Board/Tabli**, unutar ili uz odgovarajuće **Provinces/Provincije**.

### 11.3. Šta mora komunicirati

* da je igrač prisutan u tom prostoru
* da ta prisutnost ima uticaj na pritisak, konflikt ili contest logiku

### 11.4. Šta ne smije zbuniti

Ne smije biti nejasno da li jedinica sama po sebi znači i punu kontrolu ili samo prisutnost.
Ako prisutnost i kontrola nisu ista stvar, to se mora vidjeti kroz odvojeni alat.

---

## 12. Control Marker / Marker kontrole

### 12.1. Primarna funkcija

Označava formalnu kontrolu nad prostorom, kada to nije dovoljno jasno samo kroz prisutnost jedinice.

### 12.2. Gdje se koristi

Na glavnoj **Board/Tabli**, u ili uz određeni teritorijalni prostor ili relevantan čvor.

### 12.3. Šta mora komunicirati

* ko formalno drži kontrolu
* da je to stanje stabilnije ili drugačije od same prisutnosti

### 12.4. Šta ne smije zbuniti

Ne smije izgledati kao druga jedinica.
Mora biti jasno da označava status prostora, ne dodatnu prostornu silu.

---

## 13. Contested Marker / Marker osporavanja

### 13.1. Primarna funkcija

Označava da je prostor, status ili ishod formalno **Contested/Osporeno**.

### 13.2. Gdje se koristi

Na glavnoj tabli, a po potrebi i u završnim ili coronation kontekstima.

### 13.3. Šta mora komunicirati

* da stanje nije čisto zaključano
* da postoji aktivna napetost, spor ili otvoreno pitanje

### 13.4. Šta ne smije zbuniti

Ne smije se miješati sa kontrolnim markerom ili opštim podsjetnikom.
Njegova funkcija je alarm i napetost, ne vlasništvo.

---

## 14. Progress Marker / Marker napretka

### 14.1. Primarna funkcija

Označava poziciju na tracku, progres osi ili tačku kretanja kroz neki jasan numerički ili kvalitativni raspon.

### 14.2. Gdje se koristi

Najčešće na **Player Board/Tabli igrača**, a po potrebi i na zajedničkim trackovima glavne table.

### 14.3. Šta mora komunicirati

* trenutnu poziciju na nekom linearnom ili diskretnom rasponu
* stabilan i lako čitljiv napredak

### 14.4. Šta ne smije zbuniti

Ne smije izgledati kao token stanja koji se gomila, ako mu je stvarna funkcija samo pozicija na tracku.

---

## 15. Stability Marker / Marker stabilnosti

Ovaj marker može biti poseban slučaj **Progress Marker/Markera napretka** ako se stabilnost prati preko tracka.

### 15.1. Primarna funkcija

Označava trenutnu poziciju na **Stability/Stabilnost** osi.

### 15.2. Gdje se koristi

Primarno na **Player Board/Tabli igrača**.

### 15.3. Šta mora komunicirati

* trenutno unutrašnje stanje kraljevstva
* jasan odnos prema sigurnoj, napetoj ili opasnoj zoni

### 15.4. Šta ne smije zbuniti

Ne smije se miješati sa **Unrest/Nemiri** markerom ili resursnim markerima.

---

## 16. Unrest Marker / Marker nemira

Ovaj marker označava prisustvo ili poziciju **Unrest/Nemiri** pritiska tamo gdje je marker logika prikladnija od token gomile.

### 16.1. Primarna funkcija

Označava negativni unutrašnji pritisak ili njegovo poziciono stanje.

### 16.2. Gdje se koristi

Primarno na tabli igrača.

### 16.3. Šta mora komunicirati

* da postoji unutrašnji poremećaj
* da taj poremećaj nosi drugačiji signal od stabilnosti

### 16.4. Šta ne smije zbuniti

Ne smije biti previše sličan markeru stabilnosti ni po funkciji ni po vizuelnom kodu.

---

## 17. Treaty Marker / Marker sporazuma

Ako se koristi marker uz kartu ili na posebnoj političkoj zoni, njegova funkcija mora biti strogo pomoćna.

### 17.1. Primarna funkcija

Pomaže javnom čitanju statusa formalnog **Treaty/Sporazum** odnosa.

### 17.2. Gdje se koristi

Na političkom dijelu glavne table ili uz treaty komponentu.

### 17.3. Šta mora komunicirati

* da sporazum postoji, traje ili je u posebnom stanju

### 17.4. Šta ne smije zbuniti

Ne smije biti složeniji od same treaty karte ili stvarati osjećaj dodatne spreadsheet logike.

---

## 18. Coronation Marker / Marker krunisanja

### 18.1. Primarna funkcija

Označava aktivaciju, fazu ili javni status **Coronation Attempt/Pokušaj krunisanja** kada je fizički marker najbrže i najjasnije rješenje.

### 18.2. Gdje se koristi

Na završnom / coronation prostoru glavne table ili uz završnu referentnu komponentu.

### 18.3. Šta mora komunicirati

* da je partija ušla u poseban završni režim
* da je pažnja stola sada usmjerena na završni contest ili legitimitet signal

### 18.4. Šta ne smije zbuniti

Ne smije izgledati kao obični status marker ili nepotrebni dekorativni trofej.

---

## 19. Units vs Markers vs Tokens / Jedinice naspram markera naspram tokena

Ovo je najvažnija razlika u cijelom dokumentu.

### 19.1. Unit / Jedinica

Koristi se kada nešto:

* zauzima prostor
* vrši pritisak
* učestvuje u mapnom prisustvu i konfliktu

### 19.2. Marker / Marker

Koristi se kada nešto:

* označava stanje
* označava vlasništvo
* označava poziciju ili podsjetnik
* ne predstavlja samostalnog aktera

### 19.3. Token / Token

Koristi se kada nešto:

* prati izdvojenu vrijednost, broj ili formalizovani status
* treba biti fizički naglašeno kao zaseban sistemski signal
* ne mora nužno imati istu prostornu logiku kao jedinica ili marker

Ako jedna stvar može biti riješena jednostavnijim markerom, ne treba joj davati punu unit ili token logiku.

---

## 20. Veza sa board-spec dokumentom

Sve mapne jedinice i markeri moraju biti usklađeni sa:

* `components/board-spec.md`

To znači:

* ne smiju pregaziti čitljivost provincija
* moraju imati jasno mjesto na tabli
* njihova veličina i broj moraju biti realni za stvarni board load

Ako komad ne može zdravo živjeti na mapi, nije dovoljno dobro definisan.

---

## 21. Veza sa player-board-spec dokumentom

Lični markeri moraju biti usklađeni sa:

* `components/player-board-spec.md`

To znači:

* ne smiju gušiti zonu dvora, stabilnosti ili goods razvoja
* moraju se uklapati u realnu prostornu logiku table igrača
* moraju pomoći čitljivosti, ne je usporiti

---

## 22. Veza sa tokens-spec dokumentom

Ovaj dokument ne smije duplirati `components/tokens-spec.md`, nego ga dopunjavati.

Pravilo je:

* ako komad prvenstveno označava vrijednost ili formalizovani signal kroz token logiku, ide tamo
* ako komad prvenstveno označava prisutnost ili status kroz jednostavniji marker/jedinica model, ide ovdje

Ako isti komad istovremeno djeluje kao jedinica, marker i token, sistem vjerovatno nije dovoljno čist.

---

## 23. Veza sa iconography i terminology dokumentima

Sve jedinice i markeri moraju slijediti:

* `components/iconography-spec.md`
* `components/terminology-and-labels.md`

To znači:

* jasan i dosljedan vizuelni kod
* nema paralelnih naziva za isto stanje
* markeri ne smiju zavisiti samo od boje ako oblik ili kontekst nisu jasni

---

## 24. Component budget / Budžet komponenti

Broj različitih tipova jedinica i markera mora biti strogo kontrolisan.

Treba izbjegavati:

* marker za svaku mikro-situaciju
* različite forme koje rade gotovo isti posao
* posebne markere za edge cases koje aid ili karta već dovoljno rješavaju

Pravilo:

> svaki novi tip komada mora opravdati i gameplay dobitak i logistički trošak.

---

## 25. Setup and teardown disciplina / Disciplina setupa i raspremanja

Svaka jedinica i marker klasa treba da se procijeni i po tome:

* koliko otežava setup
* koliko otežava raspremanje
* koliko je intuitivna za sortiranje
* da li stvara fizički nered tokom sredine i kraja partije

Dobar komponentni sistem ne završava na estetskom opisu. Mora biti i logistički održiv.

---

## 26. Najčešće greške u ovom sloju

* jedinice i markeri izgledaju previše slično
* kontrola i prisutnost nisu jasno odvojeni
* contested marker djeluje kao obični podsjetnik umjesto važnog signala
* stability i unrest marker se miješaju
* završni marker je previše dekorativan, a premalo jasan
* previše različitih marker tipova bez dovoljno razloga

---

## 27. Workflow pravilo za novi unit ili marker tip

Ako se predlaže novi **Unit/Jedinica** ili **Marker/Marker** tip, treba provjeriti redom:

1. da li predstavlja prisutnost ili stanje
2. da li taj posao već radi postojeći komad
3. da li je fizički dovoljno važan da opravda poseban tip
4. gdje živi na stolu
5. da li povećava ili smanjuje čitljivost
6. da li povećava komponentni bloat i logistički trošak

Ako ne prolazi ova pitanja, novi tip se ne uvodi.

---

## 28. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li razlika između jedinica, markera i tokena ostaje čista?
2. da li novi komad donosi stvarni gameplay benefit?
3. da li ostaje usklađen sa tablom i tablom igrača?
4. da li ostaje kompatibilan sa ikonografijom i terminologijom?
5. da li smanjuje ili povećava logistički i komponentni teret?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 29. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/tokens-spec.md`
* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `systems/province-map-system.md`
* `systems/combat-system.md`
* `systems/stability-and-unrest.md`
* `systems/coronation-system.md`
* `ux/information-hierarchy.md`
* `GLOSSARY.md`

---

## 30. Završna napomena

**Units and Markers Specification / Specifikacija jedinica i markera** mora ostati jedan od glavnih komponentnih filtera za fizičku čitljivost i disciplinu u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* mapa se čita brže
* kontrola i prisutnost se ne miješaju
* statusi imaju jasan fizički signal
* setup i teardown ostaju pod kontrolom
* a grafički handoff dobija čist i logičan komponentni sistem

Ako radi loše:

* stol postaje konfuzan
* komadi se preklapaju u značenju
* važna stanja se teže čitaju
* a igra djeluje težom i neurednijom nego što treba

Zato ovaj dokument mora ostati strog, jasan i potpuno usklađen sa logikom **v2.7**.
