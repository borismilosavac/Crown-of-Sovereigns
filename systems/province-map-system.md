# province-map-system.md

# Crown of Sovereigns v2.7 — Province Map System / Sistem mape i provincija

## Status dokumenta

* **Dokument:** `systems/province-map-system.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** detaljno objasniti kako funkcionišu **Provinces/Provincije**, teritorijalna kontrola, mapni pritisak i prostorna logika igre
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Cleric/Klerik**
* **Povezani dokumenti:** `gdd/crown-of-sovereigns-v2.7-gdd.md`, `rules/rules-reference-v2.7.md`, `rules/setup-guide.md`, `systems/combat-system.md`, `systems/goods-and-development.md`, `systems/scaling-2p-3p-4p.md`, `components/board-spec.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument objašnjava:

* šta znači **Province/Provincija** u CoS sistemu
* kako mapa funkcioniše kao stvarni mehanički prostor
* kako se ostvaruje teritorijalna kontrola
* kako su teritorija, goods, rat, politika i stabilnost povezani
* zašto mapa ne smije biti samo pozadina za druge sisteme

Ovo nije samo opis table.
Ovo je sistemski dokument o prostornoj logici igre.

---

## 2. Zašto mapa postoji

Mapa u **Crown of Sovereigns v2.7** postoji da bi igra imala:

* stvaran geopolitički prostor
* teritorijalni pritisak
* logistički smisao rasta
* prostornu osnovu za goods, rat i diplomatiju
* osjećaj da kraljevstvo zauzima i brani stvarni svijet, a ne apstraktan skup bodova

Ako mapa ne nosi stvarnu mehaničku vrijednost, igra gubi dio identiteta i lako se pretvara u tabelarni engine sa dekorativnom tablom.

---

## 3. Osnovna definicija Provinces/Provincije

**Province/Provincija** je osnovna teritorijalna jedinica na tabli.

Svaka **Province/Provincija** može imati jednu ili više od sljedećih funkcija:

* prostornu / položajnu vrijednost
* resursnu vrijednost
* **Goods/Roba** vezu ili razvojnu vrijednost
* odbrambenu ili napadačku važnost
* politički ili diplomatski značaj
* završnu bodovnu važnost

Kritično pravilo:

> Provincija nikad ne smije biti samo prazno polje između dvije druge važne stvari.

---

## 4. Broj provincija

U v2.7 osnovna tabla koristi:

> **24 Provinces/24 Provincije**

Ova brojka je zaključana na nivou aktivne verzije i koristi se kao osnov za:

* board-spec
* setup pakete
* skaliranje
* scoring logiku
* komponentne potrebe

Ako bi se taj broj mijenjao, to više ne bi bila usputna korekcija, nego nova verziona odluka.

---

## 5. Šta dobra provincijska mapa mora raditi

Dobra mapa u CoS mora raditi 6 stvari:

1. stvarati teritorijalne odluke
2. stvarati prostorni pritisak
3. omogućiti da ekspanzija bude i prilika i rizik
4. podržati više puteva do pobjede
5. biti čitljiva za stolom
6. ostati pogodna za grafički handoff bez haotične ikonografije

Ako ne radi ovo, mapa postaje ili previše ravna ili previše komplikovana.

---

## 6. Osnovna uloga provincije u partiji

Provincija može biti važna iz različitih razloga:

### 6.1. Ekonomski razlog

Daje resurs, goods vezu ili income vrijednost.

### 6.2. Vojni razlog

Otvara ofanzivni pravac, brani granicu ili stvara stratešku dubinu.

### 6.3. Politički razlog

Pomaže legitimitetu, poziciji ili pritisaku na druge igrače.

### 6.4. Razvojni razlog

Omogućava da goods ili razvojna putanja imaju smisla.

### 6.5. Završni razlog

Učestvuje u završnom **Scoring/Bodovanje** okviru i može odlučiti tijesnu partiju.

---

## 7. Province identity / Identitet provincije

Sve provincije ne moraju biti iste, ali moraju biti dosljedno dizajnirane.

To znači:

* provincije mogu imati različitu funkciju
* ali te razlike moraju biti čitljive
* ne smiju stvarati memorijski haos
* ne smiju uvoditi desetine sitnih izuzetaka

Provincijska raznolikost treba da stvara strateški izbor, ne pravilaški teret.

---

## 8. Mapa i Court/Dvor veza

Mapa ne postoji odvojeno od **Court/Dvor** sistema.

### 8.1. **Marshal/Maršal**

