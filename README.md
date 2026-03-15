# README.md

# Crown of Sovereigns

## Status repozitorija

* **Aktivna verzija igre:** **Crown of Sovereigns v2.7**
* **Status verzije:** jedina kanonska i relevantna osnova za dalji razvoj
* **Prethodne verzije:** v2.6.1 i starije su arhiva
* **Vrsta projekta:** strateška kompetitivna board game igra upravljanja kraljevstvom

---

## 1. Šta je Crown of Sovereigns

**Crown of Sovereigns** je kompetitivna strateška društvena igra u kojoj igrači vode srednjovjekovne države i pokušavaju da izgrade najstabilniju, najuticajniju i najuspješniju krunu.

Igra je smještena u istorijski inspirisan okvir Evrope oko 1350. godine, ali nije istorijska simulacija u uskom smislu. Fokus nije na rekonstrukciji stvarnih događaja, nego na osjećaju upravljanja državom kroz:

* **dvor**
* **provincije**
* **robu i razvoj**
* **stabilnost i nemire**
* **strukturisanu diplomatiju**
* **kratak, važan rat**
* **oštru završnicu**

Centralna fantazija igre glasi:

> Igrač mora imati osjećaj da vodi državu, a ne samo vojsku.

To znači da Crown of Sovereigns nije:

* čisti **wargame**
* suhi **euro** bez političke tenzije
* igra u kojoj je mapa samo dekoracija
* igra u kojoj je diplomatija samo flavor

---

## 2. Osnovni profil igre

* **Naziv:** Crown of Sovereigns
* **Aktivna verzija:** v2.7
* **Broj igrača:** 1–4
* **Najbolje iskustvo:** 3–4 igrača
* **Trajanje partije:** približno 90–150 minuta
* **Ciljna težina:** približno BGG 3.6–3.7
* **Žanr:** strateška board game igra upravljanja kraljevstvom
* **Ključni identitetski stubovi:**

  * **Dvor** (*Court*)
  * **Provincije** (*Provinces*)
  * **Roba** (*Goods*)
  * **Stabilnost** (*Stability*)
  * **Strukturisana diplomatija** (*Structured Diplomacy*)
  * **Kratak rat** (*Condensed Warfare*)
  * **Oštra završnica** (*Sharp Endgame*)

---

## 3. Šta je novo i zaključano u v2.7

Verzija **v2.7** zaključava pravac razvoja koji je proizašao iz dijagnostičkog i repair rada na ranijim verzijama.

Najvažnije zaključane izmjene u v2.7 su:

* vremenski ograničeni i strukturisani diplomatski prozori
* kompresija toka na princip **jedna glavna dvorska akcija po potezu**
* jači i konkretniji **Balanced** srednji tempo
* **Diplomatic** put kao puni i realni put do pobjede
* lider-targetirani **Crown Pressure** u 2P modu
* **Coronation Attempt** kao glavni sistemski wow vrhunac
* pojačana kasna krizna kompresija završnice
* standardizovana borba u 3 koraka
* jači **player aid** paket
* zadržana komponentna disciplina bez slobodnog bloata

Ove tačke nisu više samo ideje ili prijedlozi. U okviru repozitorija tretiraju se kao aktivna baza za dalji razvoj.

---

## 4. Svrha ovog repozitorija

Ovaj repozitorijum postoji da bi projekat ostao:

* koherentan
* verzionisan
* pregledan
* spreman za revizije
* spreman za playtest
* spreman za grafički handoff
* spreman za budući pitch i produkciju

Repo ne služi samo za čuvanje fajlova.
On je:

* **source of truth** za aktivnu verziju
* radni prostor za razvoj dokumentacije
* mjesto gdje se prati zašto je nešto promijenjeno
* mjesto gdje se sprečavaju kontradikcije između GDD-a, pravila, sistema i komponenti

---

## 5. Kako je dokumentacija organizovana

Repo je organizovan modularno. Svaka cjelina ima svoju ulogu.

### Glavni nivoi dokumentacije

