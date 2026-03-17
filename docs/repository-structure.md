# repository-structure.md

# Crown of Sovereigns v2.7 — Repository Structure / Struktura repozitorijuma

## Status dokumenta

* **Dokument:** `docs/repository-structure.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati standardnu strukturu GitHub repozitorijuma, pravila organizacije foldera i način kako se dokumenti, vizuelni fajlovi i playtest artefakti raspoređuju
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Repository/Repozitorijum**, **Rules/Pravila**, **Systems/Sistemi**
* **Povezani dokumenti:** `README.md`, `VERSIONING.md`, `CHANGELOG.md`, `docs/version-status.md`, `gdd/canonical-decisions.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* zaključa kako je repozitorijum organizovan
* spriječi miješanje kanonskih, radnih i zastarjelih fajlova
* uspostavi dosljednu logiku imenovanja foldera i dokumenata
* pomogne da buduće revizije ostanu pregledne
* omogući da dizajn, pravila, sistemi, sadržaj i playtest dokumenti rastu bez raspada strukture

Ovo nije samo tehnički folder pregled.
Ovo je dokument koji čuva disciplinu projekta kroz vrijeme.

---

## 2. Zašto je struktura repozitorijuma kritična

Kod projekta kao što je **Crown of Sovereigns v2.7**, vrlo brzo može doći do problema ako repozitorijum nije strogo organizovan:

* više verzija istog dokumenta u različitim folderima
* radni draftovi koji izgledaju kao finalni dokumenti
* grafički i rules fajlovi bez jasne veze
* playtest nalazi koji se ne mogu povezati sa verzijom i promjenom
* folderi koji rastu bez pravila i postaju neupotrebljivi

Dobra struktura nije birokratija. Ona štedi vrijeme, smanjuje greške i olakšava svaku buduću fazu rada.

---

## 3. Osnovni princip strukture

Glavno pravilo glasi:

> repozitorijum mora biti organizovan po funkciji dokumenta i ulozi u procesu, ne po trenutnom raspoloženju ili ličnoj improvizaciji.

To znači:

* systems dokumenti idu u `systems/`
* content dokumenti idu u `content/`
* components specifikacije idu u `components/`
* visuals wireframe i vizuelne napomene idu u `visuals/`
* playtest operativa ide u `playtests/`

Ako jedan fajl može “bilo gdje”, uskoro nastaje haos.

---

## 4. Šta ova struktura jeste

Struktura repozitorijuma treba da bude:

* jasna
* stabilna
* lako pretraživa
* laka za onboarding novog saradnika
* pogodna za reviziju i buduće verzije

---

## 5. Šta ova struktura nije

Struktura repozitorijuma nije:

* zbir nasumičnih foldera koji nastaju usput
* mjesto gdje se ista tema duplira na više nivoa bez razloga
* beskonačna dubina foldera bez stvarne potrebe
* sistem u kojem dizajner, pravila i playtest materijali govore različitim organizacionim jezikom

Ako sklizne u bilo šta od ovoga, repo postaje spor za rad i nepouzdan za revizije.

---

## 6. Glavni root dokumenti

Na root nivou repozitorijuma treba da ostanu samo dokumenti koji važe za cijeli projekat:

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `GLOSSARY.md`

Ovi fajlovi imaju posebnu ulogu:

* `README.md` = ulaz u projekat
* `VERSIONING.md` = pravila verzionog rada
* `CHANGELOG.md` = istorija promjena
* `GLOSSARY.md` = kanonski pojmovnik

Root ne smije postati parking zona za sve važne fajlove.

---

## 7. Glavni folderi repozitorijuma

Preporučena glavna struktura za **v2.7** je:

* `docs/`
* `gdd/`
* `rules/`
* `systems/`
* `content/`
* `components/`
* `ux/`
* `visuals/`
* `playtests/`

Po potrebi kasnije mogu postojati i dodatni folderi, ali samo ako imaju jasnu funkciju i ne dupliraju postojeće.

