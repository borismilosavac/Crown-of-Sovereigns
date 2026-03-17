# iconography-spec.md

# Crown of Sovereigns v2.7 — Iconography Specification / Specifikacija ikonografije

## Status dokumenta

* **Dokument:** `components/iconography-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati pravila, hijerarhiju i standarde za sve ikone koje će se koristiti na tabli, kartama, player board-u, aid materijalima i ostalim komponentama
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Treaty/Sporazum**
* **Povezani dokumenti:** `components/terminology-and-labels.md`, `GLOSSARY.md`, `ux/player-aid-system.md`, `components/player-board-spec.md`, `components/board-spec.md`, `visuals/card-wireframe-notes.md`, `ux/information-hierarchy.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše kako ikonografija treba da funkcioniše u CoS v2.7
* spriječi vizuelni haos i nekontrolisano umnožavanje ikona
* uskladi ikone sa terminologijom, pravilima i onboarding logikom
* olakša rad dizajnerima i budućem grafičkom handoffu
* čuva komponentni i UX kvalitet kroz cijeli projekat

Ovo nije ilustrativni dokument.
Ovo je operativna specifikacija za to kako ikone smiju i ne smiju biti korištene.

---

## 2. Zašto je ikonografija kritična

U ovakvoj igri ikonografija može biti jedan od najvećih UX pojačivača ili jedan od najvećih izvora konfuzije.

Dobra ikonografija:

* ubrzava učenje
* smanjuje tekstualni pritisak
* olakšava čitanje table i karti
* pomaže bržem donošenju odluka

Loša ikonografija:

* zamjenjuje jasnoću sa “vizuelnom pametnošću”
* povećava onboarding težinu
* uvodi slične ikone za različite pojmove
* tjera igrače da stalno provjeravaju aid ili pravila

Zato ikonografija u CoS-u mora biti strogo disciplinovana.

---

## 3. Osnovni princip ikonografije

Glavno pravilo glasi:

> ikona postoji da pojača jasnoću, ne da zamijeni jasnoću prerano.

To znači:

* ikonografija mora pomoći terminu
* ne smije sakriti termin prije nego što je termin naučen
* ne smije nositi više značenja nego što igrač može brzo razlikovati
* ne smije postati “vizuelni sistem za sebe” odvojen od pravila i jezika igre

---

## 4. Šta ikonografija nije

Ikonografija u CoS-u nije:

* ukrasna ilustracija
* dekorativni simbol bez sistemske funkcije
* zamjena za loš wording
* izgovor da se previše pravila ugura na malu površinu
* signal da svaka mala razlika mora dobiti svoju posebnu ikonu

Ako se ikona koristi iz bilo kog od ovih razloga, vjerovatno je pogrešno upotrijebljena.

---

## 5. Glavni ciljevi ikonografskog sistema

Ikonografija mora raditi 5 stvari:

1. pojačati čitljivost
2. smanjiti tekst gdje je to bezbjedno
3. ubrzati prepoznavanje ključnih sistema
4. ostati dosljedna na svim komponentama
5. biti dovoljno jednostavna za onboarding i print/playtest realnost

Ako radi samo drugu stvar bez prve, tekst će biti kraći, ali igra nejasnija.

---

## 6. Hijerarhija ikonografije

Ikonografija u CoS-u mora biti podijeljena po nivou važnosti.

### 6.1. Primarne sistemske ikone

Ikone za najvažnije sisteme i resurse koje igrači vide stalno.

Primjeri:

* **Gold/Zlato**
* **Food/Hrana**
* **Faith/Vjera**
* **Influence/Uticaj**
* **Goods/Roba**
* **Stability/Stabilnost**
* **Unrest/Nemiri**

### 6.2. Sekundarne sistemske ikone

Ikone za važne, ali rjeđe ili kontekstualne pojmove.

Primjeri:

* **Treaty/Sporazum**
* **Contest/Osporavanje**
* **Legitimacy/Legitimnost**
* **Income/Prihod**
* **Development/Razvoj**

### 6.3. Proceduralne ikone

Ikone za faze ili korake.

Primjeri:

* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

### 6.4. Statusne ikone

Ikone za stanja, markere i jasne statusne oznake.

Primjeri:

* **Contested/Osporeno**
* **Active/Aktivno**
* treaty status gdje je relevantno

Kritično pravilo:

> što je ikona važnija i češća, to mora biti jednostavnija i vizuelno stabilnija.

---

## 7. Pravilo ikonografskog budžeta

CoS v2.7 mora imati strogo kontrolisan broj ikona.

To znači:

* ne dodavati novu ikonu osim ako postojeći skup ne može jasno nositi značenje
* svaka nova ikona mora opravdati svoje mjesto kroz stvarni UX dobitak
* ako nova ikona samo malo uljepšava nešto što tekst već rješava, ne treba je uvoditi

Praktično pravilo:

> prvo pokušaj riješiti problem terminom, layoutom ili grupisanjem; tek onda novom ikonom.

---

