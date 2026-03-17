# playtest-plan-v2.7.md

# Crown of Sovereigns v2.7 — Playtest Plan / Plan playtestiranja

## Status dokumenta

* **Dokument:** `playtests/playtest-plan-v2.7.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati metodologiju, prioritete, scenarije i način evidencije za testiranje igre **Crown of Sovereigns v2.7**
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Playtest/Playtest**, **Win Path/Put do pobjede**, **Stability/Stabilnost**
* **Povezani dokumenti:** `docs/version-status.md`, `gdd/canonical-decisions.md`, `rules/rules-reference-v2.7.md`, `systems/win-paths.md`, `systems/scaling-2p-3p-4p.md`, `systems/catch-up-and-runaway-control.md`, `systems/coronation-system.md`, `systems/ai-automa-solo.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* postavi jasan i ponovljiv okvir za testiranje **v2.7**
* odredi šta se testira prvo, šta kasnije i zašto
* spriječi da playtest razgovori ostanu na nivou utiska bez upotrebljivih zaključaka
* pomogne da se problemi razdvoje na: sistemske, UX, balansne i produkcijske
* omogući da svaka naredna revizija ima trag i logiku, a ne samo “osjećaj da je bolje”

Ovo nije dokument za opšte komentare o igri.
Ovo je operativni plan za metodičko testiranje.

---

## 2. Zašto je playtest plan kritičan

CoS v2.7 je igra sa više povezanih sistema:

* **Court/Dvor**
* mapa i **Provinces/Provincije**
* **Goods/Roba** i razvoj
* **Stability/Stabilnost** i **Unrest/Nemiri**
* **Diplomacy/Diplomatija** i **Treaty/Sporazum** logika
* **Combat/Borba**
* završni pritisak i **Coronation Attempt/Pokušaj krunisanja**

Bez strogog plana testiranja, feedback lako postane:

* previše opšti
* kontradiktoran
* fokusiran na simptome umjesto uzroke
* zavisan od najglasnijeg igrača umjesto od stvarnog sistema

Dobar plan testiranja čini da svaka partija daje upotrebljive podatke, a ne samo utiske.

---

## 3. Osnovni princip playtest metodologije

Glavno pravilo glasi:

> svaka playtest partija mora imati jasan cilj posmatranja, inače je njen rezultat previše mutan za ozbiljnu dizajnersku odluku.

To znači:

* ne testirati sve odjednom u svakoj partiji bez fokusa
* ne mijenjati previše stvari između partija bez jasne evidencije
* ne donositi veliku odluku samo zato što je jedna grupa “osjećala” nešto jako

Playtest mora biti dovoljno otvoren da otkrije neočekivano, ali dovoljno strukturisan da to možeš poslije razumjeti.

---

## 4. Šta ovaj plan jeste

Ovaj plan treba da bude:

* radni dokument za test serije
* filter za prioritete testiranja
* osnova za bilježenje nalaza
* alat za poređenje sesija i verzija

---

## 5. Šta ovaj plan nije

Ovaj plan nije:

* zamjena za GDD
* zamjena za rules dokument
* gotov zaključak da igra već radi
* improvizovana lista pitanja bez prioriteta
* birokratski formular koji guši prirodni tok testiranja

Ako plan postane pretežak za stvarnu upotrebu, biće ignorisan ili polovično korišten.

---

## 6. Glavni ciljevi testiranja v2.7

Playtest plan za **v2.7** mora provjeriti najmanje sljedeće ciljeve:

1. da li jezgro igre zaista radi kao **kingdom-management** iskustvo
2. da li su glavne **Win Paths/Putanje do pobjede** stvarno žive
3. da li **Stability/Stabilnost** zaista djeluje kao cijena moći
4. da li **Diplomatic Path/Diplomatski put** i dalje ima realan završni domet
5. da li **Aggro/Aggro** postoji, ali ne dominira
6. da li 2P, 3P i 4P ostaju zdravi u skladu sa ciljevima verzije
7. da li završnica i **Coronation Attempt/Pokušaj krunisanja** proizvode zaslužen wow bez nepoštenog swinga

Ako plan ne testira ovih sedam stvari, ne testira srce **v2.7**.

