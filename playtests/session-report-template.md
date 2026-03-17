# session-report-template.md

# Crown of Sovereigns v2.7 — Session Report Template / Šablon izvještaja sa sesije

## Status dokumenta

* **Dokument:** `playtests/session-report-template.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati standardni šablon za bilježenje rezultata jedne playtest sesije na način koji je brz za popunjavanje i koristan za kasniju analizu
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Session Report/Izvještaj sa sesije**, **Playtest/Playtest**, **Evidence/Dokaz**
* **Povezani dokumenti:** `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `playtests/balance-watchlist.md`, `docs/revision-workflow.md`, `docs/document-status-policy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* standardizuje kako se bilježi jedna playtest sesija
* spriječi da važni signali ostanu samo u sjećanju ili usmenom prepričavanju
* omogući poređenje više sesija bez improvizovanog formata
* olakša pretvaranje playtest iskustva u konkretne dizajnerske odluke
* smanji razliku između “zanimljiv utisak” i “upotrebljiv nalaz”

Ovo nije analiza sesije.
Ovo je šablon koji omogućava da analiza poslije bude moguća i pouzdana.

---

## 2. Zašto je session report template kritičan

Bez dosljednog šablona brzo nastaju problemi:

* jedna sesija ima previše detalja, druga skoro ništa
* neki moderatori pišu o emociji, drugi samo o rezultatu
* podaci o vremenu, player countu i verziji se zaborave
* balansni i UX problemi se miješaju u jednu mutnu priču
* kasnije je teško uporediti sesije ili dokazati pattern

Dobar šablon ne služi da testiranje izgleda formalno.
On služi da se signal ne izgubi u buci.

---

## 3. Osnovni princip šablona

Glavno pravilo glasi:

> izvještaj mora biti dovoljno kratak da se stvarno popuni, ali dovoljno precizan da kasnije vrijedi više od samog sjećanja.

To znači:

* ne uvoditi previše polja koja niko neće ispunjavati dosljedno
* ne ostaviti samo prazno mjesto za “utiske” bez strukture
* koristiti isti redoslijed i istu logiku iz sesije u sesiju

Ako je šablon predug, ljudi ga neće koristiti.
Ako je prekratak, neće davati dovoljno materijala za odluke.

---

## 4. Šta ovaj šablon jeste

Ovaj šablon treba da bude:

* standardna forma za jednu sesiju
* radni alat moderatora ili dizajnera
* veza između sirovog iskustva i kasnijeg **Hypothesis/Hipoteza** i **Balance/Balans** rada
* dokument koji se može popuniti odmah poslije partije ili tokom nje uz kratke bilješke

---

## 5. Šta ovaj šablon nije

Ovaj šablon nije:

* dugi narativni playtest esej
* zamjena za poseban balansni izvještaj
* zamjena za `playtests/hypothesis-tracker.md`
* formular za svaku sitnu emociju i svaki sitni potez u partiji

Ovdje se bilježi ono što je dovoljno važno da utiče na dalji razvoj.

---

## 6. Obavezna struktura izvještaja

Svaki **Session Report/Izvještaj sa sesije** treba da sadrži najmanje ove glavne blokove:

1. **Session Metadata/Metapodaci sesije**
2. **Setup and Teach/Setup i objašnjavanje**
3. **Session Flow/Tok sesije**
4. **Result and Win Path/Rezultat i put do pobjede**
5. **Key Findings/Ključni nalazi**
6. **Hypotheses Touched/Hipoteze koje je sesija dotakla**
7. **Balance Watchlist Signals/Signali za balansnu listu rizika**
8. **Actionable Next Steps/Primjenjivi sljedeći koraci**

Ovaj redoslijed treba ostati isti da bi izvještaji bili uporedivi.

---

## 7. Session Metadata / Metapodaci sesije

Ovaj blok mora sadržati najmanje:

* datum sesije
* oznaku sesije ili interni ID
* aktivnu verziju igre, npr. **v2.7** ili patch oznaku
* broj igrača
* vrstu testa
* moderatora ili osobu koja vodi bilješke
* iskustvo grupe sa igrom
* fokus sesije

### Primjeri vrste testa

* **Internal Designer Test/Interni dizajnerski test**
* **Guided External Test/Vođeni eksterni test**
* **Blind-leaning Test/Polu-slijepi test**
* **Focused Stress Test/Fokusirani stres test**
* **Solo/Automa Test/Solo/Automa test**

Bez dobrih metapodataka, izvještaj gubi dio vrijednosti već na početku.

---

## 8. Setup and Teach / Setup i objašnjavanje

Ovaj blok treba kratko zabilježiti:

* vrijeme setupa
* vrijeme teacha
* najveća mjesta konfuzije tokom setupa
* najveća mjesta konfuzije tokom objašnjavanja
* da li je **First Game Mode/Mod prve partije** korišten ili ne

Ovo je važno jer se mnogi problemi pripisuju sistemu, a zapravo dolaze iz:

* lošeg onboarding signala
* nejasnog setup redoslijeda
* aid ili komponentne nečitljivosti

---

## 9. Session Flow / Tok sesije

Ovaj blok treba sažeto zabilježiti kako je partija tekla.

Treba navesti:

* da li je tok bio gladak ili isprekidan
* gdje su nastali najveći zastoji
* kada se pojavio prvi osjećaj lidera
* kada je partija počela djelovati otvoreno ili zatvoreno
* da li je **downtime/usporenje** bio nizak, srednji ili visok

Ne treba ovdje pisati cijeli narativ potez po potez.
Treba zapisati samo najvažnije signale o ritmu partije.

---

## 10. Result and Win Path / Rezultat i put do pobjede

Ovaj blok mora sadržati:

* pobjednika
* poredak ako je relevantan
* dominantnu **Win Path/Put do pobjede** pobjednika
* koji su drugi stilovi bili u contentionu
* da li je završnica bila otvorena, napeta, lažno napeta ili zatvorena
* da li se aktivirao **Coronation Attempt/Pokušaj krunisanja** ili sličan završni contest

Ovaj blok je posebno važan za povezivanje sesije sa balansnim praćenjem.

---

## 11. Key Findings / Ključni nalazi

Ovo je najvažniji kvalitativni blok izvještaja.

Treba ga podijeliti najmanje na:

### 11.1. Šta je radilo dobro

Kratko zapisati 2–5 stvari koje su stvarno radile.

### 11.2. Šta nije radilo dobro

Kratko zapisati 2–5 najvažnijih problema.

### 11.3. Najveći izvor tenzije

Jedna ili dvije rečenice.

### 11.4. Najveći izvor frustracije

Jedna ili dvije rečenice.

### 11.5. Najjači wow moment

Ako ga je bilo, zapisati da li je djelovao zasluženo.

Ovaj blok treba biti kratak, ali ne smije ostati na nivou “bilo je zabavno / nije bilo zabavno”.

---

## 12. Hypotheses Touched / Hipoteze koje je sesija dotakla

Ovaj blok treba povezati sesiju sa `playtests/hypothesis-tracker.md`.

Za svaku relevantnu hipotezu treba zapisati:

* ID hipoteze
* da li je sesija dala signal **for/za**, **against/protiv** ili **unclear/nejasno**
* kratku napomenu zašto

Primjeri:

* `BL-01` — **for/za** — **Balanced Path/Balansirani put** ušao u stvarnu završnu borbu u 3P.
* `EG-02` — **against/protiv** — **Coronation Attempt/Pokušaj krunisanja** djelovao previše ceremonialno, bez realnog contest pritiska.

Ovaj blok je važan da sesija odmah ima trag u sistemu hipoteza.

---

## 13. Balance Watchlist Signals / Signali za balansnu listu rizika

Ovaj blok povezuje sesiju sa `playtests/balance-watchlist.md`.

Za svaku relevantnu stavku treba zapisati:

* ID watchlist stavke
* da li je sesija pokazala **signal present/signal prisutan**, **signal absent/signal odsutan** ili **unclear/nejasno**
* kratku napomenu

Primjeri:

* `WP-01` — **signal present/signal prisutan** — **Aggro/Aggro** rano stekao tempo koji drugi nisu mogli ozbiljno contestovati.
* `SC-02` — **unclear/nejasno** — 4P je bio spor, ali grupa je bila nova pa treba još sesija.

---

## 14. Actionable Next Steps / Primjenjivi sljedeći koraci

Ovaj blok mora biti posebno konkretan.

Treba zapisati:

* 1–3 najvažnija prijedloga za sljedeći test ili reviziju
* da li je potreban systems fix, UX fix, wording fix ili dodatna provjera bez odmah uvedene promjene
* šta je sljedeći preporučeni fokus naredne sesije

Loš primjer:

* “Treba još raditi na balansu.”

Dobar primjer:

* “U narednoj 3P sesiji namjerno testirati **Diplomatic Path/Diplomatski put** sa fokusom na treaty leverage i završni contest.”

---

## 15. Preporučeni mini-format za brzo popunjavanje

Ako se izvještaj popunjava odmah poslije sesije, preporučeni kratki format po bloku je:

* 1–3 reda po podsekciji
* maksimalno konkretno
* bez nepotrebne proze

Kasnije se iz više kratkih izvještaja može mnogo lakše izvući pattern nego iz nekoliko predugih i neujednačenih eseja.

---

## 16. Obavezne oznake za ton zaključka

Da bi izvještaj bio precizniji, preporučuje se korištenje kratkih oznaka kada je korisno:

* **clear/jasno**
* **likely/vjerovatno**
* **unclear/nejasno**
* **needs retest/traži ponovno testiranje**

Ove oznake pomažu da se sesija ne pretvara u lažno čvrst zaključak kada dokaz nije dovoljno jak.

---

## 17. Pravilo protiv post-session romantizacije

Poslije dobre ili loše partije lako je preuveličati ono što se desilo.

Zato izvještaj mora:

* razlikovati jak utisak od ponovljivog signala
* zapisati šta se stvarno vidjelo, ne samo šta se osjetilo
* ostaviti prostor za to da je nalaz možda specifičan za tu grupu ili taj matchup

Ovo je posebno važno za:

* wow momente
* agresivne obrte
* završne contest situacije

---

## 18. Pravilo protiv previše narativa

Narativ partije je koristan samo ako pomaže dijagnozi.

Ne treba zapisivati:

* svaki zanimljiv trenutak
* cijelu priču partije ako ne nosi signal
* duge opise socijalne dinamike koji ne utiču na sistemski zaključak

Ako narativ ne pomaže dijagnozi, treba ga skratiti.

---

## 19. Veza sa playtest-plan dokumentom

`playtests/playtest-plan-v2.7.md` kaže:

* šta i zašto testiramo

`playtests/session-report-template.md` kaže:

* kako zapisujemo rezultat jedne konkretne sesije

Jedan dokument vodi test seriju.
Drugi dokument hvata trag svake partije.

---

## 20. Veza sa hypothesis tracker i balance watchlist dokumentima

Dobar session report mora prirodno hraniti oba dokumenta:

* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`