* **docs/** — pregled projekta, identitet, pozicioniranje, publika, wow arhitektura
* **gdd/** — glavni dizajnerski dokument i kanonske odluke
* **rules/** — potpuna pravila igranja, setup, turn flow, scoring, FAQ
* **systems/** — detaljna razrada podsistema igre
* **components/** — specifikacija svih fizičkih komponenti
* **ux/** — onboarding, player aid, informacijska hijerarhija, readability
* **content/** — konkretan sadržaj koji puni sistem
* **playtests/** — planovi, metrike, session reportovi, issue log, hipoteze
* **production/** — MSRP, box scope, manufacturing rizici, pitch readiness
* **visuals/** — art direction, ikonografija, wireframe napomene, graphic handoff priprema
* **revision/** — revision log, status matrica, dependency mapa, review checklist
* **archive/** — starije verzije koje više nisu aktivna baza

---

## 6. Gdje početi ako prvi put ulaziš u projekat

Ako prvi put otvaraš repo, idi ovim redom:

### Korak 1

Pročitaj:

* `README.md`
* `docs/version-status.md`
* `VERSIONING.md`

Cilj je da odmah shvatiš:

* koja je aktivna verzija
* šta je kanonski zaključano
* kako se verzije tretiraju

### Korak 2

Pročitaj glavni GDD:

* `gdd/crown-of-sovereigns-v2.7-gdd.md`

To je centralni dokument koji objašnjava identitet igre, strukturu i glavne sisteme.

### Korak 3

Pređi na pravila:

* `rules/rules-reference-v2.7.md`
* `rules/setup-guide.md`
* `rules/turn-structure.md`
* `rules/scoring-reference.md`

To ti daje tačno kako se igra igra, ne samo zašto je dizajnirana tako.

### Korak 4

Ako radiš na specifičnom sistemu, idi u:

* `systems/`

Ako radiš na komponentama ili grafici, idi u:

* `components/`
* `ux/`
* `visuals/`

Ako radiš na testiranju i validaciji, idi u:

* `playtests/`

---

## 7. Najvažniji dokumenti u repozitoriju

### Obavezno za razumijevanje projekta

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `GLOSSARY.md`
* `gdd/crown-of-sovereigns-v2.7-gdd.md`

### Obavezno za igranje i provjeru logike

* `rules/rules-reference-v2.7.md`
* `rules/setup-guide.md`
* `rules/turn-structure.md`
* `rules/scoring-reference.md`
* `rules/quickstart-first-game.md`

### Obavezno za sistemsku razradu

* `systems/court-system.md`
* `systems/goods-and-development.md`
* `systems/stability-and-unrest.md`
* `systems/diplomacy-and-treaties.md`
* `systems/combat-system.md`
* `systems/scaling-2p-3p-4p.md`
* `systems/coronation-system.md`
* `systems/win-paths.md`

### Obavezno prije grafičke izrade

* `components/component-manifest.md`
* `components/board-spec.md`
* `components/cards-spec.md`
* `components/tokens-spec.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `ux/player-aid-system.md`
* `visuals/art-direction.md`
* `visuals/visual-hierarchy.md`
* `ux/graphic-handoff-checklist.md`

---

## 8. Pravila rada na repozitoriju

### 8.1. Single Source of Truth

Za svaku temu postoji samo jedan glavni dokument.

Primjer:

* glavni dizajnerski izvor istine = GDD
* glavni rules izvor istine = rules reference
* glavni komponentni izvor istine = component manifest

Ne smiju postojati dvije aktivne verzije istog pravila u dva različita dokumenta.

### 8.2. Prvo mijenjaj izvor, pa izvedene dokumente

Ako se mijenja pravilo, prvo se mijenja glavni dokument za tu temu, a tek onda svi zavisni dokumenti.

### 8.3. Svaka izmjena mora ostaviti trag

Kad se nešto promijeni, promjena mora biti vidljiva kroz:

* `CHANGELOG.md`
* internu revision bilješku dokumenta
* dependency propagation ako utiče na više fajlova

### 8.4. Nema paralelnih “finalnih” fajlova

Ne smiju se praviti fajlovi tipa:

* `rules-final-v3-last.md`
* `new-gdd-updated-final.md`

Repo mora ostati čist i dosljedan.

---

## 9. Status dokumenata

Svaki dokument treba imati jasno naznačen status:

* **Draft** — u radu
* **Review** — spreman za provjeru
* **Locked** — aktivni kanonski dokument
* **Deprecated** — istorijski relevantan, ali više nije aktivan
* **Archived** — zatvoren i ne koristi se dalje

Kritično pravilo:

> samo jedan glavni dokument po temi smije biti statusa **Locked**.

---

## 10. Šta mora biti zaključano prije grafičke izrade

Grafička izrada ne smije početi dok nisu zaključani:

* GDD
* full rules
* setup
* turn structure
* scoring
* court system
* diplomacy system
* stability system
* combat system
* coronation system
* win paths
* component manifest
* board spec
* cards spec
* tokens spec
* player board spec
* iconography spec
* terminology and labels
* player aid system
* visual hierarchy
* art direction
* graphic handoff checklist

Ako bilo koji od ovih dokumenata nije stabilan, grafički rad kreće prerano.

---

## 11. Kako se verzije tretiraju

Aktivna verzija je trenutno:

* **v2.7**

Sve naredne korekcije se vode kao:

* **v2.7.1**
* **v2.7.2**
* ili eventualno **v2.8** za veći razvojni korak

Sve starije verzije se čuvaju u `archive/` i ne smiju biti tretirane kao aktivna baza osim ako se eksplicitno ne radi istorijska analiza.

Za detalje o pravilima verzionisanja vidi:

* `VERSIONING.md`

---

## 12. Preporučeni redoslijed daljeg rada

Ako se dokumentacija tek razvija, idi ovim redom:

### Faza 1 — Canon Lock

* README
* version status
* GDD
* canonical decisions
* glossary
* versioning
* changelog

### Faza 2 — Rules Layer

* full rules reference
* setup guide
* turn structure
* scoring reference
* first game quickstart
* FAQ

### Faza 3 — Systems Layer

* court
* provinces
* goods
* stability
* diplomacy
* combat
* catch-up
* scaling
* crisis
* coronation
* win paths

### Faza 4 — Content Layer

* court roles
* kingdom advantages
* factions
* events
* treaties
* goods list
* coronation content

### Faza 5 — Graphic Prep Layer

* component manifest
* specs za board, cards, tokens, player boards
* iconography
* terminology
* player aid system
* art direction
* wireframe notes
* graphic handoff checklist

### Faza 6 — Validation Layer

* playtest plan
* playtest metrics
* issue log
* hypothesis tracker
* balance watchlist

---

## 13. Brutalno iskrena napomena

Najveći rizik za projekat nije nedostatak ideja.
Najveći rizik je nedisciplina dokumentacije.

To u praksi znači:

* kontradikcije između GDD-a i rules dokumenta
* preuranjen početak grafičke izrade
* različita terminologija u različitim fajlovima
* balans promjene bez revision traga
* sistemske promjene koje ne budu propagirane kroz zavisne dokumente

Ako se to ne kontroliše, kasnije dolazi:

* duplo prepravljanje
* skuplji grafički rad
* konfuzni playtest buildovi
* slabiji pitch
* i pad povjerenja u cijeli projekat

---

## 14. Gdje prijaviti problem ili izmjenu

Ako se uoči problem:

1. identifikuj glavni dokument za tu temu
2. provjeri da li je problem wording, balans, UX ili produkcija
3. evidentiraj promjenu u relevantnom logu
4. ažuriraj source-of-truth dokument
5. propagiraj promjenu na zavisne dokumente

---

## 15. Završna orijentacija

Crown of Sovereigns v2.7 treba da se razvija kao:

* koherentan sistem
* stabilna dokumentaciona cjelina
* proizvod spreman za revizije
* proizvod spreman za playtest
* proizvod spreman za budući grafički handoff

Prvo zaključaj **istinu**.
Zatim razradi **pravila**.
Zatim razdvoji **sisteme** od **sadržaja**.
Pa tek onda idi na **komponente**, **UX** i **grafički handoff**.
