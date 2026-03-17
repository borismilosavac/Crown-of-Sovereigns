# information-hierarchy.md

# Crown of Sovereigns v2.7 — Information Hierarchy / Hijerarhija informacija

## Status dokumenta

* **Dokument:** `ux/information-hierarchy.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati kako se informacije raspoređuju, prioritetizuju i prikazuju kroz sve glavne komponente igre
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Information Hierarchy/Hijerarhija informacija**, **Board/Tabla**, **Player Board/Tabla igrača**
* **Povezani dokumenti:** `components/board-spec.md`, `components/player-board-spec.md`, `ux/player-aid-system.md`, `components/iconography-spec.md`, `components/terminology-and-labels.md`, `visuals/card-wireframe-notes.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše koja vrsta informacije ide na koju komponentu
* odredi šta mora biti dominantno, šta sekundarno, a šta tercijarno u vizuelnom i funkcionalnom smislu
* spriječi da važne informacije budu potisnute ukrasom, mikrotekstom ili manje bitnim signalima
* pomogne da gameplay tok ostane brz i čitljiv
* pripremi siguran osnov za grafički handoff, aid dizajn i playtest printove

Ovo nije estetski dokument.
Ovo je UX i komponentni dokument koji štiti čitljivost cijelog sistema.

---

## 2. Zašto je hijerarhija informacija kritična

CoS v2.7 ima više povezanih sistema:

* **Court/Dvor**
* **Provinces/Provincije**
* **Goods/Roba**
* **Stability/Stabilnost**
* **Diplomacy/Diplomatija**
* **Combat/Borba**
* **Events/Događaji** i **Crises/Krize**
* završni pritisak i **Coronation Attempt/Pokušaj krunisanja**

Ako se sve te informacije prikazuju bez jasne hijerarhije, rezultat je:

* sporije odlučivanje
* veći onboarding teret
* više lookup trenutaka
* osjećaj da je igra teža i mutnija nego što zapravo jeste

Zato hijerarhija informacija nije luksuz. Ona je osnovna infrastruktura upotrebljivosti.

---

## 3. Osnovni princip hijerarhije

Glavno pravilo glasi:

> informacija mora biti onoliko vidljiva koliko je često potrebna i koliko je važna za odluku u tom trenutku.

To znači:

* najvažnije i najčešće informacije moraju biti najlakše za vidjeti
* rjeđe ili dublje informacije smiju biti diskretnije
* ukras nikad ne smije biti jači od funkcije
* aid i komponente zajedno moraju formirati jedan jasan sistem, ne tri odvojena jezika

---

## 4. Šta hijerarhija informacija nije

Hijerarhija informacija nije:

* samo pitanje veličine fonta
* samo pitanje boje
* samo pitanje “lijepog layouta”
* opravdanje da se sve trpa na jednu površinu uz nadu da će se nekako snaći

Ona je kombinacija:

* prioriteta sadržaja
* pozicije
* veličine
* kontrasta
* grupisanja
* učestalosti upotrebe

Ako bilo koji od ovih faktora radi protiv ostalih, sistem slabi.

---

## 5. Osnovni nivoi informacija

U CoS v2.7 sve informacije moraju se posmatrati kroz 4 osnovna nivoa:

### 5.1. Primary Information / Primarna informacija

Informacija koju igrač često gleda i koja direktno utiče na odluku u tom trenutku.

### 5.2. Secondary Information / Sekundarna informacija

Informacija koja podržava odluku, ali nije prvi fokus pogleda.

### 5.3. Tertiary Information / Tercijarna informacija

Informacija koja je korisna za potvrdu, podsjetnik ili dublji kontekst, ali nije stalno potrebna.

### 5.4. Decorative/Atmospheric Layer / Dekorativni i atmosferski sloj

Sve što gradi identitet i ton, ali ne smije ometati čitljivost prethodna tri nivoa.

Kritično pravilo:

> nijedan dekorativni element ne smije nadjačati primarnu ili sekundarnu informaciju.

---

## 6. Primarna informacija po komponentama

### 6.1. Na glavnoj Board/Tabli

Primarna informacija je:

* stanje mape
* **Provinces/Provincije** i kontrole
* zajednički aktivni pritisak koji direktno utiče na rundu

### 6.2. Na Player Board/Tabli igrača

Primarna informacija je:

* **Court/Dvor** fokus
* **Stability/Stabilnost**
* **Goods/Roba** i razvojno stanje

### 6.3. Na Player Aid/Pomoćni igrački vodič

Primarna informacija je:

* **Round Spine/Kičma runde**
* najvažniji pragovi i proceduralni podsjetnici

### 6.4. Na kartama ili treaty komponentama

Primarna informacija je:

* naziv
* klasa / tip
* glavni mehanički efekat

