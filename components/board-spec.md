# board-spec.md

# Crown of Sovereigns v2.7 — Board Specification / Specifikacija glavne table

## Status dokumenta

* **Dokument:** `components/board-spec.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati funkciju, sadržaj, zone i UX pravila za glavnu tablu igre
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Board/Tabla**, **Provinces/Provincije**, **Treaty/Sporazum**
* **Povezani dokumenti:** `systems/province-map-system.md`, `rules/setup-guide.md`, `rules/turn-structure.md`, `systems/diplomacy-and-treaties.md`, `systems/event-and-crisis-system.md`, `systems/coronation-system.md`, `components/terminology-and-labels.md`, `components/iconography-spec.md`, `ux/information-hierarchy.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše šta glavna **Board/Tabla** mora sadržavati
* odredi koje informacije pripadaju glavnoj tabli, a koje ne
* spriječi vizuelni i komponentni bloat na najvažnijoj površini igre
* uskladi mapu, zajedničke trake i referentne zone sa stvarnim gameplay tokom
* pripremi stabilan osnov za grafički handoff i prototip štampu

Ovo nije ilustrativna vizija table.
Ovo je operativna specifikacija za centralnu komponentu cijele igre.

---

## 2. Zašto je glavna tabla kritična

U CoS v2.7 glavna tabla nosi najveći dio zajedničke čitljivosti partije.
Ona mora pomoći da svi za stolom brzo vide:

* stanje mape
* zone pritiska
* zajedničke sisteme koji utiču na rundu
* politički i završni kontekst partije

Ako glavna tabla radi loše:

* mapa djeluje manje važna nego što jeste
* diplomatija djeluje manje vezana za prostor
* krize i događaji djeluju odvojeno od stola
* završnica gubi preglednost

Zato **Board/Tabla** mora biti sistemski alat, ne samo scena za ilustraciju.

---

## 3. Osnovni princip dizajna table

Glavno pravilo glasi:

> glavna tabla mora prije svega prikazivati zajedničko stanje partije, a ne pokušavati nositi svu dokumentaciju igre na jednoj površini.

To znači:

* tabla mora prikazati ono što svi igrači stalno gledaju
* ne treba duplicirati ono što je bolje riješeno na **Player Board/Tabli igrača** ili aid-u
* ne treba uvoditi zone samo zato što “ima mjesta”

Svaka zona table mora opravdati svoje postojanje kroz stvarni gameplay dobitak.

---

## 4. Šta glavna tabla jeste

Glavna tabla treba da bude:

* zajednički prostorni i politički centar partije
* mjesto gdje mapa ima prvenstvo
* mjesto gdje su zajednički pritisci i javni sistemi jasno vidljivi
* stabilna vizuelna osovina oko koje se ostale komponente prirodno raspoređuju

---

## 5. Šta glavna tabla nije

Glavna tabla ne smije biti:

* poster pun sitnih pravila
* skladište za sve moguće tokene i sve moguće podsjetnike
* vizuelno prenatrpan prostor koji guta mjerilo mape
* mjesto gdje dekoracija i heraldika sakrivaju funkcionalne granice i zone
* komponenta koja zahtijeva da igrač stalno naginje glavu i traži mikrotekst

Ako tabla sklizne u bilo šta od ovoga, gubi funkcionalnu vrijednost.

---

## 6. Obavezne glavne funkcije table

Glavna tabla mora raditi najmanje 6 stvari:

1. nositi **Provinces/Provincije** i prostorni identitet partije
2. prikazivati ključne zajedničke zone i napetosti
3. podržavati diplomatiju kroz javni politički kontekst
4. podržavati **Events/Događaji** i **Crises/Krize** bez gušenja mape
5. podržavati završni pritisak i **Coronation Attempt/Pokušaj krunisanja** kontekst
6. ostati čitljiva kada se na nju zaista stave tokeni, jedinice i markeri

Ako radi samo prve dvije stvari, tabla je previše gola.
Ako radi svih šest loše, tabla je prenatrpana.

---

## 7. Osnovna struktura table

