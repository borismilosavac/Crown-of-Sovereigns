# release-readiness-checklist.md

# Crown of Sovereigns v2.7 — Release Readiness Checklist / Checklista spremnosti za release

## Status dokumenta

* **Dokument:** `docs/release-readiness-checklist.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati obaveznu checklistu prije nego što se aktivna verzija ili njen paket proglasi spremnim za ozbiljniji interni release, vanjski review, pitch pripremu ili zaključavanje kao stabilna radna baza
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Release/Release**, **Readiness/Spremnost**, **Checklist/Checklista**
* **Povezani dokumenti:** `docs/version-status.md`, `docs/revision-workflow.md`, `docs/document-status-policy.md`, `docs/github-handoff-checklist.md`, `playtests/playtest-plan-v2.7.md`, `playtests/hypothesis-tracker.md`, `playtests/balance-watchlist.md`, `playtests/patch-review-log.md`, `CHANGELOG.md`, `VERSIONING.md`, `gdd/canonical-decisions.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uvede završni filter prije nego što se kaže da je verzija “spremna” za ozbiljniji release korak
* spriječi da uredna dokumentacija bude pogrešno shvaćena kao dokaz da je igra sistemski spremna
* uskladi signale iz pravila, komponenti, playtesta i patch rada u jednu provjeru spremnosti
* pomogne da se razlikuje lokalna stabilnost od stvarne release spremnosti
* zaštiti projekat od prerane samouvjerenosti

Ovo nije marketinška potvrda kvaliteta.
Ovo je radna provjera da li je verzija dovoljno stabilna za naredni ozbiljan korak.

---

## 2. Zašto je release readiness checklista kritična

Kod projekata poput **Crown of Sovereigns v2.7** vrlo je lako pomiješati tri različite stvari:

* dokumentacija je dobro organizovana
* verzija djeluje obećavajuće
* verzija je stvarno spremna za ozbiljniji release korak

To nije isto.

Može se desiti da:

* repo izgleda uredno, ali balans još pliva
* završnica još nije dovoljno potvrđena
* 2P ili 4P i dalje imaju ozbiljan rizik
* aid i komponentni UX još uvijek proizvode previše lookup-a
* patch linija još nije dovoljno stabilna

Dobra release checklista sprečava da se te stvari zamijene.

---

## 3. Osnovni princip release spremnosti

Glavno pravilo glasi:

> verzija je spremna za release korak tek kada su i sistem, i dokumentacija, i test signal dovoljno usklađeni da zajedno daju stabilnu sliku — ne kada samo jedan od tih slojeva izgleda dobro.

To znači da spremnost mora provjeriti najmanje:

* kanonsku jasnoću
* systems stabilnost
* playtest signal
* balansne rizike
* UX i komponentnu čitljivost
* patch disciplinu
* dokumentacionu usklađenost

Ako jedan od ovih slojeva ozbiljno kaska, release spremnost je upitna.

---

## 4. Šta ova checklista jeste

Ova checklista treba da bude:

* završna interna provjera
* alat za procjenu da li verzija smije ići u jači review, pitch paket ili širu test fazu
* filter protiv lažne gotovosti
* most između rada na detaljima i odluke “spremno / nije spremno”

---

## 5. Šta ova checklista nije

Ova checklista nije:

* zamjena za playtest plan
* zamjena za changelog
* dokaz da igra nema više problema
* formalnost koja se samo preleti pogledom

Ona služi da smanji rizik, ne da glumi sigurnost.

---

## 6. Kada koristiti release readiness checklistu

Checklistu treba koristiti najmanje kada:

* se procjenjuje da li je aktivna verzija spremna za ozbiljniji interni milestone
* se priprema vanjski review paket
* se sprema pitch ili publisher-facing dokumentacioni set
* se zaključava verzija prije veće naredne iteracije
* se odlučuje da li patch linija ostaje unutar iste verzije ili traži novu glavnu verziju