Ako se ova primarna logika izgubi, cijeli sistem postaje sporiji za čitanje.

---

## 7. Sekundarna informacija po komponentama

### 7.1. Na glavnoj tabli

Sekundarna informacija uključuje:

* politički kontekst i **Treaty/Sporazum** pregled
* event/crisis kontekst
* završne signale kada postanu relevantni

### 7.2. Na tabli igrača

Sekundarna informacija uključuje:

* identitet kraljevstva
* podršku resursima
* **Kingdom Advantages/Prednosti kraljevstva** reference

### 7.3. Na aid-u

Sekundarna informacija uključuje:

* sažeti podsjetnik za **Court Roles/Dvorske uloge**
* sažeti podsjetnik za **Combat/Borba**
* sažeti podsjetnik za diplomatiju i završnicu

Sekundarna informacija mora biti lako dostupna, ali ne smije dominirati.

---

## 8. Tercijarna informacija

Tercijarna informacija treba biti prisutna samo kada zaista pomaže.

To uključuje:

* kratke dodatne napomene
* mikro-podsjetnike za rjeđe korištene situacije
* pomoćni status ili kontekst koji nije potreban svaki krug

Tercijarna informacija ne smije biti raspoređena tako da izgleda važnije nego što jeste.

U protivnom, vizuelni sistem gubi signal-to-noise odnos.

---

## 9. Dekorativni i atmosferski sloj

CoS treba da ima identitet i atmosferu, ali taj sloj mora ostati strogo podređen funkcionalnoj hijerarhiji.

To znači:

* heraldika, ornamenti i teksture smiju podržati ton
* ali ne smiju smanjiti kontrast ili jasnoću
* ne smiju upadati u prostor za labele, markere i ikone
* ne smiju stvarati lažne fokalne tačke koje odvlače pogled sa važnih informacija

Dobar ukras pojačava identitet.
Loš ukras usporava igru.

---

## 10. Pravilo učestalosti korištenja

Jedan od glavnih kriterija za hijerarhiju je koliko često igrač koristi informaciju.

### Veoma često

Mora biti:

* velika
* blizu centra pažnje
* jasno odvojena

### Povremeno

Može biti:

* manja
* na rubu zone
* podržana ikonom ili aid-om

### Rijetko

Treba biti:

* sažeta
* diskretnija
* ili potpuno prebačena u aid / rules dokument ako nije vrijedna stalnog prostora

Ako se rijetka informacija ponaša kao stalna, stvara se šum.

---

## 11. Pravilo trenutka korištenja

Pored učestalosti, bitno je i kada se informacija koristi.

### Tokom svakog poteza

Informacija mora biti izuzetno vidljiva i lako dostupna.

### Tokom svake runde

Informacija mora biti jasno prisutna, ali ne mora dominirati svakom sekundom igre.

### Samo u završnici

Informacija smije biti diskretnija dok ne postane relevantna, ali mora tada brzo postati čitljiva.

To je posebno važno za:

* **Coronation Attempt/Pokušaj krunisanja** kontekst
* završne pritiske
* kasne **Crises/Krize**

---

## 12. Hijerarhija na glavnoj tabli

Na glavnoj tabli preporučeni red važnosti je:

1. **Provinces/Provincije** i stanje mape
2. aktivni zajednički pritisak koji utiče na rundu
3. politički i treaty kontekst
4. završni i coronation signali
5. pomoćne mikro-reference

Ako bilo šta sa ruba vizuelno nadjača mapu, hijerarhija je pogrešno postavljena.

---

## 13. Hijerarhija na tabli igrača

Na tabli igrača preporučeni red važnosti je:

1. **Court/Dvor**
2. **Stability/Stabilnost**
3. **Goods/Roba** i razvoj
4. ključni resursni pregled
5. identitet kraljevstva i sekundarne reference

Ovo mora ostati dosljedno kroz sve buduće grafičke iteracije.

---

## 14. Hijerarhija na Player Aid/Pomoćni igrački vodič

Na aid-u preporučeni red važnosti je:

1. **Round Spine/Kičma runde**
2. **Stability/Stabilnost** pragovi i posljedice
3. **Court/Dvor** podsjetnik
4. **Combat/Borba** i **Diplomacy/Diplomatija** mikro-podsjetnici
5. završni / coronation podsjetnik

Aid mora odgovarati stvarnom redoslijedu potrebe tokom partije.

---

## 15. Hijerarhija na kartama i manjim komponentama

Na kartama i manjim komponentama preporučeni red važnosti je:

1. naziv
2. tip / klasa
3. glavni efekat
4. trajanje / uslov / ograničenje
5. pomoćni ton ili mikro-atmosfera

Na maloj površini mora se posebno paziti da dekorativni sloj ne uguši tekstualni i mehanički signal.

---