Mapa je njegov prirodni prostor za ekspanziju, prijetnju i kontrolu.

### 8.2. **Merchant/Trgovac**

Mapa daje goods i trgovački smisao. Bez teritorijalne logike goods sistem slabi.

### 8.3. **Diplomat/Diplomata**

Mapa daje politički kontekst sporazumima: susjedstvo, tampon-zone, trgovačke veze i prijetnje.

### 8.4. **Cleric/Klerik**

Mapa utiče na to gdje unutrašnja stabilnost najviše trpi i gdje legitimitet treba braniti.

### 8.5. **Spy/Špijun**

Mapa daje geografski kontekst za ciljani pritisak i narušavanje planova.

Drugim riječima:

> mapa i dvor moraju raditi zajedno.

---

## 9. Kontrola provincije

### 9.1. Osnovna definicija

Igrač kontroliše **Province/Provinciju** kada ispunjava sve uslove kontrole definisane pravilima i kada ta kontrola nije osporena ili izgubljena prije relevantnog scoring trenutka.

### 9.2. Šta kontrola znači

Kontrola znači da provincija može dati:

* resursni benefit
* goods ili razvojni benefit
* stratešku poziciju
* scoring vrijednost
* političku ili završnu težinu

### 9.3. Šta ne znači

Kontrola ne znači da je pozicija automatski sigurna.
Provincija može biti pod pritiskom, logistički ranjiva ili politički skupa za održavanje.

---

## 10. Prostorni pritisak / Map pressure

**Map Pressure/Pritisak na mapi** znači koliko prisustvo igrača utiče na odluke drugih zbog same prostorne konfiguracije.

Dobar map pressure nastaje kada:

* teritorija prijeti važnim pravcima
* ekspanzija otvara i rizik i priliku
* protivnici moraju reagovati na raspored snaga
* neutralni ili granični prostori nisu ravnodušni

Loš map pressure izgleda ovako:

* igrači se šire bez stvarnog sudara interesa
* sve provincije vrijede skoro isto
* položaj nije važan koliko samo broj osvojenih polja

---

## 11. Ekspanzija / Expansion

### 11.1. Svrha ekspanzije

Ekspanzija omogućava rast, pozicioni pritisak i pristup novim vrijednostima.

### 11.2. Rizik ekspanzije

U CoS ekspanzija nikad ne smije biti potpuno besplatna.
Širenje mora potencijalno povećavati:

* vojni pritisak
* logističku ranjivost
* političku izloženost
* **Stability/Stabilnost** trošak

### 11.3. Dizajnerski cilj

Ekspanzija treba da bude privlačna, ali ne automatski optimalna u svakom trenutku.

---

## 12. Mapa i Goods/Roba odnos

Mapa mora podržavati goods sistem na prirodan način.

To znači:

* neke **Provinces/Provincije** treba da imaju jaču goods ili razvojnu važnost
* teritorijalna kontrola treba da utiče na ekonomsku putanju
* goods put ne smije biti potpuno odvojen od prostora

Ako goods razvoj može u potpunosti ignorisati mapu, teritorijalni i ekonomski sloj se previše razdvajaju.

---

## 13. Mapa i diplomatija

Mapa daje diplomatiji težinu.

Diplomatija je zanimljivija kada postoji stvaran razlog za sporazum, npr.:

* tampon-zona
* granica pod pritiskom
* trgovački pravac
* potreba da se obuzda lider
* politička trgovina prostorom i vremenom

Bez prostorne logike diplomatija lako postaje samo meki bonus layer.

---

## 14. Mapa i Stability/Stabilnost

Što je kraljevstvo veće i ambicioznije, to upravljanje mapom više utiče na:

* unutrašnje naprezanje
* nemire
* ranjivost na krizu
* opasnost od pretjeranog širenja

To je važno jer CoS ne želi da teritorija bude samo nagrada bez sistemske cijene.

---

## 15. Mapa i završnica

Dobra završnica zavisi i od mape.

Mapa mora omogućiti:

* kasne pokušaje presijecanja bodovne razlike
* politički i vojni contest važnih zona
* napet završni teritorijalni obračun
* mogućnost da nekoliko ključnih provincija odluči tijesnu partiju

Ako kraj partije ne zavisi dovoljno od prostorne pozicije, završnica može postati suviše tabelarna.

---

## 16. 2P mapa i Crown Pressure / Pritisak krune

### 16.1. Problem 2P mape

U 2P modu nema prirodnog trećeg aktera koji usporava runaway lidera.