U v2.7 glavna tabla treba da bude organizovana oko ovih glavnih zona:

### 7.1. Map Core / Jezgro mape

Glavna i najveća zona table, sa **24 Provinces/24 Provincije**.

### 7.2. Shared System Margin / Zajednički sistemski rub

Rubne ili bočne zone za zajedničke informacije koje ne smiju prekriti mapu.

### 7.3. Event and Crisis Zone / Zona događaja i kriza

Mjesto za aktivni **Event/Događaj** i/ili **Crisis/Kriza** prikaz.

### 7.4. Treaty and Political Context Zone / Zona sporazuma i političkog konteksta

Mjesto za formalni pregled zajedničkih političkih odnosa, ali samo u onoj mjeri u kojoj to ubrzava sto.

### 7.5. Endgame and Coronation Context Zone / Zona završnice i krunisanja

Mjesto za zajedničke završne signale i javan kontekst **Coronation Attempt/Pokušaj krunisanja** kada je relevantno.

---

## 8. Map Core / Jezgro mape

Ovo je najvažnija zona cijele table.

### 8.1. Zašto

Mapa je jedan od glavnih identitetskih stubova CoS-a. Ona mora dominirati prostorom table.

### 8.2. Šta mora sadržavati

* **24 Provinces/24 Provincije**
* jasna susjedstva
* jasne granice i pravce kretanja / pritiska gdje je to relevantno
* dovoljno prostora za jedinice, markere kontrole i contest stanje

### 8.3. Šta ne smije sadržavati

Ne smije biti zatrpana:

* previše sitnim ikonama
* viškom dekorativnih tekstura
* suvišnim rules podsjetnicima preko provincija

Mapa mora ostati čitljiva kada se na njoj zaista igra.

---

## 9. Province / Provincija čitljivost standard

Svaka **Province/Provincija** na tabli mora biti:

* jasno odvojena od susjednih provincija
* dovoljno velika za realan gameplay marker load
* dovoljno čista da se njena funkcija može prepoznati bez mikroskopskog čitanja

Ako province izgledaju dobro samo prazne, a loše kada se napune jedinicama i markerima, dizajn nije uspješan.

---

## 10. Mapa i ikonografija

Mapa ne smije postati polje za demonstraciju kompletnog ikonografskog sistema.

To znači:

* koristiti samo ikonografiju koja stvarno pomaže prostornoj čitljivosti
* ne uvoditi dodatne male simbole po provinciji ako ne nose stvarnu mehaničku vrijednost
* favorizovati čitljivost susjedstva i kontrole ispred ornamentalne složenosti

U slučaju konflikta između dekoracije i funkcije, funkcija ima prednost.

---

## 11. Shared System Margin / Zajednički sistemski rub

Zajednički rub table služi da glavna mapa ostane čista, a da zajednički sistemi i dalje budu vidljivi.

Ovaj rub može nositi:

* aktivni **Event/Događaj** i **Crisis/Kriza** prostor
* ograničeni politički pregled
* završne ili coronation reference gdje je relevantno
* zajedničke proceduralne podsjetnike u veoma sažetom obliku

Ali ovaj rub ne smije postati sekundarna tabla puna teksta.

---

## 12. Event and Crisis Zone / Zona događaja i kriza

Ova zona mora biti lako uočljiva, ali ne dominantnija od mape.

### 12.1. Šta treba raditi

Mora omogućiti:

* jasan prikaz aktivnog **Event/Događaj** sadržaja
* jasan prikaz aktivne **Crisis/Kriza** logike kada je relevantna
* javnu i brzu referencu za sve igrače

### 12.2. Šta ne smije raditi

Ne smije:

* preuzeti previše prostora sa mape
* biti toliko tekstualna da zahtijeva dugo čitanje direktno sa table
* glumiti zamjenu za punu event/crisis kartu ili aid

Tabla treba da signalizira i sažme, ne da nosi kompletan pravni tekst sistema.

---

## 13. Treaty and Political Context Zone / Zona sporazuma i političkog konteksta

Ova zona treba da bude veoma pažljivo limitirana.