## 8. Veza sa terminology-and-labels standardom

Ikonografija mora biti potpuno usklađena sa `components/terminology-and-labels.md`.

To znači:

* jedna ikona = jedno stabilno značenje
* ista ikona ne smije značiti dva slična, ali različita termina
* dvojezični termini i ikone moraju raditi zajedno, ne protivno jedno drugom

Ako ikona i label vuku u različitim smjerovima, label ima prednost dok se ikona ne popravi.

---

## 9. Pravilo prvog susreta

Kada se igrač prvi put susreće sa važnim pojmom, preporučeni format je:

* **ikona + puni termin**

Primjeri:

* ikona za **Stability/Stabilnost** uz puni naziv
* ikona za **Goods/Roba** uz puni naziv
* ikona za **Treaty/Sporazum** uz puni naziv

Tek nakon što sistem pretpostavlja da je pojam naučen, može se koristiti:

* ikona + skraćeni label
* ili samo ikona na vrlo ograničenim mjestima, uz aid podršku

---

## 10. Pravilo siluete i razlikovnosti

Svaka ikona mora biti prepoznatljiva po silueti, ne samo po sitnim detaljima.

To znači:

* ne oslanjati se na previše finih linija
* ne oslanjati se na malu razliku u unutrašnjem detalju
* ne koristiti dvije ikone koje iz daljine ili na manjim printovima djeluju skoro isto

Ovo je posebno važno za:

* playtest printove
* manje kartice
* aid referentne blokove
* slabije osvijetljene stolove

---

## 11. Pravilo konzistentnog stila

Sve ikone moraju pripadati istom vizuelnom jeziku.

To znači da moraju dijeliti:

* sličan nivo detalja
* sličnu debljinu linije
* sličan odnos punih i praznih površina
* sličan stepen apstrakcije

Ne smije se desiti da:

* jedna ikona izgleda gotovo realistično
* druga kao ultra-flat geometrija
* treća kao dekorativni heraldic simbol

Takva mješavina izgleda neprofesionalno i usporava učenje.

---

## 12. Pravilo boje i oblikа

Boja smije pomagati ikonografiji, ali ne smije biti jedini nosilac značenja.

To znači:

* ikona mora biti prepoznatljiva i bez boje kad god je moguće
* boja služi za dodatno pojačanje, ne za osnovno razlikovanje
* status ili tip treba idealno razlikovati kombinacijom: oblik + tekst + boja gdje je relevantno

Ovo je posebno važno za:

* pristupačnost
* print testove
* crno-bijele prototipe
* igrače koji boje vide slabije ili drugačije

---

## 13. Primarne ikone resursa i sistema

Ove ikone moraju biti među najstabilnijima i najlakšima za učenje.

### 13.1. **Gold/Zlato**

Mora djelovati kao valuta, bogatstvo i plaćanje.

### 13.2. **Food/Hrana**

Mora djelovati kao osnovna održivost i ishrana.

### 13.3. **Faith/Vjera**

Mora djelovati kao legitimacijska ili simbolička osovina, ne kao magični resurs.

### 13.4. **Influence/Uticaj**

Mora djelovati kao politička i društvena moć, ne kao novac.

### 13.5. **Goods/Roba**

Mora djelovati kao razvoj i proizvodna/trgovačka vrijednost, ne kao puki resurs token.

### 13.6. **Stability/Stabilnost**

Mora djelovati kao unutrašnji red, balans i održivost.

### 13.7. **Unrest/Nemiri**

Mora djelovati kao poremećaj, pritisak i unutrašnja ranjivost.

---

## 14. Ikone za Court Roles / Dvorske uloge

Ikone dvorskih uloga moraju biti posebno pažljivo dizajnirane, jer su među najčešće viđenim identitetskim signalima igre.

### 14.1. **Marshal/Maršal**

Mora signalizirati vojni autoritet, pritisak i mapni konflikt.

### 14.2. **Diplomat/Diplomata**

Mora signalizirati formalnu vezu, sporazum i političku težinu.

### 14.3. **Merchant/Trgovac**

Mora signalizirati trgovinu, goods i razvoj, a ne samo novac.

### 14.4. **Cleric/Klerik**

Mora signalizirati legitimnost, red i stabilizaciju, ne fantasy religijsku magiju.

### 14.5. **Spy/Špijun**

Mora signalizirati prikriveni uticaj, contest i poremećaj, ne opšti haos.

Kritično pravilo:

> dvorske ikone moraju biti lako razlikovive i na prvi pogled, bez potrebe da igrač čita puni naziv svaki put.

---

## 15. Ikone za Treaty klase

Ikonografija za treaty sistem mora jasno razlikovati glavne klase bez pretjerane sličnosti.

### 15.1. **Alliance/Savez**

Mora signalizirati jači politički odnos i obavezu.

### 15.2. **Truce/Primirje**

Mora signalizirati obustavu ili ograničenje sukoba.

### 15.3. **Trade Pact/Trgovački pakt**

