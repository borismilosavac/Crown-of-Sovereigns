# tokens-spec.md

# Crown of Sovereigns v2.7 — Tokens Specification / Specifikacija tokena

## Status dokumenta

* **Dokument:** `components/tokens-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati vrste, funkciju, pravila upotrebe i komponentne granice za sve **Tokens/Tokeni** elemente u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Token/Token**, **Control Token/Token kontrole**, **Stability Token/Token stabilnosti**
* **Povezani dokumenti:** `components/board-spec.md`, `components/player-board-spec.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `systems/province-map-system.md`, `systems/stability-and-unrest.md`, `systems/diplomacy-and-treaties.md`, `systems/coronation-system.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše koje vrste **Tokens/Tokeni** postoje u CoS v2.7
* objasni čemu svaki token služi i gdje pripada
* spriječi da se različita stanja rješavaju stihijski kroz previše sličnih ili nepotrebnih tokena
* uskladi token logiku sa tablom, tablom igrača, aid-om i ikonografijom
* pripremi čist osnov za kasniji grafički handoff i produkcijsku disciplinu

Ovo nije samo lista tokena.
Ovo je dokument koji čuva komponentnu jasnoću i mehaničku disciplinu.

---

## 2. Zašto je token sistem kritičan

Kod strateške board game igre, tokeni su često najbrži put i do jasnoće i do haosa.

Dobri **Tokens/Tokeni**:

* ubrzavaju čitanje stanja
* smanjuju potrebu za dodatnim lookup-om
* pomažu da se važna stanja vide odmah
* održavaju fizički red na stolu

Loši **Tokens/Tokeni**:

* povećavaju bookkeeping
* pretrpavaju tablu
* djeluju previše slično jedni drugima
* uvode više fizičke administracije nego stvarne vrijednosti

Zato CoS token sistem mora biti strogo kontrolisan.

---

## 3. Osnovni princip token dizajna

Glavno pravilo glasi:

> svaki token mora predstavljati stanje ili vrijednost koja je dovoljno važna, dovoljno česta i dovoljno prostorno relevantna da opravda fizički marker.

To znači da token ne smije postojati samo zato što:

* bi izgledao lijepo
* čini sistem “bogatijim”
* pomaže zamisliti još jedan podsistem koji zapravo nije potreban

Ako stanje može biti bolje riješeno track-om, kartom, aid-om ili jednostavnijim markerom, treba izbjeći novi token.

---

## 4. Šta token sistem jeste

Token sistem treba da bude:

* funkcionalan
* ograničen
* lako čitljiv
* fizički praktičan
* usklađen sa informacijskom hijerarhijom i komponentnim layoutom

---

## 5. Šta token sistem nije

Token sistem nije:

* dekorativna zbirka markera
* način da se svaka mala nijansa sistema materijalizuje kao poseban komad
* izgovor za rješavanje rules nejasnoće kroz još više fizičkih elemenata
* zamjena za dobar UI na tabli ili tabli igrača

Ako tokeni postanu zamjena za jasnoću dizajna, to je znak slabijeg sistema, ne bogatijeg.

---

## 6. Glavne funkcije tokena u CoS v2.7

Tokeni u ovoj verziji treba da služe najmanje ovim funkcijama:

1. označavanje prostorne kontrole i spornog stanja
2. označavanje važnih ličnih ili javnih stanja koja se često mijenjaju
3. podrška **Stability/Stabilnost** i završnim pritiscima gdje je fizički marker koristan
4. podrška treaty, contest ili završnim javnim signalima kada to ubrzava čitanje
5. održavanje reda na stolu bez nepotrebne komponentne inflacije

Ako token radi samo petu stvar bez prve četiri, vjerovatno nije potreban.

---

## 7. Osnovne klase tokena

Sve **Tokens/Tokeni** elemente treba podijeliti najmanje na ove klase:

### 7.1. Map Tokens / Mapni tokeni

Tokeni koji žive prvenstveno na glavnoj **Board/Tabli**.

### 7.2. Player State Tokens / Tokeni ličnog stanja

Tokeni koji prvenstveno žive na **Player Board/Tabli igrača**.

### 7.3. System Status Tokens / Tokeni sistemskog statusa

Tokeni koji označavaju šire zajedničke ili fazne signale.

### 7.4. Diplomatic Tokens / Diplomatski tokeni

Tokeni koji označavaju formalne političke odnose, raskide ili contest status gdje je to korisno.

### 7.5. Endgame Tokens / Tokeni završnice

Tokeni koji signaliziraju završni pritisak, **Coronation Attempt/Pokušaj krunisanja** ili povezane contest statuse.

Kritično pravilo:

> svaki token mora imati jednu primarnu klasu čak i ako dodiruje više sistema.

---

## 8. Obavezna struktura jedne token specifikacije

Svaki token tip treba biti dokumentovan ovim redom:

1. **Naziv:** English/Srpski
2. **Klasa tokena**
3. **Primarna funkcija**
4. **Gdje stoji**
5. **Ko ga koristi**
6. **Kada ulazi i izlazi iz igre**
7. **Šta ne smije da zbuni**
8. **Ikonografska i label napomena**

Ova struktura pomaže da svi tokeni ostanu međusobno uporedivi i produkcijski čisti.

---

## 9. Map Tokens / Mapni tokeni

Ova grupa mora biti najstrože kontrolisana, jer glavna tabla već nosi mnogo informacija.

Mapni tokeni smiju postojati ako:

* označavaju važno prostorno stanje
* to stanje se mora vidjeti brzo i zajednički
* marker pomaže više nego što guši mapu

Mapni tokeni ne smiju:

* prekriti čitljivost provincija
* natjerati tablu da djeluje kao pretrpano skladište statusa
* duplirati informaciju koju jedinice ili postojeći marker već dovoljno jasno prikazuju

---

## 10. Control Token / Token kontrole

### 10.1. Primarna funkcija

Označava ko kontroliše ili drži relevantnu vlast nad teritorijom, čvorom ili važnim prostorom, ako to nije dovoljno jasno samo iz jedinica ili položaja.

### 10.2. Gdje stoji

Na glavnoj **Board/Tabli**, u ili uz odgovarajuću **Province/Provincija** zonu.

### 10.3. Dizajnerski cilj

Mora biti dovoljno jasan da se kontrola brzo čita, ali dovoljno nenametljiv da ne proguta mapni prostor.

### 10.4. Glavna opasnost

Ako je token prevelik ili previše dekorativan, može sakriti ono što treba da označi.

---

## 11. Contested Token / Token osporavanja

### 11.1. Primarna funkcija

Označava da je prostor, status ili završni ishod formalno **Contested/Osporeno**.

### 11.2. Gdje stoji

Najčešće na glavnoj tabli, ali može postojati i kao dio završnog ili coronation konteksta.

### 11.3. Dizajnerski cilj

Mora biti odmah vidljiv kao upozorenje na nestabilno ili sporno stanje.

### 11.4. Glavna opasnost

Ne smije biti vizuelno previše sličan markerima kontrole ili opštim status tokenima.

---

## 12. Stability Token / Token stabilnosti

### 12.1. Primarna funkcija

Označava trenutno stanje ili pomak na **Stability/Stabilnost** osi kada je fizički marker koristan za brzu ličnu ili javnu čitljivost.

### 12.2. Gdje stoji

Primarno na **Player Board/Tabli igrača**.

### 12.3. Dizajnerski cilj

Mora jasno podržavati ideju da stabilnost nije apstraktna brojka nego stanje države koje se prati i osjeća.

### 12.4. Glavna opasnost

Ne smije se miješati sa opštim resursnim tokenima ili ostalim ličnim markerima koji ne nose isti strateški značaj.

---

## 13. Unrest Token / Token nemira

### 13.1. Primarna funkcija

Označava prisustvo ili nivo **Unrest/Nemiri** pritiska gdje je potrebno jasno fizičko razlikovanje od stabilnosti.

### 13.2. Gdje stoji

Primarno na **Player Board/Tabli igrača**, a po potrebi u usko definisanim javnim kontekstima ako sistem to traži.

### 13.3. Dizajnerski cilj

Mora djelovati kao negativan ili alarmni signal, ali ne kroz konfuziju ili vizuelni šum.

### 13.4. Glavna opasnost

Ne smije biti toliko sličan **Stability Token/Token stabilnosti** da igrač na prvi pogled ne razlikuje šta raste, a šta pada.

---

## 14. Goods Marker vs Goods Token / Marker robe naspram tokena robe

Za **Goods/Roba** treba biti posebno oprezan.

Dobro pravilo je:

* ako goods stanje može biti bolje riješeno kroz track, slot ili kontrolisani marker sistem, ne treba uvoditi velik broj različitih goods tokena
* ako postoji goods token, mora jasno predstavljati razvojnu ili trgovačku vrijednost, ne samo “još jedan resurs komadić”

Glavna opasnost:

* goods lako skliznu u komponentni bloat ako svaka roba dobije poseban fizički komad bez dovoljnih benefita za gameplay čitljivost.

---

## 15. Treaty Status Token / Token statusa sporazuma

### 15.1. Primarna funkcija

Označava da formalni **Treaty/Sporazum** odnos postoji, aktivan je ili je u posebnom statusu koji treba javno vidjeti.

### 15.2. Gdje stoji

U političkom/treaty prostoru glavne table ili uz odgovarajuću treaty komponentu.

### 15.3. Dizajnerski cilj

Treba pomoći da formalna diplomatija bude javno čitljiva bez stvaranja spreadsheet utiska.

### 15.4. Glavna opasnost

Ne smije se pretvoriti u veliki mrežni sistem tokena koji guši političku preglednost i usporava partiju.

---

## 16. Betrayal or Broken Treaty Token / Token izdaje ili prekinutog sporazuma

Ovu vrstu tokena treba koristiti samo ako stvarno ubrzava čitanje posljedice raskida.

Ako se uvede, mora:

* imati jasan vremenski okvir
* imati jasan razlog postojanja
* ne miješati se sa opštim contested ili status tokenima

Ako ista stvar može biti jasnije riješena kroz treaty kartu ili kraći marker status, treba izbjeći novi token tip.

---

## 17. Coronation Token / Token krunisanja

### 17.1. Primarna funkcija

Označava da je **Coronation Attempt/Pokušaj krunisanja** aktivan, javan ili u contest režimu.

### 17.2. Gdje stoji

U završnoj / coronation zoni glavne table ili uz odgovarajuću završnu komponentu.

### 17.3. Dizajnerski cilj

Treba pojačati završni signal i fokus pažnje bez da od početka partije dominira stolom.

### 17.4. Glavna opasnost

Ne smije izgledati kao zaseban mini-game marker niti vizuelno pojesti mapu ili završni scoring pregled.

---

## 18. Event/Crisis Reminder Token / Token podsjetnika događaja ili krize

Ovaj token tip treba koristiti samo ako:

* stvarno smanjuje zaboravljanje važnog javnog efekta
* ne može biti jednako jasno riješen kroz samu kartu, rubnu zonu ili aid

Dobro pravilo:

* reminder tokeni su korisni samo za efekte koji se često zaboravljaju i imaju dovoljno jak gameplay uticaj
* ne treba praviti poseban token za svaki mali event ili crisis detalj

---

## 19. Token i board/player-board odnos

Svaki token mora imati jasno mjesto stanovanja.

Pravilo je:

* zajedničko i prostorno stanje = glavna **Board/Tabla**
* lično i često interno stanje = **Player Board/Tabla igrača**
* pomoćno i rijetko stanje = možda aid, karta ili uopšte bez posebnog tokena

Ako token nema jasno prirodno mjesto, često znači da nije dovoljno dobro opravdan.

---

## 20. Token i iconography odnos

Tokeni moraju biti usklađeni sa `components/iconography-spec.md`.

To znači:

* ako token koristi ikonu, ta ikona mora biti dosljedna ostatku sistema
* ikona na tokenu ne smije biti jedini nosilac značenja ako kontekst nije jasan
* token mora biti razlikoviv po obliku, funkciji ili poziciji, ne samo po nijansi boje

Ovo je posebno važno za prototip štampu i brzu stolnu čitljivost.

---

## 21. Token i terminology odnos

Svi tokeni moraju slijediti `components/terminology-and-labels.md`.

To znači:

* dosljedni nazivi
* nema paralelnih imena za isto stanje
* dvojezična logika tamo gdje je prikaz tekstualno relevantan

Ako token terminologija nije čista, komponentni sistem brzo postaje mutan.

---

## 22. Token shape and size / Oblik i veličina tokena

Tokeni treba da se razlikuju ne samo po grafici nego i po fizičkoj logici gdje je korisno.

To znači:

* najvažniji i najčešći tokeni mogu imati najjasniju siluetu
* status tokeni ne smiju biti svi isti mali kružići ako time nastaje konfuzija
* veličina mora odgovarati važnosti i prostoru na kojem token stoji

Prevelik token guši prostor.
Premalen token nestaje iz pažnje.

---

## 23. Token budget / Budžet tokena

CoS v2.7 mora imati strogu disciplinu broja token tipova.

Praktično pravilo:

* novi token tip se uvodi samo ako donosi stvarni UX ili rules benefit koji drugi komponentni alat ne daje dovoljno dobro

Treba izbjegavati:

* token tipove koji postoje samo za rijetke edge cases
* token tipove koji dupliraju postojeće markere
* token tipove koji uvode više setup i teardown rada nego što ubrzavaju partiju

---

## 24. Setup and teardown disciplina / Disciplina setupa i raspremanja

Svaki token tip treba procijeniti i po tome:

* koliko otežava setup
* koliko otežava raspremanje
* koliko traži sortiranja i traženja tokom partije

Ako token donosi malu čitljivost, a visok logistički trošak, vjerovatno ne treba da postoji.

---

## 25. Najčešće greške u token sistemu

* previše različitih status tokena za slična stanja
* goods tokeni koji djeluju kao dupli resursi
* mapni tokeni koji prekrivaju provincije
* stability/unrest markeri koji su previše slični
* diplomatski tokeni koji pretvaraju politički prostor u spreadsheet
* završni tokeni koji prerano dominiraju stolom

---

## 26. Workflow pravilo za novi token tip

Ako se predlaže novi **Token/Token** tip, treba provjeriti redom:

1. koje stanje ili vrijednost označava
2. da li je to stanje dovoljno važno i često
3. da li već postoji drugi način da se to bolje prikaže
4. gdje token fizički živi
5. da li povećava ili smanjuje čitljivost
6. da li povećava komponentni bloat, setup ili bookkeeping

Ako ne prolazi ova pitanja, novi token tip se ne uvodi.

---

## 27. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li token sistem ostaje ograničen i jasan?
2. da li novi token donosi stvarni gameplay benefit?
3. da li ostaje usklađen sa tablom, tablom igrača i aid logikom?
4. da li ostaje kompatibilan sa ikonografijom i terminologijom?
5. da li smanjuje ili povećava komponentni i logistički teret?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 28. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `systems/province-map-system.md`
* `systems/stability-and-unrest.md`
* `systems/diplomacy-and-treaties.md`
* `systems/coronation-system.md`
* `ux/information-hierarchy.md`
* `GLOSSARY.md`

---

## 29. Završna napomena

**Tokens Specification / Specifikacija tokena** mora ostati jedan od glavnih filtera protiv komponentnog i UX bloata u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* stanje partije se čita brzo
* tabla i tabla igrača ostaju uredne
* setup i teardown ostaju pod kontrolom
* sistemi dobijaju pravi fizički signal bez suvišne mase
* a grafički handoff dobija čist i disciplinovan token set

Ako radi loše:

* komponente se množe bez potrebe
* stol postaje vizuelno i logistički teži
* igra djeluje složenije nego što treba
* a važni signali se gube među markerima

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