### 13.1. Zašto postoji

Da bi formalna **Diplomacy/Diplomatija** ostala javno čitljiva i povezana sa zajedničkim prostorom.

### 13.2. Šta treba raditi

Treba omogućiti:

* pregled aktivnih **Treaty/Sporazum** odnosa gdje je to UX korisno
* signal političkog stanja stola
* brzu provjeru formalnih odnosa bez stalnog listanja kartica

### 13.3. Šta ne smije raditi

Ne smije:

* postati velika matrica puna mikroteksta
* preuzeti ulogu punog diplomatskog rules reference-a
* konkurisati mapi po vizuelnoj težini

Politički sloj mora biti vidljiv, ali i dalje podređen cjelini table.

---

## 14. Endgame and Coronation Context Zone / Zona završnice i krunisanja

Ova zona treba da bude tihi, ali važan završni signal.

### 14.1. Šta treba raditi

Treba omogućiti:

* javan osjećaj kada partija ulazi u završni politički vrh
* jasan referentni prostor za **Coronation Attempt/Pokušaj krunisanja** kontekst kada je aktivan
* dovoljno prostora za završni marker, contest signal ili scoring podsjetnik gdje je relevantno

### 14.2. Šta ne smije raditi

Ne smije:

* stalno dominirati tablom od početka partije
* izgledati kao zasebna mini-igra
* tražiti previše stalnog prostora za sistem koji je aktivan samo u kasnijem dijelu partije

Završna zona mora biti prisutna, ali diskretna dok ne postane relevantna.

---

## 15. Veza sa setup-guide logikom

Glavna tabla mora biti dizajnirana tako da setup po `rules/setup-guide.md` bude:

* brz
* logičan
* lako ponovljiv
* bez previše “gdje ide koji marker?” pitanja

Ako tabla traži da igrači stalno konsultuju dodatne sheme samo da bi pravilno postavili komponente, layout nije dovoljno dobar.

---

## 16. Veza sa turn structure / tokom runde

Tabela mora podržavati prirodan tok runde.

To znači da zone za:

* **Event/Crisis Phase/Fazu događaja i krize**
* politički javni kontekst
* završnu contest logiku

moraju biti raspoređene tako da prate pažnju igrača kroz tok partije, a ne da je rasipaju.

---

## 17. Veza sa Player Board / Tablom igrača

Glavna tabla i tabla igrača ne smiju se boriti za iste informacije.

Pravilo je jednostavno:

* ono što je lično i često interno = ide na **Player Board/Tablu igrača**
* ono što je zajedničko i važno za cijeli sto = ide na glavnu **Board/Tablu**

Ako se isto stanje prati na dvije površine bez dobrog razloga, raste konfuzija i mogućnost greške.

---

## 18. Veza sa terminology-and-labels standardom

Sve labele na glavnoj tabli moraju slijediti:

* `components/terminology-and-labels.md`

To znači:

* dosljedne dvojezične forme kada je prostor dovoljan
* kontrolisane skraćene forme samo kada su unaprijed definisane
* bez proizvoljnih alternativnih naziva radi layouta

Ako je layout problem, prvo se rješava layout — ne terminologija.

---

## 19. Veza sa iconography standardom

Glavna tabla mora koristiti ikonografiju štedljivo i pametno.

To znači:

* najvažnije ikone samo tamo gdje stvarno ubrzavaju čitanje
* bez ikonografskog zasićenja po provincijama i rubnim zonama
* ikone moraju imati tekstualnu podršku kad god je to potrebno za prvi susret ili važnu razliku

Tabla ne smije izgledati kao legenda ikona. Ona mora izgledati kao igrivi prostor.

---

## 20. Vizuelna hijerarhija table

Preporučena hijerarhija glavne table je:

1. **Provinces/Provincije** i prostorni odnosi
2. zajednički aktivni pritisak (**Event/Događaj**, **Crisis/Kriza**)
3. politički kontekst i **Treaty/Sporazum** pregled
4. završni / coronation signali
5. pomoćni mikro-podsjetnici