Ne treba je aktivirati poslije svake male izmjene.
Ona služi za veće pragove odluke.

---

## 7. Glavne kategorije provjere

Release readiness checklista treba biti organizovana kroz ove glavne kategorije:

1. **Canonical Basis Check/Provjera kanonske osnove**
2. **Rules and Systems Stability/Provjera stabilnosti pravila i sistema**
3. **Playtest Evidence Check/Provjera playtest dokaza**
4. **Balance Risk Check/Provjera balansnih rizika**
5. **UX and Component Readiness/Provjera UX i komponentne spremnosti**
6. **Patch Discipline Check/Provjera discipline zakrpa**
7. **Documentation Readiness/Provjera spremnosti dokumentacije**
8. **Release Decision/Odluka o release spremnosti**

Ovaj redoslijed treba ostati isti jer ide od temelja ka završnoj odluci.

---

## 8. Canonical Basis Check / Provjera kanonske osnove

Prvo treba provjeriti:

* da li je aktivna verzija jasno definisana u `docs/version-status.md`
* da li postoji samo jedna aktivna kanonska baza za dalji rad
* da li su ključne odluke usklađene sa `gdd/canonical-decisions.md`
* da li nema paralelne “skoro-kanonske” linije koja bi mogla zbuniti tim

Ako kanonska osnova nije čista, release spremnost se ne smije potvrditi.

---

## 9. Rules and Systems Stability / Provjera stabilnosti pravila i sistema

Treba provjeriti:

* da li glavni systems dokumenti više nemaju otvorene velike kontradikcije
* da li `rules/rules-reference-v2.7.md` i systems dokumenti govore istu stvar
* da li su **Court/Dvor**, **Goods/Roba**, **Stability/Stabilnost**, **Diplomacy/Diplomatija**, **Combat/Borba** i **Coronation Attempt/Pokušaj krunisanja** dovoljno stabilni za ozbiljniji ciklus
* da li su otvorena pitanja još uvijek lokalna ili diraju samo srce verzije

Release ne traži savršenstvo, ali traži da jezgro ne bude klimavo.

---

## 10. Playtest Evidence Check / Provjera playtest dokaza

Treba provjeriti:

* da li postoji dovoljan broj smislenih sesija za ovu verziju ili patch liniju
* da li session reportovi i tester feedback daju konzistentan signal ili i dalje pričaju previše različitih priča
* da li su ključni modovi 2P, 3P i 4P testirani dovoljno da daju osnovni nivo povjerenja
* da li su rizični sistemi testirani ciljano, ne samo usput

Ako playtest signal još uvijek previše liči na fragmente i utiske, release spremnost je prerana.

---

## 11. Balance Risk Check / Provjera balansnih rizika

Treba provjeriti `playtests/balance-watchlist.md` i pitati:

* da li postoje stavke koje su i dalje **Escalated/Eskaliran** ili **Critical/Kritična**
* da li su najvažniji rizici barem spušteni na nivo koji je pod kontrolom
* da li glavne putanje do pobjede djeluju stvarno žive
* da li 2P ili 4P imaju problem koji je prevelik da bi verzija djelovala stabilno

Ako i dalje postoji jedan ili više kritičnih balansnih rizika u jezgri verzije, treba biti vrlo oprezan sa release tvrdnjom.

---

## 12. UX and Component Readiness / Provjera UX i komponentne spremnosti

Treba provjeriti:

* da li su aid, tabla, tabla igrača i terminologija dovoljno čitljivi
* da li onboarding više ne puca na istim mjestima kroz više grupa
* da li komponente šalju ispravan signal o važnosti sistema
* da li su ikonografija i label standard dovoljno stabilni za narednu fazu

Važno pravilo:

* čak i dobar sistem nije release-spreman ako ga komponente stalno predstavljaju pogrešno.

---

## 13. Patch Discipline Check / Provjera discipline zakrpa

Treba provjeriti:

* da li je patch linija čista i dovoljno razumljiva
* da li `playtests/patch-review-log.md` pokazuje stvarni napredak ili samo niz polovično testiranih korekcija
* da li postoje patch-evi koji su i dalje samo **Implemented/Primijenjena**, ali još ne **Validated/Potvrđena**, a diraju srce verzije
* da li je problem zakrpa previše nagomilan bez jasnog rezultata

Ako patch linija i dalje više liči na eksperimente nego na stabilizaciju, release spremnost je upitna.

---

## 14. Documentation Readiness / Provjera spremnosti dokumentacije

Treba provjeriti:

* da li su glavni dokumenti prisutni i dovoljno usklađeni
* da li statusi dokumenata imaju smisla
* da li je terminologija čista kroz rules, systems, content, components, UX i playtests sloj
* da li postoji jasan trag revizija i promjena gdje treba
* da li bi novi saradnik ili vanjski reviewer mogao razumjeti bazu bez traženja po haotičnim draftovima

Ovdje je cilj da dokumentacija bude spremna da nosi verziju, ne samo da postoji.

---

## 15. Minimalna release odluka

Na kraju checkliste treba dati jednu od sljedećih odluka:

### 15.1. **Not Ready/Nije spremno**

Verzija još nema dovoljno stabilnosti ili signala.

### 15.2. **Conditionally Ready/Uslovno spremno**

Verzija je dovoljno stabilna za ograničen naredni korak, ali i dalje ima jasno označene rizike.

### 15.3. **Ready/Spremno**

Verzija je dovoljno usklađena i stabilna za namijenjeni release korak.

Kritično pravilo:

> “Ready/Spremno” mora uvijek značiti “spremno za konkretan naredni korak”, ne “zauvijek završeno”.

---

## 16. Preporučeni minimalni checklist format

Praktični minimalni format prije odluke:

* **Canonical Basis/Kanonska osnova:** pass / fail
* **Rules & Systems/Pravila i sistemi:** pass / risk / fail
* **Playtest Evidence/Playtest dokaz:** pass / risk / fail
* **Balance Risks/Balansni rizici:** pass / risk / fail
* **UX & Components/UX i komponente:** pass / risk / fail
* **Patch Discipline/Disciplina zakrpa:** pass / risk / fail
* **Documentation/ Dokumentacija:** pass / risk / fail
* **Release Decision/Odluka:** not ready / conditionally ready / ready

Ako više od jedne ključne kategorije padne na **fail**, treba izbjegavati optimističnu release odluku.

---

## 17. Dodatna pitanja prije release odluke

Prije konačne odluke korisno je pitati:

* da li verzija zaista drži svoju centralnu fantaziju?
* da li su najveći problemi sada lokalni ili još uvijek sistemski?
* da li je wow prisutan bez raspada pravičnosti?
* da li bi ozbiljan vanjski reviewer vidio disciplinu ili previše šavova?
* da li tim zna tačno šta su preostali rizici ili ih samo osjeća mutno?

Ova pitanja pomažu da odluka ne bude samo tehnička, nego i stvarno razvojno smislena.

---

## 18. Kada treba izabrati “Conditionally Ready / Uslovno spremno”

Ova odluka je zdrava kada:

* jezgro radi dovoljno dobro
* dokumentacija i komponentna baza su stabilne
* nema kritičnog raspada
* ali još postoje 1–3 jasno označena rizika koja treba pratiti u narednom koraku

To je često realnija odluka od prerane **Ready/Spremno** oznake.

---

## 19. Kada “Ready / Spremno” ne treba dati

Ne treba dati punu **Ready/Spremno** oznaku ako:

* glavne hipoteze još nisu dovoljno potvrđene
* watchlist i dalje sadrži kritične balansne pukotine
* završnica i wow još nisu dovoljno stabilni
* 2P ili 4P imaju ozbiljan neadresiran problem
* dokumenti i patch logika još ne djeluju dovoljno čisto za ozbiljniji korak