## 16. Veza sa terminology-and-labels standardom

Hijerarhija informacija direktno zavisi od dosljedne terminologije.

To znači:

* isti pojam mora izgledati isto važan kad god je u istom kontekstu važnosti
* label mora biti dosljedan po formi i težini
* ne smije se desiti da isti termin na jednoj komponenti izgleda kao glavni sistem, a na drugoj kao sporedna fusnota bez razloga

Terminološka nedosljednost uvijek ruši i hijerarhiju.

---

## 17. Veza sa ikonografijom

Ikone pomažu hijerarhiji samo ako su pravilno korištene.

To znači:

* primarne informacije mogu koristiti najjače i najjasnije ikone
* sekundarne mogu koristiti skromnije ili manje istaknute ikone
* tercijarne ne trebaju nužno dobiti posebne ikone

Ne treba svaka informacija dobiti ikonu samo zato što postoji mjesto za nju.

---

## 18. Veza sa onboardingom

Dobra hijerarhija informacija direktno smanjuje onboarding težinu.

Nova grupa treba da može pogledom razumjeti:

* šta je najvažnije na tabli
* šta je najvažnije na tabli igrača
* šta aid služi da podsjeti
* šta je sporedno i može se učiti kasnije

Ako nova grupa ne može intuitivno razlikovati glavno od sporednog, hijerarhija nije uspješna.

---

## 19. Veza sa pristupačnošću

Hijerarhija informacija ne smije zavisiti samo od:

* boje
* fine linije
* vrlo male razlike u nijansi

Mora koristiti kombinaciju:

* pozicije
* veličine
* kontrasta
* grupisanja
* teksta
* oblika

To je važno za:

* čitljivost u printu
* različite uslove osvjetljenja
* različite tipove igrača
* WCAG-inspirisanu pristupačnost gdje je primjenjivo na štampane materijale

---

## 20. Najčešće greške u hijerarhiji informacija

* sporedni podsjetnici veći od glavnih sistema
* dekoracija koja privlači više pažnje od funkcije
* ista vizuelna težina za previše različitih nivoa informacija
* mikrotekst na mjestu koje bi trebalo biti brzo skenabilno
* dupliranje informacija na više mjesta bez jasnog prioriteta
* aid koji pokušava nositi i glavno i sporedno i rijetko sve jednako

---

## 21. Workflow pravilo za novu informaciju

Ako se uvodi nova informacija na komponentu, mora se provjeriti redom:

1. da li je to primarna, sekundarna ili tercijarna informacija
2. koliko često se koristi
3. u kojem trenutku partije je relevantna
4. kojoj komponenti najprirodnije pripada
5. da li već postoji druga površina koja to bolje nosi
6. da li nova informacija potiskuje nešto važnije

Ako ne prolazi ovu logiku, ne uvodi se ili se prebacuje na drugu površinu.

---

## 22. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li povećava ili smanjuje čitljivost?
2. da li pomaže ili otežava onboarding?
3. da li pojačava glavno i utišava sporedno kako treba?
4. da li ostaje usklađena sa terminologijom i ikonografijom?
5. da li smanjuje ili povećava vizuelni šum?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar v2.7.x korak.

---

## 23. Veza sa grafičkom pripremom

Ovaj dokument direktno utiče na:

* `components/board-spec.md`
* `components/player-board-spec.md`
* `ux/player-aid-system.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `visuals/card-wireframe-notes.md`

Ako hijerarhija informacija nije zaključana prije ozbiljnog grafičkog rada, gotovo sigurno dolazi do:

* prenatrpanih layouta
* više iteracija bez jasnog razloga
* vizuelno lijepih, ali gameplay slabih rješenja
* sporijeg i skupljeg handoffa

---

## 24. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/board-spec.md`
* `components/player-board-spec.md`
* `ux/player-aid-system.md`
* `components/iconography-spec.md`
* `components/terminology-and-labels.md`
* `visuals/card-wireframe-notes.md`
* `GLOSSARY.md`

---

## 25. Završna napomena

**Information Hierarchy / Hijerarhija informacija** mora ostati jedan od glavnih kontrolnih dokumenata cijelog UX sloja u CoS v2.7.

Ako radi dobro:

* igra se čita brže
* onboarding postaje lakši
* komponente djeluju čišće i inteligentnije
* pravila izgledaju jasnije nego što bi bez nje djelovala
* a grafički handoff postaje daleko sigurniji

Ako radi loše:

* sve komponente počinju govoriti istovremeno
* igra djeluje težom nego što jeste
* aid i table gube jasnoću
* a cijeli proizvod izgleda manje disciplinovano nego što sistem zaslužuje

Zato ovaj dokument mora ostati strogo funkcionalan, hijerarhijski jasan i trajno usklađen sa jezgrom **v2.7**.