---

## 8. docs/ folder

`docs/` sadrži infrastrukturne i projektne dokumente koji nisu direktno pravila ili sadržaj sistema.

Tipični dokumenti ovdje:

* `docs/version-status.md`
* `docs/repository-structure.md`
* eventualni budući pipeline, revision ili handoff dokumenti

`docs/` je mjesto za meta-dokumentaciju projekta, ne za systems ili rules sadržaj.

---

## 9. gdd/ folder

`gdd/` sadrži dokumente koji nose kanonsku projektnu i dizajnersku bazu.

Tipični dokumenti ovdje:

* `gdd/canonical-decisions.md`
* budući glavni GDD dokument ili njegovi segmenti

Važno pravilo:

* `gdd/` ne smije postati folder za sve detaljne systems i content dokumente
* on treba da nosi okvir, odluke i glavnu dizajnersku kičmu projekta

---

## 10. rules/ folder

`rules/` sadrži sve što se direktno odnosi na igranje i pravila iz perspektive igrača.

Tipični dokumenti ovdje:

* `rules/rules-reference-v2.7.md`
* `rules/setup-guide.md`
* `rules/turn-structure.md`
* `rules/scoring-reference.md`
* `rules/quickstart-first-game.md`
* `rules/faq-rules.md`

Ovdje idu pravila koja igrač koristi ili uči, ne duboka dizajnerska analiza sistema.

---

## 11. systems/ folder

`systems/` sadrži mehaničku i dizajnersku arhitekturu glavnih sistema igre.

Tipični dokumenti ovdje:

* `systems/court-system.md`
* `systems/province-map-system.md`
* `systems/goods-and-development.md`
* `systems/stability-and-unrest.md`
* `systems/diplomacy-and-treaties.md`
* `systems/combat-system.md`
* `systems/catch-up-and-runaway-control.md`
* `systems/scaling-2p-3p-4p.md`
* `systems/event-and-crisis-system.md`
* `systems/coronation-system.md`
* `systems/win-paths.md`
* `systems/ai-automa-solo.md`

Ovo je mjesto za “kako sistem radi i zašto”, ne za finalni kartični tekst ili grafički layout.

---

## 12. content/ folder

`content/` sadrži konkretizaciju sistema u sadržajne okvire, liste i tipove zapisa.

Tipični dokumenti ovdje:

* `content/court-roles.md`
* `content/kingdom-advantages.md`
* `content/events-and-crises.md`
* `content/treaties-list.md`
* `content/goods-list.md`
* `content/coronation-content.md`

Ovo je mjesto gdje sistem dobija sadržajni identitet, ali još ne kroz finalne ilustracije ili production fajlove.

---

## 13. components/ folder

`components/` sadrži specifikacije fizičkih i informacijskih komponenti.

Tipični dokumenti ovdje:

* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `components/player-board-spec.md`
* `components/board-spec.md`

Kasnije ovdje mogu ući i dodatni dokumenti poput:

* `components/tokens-spec.md`
* `components/cards-spec.md`
* `components/box-insert-notes.md`

Ali samo ako ne dupliraju sadržaj koji već postoji u `visuals/` ili `ux/`.

---

## 14. ux/ folder

`ux/` sadrži dokumente koji kontrolišu čitljivost, tok informacija i pomoćne materijale.

Tipični dokumenti ovdje:

* `ux/player-aid-system.md`
* `ux/information-hierarchy.md`

Kasnije ovdje mogu doći dodatni UX dokumenti, npr.:

* setup ergonomija
* accessibility za print
* lookup reduction analiza

Ali samo ako imaju jasnu funkciju i nisu već pokriveni drugim folderima.

---

## 15. visuals/ folder

`visuals/` sadrži wireframe, vizuelne napomene i dokumente koji pripremaju grafički rad bez da budu finalni art fajlovi.

Tipični dokumenti ovdje:

* `visuals/card-wireframe-notes.md`
* `visuals/board-wireframe-notes.md`

