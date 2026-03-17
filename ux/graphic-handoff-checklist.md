# graphic-handoff-checklist.md

# Crown of Sovereigns v2.7 — Graphic Handoff Checklist / Checklista za grafički handoff

## Status dokumenta

* **Dokument:** `ux/graphic-handoff-checklist.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati obaveznu checklistu prije prelaska iz dokumentacione i UX faze u ozbiljniji grafički, layout i vizuelni produkcijski rad
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Graphic Handoff/Grafički handoff**, **Readability/Čitljivost**, **Layout/Layout**
* **Povezani dokumenti:** `visuals/art-direction.md`, `visuals/visual-hierarchy.md`, `visuals/board-wireframe-notes.md`, `visuals/card-wireframe-notes.md`, `ux/information-hierarchy.md`, `ux/player-aid-system.md`, `components/component-manifest.md`, `components/board-spec.md`, `components/player-board-spec.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `docs/github-handoff-checklist.md`, `docs/release-readiness-checklist.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uvede završni filter prije ozbiljnijeg grafičkog rada
* spriječi da se layout, ilustracija i vizuelni polish rade nad dokumentima i sistemima koji još nisu dovoljno zaključani
* uskladi komponente, wireframe logiku, ikonografiju, terminologiju, UX prioritete i art direction u jedan praktičan handoff okvir
* smanji rizik da se grafički rad kasnije mora masovno vraćati zbog rule, systems ili hijerarhijskih promjena
* osigura da grafički sloj u CoS-u ne ide ispred dizajnerske i funkcionalne jasnoće

Ovo nije samo estetska checklista.
Ovo je kontrolni dokument koji čuva da vizuelna realizacija prati stvarno zaključanu logiku igre.

---

## 2. Zašto je graphic handoff checklist kritična

Kod ambicioznih board game projekata grafički rad često krene prerano.
Tada nastaju tipični problemi:

* layout se radi nad sistemom koji još nije dovoljno stabilan
* vizuelna hijerarhija nije zaključana, ali se već crta finalni board
* ikonografija se razvija prije nego što su termini i funkcije dovoljno čisti
* karta ili tabla izgledaju dobro, ali ne podržavaju setup, aid ili tok runde
* veliki dio rada mora kasnije nazad u reviziju

Dobar **Graphic Handoff/Grafički handoff** ne usporava projekat bez razloga.
On sprječava skupe i frustrirajuće povratke unazad.

---

## 3. Osnovni princip handoffa

Glavno pravilo glasi:

> grafički handoff se smije desiti tek kada su identitet, hijerarhija, funkcionalne komponente i osnovna pravila dovoljno stabilni da vizuelni rad ne postane puko gađanje pokretne mete.

To znači da prije handoffa mora biti dovoljno jasno:

* šta komponenta radi
* šta mora biti primarno vidljivo
* koji nazivi i ikone su zaključani
* šta je dekorativno, a šta sistemski nepromjenjivo važno

Ako to nije jasno, grafički tim ne dobija pravi brief nego problem.

---

## 4. Šta ova checklista jeste

Ova checklista treba da bude:

* završni UX i vizuelni filter
* praktična provjera spremnosti za layout i art handoff
* alat za samoprovjeru prije Figma ili drugog dizajnerskog rada
* zajednički most između systems, components, rules i visuals sloja

---

## 5. Šta ova checklista nije

Ova checklista nije:

* zamjena za art direction
* zamjena za wireframe dokumente
* zamjena za release readiness provjeru cijele igre
* automatska dozvola da se sve radi finalno bez ikakve revizije

Ona samo kaže:

* da li je baza dovoljno čista da grafički rad počne ozbiljno i smisleno

---

## 6. Glavne kategorije provjere

Graphic handoff checklista treba biti organizovana kroz sljedeće kategorije:

1. **Version and Canon Check/Provjera verzije i kanona**
2. **Rules and Systems Readiness/Provjera spremnosti pravila i sistema**
3. **Component Definition Check/Provjera definicije komponenti**
4. **Hierarchy and UX Check/Provjera hijerarhije i UX-a**
5. **Visual Direction Check/Provjera vizuelnog smjera**
6. **Terminology and Iconography Check/Provjera terminologije i ikonografije**
7. **Layout Readiness Check/Provjera spremnosti layouta**
8. **Handoff Decision/Odluka o handoffu**

Ovaj redoslijed treba ostati stabilan jer ide od kanonske osnove ka stvarnom vizuelnom radu.

---

## 7. Version and Canon Check / Provjera verzije i kanona

Prije grafičkog handoffa treba provjeriti:

* da li svi glavni dokumenti jasno nose oznaku **v2.7**
* da li ne postoji paralelna eksperimentalna verzija koja bi mogla kontaminirati layout odluke
* da li `docs/version-status.md` i `gdd/crown-of-sovereigns-v2.7-gdd.md` podržavaju isti identitet i status verzije
* da li su ključne odluke dovoljno zaključane da grafički rad ne bude rađen nad nečim što se odmah mijenja

Ako verziona osnova nije čista, graphic handoff ne treba odobriti.

---

## 8. Rules and Systems Readiness / Provjera spremnosti pravila i sistema

Treba provjeriti:

* da li su glavni systems dokumenti prisutni i dovoljno stabilni
* da li `rules/rules-reference-v2.7.md`, `rules/turn-structure.md`, `rules/scoring-reference.md` i `rules/setup-guide.md` govore istim jezikom
* da li su **Court/Dvor**, mapa, **Goods/Roba**, **Stability/Stabilnost**, diplomatija i završnica dovoljno jasno definisani da njihov vizuelni tretman ima smisla

Grafički rad ne smije pogađati kako sistem radi.
Mora ga naslijediti iz stabilne dokumentacije.

---

## 9. Component Definition Check / Provjera definicije komponenti

Treba provjeriti:

* da li postoji `components/component-manifest.md`
* da li `board-spec`, `player-board-spec`, `cards-spec`, `tokens-spec` i `units-and-markers-spec` imaju dovoljno jasne funkcionalne granice
* da li se zna koje su glavne komponente primarne, koje sekundarne, a koje pomoćne
* da li nema novih ili nedovoljno definisanih komponenti koje bi grafički rad morao da izmišlja usput

Ako komponentni sloj nije čist, layout će biti lažno uredan, ali sistemski slab.

---

## 10. Hierarchy and UX Check / Provjera hijerarhije i UX-a

Treba provjeriti:

* da li su `ux/information-hierarchy.md` i `visuals/visual-hierarchy.md` usklađeni
* da li je jasno šta mora biti **Primary/Primarno**, **Secondary/Sekundarno** i **Tertiary/Tercijarno**
* da li `ux/player-aid-system.md` podržava istu proceduralnu logiku kao `rules/turn-structure.md`
* da li je onboarding dovoljno definisan da layout ne mora sam rješavati nejasan teach

Glavni guardrail:

* grafički rad ne smije biti korišten da “spasi” nečistu hijerarhiju.

---

## 11. Visual Direction Check / Provjera vizuelnog smjera

Treba provjeriti:

* da li `visuals/art-direction.md` postoji i daje dovoljno jasan ton
* da li je ton igre politički, državnički i čitljiv, a ne generičan medieval fantasy
* da li završni i coronation elementi imaju definisan vizuelni prioritet
* da li je odnos između atmosfere i funkcije dovoljno jasan

Ako vizuelni smjer nije zaključen, layout rad lako odlazi u estetske pokušaje bez koherentnog identiteta.

---

## 12. Terminology and Iconography Check / Provjera terminologije i ikonografije

Treba provjeriti:

* da li `components/terminology-and-labels.md` postoji i da li su ključni pojmovi zaključani
* da li `components/iconography-spec.md` dovoljno jasno razlikuje šta je ikona, šta je simbol, a šta je dekoracija
* da li ista riječ i isti sistem imaju isti naziv kroz rules, systems, components i visuals dokumente
* da li ikone imaju dovoljno čistu funkcionalnu osnovu za razvoj

Ikonografija ne smije početi prije nego što je terminologija čista.

---

## 13. Layout Readiness Check / Provjera spremnosti layouta

Treba provjeriti:

* da li postoje `visuals/board-wireframe-notes.md` i `visuals/card-wireframe-notes.md`
* da li wireframe logika prati komponentne i UX prioritete
* da li se zna koje informacije moraju stalno živjeti na tabli, koje na tabli igrača, koje na kartama, a koje na aid-u
* da li je prostor planiran prema stvarnoj komponentnoj logici, a ne samo prema željenom izgledu

Ako layout nije spreman, prerano je za ozbiljniji grafički polish.

---

## 14. Setup and usability cross-check / Unakrsna provjera setupa i upotrebljivosti

Prije handoffa treba provjeriti i:

* da li `rules/setup-guide.md` može biti podržan trenutnim komponentnim i layout planom
* da li `components/box-and-insert-notes.md` ima smisla sa planiranim grupisanjem elemenata
* da li će budući grafički raspored pomoći ili odmoći setupu, teardownu i prvoj partiji

Glavni guardrail:

* lijep layout koji otežava setup nije dobar layout za CoS.

---

## 15. Minimum asset maturity / Minimalna zrelost asset osnove

Prije ozbiljnijeg handoffa treba biti jasno:

* koje komponente zahtijevaju poseban vizuelni tretman
* koje komponente mogu koristiti standardizovan template pristup
* gdje su neophodni jedinstveni završni ili politički elementi
* gdje dekoracija mora ostati skromna da bi čitljivost preživjela

Drugim riječima:

* mora biti poznato šta je “custom high-priority asset”, a šta je “templated functional asset”.

---

## 16. Red flags / Crvene zastavice koje blokiraju handoff

Graphic handoff treba blokirati ako je prisutno bilo šta od sljedećeg:

* aktivna verzija nije čista
* ključni systems dokumenti još nemaju stabilnu logiku
* board ili player board spec nisu dovoljno definisani
* vizuelna hijerarhija nije zaključana
* terminologija i ikonografija nisu dosljedne
* završni sistem i coronation signal još nemaju jasan vizuelni prioritet
* layout bi morao da izmišlja sistemsku logiku umjesto da je naslijedi

Jedna jaka crvena zastavica je često dovoljna da handoff bude prerano odobren.

---

## 17. Minimalni pass format / Minimalni format prolaza

Prije handoffa preporučeni minimalni status format je:

* **Version & Canon/Verzija i kanon:** pass / fail
* **Rules & Systems/Pravila i sistemi:** pass / risk / fail
* **Components/Komponente:** pass / risk / fail
* **Hierarchy & UX/Hijerarhija i UX:** pass / risk / fail
* **Visual Direction/Vizuelni smjer:** pass / risk / fail
* **Terminology & Iconography/Terminologija i ikonografija:** pass / risk / fail
* **Layout Readiness/Spremnost layouta:** pass / risk / fail
* **Graphic Handoff/Odluka:** not ready / conditionally ready / ready

Ako bilo koja ključna funkcionalna kategorija padne na **fail**, handoff ne treba tretirati kao spreman.

---

## 18. Conditionallly ready / Uslovno spremno

**Conditionally Ready/Uslovno spremno** je zdrava odluka kada:

* baza je dovoljno čista za početni layout rad
* ali postoje 1–3 jasno označene tačke koje još ne smiju u finalni polish ili zaključani asset rad

To je često poštenija odluka nego prerano **Ready/Spremno**.

---

## 19. Relationship to GitHub handoff / Odnos prema GitHub handoffu

Ovaj dokument mora se čitati zajedno sa:

* `docs/github-handoff-checklist.md`

Razlika je:

* **GitHub handoff** pita da li dokumenti mogu u repo kao čista radna baza
* **Graphic handoff** pita da li je ta baza dovoljno stabilna za vizuelnu realizaciju

Repo higijena nije isto što i grafička spremnost.

---

## 20. Relationship to release readiness / Odnos prema release spremnosti

Ovaj dokument nije isto što i:

* `docs/release-readiness-checklist.md`

Verzija može biti dovoljno čista za grafički handoff, a da još nije potpuno release-spremna.
I obrnuto: može izgledati dovoljno zrela kao dizajn, ali još ne biti čista za vizuelni rad.

To treba držati odvojeno.

---

## 21. Najčešće greške prije graphic handoffa

* art kreće prije nego što je hijerarhija zaključana
* board layout se radi prije nego što je komponentni manifest čist
* ikonografija se crta prije terminološkog zaključavanja
* quickstart i player aid ostaju izvan vizuelnog sistema do prekasno
* završnica i coronation elementi vizuelno se rješavaju usput, umjesto planski
* grafički rad pokušava zakrpiti sistemske i UX probleme umjesto da ih naslijedi kao riješene

---

## 22. Workflow pravilo za korištenje checkliste

Kad se procjenjuje graphic handoff, preporučeni redoslijed je:

1. provjeriti kanon i verziju
2. provjeriti systems i rules stabilnost
3. provjeriti komponentni sloj
4. provjeriti hijerarhiju i UX
5. provjeriti art direction i ikonografiju
6. provjeriti wireframe i layout spremnost
7. donijeti jasnu odluku: nije spremno / uslovno spremno / spremno

Ako se krene od moodboard ili estetskog entuzijazma pa se tek kasnije traži sistemska osnova, proces je pogrešno postavljen.

---

## 23. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li checklista ostaje praktična?
2. da li i dalje štiti čitljivost i UX od prerane estetizacije?
3. da li ostaje usklađena sa components, visuals i rules slojem?
4. da li pomaže smanjenju povratnih revizija?
5. da li jasno razlikuje funkcionalnu spremnost od estetske želje?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 24. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `visuals/art-direction.md`
* `visuals/visual-hierarchy.md`
* `visuals/board-wireframe-notes.md`
* `visuals/card-wireframe-notes.md`
* `ux/information-hierarchy.md`
* `ux/player-aid-system.md`
* `components/component-manifest.md`
* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `docs/github-handoff-checklist.md`
* `docs/release-readiness-checklist.md`
* `GLOSSARY.md`

---

## 25. Završna napomena

**Graphic Handoff Checklist / Checklista za grafički handoff** mora ostati jedan od glavnih završnih filtera prije nego što **Crown of Sovereigns v2.7** uđe u ozbiljniji vizuelni i layout rad.

Ako radi dobro:

* grafički rad počinje na čistoj osnovi
* manje se vraća unazad
* hijerarhija i čitljivost ostaju pod kontrolom
* art direction dobija stabilan temelj
* a cijeli proizvod izgleda koherentnije i zrelije

Ako radi loše:

* vizuelni rad preuzima probleme koje ne treba rješavati
* layout i ilustracija kreću prerano
* broj povratnih revizija raste
* a proizvod izgleda elegantnije nego što je stvarno funkcionalno spreman

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