---

## 7. Redoslijed test prioriteta

Testiranje v2.7 ne treba raditi haotično. Preporučeni redoslijed prioriteta je:

### 7.1. Phase A — Core Functionality / Jezgrena funkcionalnost

Testira se:

* tok runde
* čitljivost glavnih sistema
* osnovna stabilnost pravila
* da li partija uopšte teče kako treba

### 7.2. Phase B — Balance and Win Paths / Balans i putanje do pobjede

Testira se:

* da li su **Aggro/Aggro**, **Balanced Path/Balansirani put**, **Diplomatic Path/Diplomatski put** i **Economic Path/Ekonomski put** stvarno živi
* da li neka putanja očigledno bježi ispred drugih

### 7.3. Phase C — Scaling and Session Health / Skaliranje i zdravlje partije

Testira se:

* 2P
* 3P
* 4P
* session length
* **downtime/usporenje**
* završna napetost

### 7.4. Phase D — UX and Production Readiness / UX i spremnost za produkciju

Testira se:

* onboarding
* aid kvalitet
* čitljivost komponenti
* potreba za dodatnim oznakama, layout promjenama ili terminološkim korekcijama

Ne treba preskakati jezgro i odmah donositi zaključke o finalnom balansu.

---

## 8. Obavezni tipovi playtest partija

Plan mora uključivati više vrsta partija.

### 8.1. Internal Designer Tests / Interni dizajnerski testovi

Za brzo otkrivanje očiglednih problema i proceduralnih kvarova.

### 8.2. Guided External Tests / Vođeni eksterni testovi

Testeri igraju uz prisutnog moderatora koji bilježi reakcije i pomaže samo gdje je nužno.

### 8.3. Blind-leaning Tests / Polu-slijepi testovi

Grupa dobija pravila i aid uz minimalnu pomoć, da se vidi koliko sistem i materijali zaista nose sami.

### 8.4. Focused Stress Tests / Fokusirani stres testovi

Namjerno se testiraju konkretni sistemi, npr.:

* jaka **Aggro/Aggro** linija
* goods-heavy partija
* treaty-heavy partija
* završni coronation contest

### 8.5. Solo/Automa Tests / Solo/Automa testovi

Samo za provjeru da li **Automa/Automa** radi kao koristan trening i solo pritisak, ne kao glavni fokus projekta.

---

## 9. Obavezni player-count test paket

Plan v2.7 mora sadržati najmanje ove player-count linije:

### 9.1. 2P testovi

Fokus:

* **Crown Pressure/Pritisak krune**
* runaway rizik
* da li rat previše dominira
* da li goods i stabilnost ostaju relevantni

### 9.2. 3P testovi

Fokus:

* politička čitljivost
* balans glavnih putanja
* lider exposure
* prirodna diplomatska tenzija

### 9.3. 4P testovi

Fokus:

* pregovarački tempo
* treaty smisao
* **downtime/usporenje**
* završna napetost i contest

Pošto je **3P/4P** ciljano najbolje iskustvo, tu mora biti najveći broj ozbiljnih testova.

---

## 10. Obavezne test hipoteze za v2.7

Plan mora formalno pratiti najmanje ove hipoteze:

### H1

**Balanced Path/Balansirani put** je stvarna, a ne samo teorijska putanja do pobjede.

### H2

**Diplomatic Path/Diplomatski put** može realno zatvoriti partiju bez oslanjanja samo na tuđe greške.

### H3

**Aggro/Aggro** je snažan, ali ga **Stability/Stabilnost** i contest dovoljno drže pod kontrolom.

### H4

Kasni pritisak i **Coronation Attempt/Pokušaj krunisanja** pojačavaju wow bez reset osjećaja.

### H5

2P ostaje napet i fer, bez prečestog runaway obrasca.

### H6

Aid i komponentni UX dovoljno nose tok runde bez previše lookup-a.

### H7

**Events/Događaji** i **Crises/Krize** mijenjaju prioritete, ali ne guše agency.

Ako ove hipoteze nisu praćene, testiranje neće dovoljno čuvati duh **v2.7**.

---

## 11. Šta se bilježi prije partije