Kasnije ovdje mogu doći:

* vizuelni template dokumenti
* layout note-ovi
* priprema za Figma ili print layout

Ali `visuals/` ne smije postati folder za gotove eksportovane art fajlove bez dodatne organizacije.

---

## 16. playtests/ folder

`playtests/` sadrži operativne dokumente za testiranje i evaluaciju.

Tipični dokumenti ovdje:

* `playtests/playtest-plan-v2.7.md`
* `playtests/hypothesis-tracker.md`
* `playtests/balance-watchlist.md`

Kasnije ovdje mogu doći:

* test report template-i
* session logs
* tester feedback forms
* matchup ili patch review bilješke

Ali moraju ostati jasno povezani sa verzijom i datumom.

---

## 17. Pravilo imenovanja fajlova

Svi fajlovi treba da koriste:

* mala slova
* `kebab-case`
* jasna, funkcionalna imena
* bez proizvoljnih skraćenica

Primjeri dobrih imena:

* `court-system.md`
* `goods-list.md`
* `player-board-spec.md`
* `board-wireframe-notes.md`

Primjeri loših imena:

* `CourtStuff.md`
* `final-final-rules-new.md`
* `boris_notes_2.md`
* `GDD_FINAL_REAL.md`

Ime fajla mora objašnjavati funkciju, ne emociju autora u tom trenutku.

---

## 18. Pravilo verzije u nazivu fajla

Verzija se ne stavlja u naziv svakog dokumenta osim kada postoji jasan razlog.

### Kada verzija ide u ime

* kada je dokument specifično vezan za jednu rules verziju koja će možda imati paralelne varijante
* kada je potreban jasan istorijski trag, npr. `rules-reference-v2.7.md`
* kada playtest ili izvještaj dokument mora biti striktno vezan za verziju, npr. `playtest-plan-v2.7.md`

### Kada verzija ne ide u ime

* kada dokument predstavlja aktivni kanonski dokument za taj folder i nema potrebe za paralelnim fajlovima
* kada verzioni status već jasno stoji u samom dokumentu

Ovo pravilo smanjuje nepotrebno dupliranje i haos u nazivima.

---

## 19. Pravilo statusa dokumenta

Svaki dokument mora unutar sebe imati:

* naziv dokumenta
* aktivnu verziju igre
* status dokumenta
* povezane dokumente

To znači da status ne smije zavisiti samo od foldera ili od sjećanja osobe koja radi.

Tipični statusi:

* Draft
* Review
* Locked
* Deprecated

Ovi statusi moraju biti korišteni dosljedno kroz cijeli repo.

---

## 20. Pravilo deprecated i archival logike

Zastarjeli ili zamijenjeni dokumenti ne smiju ostati da plutaju kao da su i dalje aktivni.

Postoje dvije zdrave opcije:

### 20.1. Deprecated in place / Zastarjelo na mjestu

Dokument ostaje gdje jeste, ali jasno nosi status **Deprecated** i referencu na novi dokument.

### 20.2. Archive folder / Arhivski folder

Ako broj starih dokumenata raste, može se uvesti strukturisan `archive/` ili podfolder arhive po vrsti.

Ali pravilo je:

* ne arhivirati prerano ako to otežava rad
* ne ostavljati zastarjele fajlove bez jasnog statusa

---

## 21. Pravilo jednog izvora istine

Za svaku temu mora postojati jedan glavni dokument koji je izvor istine.

Primjeri:

* terminologija = `GLOSSARY.md` + operativni prikaz u `components/terminology-and-labels.md`
* systems logika = relevantni dokument u `systems/`
* content lista = relevantni dokument u `content/`

Ne smije postojati situacija gdje su dva jednako važna dokumenta “možda tačna” za istu stvar.

Ako postoji konflikt, mora se riješiti, ne tolerisati.

---

## 22. Pravilo linkovanja između dokumenata

Svaki dokument treba imati sekciju **Povezani dokumenti** i po potrebi **Dependency notes**.