Ako nešto sa ruba vizuelno nadjača mapu, hijerarhija je pogrešno postavljena.

---

## 21. Pristupačnost i upotrebljivost

Glavna tabla mora ostati čitljiva:

* pod različitim uglovima gledanja
* u normalnom stolnom svjetlu
* uz realne print ograničenosti
* bez oslanjanja samo na boju

To znači:

* dovoljno jak kontrast granica i zona
* dovoljan vizuelni razmak između važnih područja
* kombinaciju: tekst + oblik + ikona gdje je potrebno

---

## 22. Onboarding uloga glavne table

Za novu grupu glavna tabla mora u prvih nekoliko minuta jasno komunicirati:

* gdje je mapa
* gdje se vide zajednički pritisci
* gdje se vidi politički kontekst
* gdje se pojavljuje završni contest signal kada dođe vrijeme

Ako nova grupa ne može to brzo “čitati pogledom”, tabla nije uspješno organizovana.

---

## 23. Najčešće greške u dizajnu glavne table

* mapa je premala u odnosu na rubne zone
* province su lijepe, ali nepraktične za stvarne markere
* previše mikroteksta direktno na tabli
* event/crisis zona izgleda kao zaseban modul koji guta pažnju
* politički pregled je ili nevidljiv ili prevelik
* završna zona stalno dominira i kad nije aktivna
* ilustracija i dekoracija smanjuju stvarnu čitljivost

---

## 24. Workflow pravilo za novu zonu na glavnoj tabli

Ako se predlaže nova zona na glavnoj tabli, mora se provjeriti redom:

1. da li je to zaista zajednička informacija za cijeli sto
2. da li se koristi dovoljno često da opravda stalni prostor
3. da li se problem može riješiti aid-om ili posebnom kartom umjesto stalne table zone
4. da li nova zona smanjuje prostor ili čitljivost mape
5. da li nova zona povećava onboarding težinu
6. da li postoji postojeći rub ili zajednička zona koja to već može nositi

Ako ne prolazi ova pitanja, nova zona se ne uvodi.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li mapa ostaje dominantna?
2. da li zajedničke zone ostaju korisne, ali ne prevelike?
3. da li terminologija i ikonografija ostaju dosljedne?
4. da li tabla ostaje čitljiva kada je stvarno puna komponenti?
5. da li promjena pomaže onboarding ili ga otežava?
6. da li grafički handoff postaje lakši ili teži?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 26. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `ux/player-aid-system.md`
* `ux/information-hierarchy.md`
* `visuals/card-wireframe-notes.md`
* `visuals/board-wireframe-notes.md`

Ako glavna tabla nije dovoljno čista prije grafičke faze, gotovo sigurno dolazi do:

* više krugova korekcije board layouta
* slabije čitljivosti prototipa
* sporijeg setupa i gameplaya
* skupljih print test iteracija

---

## 27. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `systems/province-map-system.md`
* `rules/setup-guide.md`
* `rules/turn-structure.md`
* `systems/diplomacy-and-treaties.md`
* `systems/event-and-crisis-system.md`
* `systems/coronation-system.md`
* `components/terminology-and-labels.md`
* `components/iconography-spec.md`
* `components/player-board-spec.md`
* `ux/information-hierarchy.md`

---

## 28. Završna napomena

**Board Specification / Specifikacija glavne table** mora ostati jedan od najvažnijih infrastrukturnih dokumenata cijelog projekta.

Ako radi dobro:

* mapa ostaje srce partije
* zajednički sistemi se čitaju brzo
* diplomatija i završni pritisak dobijaju pravi zajednički prostor
* onboarding je lakši
* a grafički handoff postaje mnogo sigurniji

Ako radi loše:

* igra djeluje zamornije nego što jeste
* mapa gubi snagu
* zajednički sistemi se slabo čitaju
* a fizički proizvod djeluje manje profesionalno nego što sistem zaslužuje

Zato ovaj dokument mora ostati strogo funkcionalan, hijerarhijski čist i potpuno usklađen sa jezgrom **v2.7**.