Ako izvještaj ne daje materijal za ove dvije liste, vjerovatno je previše opšti ili previše narativan.

---

## 21. Veza sa revision workflow dokumentom

Kada više session reportova pokaže isti problem ili isti signal, to može biti okidač za:

* **Proposal/Prijedlog** revizije
* patch test
* ili promjenu statusa određene hipoteze ili balansnog rizika

Zato ovaj šablon mora biti dovoljno jasan da kasniji revizioni workflow ima na čemu da stoji.

---

## 22. Najčešće greške u session report pisanju

* zaboraviti metapodatke sesije
* pisati previše opštih utisaka
* ne zapisati dominantni **Win Path/Put do pobjede**
* ne razlikovati UX problem od balansnog problema
* ne povezati sesiju sa hipotezama i watchlist stavkama
* ne zapisati konkretan sljedeći korak

---

## 23. Workflow pravilo za korištenje ovog šablona

Nakon svake ozbiljne sesije preporučeni redoslijed je:

1. popuniti metapodatke odmah
2. tokom ili odmah nakon partije zabilježiti tok i rezultat
3. zatim dopuniti ključne nalaze
4. povezati nalaze sa hipotezama i watchlist stavkama
5. završiti sa 1–3 konkretna sljedeća koraka

Ako se izvještaj odgađa predugo, kvalitet sjećanja i preciznost naglo padaju.

---

## 24. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li šablon postaje praktičniji ili teži za popunjavanje?
2. da li daje više signala ili više buke?
3. da li olakšava povezivanje sa hipotezama i balansnim rizicima?
4. da li ostaje dovoljno kratak za stvarnu upotrebu?
5. da li smanjuje ili povećava post-session konfuziju?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`
* `docs/revision-workflow.md`
* `docs/document-status-policy.md`
* `GLOSSARY.md`

---

## 26. Završna napomena

**Session Report Template / Šablon izvještaja sa sesije** mora ostati jedan od najpraktičnijih playtest dokumenata u cijelom projektu.

Ako radi dobro:

* svaka partija ostavlja jasan trag
* lakše je uporediti sesije
* lakše je prepoznati pattern
* hipoteze i balansna lista dobijaju stvarni materijal
* a revizije postaju manje improvizovane

Ako radi loše:

* signal se gubi
* nalazi ostaju u glavi umjesto u repozitorijumu
* različiti testovi se ne mogu uporediti
* a razvoj postaje sporiji i manje siguran nego što mora biti

Zato ovaj dokument mora ostati kratak, strog i potpuno usklađen sa logikom **v2.7**.