To služi da:

* buduće izmjene odmah znaju šta još treba provjeriti
* revizije budu manje opasne
* repo funkcioniše kao povezan sistem, ne kao kolekcija izolovanih tekstova

Linkovanje ne smije biti nasumično. Treba navoditi samo stvarno relevantne zavisnosti.

---

## 23. Pravilo za nove foldere

Novi folder ne smije se uvoditi samo zato što trenutno “djeluje zgodno”.

Prije uvođenja novog foldera mora se provjeriti:

1. da li postojeći folder već može zdravo nositi taj dokument
2. da li novi folder ima jasnu trajnu funkciju
3. da li novi folder smanjuje ili povećava fragmentaciju
4. da li će ga budući saradnik odmah razumjeti bez dodatnog objašnjavanja

Ako ne prolazi ova pitanja, novi folder se ne uvodi.

---

## 24. Pravilo za radne i privremene fajlove

Radni, interni ili privremeni fajlovi ne smiju ostati pomiješani sa kanonskim dokumentima.

Ako su potrebni, treba ih jasno odvojiti kroz:

* status u dokumentu
* radni podfolder ako zaista postoji kontinuirana potreba
* ili van repozitorijuma ako su potpuno privremeni i lični

Repo nije mjesto za trajno skladištenje ličnog improvizovanog draft otpada.

---

## 25. Veza sa verzionom disciplinom

Struktura repozitorijuma mora raditi zajedno sa:

* `VERSIONING.md`
* `CHANGELOG.md`
* `docs/version-status.md`

To znači da fajl organizacija mora olakšati odgovor na pitanja:

* šta je trenutno kanonsko
* šta je promijenjeno
* šta je zastarjelo
* gdje se nalazi aktivna dokumentacija za ovu verziju

Ako struktura to otežava, nije dovoljno dobra.

---

## 26. Najčešće greške u organizaciji repozitorijuma

* više verzija istog dokumenta bez jasnog statusa
* previše duboka struktura foldera bez stvarne potrebe
* root zatrpan tematskim dokumentima
* systems i content dokumenti pomiješani u isti folder
* visuals i components dokumenti koji rade istu stvar iz dva ugla bez jasne razlike
* playtest nalazi koji nisu vezani za verziju ili datum

---

## 27. Workflow pravilo za novi dokument

Kad se pravi novi dokument, prije kreiranja treba provjeriti:

1. kojoj glavnoj funkciji pripada
2. u koji folder prirodno ide
3. da li već postoji sličan dokument koji treba dopuniti umjesto duplirati
4. da li ime fajla jasno opisuje ulogu
5. da li dokument treba biti verzijski specifičan u imenu ili ne
6. koje povezane dokumente i dependency napomene mora imati

Ako ne prolazi ova pitanja, novi dokument ne treba praviti dok se ne razjasni funkcija.

---

## 28. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li struktura postaje jasnija ili mutnija?
2. da li smanjuje ili povećava dupliranje?
3. da li pomaže verzionoj disciplini?
4. da li novi saradnik može brže razumjeti repo?
5. da li buduće revizije postaju lakše ili teže?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 29. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `docs/version-status.md`
* `gdd/canonical-decisions.md`
* `GLOSSARY.md`

---

## 30. Završna napomena

**Repository Structure / Struktura repozitorijuma** mora ostati jedan od glavnih infrastrukturnih dokumenata projekta.

Ako radi dobro:

* lakše je znati šta je aktivno
* lakše je uvoditi nove dokumente
* manje se miješaju verzije i draftovi
* revizije i handoff su sigurniji
* a cijeli projekat djeluje ozbiljnije i profesionalnije

Ako radi loše:

* fajlovi se gube
* statusi se miješaju
* razvoj postaje sporiji
* a sve buduće promjene postaju skuplje i haotičnije nego što moraju biti

Zato ovaj dokument mora ostati strog, jasan i potpuno usklađen sa kanonskom logikom **v2.7**.