Ovdje je poštena procjena važnija od optimizma.

---

## 20. Veza sa version-status dokumentom

Ako se donese ozbiljna release odluka, treba provjeriti da li to utiče na:

* `docs/version-status.md`

Taj dokument mora odražavati stvarno stanje verzije:

* aktivna baza
* stepen stabilnosti
* naredni očekivani korak

Release readiness odluka ne smije ostati izolovana od status dokumenta.

---

## 21. Veza sa revision workflow i patch review log dokumentima

Ova checklista mora se čitati zajedno sa:

* `docs/revision-workflow.md`
* `playtests/patch-review-log.md`

Zašto?
Zato što release spremnost ne zavisi samo od finalnog stanja, nego i od toga koliko je put do tog stanja bio čist i razumljiv.

Ako patch istorija djeluje haotično, to smanjuje povjerenje i u trenutnu stabilnost verzije.

---

## 22. Veza sa github handoff checklistom

`docs/github-handoff-checklist.md` pita:

* da li je dokument ili paket dokumenata spreman da uđe u repo bez kvarenja strukture?

`docs/release-readiness-checklist.md` pita:

* da li je sama verzija ili release paket dovoljno stabilan za ozbiljniji korak?

Jedno je repo higijena.
Drugo je verziona i sistemska spremnost.
Oboje je potrebno, ali nije isto.

---

## 23. Najčešće greške pri procjeni release spremnosti

* brkati urednu dokumentaciju sa stabilnim sistemom
* dati **Ready/Spremno** samo zato što je posljednja partija bila dobra
* ignorisati jedan ozbiljan rizik jer “sve ostalo djeluje super”
* precijeniti patch koji je tek djelimično provjeren
* ne razlikovati “spremno za dalje testiranje” od “spremno za pitch”

Ove greške su posebno opasne jer proizvode lažnu sigurnost.

---

## 24. Workflow pravilo za korištenje checkliste

Kad se radi release procjena, preporučeni redoslijed je:

1. provjeriti kanonsku osnovu
2. provjeriti systems i rules stabilnost
3. provjeriti playtest i balansne signale
4. provjeriti UX, komponente i dokumentaciju
5. provjeriti patch disciplinu
6. donijeti jednu jasnu odluku i zapisati preostale rizike

Ako se krene od “osjećaja da je verzija spremna”, pa tek onda traže argumenti za to, proces je pogrešno postavljen.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li checklista ostaje stroga, ali upotrebljiva?
2. da li razlikuje lokalnu stabilnost od stvarne release spremnosti?
3. da li smanjuje lažnu sigurnost?
4. da li ostaje kompatibilna sa playtest i revizionim dokumentima?
5. da li je i dalje dovoljno kratka da se stvarno koristi prije odluke?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `docs/version-status.md`
* `docs/revision-workflow.md`
* `docs/document-status-policy.md`
* `docs/github-handoff-checklist.md`
* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`
* `playtests/patch-review-log.md`
* `CHANGELOG.md`
* `VERSIONING.md`
* `gdd/canonical-decisions.md`
* `GLOSSARY.md`

---

## 27. Završna napomena

**Release Readiness Checklist / Checklista spremnosti za release** mora ostati jedan od glavnih zaštitnih dokumenata prije bilo kakve ozbiljnije tvrdnje da je verzija **v2.7** spremna za naredni korak.

Ako radi dobro:

* lažna gotovost se hvata na vrijeme
* sistemi, dokumenti i test signal se gledaju zajedno
* release odluke postaju poštenije i stabilnije
* tim tačno zna koje rizike nosi dalje
* a prelazak u novi milestone djeluje mnogo sigurnije

Ako radi loše:

* repo može izgledati uredno dok je verzija još klimava
* patch i balansni problemi ostaju zamaskirani
* release odluka postaje više emocionalna nego razvojna
* a naredna faza rada ulazi sa više skrivenih rizika nego što je potrebno

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