Prije svake partije treba zapisati:

* datum
* verziju igre: **v2.7** ili precizniji patch ako postoji
* broj igrača
* vrstu testa
* ime ili oznaku grupe
* nivo iskustva testera
* specifičan fokus partije
* sve namjerne setup razlike ili eksperimente

Bez ovoga, poređenje partija brzo postaje nepouzdano.

---

## 12. Šta se bilježi tokom partije

Tokom partije treba pratiti najmanje:

* trajanje setupa
* trajanje teacha
* ukupno trajanje partije
* broj većih lookup momenata
* broj većih pravilaških zastoja
* koliko često se gubio tok runde
* kada je prvi put nastao osjećaj lidera
* kada je prvi put nastao osjećaj da partija možda više nije otvorena
* da li se i kada aktivirao **Coronation Attempt/Pokušaj krunisanja** ili sličan završni contest

Ne treba pisati roman tokom partije, ali mora ostati trag stvarnih problema u vremenu.

---

## 13. Šta se bilježi poslije partije

Poslije svake partije treba zapisati:

* ko je pobijedio
* koja je bila dominantna putanja pobjede
* da li su druge putanje djelovale žive ili mrtve
* koji je bio najveći izvor tenzije
* koji je bio najveći izvor frustracije
* da li je završnica bila otvorena, napeta, lažno napeta ili zatvorena
* da li je wow bio prisutan i da li je djelovao zasluženo
* da li bi igrači htjeli igrati ponovo i zašto

Ovo je važnije od opštih “sviđalo mi se / nije mi se svidjelo” komentara.

---

## 14. Obavezni kvantitativni indikatori

Plan treba pratiti najmanje ove brojeve ili procjene:

* **setup time/vrijeme setupa**
* **teach time/vrijeme objašnjavanja**
* **session length/dužina partije**
* **downtime/usporenje** po osjećaju i po zabilježenim zastojima
* broj rules lookup trenutaka
* broj ozbiljnih contest ili combat momenata
* broj aktivnih treaty odnosa tokom partije
* broj kriznih ili završnih obrta koji su stvarno promijenili odluke

Ovi brojevi nisu savršena istina, ali pomažu da se utisci usidre u nešto uporedivo.

---

## 15. Obavezni kvalitativni indikatori

Pored brojeva, plan mora pratiti i ove kvalitativne stvari:

* da li igra djeluje kao vođenje države ili kao samo nadmetanje mehanika
* da li su dvorske uloge osjećajne i čitljive
* da li je mapa stalno važna ili samo povremeno
* da li se goods osjećaju kao razvoj, a ne kao drugi resursi
* da li stabilnost djeluje kao stvarna cijena moći
* da li diplomatija djeluje formalno i relevantno
* da li završnica ima političku težinu

Ovi odgovori su često korisniji od čistog “zabavno / nezabavno”.

---

## 16. Posebni testovi za Win Paths / Putanje do pobjede

Plan mora imati i namjerne partije gdje se testeri podstiču da igraju određene stilove.

### Primjeri

* jedna partija sa namjerno jakim **Aggro/Aggro** pokušajem
* jedna partija sa goods-heavy **Economic Path/Ekonomski put** pristupom
* jedna partija sa treaty-heavy **Diplomatic Path/Diplomatski put** pristupom
* jedna partija sa disciplinovanim **Balanced Path/Balansirani put** fokusom

Ovo ne služi da se igra “na silu”, nego da se vidi da li sistem zaista podržava ono što tvrdi da podržava.

---

## 17. Posebni testovi za završnicu

Pošto je **v2.7** snažno fokusiran na završni pritisak, plan mora uključivati posebne testove koji ciljaju:

* kasne **Crises/Krize**
* contest za lidera
* **Coronation Attempt/Pokušaj krunisanja**
* osjećaj **Photo Finish/Fotofiniš** završnice
* razliku između zasluženog obrta i lažnog swinga

Ako završnica nije zasebno testirana, postoji rizik da cijela verzija djeluje dobro do posljednjih 20 minuta, a slabo baš tamo gdje treba da zablista.

---

## 18. Posebni testovi za onboarding i UX

Plan mora imati i sesije koje nisu fokusirane samo na balans, nego na:

* čitljivost aid-a
* terminologiju
* ikonografiju
* tok setupa
* mjesta gdje nova grupa zapinje

To znači da se mora posebno pratiti:

* šta su igrači pitali više puta
* koje su stvari miješali
* šta su previdjeli iako je bilo “na stolu”
* gdje su komponente slale pogrešan signal

Ovi nalazi često ne izgledaju glamurozno, ali su presudni za stvarni kvalitet proizvoda.

---

## 19. Pravilo jedne veće promjene po test ciklusu

Između ozbiljnih test serija ne treba uvoditi previše velikih promjena odjednom.

Dobro pravilo je:

* jedna velika promjena ili
* nekoliko usko povezanih malih promjena

Ako promijeniš pet velikih stvari odjednom, gotovo je nemoguće znati šta je zapravo poboljšalo ili pokvarilo igru.

---

## 20. Pravilo evidencije verzija

Svaka test serija mora biti vezana za tačnu verzionu oznaku.

To znači:

* **v2.7** kao osnovna baza
* a po potrebi i interni patch oznake, npr. **v2.7a**, **v2.7b**, ako se uvode precizne testne korekcije

Bez toga playtest feedback brzo počne miješati stare i nove verzije, što je posebno opasno kod ovog projekta.

---

## 21. Najčešće greške u playtest procesu

* testirati “sve” bez fokusa
* ne zapisivati dovoljno da se sesije mogu uporediti
* donositi velike zaključke iz jedne partije
* miješati UX problem i balans problem kao da su isto
* kriviti igrače za konfuziju koju zapravo stvara komponenta ili aid
* ignorisati završnicu jer je “većina partije djelovala dobro”
* ne testirati namjerno najrizičnije stilove igre

---

## 22. Workflow pravilo za playtest zaključke

Kad se poslije test serije izvuče zaključak, treba ga zapisati ovim redom:

1. **Problem/Problem**
2. **Evidence/Dokaz**
3. **Severity/Ozbiljnost**
4. **Likely Cause/Vjerovatni uzrok**
5. **Proposed Fix/Predloženi popravak**
6. **Next Test Focus/Sljedeći fokus testiranja**

To pomaže da razvoj ne sklizne u nejasne rasprave bez operativnog ishoda.

---

## 23. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li plan postaje praktičniji ili birokratskiji?
2. da li pomaže da se nalaz pretvori u odluku?
3. da li bolje odvaja balans, UX i sistemske probleme?
4. da li čuva fokus na stvarne rizike v2.7?
5. da li ostaje dovoljno jednostavan da se stvarno koristi za stolom?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 24. Veza sa grafičkom i produkcijskom pripremom

Playtest plan direktno utiče na:

* `ux/player-aid-system.md`
* `components/player-board-spec.md`
* `components/board-spec.md`
* `components/iconography-spec.md`
* `visuals/card-wireframe-notes.md`
* `visuals/board-wireframe-notes.md`

Ako testiranje ne bilježi dovoljno jasno šta igračima smeta na komponentama i toku, grafički tim će kasnije rješavati simptome umjesto uzroka.

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `docs/version-status.md`
* `gdd/canonical-decisions.md`
* `rules/rules-reference-v2.7.md`
* `systems/win-paths.md`
* `systems/scaling-2p-3p-4p.md`
* `systems/catch-up-and-runaway-control.md`
* `systems/coronation-system.md`
* `systems/ai-automa-solo.md`
* `GLOSSARY.md`

---

## 26. Završna napomena

**Playtest Plan / Plan playtestiranja** mora ostati jedan od glavnih razvojnih operativnih dokumenata za **Crown of Sovereigns v2.7**.

Ako radi dobro:

* problemi se vide ranije
* odluke postaju jasnije
* balans i UX se ne miješaju bez potrebe
* verzije ostaju čiste i uporedive
* a cijeli projekat napreduje mnogo sigurnije

Ako radi loše:

* playtest sesije daju previše buke, a premalo signala
* zaključci postaju subjektivni i nestabilni
* verzije se miješaju
* a razvoj ide sporije i skuplje nego što mora

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa jezgrom **v2.7**.