### 16.2. Rješenje u v2.7

Zato 2P koristi poseban **Crown Pressure/Pritisak krune** okvir koji targetira lidera.

### 16.3. Šta to znači za mapu

Mapa u 2P mora ostati:

* dovoljno otvorena da ima strategiju
* dovoljno kontrolisana da jedan rani prodor ne presudi partiju prebrzo

### 16.4. Dizajnerska posljedica

2P nije posebna mini-igra, ali mapa u 2P mora biti pažljivije podešena nego u 3P / 4P.

---

## 17. 3P i 4P mapa

### 17.1. 3P

U 3P mapa često daje najčistiju političku dinamiku jer su svi prisiljeni da prate međusobni balans prostora.

### 17.2. 4P

U 4P mapa mora podržati širi diplomatski prostor bez kolapsa u gužvu i bez pretvaranja svake runde u predug teritorijalni nered.

### 17.3. Skaliranje princip

Broj igrača smije mijenjati intenzitet pritiska, ali ne smije promijeniti osnovni identitet mape.

---

## 18. Čitljivost mape

Mapa mora biti vizuelno i mehanički čitljiva.

To znači:

* susjedstva moraju biti jasna
* kontrola mora biti vidljiva
* goods i posebne vrijednosti ne smiju zatrpati prostor
* boje i ikonografija moraju ostati disciplinovane
* važna područja moraju biti uočljiva bez prevelikog vizuelnog šuma

Ovaj sistem direktno utiče na kasniji **board-spec** i **visual hierarchy** rad.

---

## 19. Province value balans

Sve provincije ne moraju biti potpuno jednake, ali nijedna ključna provincija ne smije biti toliko premoćna da sama presudi partiju bez odgovora.

Balans dobrog provincijskog sistema znači:

* postoji nekoliko važnih zona
* ali ne postoji jedna “obavezna” provincija koja uvijek odlučuje pobjednika
* razne putanje igre mogu cijeniti različite prostore iz različitih razloga

---

## 20. Najčešće greške u mapnom sistemu

* previše ravne provincije bez identiteta
* previše specijalnih slučajeva po provinciji
* goods i teritorija potpuno odvojeni
* stabilnost nema veze sa veličinom i rasporedom carstva
* mapa je bitna samo na početku ili samo na kraju, ali ne kroz cijelu partiju
* 2P prostor previše rano otvara runaway liniju

---

## 21. Pravila za buduće izmjene mape

Svaka promjena mape mora proći ovu provjeru:

1. da li povećava ili smanjuje prostorni pritisak?
2. da li jača mapu kao stvarni stub ili je svodi na dekoraciju?
3. da li pomaže više putanja do pobjede ili samo agresivnoj ekspanziji?
4. da li komplikuje setup?
5. da li uvodi previše ikonografije?
6. da li šteti 2P ili 4P ravnoteži?

Ako promjena pada na ovim pitanjima, vjerovatno nije dobar tuning korak.

---

## 22. Veza sa grafičkim handoffom

Mapni sistem direktno utiče na:

* `components/board-spec.md`
* `components/iconography-spec.md`
* `visuals/board-wireframe-notes.md`
* `visuals/visual-hierarchy.md`
* `ux/information-hierarchy.md`

Ako ovaj dokument nije čist, grafička izrada table gotovo sigurno postaje skuplja i konfuznija.

---

## 23. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `rules/rules-reference-v2.7.md`
* `rules/setup-guide.md`
* `rules/scoring-reference.md`
* `systems/combat-system.md`
* `systems/goods-and-development.md`
* `systems/scaling-2p-3p-4p.md`
* `components/board-spec.md`
* `components/iconography-spec.md`
* `visuals/board-wireframe-notes.md`

---

## 24. Završna napomena

**Province Map System / Sistem mape i provincija** je jedan od glavnih razloga zašto Crown of Sovereigns djeluje kao stvarna igra vođenja kraljevstva, a ne samo kao apstraktni engine.

Ako radi dobro:

* mapa stalno proizvodi odluke
* ekspanzija je uzbudljiva i rizična
* goods, rat, politika i stabilnost ostaju povezani
* završnice dobijaju prostorni smisao

Ako radi loše:

* teritorija postaje brojka
* goods postaju odvojeni spreadsheet
* rat postaje ili prejak ili besmislen
* a politički identitet igre slabi

Zato ovaj sistem mora ostati strogo usklađen sa ostatkom jezgra v2.7.
