# matchup-matrix.md

# Crown of Sovereigns v2.7 — Matchup Matrix / Matrica susreta

## Status dokumenta

* **Dokument:** `playtests/matchup-matrix.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati standard za praćenje i analizu susreta između različitih **Win Paths/Putanja do pobjede**, player count modova i fokusiranih test scenarija
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Matchup/Susret**, **Win Path/Put do pobjede**, **Player Count/Broj igrača**
* **Povezani dokumenti:** `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `playtests/balance-watchlist.md`, `playtests/session-report-template.md`, `systems/win-paths.md`, `systems/scaling-2p-3p-4p.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uvede disciplinovan način praćenja kako različiti stilovi igre međusobno funkcionišu
* pomogne da se balans ne procjenjuje samo na osnovu ukupnog osjećaja partije
* omogući poređenje susreta kroz više sesija i različite brojeve igrača
* otkrije koji susreti djeluju zdravo, a koji proizvode sistemski problem
* da dodatnu strukturu fokusiranim balansnim i stres testovima

Ovo nije lista svih mogućih partija.
Ovo je radni alat za razumijevanje sudara stilova i sistema.

---

## 2. Zašto je matchup matrix kritična

Ukupan balans igre može djelovati dobar, a da određeni susreti ipak stalno proizvode problem.

Na primjer:

* **Aggro/Aggro** može izgledati zdravo ukupno, ali previše lako gaziti **Economic Path/Ekonomski put** u 2P
* **Diplomatic Path/Diplomatski put** može djelovati živ u 4P, ali slab u 3P
* **Balanced Path/Balansirani put** može izgledati korektno protiv jednog profila, ali preslabo protiv drugog

Bez matrice susreta, ovi obrasci se lako izgube u opštim playtest utiscima.

---

## 3. Osnovni princip dokumenta

Glavno pravilo glasi:

> balans treba posmatrati i kroz ukupnu sliku i kroz konkretne sudare stilova, jer igra često puca u odnosu između dva ili tri pristupa, a ne u apstraktnom prosjeku.

To znači da nije dovoljno samo pitati:

* “da li je igra balansirana?”

Treba pitati i:

* “kako se **Aggro/Aggro** ponaša protiv **Balanced Path/Balansirani put** u 3P?”
* “kako se **Diplomatic Path/Diplomatski put** ponaša kada je za stolom i jak goods profil?”
* “u kojim matchupovima završnica ostaje najzdravija?”

---

## 4. Šta matchup matrix jeste

Ovaj dokument treba da bude:

* pregled fokusa po susretima stilova
* alat za planiranje ciljnih test sesija
* pomoć pri čitanju balansnih patterna kroz vrijeme
* veza između session reportova i širih balansnih zaključaka

---

## 5. Šta matchup matrix nije

Ovaj dokument nije:

* zamjena za puni session report
* automatska presuda da je jedan stil “jači” samo na osnovu malog uzorka
* spreadsheet opsesija koja ignoriše kvalitet sesije i kontekst testera
* lista svakog mogućeg ljudskog ponašanja za stolom

Matrica mora pomagati prosudbi, a ne glumiti egzaktni dokaz gdje ga nema dovoljno.

---

## 6. Osnovne osi matrice

Matrica mora pratiti najmanje ove tri osi:

### 6.1. Win Path vs Win Path / Put do pobjede protiv puta do pobjede

Kako se različiti glavni stilovi sudaraju.

### 6.2. Player Count / Broj igrača

Kako se isti susret ponaša u 2P, 3P i 4P.

### 6.3. Session Type / Tip sesije

Da li je nalaz došao iz:

* normalne sesije
* fokusiranog stres testa
* onboarding grupe
* internog testa

Bez ove treće ose lako se miješaju podaci iz vrlo različitih testnih konteksta.

---

## 7. Glavni stilovi koji ulaze u matricu

Za v2.7 matrica mora najmanje koristiti ove glavne stilove:

* **Aggro/Aggro**
* **Balanced Path/Balansirani put**
* **Diplomatic Path/Diplomatski put**
* **Economic Path/Ekonomski put**
* **Opportunist/Oportunista**
* **Defender/Branilac**

Kritično pravilo:

* prva četiri su glavni nosioci **Win Path/Put do pobjede** logike
* posljednja dva su više ponašajni profili i treba ih koristiti pažljivo, kao dodatni sloj, ne kao zamjenu za glavne putanje

---

## 8. Osnovni format jedne matchup stavke

Svaki matchup zapis treba sadržati najmanje:

1. **ID susreta**
2. **Player count/Broj igrača**
3. **Stilovi u susretu**
4. **Broj relevantnih sesija**
5. **Dominantni pattern**
6. **Signal balansa**
7. **Confidence/Pouzdanost**
8. **Next test focus/Sljedeći test fokus**

Ovo mora biti dovoljno kratko da matrica ostane upotrebljiva, ali dovoljno konkretno da nešto znači.

---

## 9. Standard za ID oznake

Preporučeni format ID-a:

* `MU-2P-01`
* `MU-3P-02`
* `MU-4P-03`

Oznaka treba odmah da kaže:

* da je riječ o **Matchup/Susret** zapisu
* za koji player count važi
* koji je redni broj susreta u toj grupi

Po potrebi se u internim bilješkama može dodati i opisni tekst, ali osnovni ID treba ostati kratak i stalan.

---

## 10. Standard za “Signal balansa”

Preporučene oznake za signal balansa su:

* **Healthy/Zdravo**
* **Watch/Pratiti**
* **Strained/Napeto**
* **Problematic/Problematično**
* **Unclear/Nejasno**

### Kako koristiti

* **Healthy/Zdravo** = susret djeluje fer i daje prostor oboma ili svima relevantnim stilovima
* **Watch/Pratiti** = nema jasnog problema, ali postoje rani signali asimetrije
* **Strained/Napeto** = matchup još funkcioniše, ali se vidi da je pod pritiskom i može skliznuti
* **Problematic/Problematično** = susret stalno proizvodi loš ili previše jednosmjeran rezultat
* **Unclear/Nejasno** = nema dovoljno kvalitetnih sesija za zaključak

---

## 11. Standard za confidence / pouzdanost

Pouzdanost treba označiti kao:

* **Low/Niska**
* **Medium/Srednja**
* **High/Visoka**

### Pravilo korištenja

* **Low/Niska** kada ima malo sesija ili su sesije međusobno previše različite
* **Medium/Srednja** kada postoji više uporedivih sesija i pattern počinje da se nazire
* **High/Visoka** tek kada je susret viđen dovoljno puta, u dovoljno sličnim i upotrebljivim uslovima

Pouzdanost se odnosi na kvalitet nalaza, ne na jačinu mišljenja.

---

## 12. Početna obavezna matchup grupa — 2P

U 2P treba najmanje pratiti ove ključne susrete:

### 12.1.

**Aggro/Aggro** vs **Balanced Path/Balansirani put**

### 12.2.

**Aggro/Aggro** vs **Economic Path/Ekonomski put**

### 12.3.

**Balanced Path/Balansirani put** vs **Economic Path/Ekonomski put**

### 12.4.

**Aggro/Aggro** vs **Diplomatic Path/Diplomatski put**

Zašto su važni:

* 2P je najosjetljiviji na runaway i preranu dominaciju tempa
* ovdje se najbrže vidi da li goods i stabilnost zaista drže agresiju pod kontrolom

---

## 13. Početna obavezna matchup grupa — 3P

U 3P treba najmanje pratiti ove ključne susrete:

### 13.1.

**Aggro/Aggro** + **Balanced Path/Balansirani put** + **Diplomatic Path/Diplomatski put**

### 13.2.

**Aggro/Aggro** + **Economic Path/Ekonomski put** + **Balanced Path/Balansirani put**

### 13.3.

**Diplomatic Path/Diplomatski put** + **Economic Path/Ekonomski put** + **Balanced Path/Balansirani put**

### 13.4.

**Aggro/Aggro** + **Diplomatic Path/Diplomatski put** + **Economic Path/Ekonomski put**

Zašto su važni:

* 3P je vjerovatno najčistiji prozor za čitanje odnosa između glavnih stilova
* politički prostor postoji, ali nije još previše zasićen kao u nekim 4P partijama

---

## 14. Početna obavezna matchup grupa — 4P

U 4P treba najmanje pratiti ove ključne susrete:

### 14.1.

Prisustvo sva 4 glavna stila u istoj partiji

### 14.2.

Dva političko-ekonomska profila protiv dva agresivnije-prostorna profila

### 14.3.

Jedan izrazito diplomatski profil u stolu sa tri profila koji manje koriste treaty igru

### 14.4.

Partije u kojima **Balanced Path/Balansirani put** pokušava ostati u contentionu između jačeg političkog i jačeg vojnog pritiska

Zašto su važni:

* 4P je najbogatiji mod za diplomatiju, ali i najrizičniji za tempo i pregovaračko usporenje

---

## 15. Šta tačno treba posmatrati u matchupu

Za svaki susret treba pratiti najmanje:

* ko dobija inicijalni tempo
* ko dobija srednju partiju
* da li sporiji stil dobija realan comeback ili sazrijevanje prozor
* kada matchup prestaje biti otvoren
* da li završnica vraća contest ili samo potvrđuje ranijeg lidera
* da li stilovi izgledaju kao da igraju istu igru ili jedan gazi drugi bez pravog dijaloga

Ovo je važnije od samog konačnog pobjednika.

---

## 16. Matchup i Stability / Stabilnost

Svaki susret treba čitati i kroz pitanje:

* da li **Stability/Stabilnost** dovoljno utiče na odnos stilova?

Na primjer:

* ako **Aggro/Aggro** stalno dobija bez ozbiljne unutrašnje cijene, to nije samo matchup problem nego i stabilnost problem
* ako **Balanced Path/Balansirani put** i **Economic Path/Ekonomski put** nikad ne stignu do završnog leverage-a, možda je tempo ili stabilnost okvir pogrešno postavljen

Matrica susreta ne smije biti odvojena od sistemskih uzroka.

---

## 17. Matchup i Endgame / Završnica

Važno je pratiti i:

* koji susreti proizvode najbolju završnu tenziju
* koji susreti proizvode lažnu tenziju
* gdje **Coronation Attempt/Pokušaj krunisanja** djeluje snažno, a gdje ceremonialno
* gdje kasni pritisak realno vraća contest, a gdje samo pravi buku

Neki susreti mogu izgledati zdravo do 80% partije, a da se raspadnu baš u završnici.

---

## 18. Matchup i player skill / vještina igrača

Ovaj dokument mora paziti i na nivo testera.

Susret ne smije biti pogrešno tumačen ako je:

* jedan tester mnogo bolji od ostalih
* grupa potpuno nova
* fokus sesije bio na učenju, a ne na optimalnoj igri

Zato svaki matchup zapis mora imati kontekst kvaliteta sesija, ne samo ishod.

---

## 19. Matchup i session type / tip sesije

Važno je razlikovati:

* normalne sesije
* fokusirane stres testove
* onboarding sesije
* interne dizajnerske probe

Stres test može namjerno pojačati problem i zato je vrlo koristan, ali ne smije se tretirati kao obična “prirodna partija”.

Matrica mora čuvati tu razliku.

---

## 20. Veza sa hypothesis tracker dokumentom

Ako matchup obrazac stalno potvrđuje ili ruši neku tvrdnju, to treba prebaciti u:

* `playtests/hypothesis-tracker.md`

Primjeri:

* ako **Balanced Path/Balansirani put** u više 3P susreta redovno ulazi u završni contention, to podržava relevantnu hipotezu
* ako **Diplomatic Path/Diplomatski put** prečesto ostaje bez finishing power-a, to ide protiv odgovarajuće hipoteze

---

## 21. Veza sa balance watchlist dokumentom

Ako neki matchup stalno pokazuje isti problem, to mora hraniti:

* `playtests/balance-watchlist.md`

Primjeri:

* 2P **Aggro/Aggro** vs **Economic Path/Ekonomski put** redovno ide u runaway obrazac
* 4P politički matchup stalno usporava pregovaranje preko zdrave granice

Matchup matrix je jedan od najboljih izvora signala za watchlist.

---

## 22. Najčešće greške u radu sa matchup matricom

* previše brzo izvlačiti zaključak iz premalog uzorka
* tretirati svaki matchup kao da ima isti značaj za identitet igre
* zaboraviti player count kontekst
* ne razlikovati skill gap od sistemske prednosti
* pokušati napraviti matricu za previše sitnih kombinacija pa izgubiti fokus

---

## 23. Workflow pravilo za novi matchup unos

Kad se uvodi novi matchup zapis, treba provjeriti:

1. da li je susret dovoljno važan za v2.7 identitet i balans
2. da li već postoji sličan zapis koji treba dopuniti umjesto duplirati
3. da li ima dovoljno sesija ili mora ostati **Unclear/Nejasno**
4. da li je signal stvarno balansni ili je prvenstveno UX / onboarding artefakt
5. da li je sljedeći test fokus jasno definisan

Ako ne prolazi ova pitanja, zapis još nije spreman ili ga ne treba uvoditi.

---

## 24. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li matrica ostaje praktična za korištenje?
2. da li razlikuje kontekst sesije dovoljno jasno?
3. da li daje upotrebljiv signal, a ne lažnu preciznost?
4. da li pomaže balansu i hipotezama umjesto da ih duplira?
5. da li ostaje fokusirana na stvarno važne susrete?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`
* `playtests/session-report-template.md`
* `systems/win-paths.md`
* `systems/scaling-2p-3p-4p.md`
* `GLOSSARY.md`

---

## 26. Završna napomena

**Matchup Matrix / Matrica susreta** mora ostati jedan od najkorisnijih balansnih alata za čitanje zdravlja verzije **v2.7**.

Ako radi dobro:

* vidi se gdje susreti stilova zaista pucaju
* balans se prati konkretnije
* test sesije daju više uporedivih signala
* hipoteze i watchlist dobijaju jači dokazni trag
* a patch odluke postaju manje nasumične

Ako radi loše:

* sve se svodi na opšti utisak
* stvarni problematični susreti ostaju skriveni
* uzorak se pogrešno tumači kao dokaz
* a razvoj gubi jednu od najkorisnijih balansnih mapa

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
