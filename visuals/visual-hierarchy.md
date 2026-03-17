# visual-hierarchy.md

# Crown of Sovereigns v2.7 — Visual Hierarchy / Vizuelna hijerarhija

## Status dokumenta

* **Dokument:** `visuals/visual-hierarchy.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati kanonsku hijerarhiju vidljivosti, prioriteta i vizuelne pažnje za sve glavne slojeve igre: **Board/Tablu**, **Player Boards/Table igrača**, **Cards/Karte**, **Tokens/Tokene**, **Units/Jedinice**, **Markers/Markere** i aid materijale
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Visual Hierarchy/Vizuelna hijerarhija**, **Primary/Primarno**, **Secondary/Sekundarno**, **Tertiary/Tercijarno**
* **Povezani dokumenti:** `visuals/art-direction.md`, `visuals/board-wireframe-notes.md`, `visuals/card-wireframe-notes.md`, `ux/information-hierarchy.md`, `components/board-spec.md`, `components/player-board-spec.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `gdd/crown-of-sovereigns-v2.7-gdd.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* zaključa šta u igri mora prvo privlačiti pažnju, šta drugo, a šta tek treće
* spriječi da svi sistemi pokušaju biti jednako glasni u istom trenutku
* uskladi art direction, wireframe logiku, ikonografiju i UX u jedan jasan sistem prioriteta
* pomogne da tabla, table igrača, karte i aid materijali budu skenabilni pod stvarnim stolnim uslovima
* zaštiti CoS od vizuelne konfuzije u kojoj važni signali tonu među dekoracijom i sekundarnim informacijama

Ovo nije dokument o estetici sam po sebi.
Ovo je dokument o tome kako pažnja igrača mora biti vođena kroz vizuelni sistem igre.

---

## 2. Zašto je vizuelna hijerarhija kritična

Kod kompleksnije strateške igre najveći vizuelni problem nije nužno “ružnoća”, nego to što igrač ne zna:

* gdje prvo da gleda
* šta je trenutno najvažnije
* koja informacija je centralna, a koja samo pomoćna
* kada vizuelni signal znači državni, politički ili završni prioritet

Ako vizuelna hijerarhija radi loše:

* igra djeluje težom nego što jeste
* downtime raste jer ljudi traže informacije duže nego što bi morali
* novi igrači ne osjećaju šta je važno
* čak i dobar art i dobar sistem počinju da rade jedan protiv drugog

Zato vizuelna hijerarhija mora biti jedna od najstrožih disciplina u cijelom projektu.

---

## 3. Osnovni princip vizuelne hijerarhije

Glavno pravilo glasi:

> u svakom trenutku igrač mora moći brzo razlikovati: šta je trenutno centralni signal igre, šta je podrška odluci i šta je samo pozadinska ili referentna informacija.

To znači da CoS vizuelni sistem mora uvijek praviti razliku između:

* **Primary/Primarno** — ono što igrač prvo mora vidjeti
* **Secondary/Sekundarno** — ono što pomaže odluci odmah nakon toga
* **Tertiary/Tercijarno** — ono što je korisno, ali ne smije upadati prije važnijih stvari

Ako se ta tri sloja pomiješaju, igra gubi čitljivost i identitet.

---

## 4. Šta visual hierarchy jeste

Ovaj dokument treba da bude:

* centralni vizuelni prioritetni okvir
* most između UX i art direction logike
* alat za evaluaciju table, karti, aidova i markera
* guardrail protiv “sve je važno” dizajna

---

## 5. Šta visual hierarchy nije

Ovaj dokument nije:

* detaljan layout dokument
* zamjena za wireframe specifikacije
* samo lista boja ili font veličina
* estetski komentar bez sistemske funkcije

Ovdje nije tema samo “kako nešto izgleda”, nego “kako pažnja treba da teče”.

---

## 6. Tri nivoa hijerarhije

### 6.1. Primary / Primarno

Informacije i signali koje igrač mora vidjeti prvo i bez traženja.

### 6.2. Secondary / Sekundarno

Informacije koje odmah pomažu razumjeti ili riješiti primarni signal.

### 6.3. Tertiary / Tercijarno

Informacije koje su korisne, ali ne smiju konkurisati prvim dvjema grupama.

Ova tri nivoa moraju postojati na:

* tabli
* tabli igrača
* kartama
* aid materijalima
* markerima i tokenima

---

## 7. Global primary signals / Globalni primarni signali

Na nivou cijele igre, sljedeće stvari moraju gotovo uvijek imati pravo na primarnu vidljivost:

* trenutni zajednički kontekst runde
* prostori i statusi koji su **Contested/Osporeni**
* najvažniji **Court/Dvor** signal igrača tamo gdje utiče na tok runde
* kritični **Stability/Stabilnost** i **Unrest/Nemiri** pragovi
* završni i **Coronation Attempt/Pokušaj krunisanja** signali kada postanu aktivni

Ako bilo koji od ovih elemenata vizuelno izgubi utrku od dekoracije ili manjih podsjetnika, hijerarhija je loša.

---

## 8. Global secondary signals / Globalni sekundarni signali

Sekundarni signali na nivou cijele igre treba da budu:

* active **Treaty/Sporazum** odnosi
* goods i razvojni indikatori koji hrane odluku
* kontrolni markeri i prostorni statusi koji objašnjavaju zašto je nešto contested ili važno
* redoslijed, inicijativa ili proceduralni podsjetnici relevantni za tu rundu

Oni moraju biti lako dostupni, ali ne smiju preglasati primarne političke i završne signale.

---

## 9. Global tertiary signals / Globalni tercijarni signali

Tercijarni signali su:

* dekorativne teksture
* sekundarni oznakovni okviri
* flavor ilustrativni elementi
* rijetko korištene referentne napomene
* rubne informacije koje nisu dio trenutne odluke

Oni smiju obogatiti proizvod, ali ne smiju biti prvi sloj pažnje.

---

## 10. Board/Tabla hierarchy / Hijerarhija na tabli

### 10.1. Primary na tabli

Na glavnoj tabli primarno moraju biti vidljivi:

* **Provinces/Provincije** kao čitljive teritorijalne jedinice
* contested prostori i važni mapni pritisci
* završna / coronation zona kada postane relevantna
* zajednički rundni kontekst ako živi na tabli

### 10.2. Secondary na tabli

Sekundarno treba da budu vidljivi:

* kontrolni markeri
* prostorni modifikatori i povezane zone
* diplomatski ili event/currency signali koji utiču na čitanje prostora

### 10.3. Tertiary na tabli

Tercijarno treba da budu:

* dekorativna pozadinska karta
* heraldički ili istorijski stilizovani detalji
* rubni ukrasi i ornamentalne linije

Glavni guardrail:

* tabla nikad ne smije izgledati kao ilustracija preko koje je kasnije “nalijepljen” gameplay.

---

## 11. Player Board hierarchy / Hijerarhija na tabli igrača

### 11.1. Primary na tabli igrača

Primarno moraju biti vidljivi:

* **Court/Dvor** fokus i glavna lična upravna odluka
* **Stability/Stabilnost** stanje i alarmni pragovi
* ključni goods / razvojni statusi koji direktno hrane odluku

### 11.2. Secondary na tabli igrača

Sekundarno treba da budu:

* pomoćni track-ovi
* podsjetnici za lične efekte
* pozicije koje pomažu narednim akcijama, ali nisu alarmne ili centralne

### 11.3. Tertiary na tabli igrača

Tercijarno treba da budu:

* dekorativni okviri
* pozadinske teksture
* flavor simboli koji ne nose ključnu odluku

Glavni guardrail:

* player board ne smije djelovati kao administrativna knjigovodstvena ploča gdje ništa nije dovoljno važno na prvi pogled.

---

## 12. Court/Dvor hierarchy / Hijerarhija dvora

Pošto je **Court/Dvor** centralni identitetski sistem, njegova hijerarhija mora biti posebno jasna.

### Primary

* glavni dvorski fokus te runde
* trenutno aktivna ili presudna dvorska odluka

### Secondary

* povezani pomoćni efekti ili uslovi
* podsjetnici za redoslijed ili posljedicu

### Tertiary

* dekorativna heraldika, politički ornament i flavor detalji

Ako dvor vizuelno djeluje kao isti nivo kao i obični pomoćni moduli, art i UX su promašili identitet igre.

---

## 13. Stability/Stabilnost hierarchy / Hijerarhija stabilnosti

### Primary

* trenutna pozicija **Stability/Stabilnost**
* zone sigurnosti, napetosti i rizika
* prisustvo ozbiljnog **Unrest/Nemiri** signala

### Secondary

* manji modifikatori ili pomoćne napomene koje objašnjavaju uzrok ili posljedicu

### Tertiary

* dekorativni background trake ili flavor teksture

Glavni guardrail:

* **Stability/Stabilnost** mora djelovati kao živi politički signal, ne kao mala tehnička brojka na sporednom rubu.

---

## 14. Diplomacy hierarchy / Hijerarhija diplomatije

### Primary

* aktivni formalni **Treaty/Sporazum** odnos
* stanje raskida ili aktivne političke napetosti ako je direktno relevantno

### Secondary

* uslovi, benefiti i obaveze sporazuma
* podsjetnici za trajanje ili specifične posljedice

### Tertiary

* dekorativni pečati, ornamenti i flavor elementi

Glavni guardrail:

* diplomatija mora izgledati formalno i važno, ali ne smije se pretvoriti u pravnu tablicu koja guši ostatak vizuelnog sistema.

---

## 15. Cards/Karte hierarchy / Hijerarhija karata

Na kartama mora vrijediti ista logika.

### Primary na karti

* tip karte
* naziv karte
* glavni efekat ili glavni politički sadržaj

### Secondary na karti

* trajanje
* uslov
* posljedica ili dodatna obaveza

### Tertiary na karti

* flavor art detalj
* atmosferski tekst gdje postoji
* sekundarni ukrasni elementi

Najvažnije pravilo:

* ilustracija i okvir ne smiju pobijediti glavni efekat u utrci za pažnju.

---

## 16. Event vs Crisis visual priority / Prioritet događaja naspram krize

Pošto CoS koristi i **Event/Događaj** i **Crisis/Kriza** sloj, njihova hijerarhija mora biti jasna.

* **Event/Događaj** treba da djeluje kao zajednički kontekst
* **Crisis/Kriza** treba da djeluje ozbiljnije i alarmnije od običnog događaja

Ako event i crisis izgledaju isto ili gotovo isto, igrači teže osjećaju skok u ozbiljnosti i političkom pritisku.

---

## 17. Endgame and Coronation hierarchy / Hijerarhija završnice i krunisanja

Kad završni dio partije postane aktivan, hijerarhija se mora djelimično pomjeriti.

### Primary

* **Coronation Attempt/Pokušaj krunisanja** status
* glavni završni contested signal
* elementi koji direktno govore “partija je sada u završnom legitimacijskom testu”

### Secondary

* pomoćni bodovni ili proceduralni podsjetnici završnice
* dodatni statusi koji objašnjavaju contest

### Tertiary

* sve dekorativno i flavor što ne nosi direktnu završnu informaciju

Glavni guardrail:

* završnica mora pojačati fokus, ali ne smije stvoriti vizuelni haos koji guta ostatak stanja partije.

---

## 18. Units/Jedinice and Markers/Markeri hierarchy / Hijerarhija jedinica i markera

### Primary

* prisutnost gdje direktno mijenja mapni pritisak
* **Contested/Osporeno** statusi
* kontrolni signali kada odlučuju prostor

### Secondary

* pomoćni ili proceduralni status markeri
* manje hitni podsjetnici

### Tertiary

* dekorativna forma komada koja ne nosi dodatnu gameplay informaciju

Pravilo:

* figura ili marker ne smije biti fizički atraktivniji nego čitljiviji. Silueta i funkcija moraju pobijediti dekorativni višak.

---

## 19. Aid hierarchy / Hijerarhija aid materijala

**Player Aid/Pomoćni igrački vodič** mora imati brutalno jasnu hijerarhiju.

### Primary

* kičma runde
* glavne faze i redoslijed
* najvažniji završni i bodovni podsjetnici

### Secondary

* kratki podsjetnici za ključne sisteme
* sažeti uslovi i upozorenja

### Tertiary

* objašnjenja koja nisu nužna za svaku rundu
* flavor ili estetski detalji

Aid mora biti alat, ne mini-poster.

---

## 20. Typography and scale logic / Logika tipografije i skale

Iako ovaj dokument ne zaključava finalne fontove, zaključava logiku:

* primarne informacije moraju imati najjaču vizuelnu težinu
* sekundarne informacije moraju biti čitljive, ali manje dominantne
* tercijarne informacije moraju ostati dostupne bez ulaska u centralni tok pažnje

Skala, kontrast i raspored moraju raditi zajedno.
Nije dovoljno samo “uvećati naslov” ako ostatak sistema ostaje hijerarhijski mutan.

---

## 21. Contrast and emphasis logic / Logika kontrasta i naglaska

Kontrast se mora koristiti štedljivo i namjenski.

To znači:

* najjači kontrast za najvažnije signale
* umjeren kontrast za sekundarne zone
* tihi kontrast za tercijarne slojeve

Ako se najjači kontrast koristi preširoko, hijerarhija se raspada i sve postaje jednako glasno.

---

## 22. Relationship to information hierarchy / Odnos prema informacionoj hijerarhiji

Ovaj dokument mora ostati usklađen sa:

* `ux/information-hierarchy.md`

Pravilo je:

* **information hierarchy/informaciona hijerarhija** definiše logiku šta je važno
* **visual hierarchy/vizuelna hijerarhija** definiše kako se ta važnost vidi

Ako se ta dva sloja raziđu, igra će reći jedno pravilima, a drugo očima igrača.

---

## 23. Relationship to art direction / Odnos prema umjetničkom smjeru

Ovaj dokument mora biti usklađen sa:

* `visuals/art-direction.md`

Art direction definiše ton.
Visual hierarchy definiše red pažnje.

Ako ton naruši red pažnje, hijerarhija ima prednost dok se ne nađe bolji kompromis.

---

## 24. Relationship to wireframes / Odnos prema wireframe dokumentima

Wireframe dokumenti su mjesta gdje se ova hijerarhija pretvara u konkretan raspored.

Zato ovaj dokument mora biti usklađen sa:

* `visuals/board-wireframe-notes.md`
* `visuals/card-wireframe-notes.md`

Visual hierarchy ne smije ostati teorijski sloj. Mora biti direktno primjenjiva na layout odluke.

---

## 25. Main visual hierarchy risks / Glavni rizici vizuelne hijerarhije

Najveći rizici koje ovaj dokument mora spriječiti su:

* da sve izgleda podjednako važno
* da dekoracija pojede gameplay signal
* da **Court/Dvor** ne dobije dovoljan vizuelni prioritet
* da **Stability/Stabilnost** djeluje sporedno
* da završni i coronation signal kasno djeluje previše tih ili odjednom previše glasan
* da kartice i aid materijali budu lijepi, ali spori za skeniranje

---

## 26. Workflow pravilo za novu hijerarhijsku odluku

Ako se predlaže velika promjena u vizuelnoj hijerarhiji, treba provjeriti redom:

1. šta će igrač sada prvo vidjeti
2. da li je to zaista najvažniji signal
3. šta je potisnuto na drugi i treći nivo
4. da li promjena pomaže ili odmaže toku runde i donošenju odluka
5. da li ostaje kompatibilna sa art direction, wireframe i UX logikom

Ako ne prolazi ova pitanja, promjena nije dobra za CoS.

---

## 27. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li hijerarhija ostaje jasna?
2. da li i dalje razlikuje primarno, sekundarno i tercijarno bez sivih zona?
3. da li ostaje usklađena sa art direction i UX logikom?
4. da li pojačava ili slabi politički i državni identitet igre?
5. da li smanjuje ili povećava vizuelni haos i lookup trenje?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 28. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `visuals/art-direction.md`
* `visuals/board-wireframe-notes.md`
* `visuals/card-wireframe-notes.md`
* `ux/information-hierarchy.md`
* `components/board-spec.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `gdd/crown-of-sovereigns-v2.7-gdd.md`
* `GLOSSARY.md`

---

## 29. Završna napomena

**Visual Hierarchy / Vizuelna hijerarhija** mora ostati jedan od glavnih zaštitnih dokumenata protiv vizuelnog i UX haosa u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* igra se čita brže
* važni signali iskaču kada treba
* aid i tabla djeluju koherentnije
* art direction i UX rade zajedno
* a proizvod djeluje ozbiljnije, čistije i profesionalnije

Ako radi loše:

* igra izgleda bogatije nego što je čitljiva
* nova grupa ne zna gdje da gleda
* downtime raste zbog čistog lookup tereta
* a najvažniji sistemi gube dio svoje snage samo zato što nisu dovoljno dobro vizuelno rangirani

Zato ovaj dokument mora ostati strog, operativan i potpuno usklađen sa logikom **v2.7**.
