# balance-watchlist.md

# Crown of Sovereigns v2.7 — Balance Watchlist / Lista balansnih rizika

## Status dokumenta

* **Dokument:** `playtests/balance-watchlist.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati prioritetnu listu balansnih rizika koje treba pratiti kroz playtest cikluse i patch iteracije
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Balance/Balans**, **Aggro/Aggro**, **Balanced Path/Balansirani put**
* **Povezani dokumenti:** `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `systems/win-paths.md`, `systems/scaling-2p-3p-4p.md`, `systems/catch-up-and-runaway-control.md`, `systems/coronation-system.md`, `systems/goods-and-development.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* odvoji najvažnije balansne rizike od opšteg playtest šuma
* pomogne da testiranje ostane fokusirano na stvarne konkurentske i sistemske slabosti
* spriječi da se balansne odluke donose na osnovu jedne glasne partije ili jednog upečatljivog momenta
* poveže konkretne rizike sa jasnim signalima koje treba tražiti u partiji
* omogući da svaka naredna iteracija zna šta je još uvijek rizično, šta je stabilizovano, a šta je eskaliralo

Ovo nije kompletan izvještaj o stanju balansa.
Ovo je operativna lista onoga što treba posebno nadzirati.

---

## 2. Zašto je balance watchlist kritičan

U kompleksnijim strateškim igrama balans vrlo rijetko puca samo na jednom mjestu.
Češće se dešava da:

* jedan stil igre dobije previše tempa
* drugi stil formalno postoji, ali nema stvarni finishing power
* 2P i 4P traže različite korektive
* završnica izgleda napeto, ali zapravo favorizuje isti profil igrača
* goods, diplomatija ili stabilnost djeluju važno, ali ne nose dovoljno stvarne vrijednosti

Bez **Balance Watchlist/ Liste balansnih rizika**, tim lako testira “opšti osjećaj igre” umjesto konkretnih slabih tačaka.

---

## 3. Osnovni princip dokumenta

Glavno pravilo glasi:

> balans ne treba pratiti kao apstraktnu ocjenu, nego kao skup konkretnih rizika koji imaju jasne simptome i jasne posljedice.

To znači da svaki balansni rizik mora imati:

* jasan opis
* razlog zašto je opasan
* signal kako se prepoznaje u partiji
* šta treba posmatrati dalje

Bez toga “balans” ostaje previše mutna riječ.

---

## 4. Šta balance watchlist jeste

Ovaj dokument treba da bude:

* fokus lista za playtest moderaciju
* alat za brzu identifikaciju prioriteta između sesija
* podsjetnik šta se ne smije izgubiti iz vida dok se igra polira
* veza između playtest nalaza i balansnih odluka

---

## 5. Šta balance watchlist nije

Ovaj dokument nije:

* zamjena za `playtests/hypothesis-tracker.md`
* konačna presuda da je nešto pokvareno
* lista svih mogućih sitnih nepravilnosti
* detaljan patch dokument

Ovdje treba držati ono što je dovoljno važno da zaslužuje stalnu pažnju.

---

## 6. Osnovne klase balansnih rizika

Sve stavke na watchlisti treba podijeliti najmanje na ove klase:

### 6.1. Win Path Risks / Rizici putanja do pobjede

Rizici da jedna putanja bude preslaba, prejaka ili lažno prisutna.

### 6.2. Tempo Risks / Rizici tempa

Rizici da jedan stil prebrzo zatvara partiju ili da drugi stil ne stiže da sazri.

### 6.3. Scaling Risks / Rizici skaliranja

Rizici vezani za 2P, 3P, 4P i solo/automa gdje različiti player count modovi guraju igru u različite probleme.

### 6.4. Endgame Risks / Rizici završnice

Rizici da kraj partije bude previše zatvoren, previše swingy ili nedovoljno pamtljiv.

### 6.5. System Value Risks / Rizici sistemske vrijednosti

Rizici da neki sistem djeluje važnije ili slabije nego što v2.7 identitet traži.

Kritično pravilo:

> svaka balansna stavka mora imati jednu glavnu klasu, iako može doticati više njih.

---

## 7. Obavezna struktura jedne watchlist stavke

Svaka stavka na watchlisti treba da bude zapisana ovim redom:

1. **ID**
2. **Naziv rizika**
3. **Klasa**
4. **Opis rizika**
5. **Zašto je važan**
6. **Signal u partiji**
7. **Šta pratiti**
8. **Trenutni status**
9. **Ozbiljnost**
10. **Sljedeći test fokus**

Ovaj format mora ostati isti kako bi watchlist ostala pregledna i uporediva kroz vrijeme.

---

## 8. Standard za ID oznake

Preporučeni format ID-a:

* `WP-01`, `WP-02` za **Win Path Risks**
* `TP-01`, `TP-02` za **Tempo Risks**
* `SC-01`, `SC-02` za **Scaling Risks**
* `EG-01`, `EG-02` za **Endgame Risks**
* `SV-01`, `SV-02` za **System Value Risks**

Ovo omogućava da se balansni rizici brzo povežu sa playtest bilješkama i kasnijim patch odlukama.

---

## 9. Standard za trenutni status

Svaka stavka mora imati jedan od sljedećih statusa:

### 9.1. **Watch/Pratiti**

Rizik postoji i treba ga pažljivo pratiti, ali još nema dovoljno signala da se tretira kao aktivni problem.

### 9.2. **Active/Aktivan**

Rizik se već pojavljuje dovoljno često ili dovoljno snažno da zahtijeva prioritetno praćenje.

### 9.3. **Escalated/Eskaliran**

Rizik je ozbiljan i vjerovatno traži dizajnerski ili UX odgovor u narednom patch ciklusu.

### 9.4. **Stabilizing/Stabilizuje se**

Postoje signali da problem slabi, ali još nije dovoljno sigurno da se skine sa liste.

### 9.5. **Closed/Zatvoren**

Trenutno nema dovoljno razloga da ostane na aktivnoj watchlisti za ovu verziju ili patch liniju.

---

## 10. Standard za ozbiljnost

Ozbiljnost treba označiti kao:

* **Low/Niska**
* **Medium/Srednja**
* **High/Visoka**
* **Critical/Kritična**

### Kako koristiti

* **Low/Niska** = pratiti, ali nije prioritetna opasnost
* **Medium/Srednja** = može narasti u ozbiljan problem ako se ponavlja
* **High/Visoka** = već osjetno narušava kvalitet partije ili identitet sistema
* **Critical/Kritična** = direktno prijeti identitetu, završnici ili zdravlju jedne ili više ključnih player-count linija

---

## 11. Početna obavezna watchlist stavka — Aggro dominance

### ID

`WP-01`

### Naziv rizika

**Aggro/Aggro** postaje najočigledniji i najsigurniji put do pobjede.

### Zašto je važan

Ako ovaj rizik eskalira:

* **Balanced Path/Balansirani put** slabi
* **Diplomatic Path/Diplomatski put** djeluje ornamentalno
* goods razvoj postaje prespor ili sekundaran
* mapa ostaje važna, ali igra gubi širinu

### Signal u partiji

* agresivni igrač prečesto dobija najbolji tempo i završni leverage
* drugi stilovi igraju reaktivno umjesto proaktivno
* **Stability/Stabilnost** ne kažnjava dovoljno pregrijanu ekspanziju

### Šta pratiti

* pobjednički procenat aggro stilova
* vrijeme kada agresor prvi put “zaključa” osjećaj vodstva
* koliko često goods ili diplomatija realno contestuju agresora

---

## 12. Početna obavezna watchlist stavka — Balanced path weakness

### ID

`WP-02`

### Naziv rizika

**Balanced Path/Balansirani put** ostaje ispravan, ali ne dovoljno pobjednički.

### Zašto je važan

Ovo direktno pogađa srce CoS fantazije: vođenje države, a ne samo forsiranje jedne uske mašine.

### Signal u partiji

* balansirani igrač djeluje pametno, ali rijetko zatvara partiju
* završni scoring i pritisak više nagrađuju oštriji specijalizovani stil
* balansirani pristup prečesto ostaje “drugo mjesto” strategija

### Šta pratiti

* koliko često **Balanced Path/Balansirani put** ulazi u realnu završnu borbu
* da li igrači koji vode “zdravu državu” ipak gube od jednostavnijeg tempa
* da li stabilnost i višestruka efikasnost dobijaju stvarnu završnu težinu

---

## 13. Početna obavezna watchlist stavka — Diplomatic path softness

### ID

`WP-03`

### Naziv rizika

**Diplomatic Path/Diplomatski put** izgleda zanimljivo, ali nema dovoljno finishing power.

### Zašto je važan

Ako diplomatija ne može zatvoriti partiju, jedan od glavnih diferencijatora igre postaje slabiji nego što v2.7 traži.

### Signal u partiji

* treaty igra daje osjećaj uticaja, ali ne i dovoljno stvarnog score / leverage završnog efekta
* diplomatski igrač previše zavisi od tuđih grešaka
* završni contest ne pretvara političku prednost u stvarnu prijetnju pobjedi

### Šta pratiti

* koliko često treaty-heavy igra ulazi u top contention
* da li politički leverage utiče na finalni poredak ili samo usporava druge
* da li se igrači osjećaju kao da diplomatija “vodi” ili samo “pravi buku”

---

## 14. Početna obavezna watchlist stavka — Economic isolation

### ID

`WP-04`

### Naziv rizika

**Economic Path/Ekonomski put** djeluje odvojeno od mape i politike.

### Zašto je važan

Goods sistem treba da bude razvojni stub kraljevstva, ne privatni spreadsheet.

### Signal u partiji

* goods-heavy igra može ignorisati mapu predugo bez realne cijene
* ili suprotno: goods igra nikad ne stigne do relevantnosti jer je prostor i rat pregaze prije nego sazri

### Šta pratiti

* koliko goods utiču na srednji i kasni game leverage
* da li goods razvoj stvara političku ili teritorijalnu težinu
* da li ekonomija ostaje u kontaktu sa ostatkom sistema

---

## 15. Početna obavezna watchlist stavka — Stability underweight

### ID

`SV-01`

### Naziv rizika

**Stability/Stabilnost** djeluje važno na papiru, ali preslabo u stvarnoj partiji.

### Zašto je važan

Ako stabilnost nije stvarna cijena moći, CoS gubi jedan od glavnih identitetskih stubova.

### Signal u partiji

* igrači previše guraju širenje i rat bez ozbiljne posljedice
* stabilnost se prati formalno, ali rijetko mijenja odluku
* završnica ne razlikuje dovoljno održivu od prenapregnute države

### Šta pratiti

* koliko često stabilnost promijeni tok partije
* koliko puta igrači svjesno odustanu od poteza zbog stabilnosti rizika
* koliko često nestabilna država ipak prelagano pobijedi

---

## 16. Početna obavezna watchlist stavka — Stability overweight

### ID

`SV-02`

### Naziv rizika

**Stability/Stabilnost** postaje previše kaznena i guši ambiciju.

### Zašto je važan

Prejaka stabilnost logika može ubiti zamah, agresiju i uzbudljiv rizik.

### Signal u partiji

* igrači previše igraju sigurno
* agresivniji ili rizičniji potezi djeluju kao greška i prije nego ih probaš
* partija djeluje administrativnije i opreznije nego što treba

### Šta pratiti

* koliko često igrači odustaju od jakih poteza jer stabilnost djeluje “previše skupo”
* da li se sredina partije usporava zbog pretjeranog opreza
* da li wow momenti slabe jer niko ne želi gurnuti sistem do ruba

---

## 17. Početna obavezna watchlist stavka — 2P runaway fragility

### ID

`SC-01`

### Naziv rizika

2P partija previše lako sklizne u runaway duel.

### Zašto je važan

Iako je 3P/4P glavni fokus, v2.7 eksplicitno želi ozbiljno podržan 2P mod.

### Signal u partiji

* jedan rani proboj ili goods lead prerano odluči partiju
* **Crown Pressure/Pritisak krune** nije dovoljan ili djeluje previše slab
* comeback prozor u 2P ostaje premalen

### Šta pratiti

* koliko često 2P partija djeluje zatvoreno prije završnice
* koliko **Crown Pressure/Pritisak krune** stvarno contestuje lidera
* koliko goods, stabilnost i završni pritisak ostaju relevantni u 2P

---

## 18. Početna obavezna watchlist stavka — 4P negotiation drag

### ID

`SC-02`

### Naziv rizika

4P diplomatija i pregovaranje previše usporavaju partiju.

### Zašto je važan

4P treba biti najbogatiji mod, ali ne smije postati pregovarački mulj.

### Signal u partiji

* previše vremena odlazi na treaty razgovore
* akcioni tempo pada zbog političkog drifta
* igrači čekaju duže nego što je uzbudljivo

### Šta pratiti

* broj većih pregovaračkih zastoja
* ukupni osjećaj **downtimea/usporenja** u 4P
* da li formalna diplomatija pomaže ili ne pomaže da se razgovor zadrži pod kontrolom

---

## 19. Početna obavezna watchlist stavka — Endgame fake tension

### ID

`EG-01`

### Naziv rizika

Završnica djeluje napeto, ali je realno već zatvorena.

### Zašto je važan

Lažna tenzija je jedan od najgorih tipova završnice: izgleda dobro, ali ne daje stvarnu agenciju.

### Signal u partiji

* svi pričaju kao da je otvoreno, ali lider je realno van dometa
* završni contest samo malo mijenja razliku, ali ne i stvarnu borbu za pobjedu
* **Coronation Attempt/Pokušaj krunisanja** djeluje više ceremonialno nego rizično

### Šta pratiti

* kada se zapravo zna pobjednik naspram kada to sto misli da zna
* koliko završni contest realno mijenja odluke
* koliko često završnica stvara stvaran **Photo Finish/Fotofiniš** osjećaj

---

## 20. Početna obavezna watchlist stavka — Endgame swing excess

### ID

`EG-02`

### Naziv rizika

Završni pritisak i coronation uvode prevelik swing koji briše raniju igru.

### Zašto je važan

V2.7 želi wow, ali ne na račun zasluženosti.

### Signal u partiji

* vodeći igrač djeluje pošteno kažnjen više nego contestovan
* završni obrt izgleda kao reset umjesto kulminacije
* igrači osjećaju da prethodnih 90 minuta nije imalo dovoljnu težinu

### Šta pratiti

* tester reakciju na završni obrt
* razliku između “ovo je bilo brutalno ali pošteno” i “ovo je bilo previše”
* koliko coronation ili kasna kriza realno brišu prethodnu prednost

---

## 21. Početna obavezna watchlist stavka — System value mismatch

### ID

`SV-03`

### Naziv rizika

Neki sistem djeluje važnije u dokumentaciji nego u stvarnom gameplayu.

### Zašto je važan

To je čest simptom da igra ima dobar narativ o sebi, ali ne i stvarnu mehaničku potvrdu tog narativa.

### Signal u partiji

* igrači rijetko koriste ili ozbiljno cijene sistem koji bi trebao biti centralan
* sistem se spominje u teachu, ali ne mijenja mnogo odluka
* tester feedback pokazuje da ljudi razumiju da “treba biti važno”, ali to ne osjećaju za stolom

### Šta pratiti

* **Court/Dvor** važnost
* **Goods/Roba** kao razvoj
* **Stability/Stabilnost** kao cijena moći
* diplomatiju kao realan put, ne ukras
* coronation kao završni vrhunac, ne proceduralni dodatak

---

## 22. Kako se watchlist koristi poslije svake sesije

Poslije svake relevantne partije ili test serije treba uraditi:

1. označiti koje stavke su sesijom stvarno dotaknute
2. dodati signal “za” ili “protiv” rizika
3. po potrebi promijeniti status i ozbiljnost
4. zapisati da li rizik prelazi u patch prioritet
5. povezati nalaz sa `playtests/hypothesis-tracker.md` ako se radi o istoj temi

Ne treba mijenjati cijelu watchlistu poslije svake partije. Samo ono što je sesija stvarno osvijetlila.

---

## 23. Pravilo protiv overreaction reakcije

Jedna jaka partija ne smije automatski prebaciti rizik u **Critical/Kritična** ili **Closed/Zatvorena** stanja.

Treba gledati:

* pattern
* ponavljanje
* različite grupe
* različite player count modove

Balans posebno traži otpornost na impulsivne zaključke.

---

## 24. Veza sa hypothesis tracker dokumentom

`playtests/hypothesis-tracker.md` prati da li su tvrdnje o igri tačne.

`playtests/balance-watchlist.md` prati gdje su balansne pukotine najvjerovatnije i najopasnije.

Jedan dokument pita:

* “da li ovo radi?”

Drugi pita:

* “gdje bi to prvo moglo prestati da radi?”

Oni moraju stalno biti usklađeni.

---

## 25. Najčešće greške u radu sa balance watchlistom

* stavljati previše sitnih problema na listu pa izgubi fokus
* tretirati watchlist kao dokaz da problem već postoji umjesto da je to lista rizika
* ne razlikovati UX konfuziju od stvarne balansne pukotine
* skidati stavku sa liste prerano jer je jedna grupa “nije osjetila”
* držati stavku predugo aktivnom iako je sistem već stabilizovan

---

## 26. Workflow pravilo za novu watchlist stavku

Ako se uvodi nova balansna stavka, mora se provjeriti redom:

1. da li rizik direktno dotiče važan identitetski ili takmičarski kvalitet v2.7
2. da li ima jasan signal u partiji
3. da li se razlikuje od postojeće stavke dovoljno da opravda novi unos
4. da li postoji jasan način da se prati kroz više sesija
5. da li je to stvarno balansni problem, a ne rules ili UX problem

Ako ne prolazi ova pitanja, stavka se ne uvodi ili ide u drugi dokument.

---

## 27. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li lista ostaje fokusirana?
2. da li prioriteti ostaju jasni?
3. da li pomaže konkretnim playtest odlukama?
4. da li razlikuje rizik od dokazane greške?
5. da li ostaje kompatibilna sa ostatkom playtest dokumentacije?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 28. Veza sa grafičkim i UX slojem

Iako je ovo balansni dokument, mnoge stavke će indirektno pokazati da problem možda nije čist balans nego:

* aid slabost
* loša terminologija
* preslaba čitljivost table ili player board-a
* loša signalizacija završnice

Zato watchlist mora stalno biti čitana zajedno sa:

* `ux/player-aid-system.md`
* `components/player-board-spec.md`
* `components/board-spec.md`
* `components/iconography-spec.md`

---

## 29. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `systems/win-paths.md`
* `systems/scaling-2p-3p-4p.md`
* `systems/catch-up-and-runaway-control.md`
* `systems/coronation-system.md`
* `systems/goods-and-development.md`
* `GLOSSARY.md`

---

## 30. Završna napomena

**Balance Watchlist / Lista balansnih rizika** mora ostati jedan od glavnih radnih filtera za testiranje i patch odluke u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* znaš gdje da gledaš
* znaš šta je stvarni rizik
* znaš šta još nije sigurno
* playtest sesije daju više signala, a manje buke
* a patch odluke postaju čišće i manje impulsivne

Ako radi loše:

* balans se prati previše opšto
* važni rizici se izgube u utiscima
* reakcije postaju prebrze ili prekasne
* a razvoj gubi fokus baš tamo gdje mora biti najprecizniji

Zato ovaj dokument mora ostati strog, fokusiran i stalno usklađen sa jezgrom **v2.7**.