Mora signalizirati razmjenu, goods vrijednost i formalnu saradnju.

Ako ove tri ikone djeluju previše slično, diplomatski sloj postaje sporiji za čitanje.

---

## 16. Ikone za proceduralne korake

Proceduralne ikone treba koristiti štedljivo i uvijek uz veoma jasan kontekst.

### Koraci

* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

Njihova uloga je da:

* ubrzaju podsjećanje
* podrže aid i combat reference
* pojačaju sekvencu

Ne smiju postati dodatni sloj koji komplikuje faze više nego što pomaže.

---

## 17. Ikone za završne i posebne sisteme

Posebni sistemi poput:

* **Legitimacy/Legitimnost**
* **Contest/Osporavanje**
* **Coronation Attempt/Pokušaj krunisanja**

moraju imati ikonografiju koja je:

* dovoljno posebna da se osjeti važnost
* ali i dalje u istom sistemu jednostavnosti

Ovdje je posebno opasno pretjerati sa heraldikom, ornamentalnošću i “epic” simbolima koji djeluju lijepo, ali nečitljivo.

---

## 18. Pravilo teksta uz ikonu na važnim komponentama

Na važnim komponentama kao što su:

* player board
* aid
* treaty kartice
* završni reference elementi

ikona po pravilu treba da ide uz tekst, barem dok igrač nije već u duboko naučenom dijelu partije.

Pravilo glasi:

* važnost sistema raste → raste i potreba za potvrdom ikone tekstom

---

## 19. Pravilo veličine i minimalne čitljivosti

Svaka ikona mora imati definisan minimalni prag čitljivosti.

To znači da mora ostati prepoznatljiva kada je:

* smanjena na malu veličinu na karti
* odštampana na prosječnom prototip štampaču
* viđena pod uglom na stolu

Ako ikona radi samo u velikoj, savršenoj prezentaciji, ne pripada stvarnoj board game produkciji.

---

## 20. Pravilo za aid i player board prioritet

Na aid i player board komponentama prednost imaju:

* najvažnije sistemske ikone
* najčešće korištene proceduralne ikone
* ikone koje direktno smanjuju lookup vrijeme

Ne treba koristiti previše rijetkih ili ukrasnih ikona na ovim površinama.

---

## 21. Najčešće greške u ikonografiji

* previše ikona za previše sitnih pojmova
* dvije različite ikone za isti pojam
* ista ili veoma slična ikona za dva različita pojma
* oslanjanje na boju bez dovoljno različitog oblika
* dekorativna ikonografija koja izgleda lijepo, ali ne čita dobro
* ikona bez teksta tamo gdje igrač još ne zna značenje
* ikonografija koja nije dosljedna između table, aid-a i karata

---

## 22. Workflow pravilo za novu ikonu

Ako se predlaže nova ikona, mora se provjeriti redom:

1. da li pojam već ima postojeću ikonu
2. da li problem može riješiti bolji label ili layout
3. da li nova ikona unosi stvarni UX dobitak
4. da li je razlikoviva od svih postojećih ikona
5. da li je održiva kroz tablu, kartu, aid i print test
6. da li je usklađena sa `components/terminology-and-labels.md`

Ako ne prolazi ova pitanja, nova ikona se ne uvodi.

---

## 23. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li povećava ili smanjuje čitljivost?
2. da li smanjuje ili povećava onboarding težinu?
3. da li održava isti vizuelni jezik?
4. da li je kompatibilna sa terminologijom i label standardom?
5. da li uvodi nepotreban ikonografski bloat?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 24. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/player-board-spec.md`
* `components/board-spec.md`
* `ux/player-aid-system.md`
* `visuals/card-wireframe-notes.md`
* `ux/information-hierarchy.md`
* `components/terminology-and-labels.md`

Ako ikonografija nije zaključana prije ozbiljne grafičke faze, kasnije će gotovo sigurno doći do:

* redizajna aid-a
* razbijenog layouta karti
* skupih iteracija na tabli
* neujednačenih print testova

---

## 25. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/terminology-and-labels.md`
* `GLOSSARY.md`
* `content/court-roles.md`
* `content/treaties-list.md`
* `content/goods-list.md`
* `ux/player-aid-system.md`
* `components/player-board-spec.md`
* `components/board-spec.md`
* `visuals/card-wireframe-notes.md`

---

## 26. Završna napomena

**Iconography Specification / Specifikacija ikonografije** je jedan od glavnih UX temelja projekta.

Ako radi dobro:

* igra se brže čita
* onboarding je lakši
* komponente djeluju profesionalnije
* pravila postaju lakša za praćenje
* grafički handoff postaje sigurniji

Ako radi loše:

* igra djeluje složenije nego što jeste
* aid i karta postaju teži za korištenje
* pravila izgledaju mutnije
* a dizajn plaća cijenu kroz beskrajne mikro-ispravke

Zato ovaj dokument mora ostati strogo kontrolisan i stalno usklađen sa cijelim jezičkim i sistemskim slojem **v2.7**.
