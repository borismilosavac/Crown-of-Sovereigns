# document-status-policy.md

# Crown of Sovereigns v2.7 — Document Status Policy / Politika statusa dokumenata

## Status dokumenta

* **Dokument:** `docs/document-status-policy.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati službene statuse dokumenata, pravila njihove upotrebe i način na koji status utiče na reviziju, kanoničnost i rad u repozitorijumu
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Draft/Nacrt**, **Review/U provjeri**, **Locked/Zaključano**, **Deprecated/Zastarjelo**
* **Povezani dokumenti:** `docs/revision-workflow.md`, `docs/repository-structure.md`, `docs/version-status.md`, `VERSIONING.md`, `CHANGELOG.md`, `gdd/canonical-decisions.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uspostavi jedinstven standard za status svakog dokumenta u repozitorijumu
* spriječi da fajl izgleda aktivno i kanonski iako je još samo radni nacrt
* olakša da se odmah vidi šta je stabilno, šta je otvoreno za izmjene, a šta više ne važi
* poveže status dokumenta sa revizionim workflow-om i verzionom disciplinom
* smanji rizik da se u radu koristi pogrešan ili zastario dokument

Ovo nije samo pomoćna oznaka.
Ovo je operativni sigurnosni sloj za cijeli repo.

---

## 2. Zašto je politika statusa kritična

Bez jasnih statusa vrlo brzo nastaju problemi:

* radni nacrt izgleda kao finalni dokument
* dva dokumenta djeluju podjednako validno iako jedan više nije aktivan
* tim ne zna da li smije slobodno mijenjati dokument ili mora proći formalniju reviziju
* playtest i rules rad se oslanjaju na tekst koji još nije dovoljno stabilan
* stare verzije ostaju u opticaju bez jasnog upozorenja

Dobra politika statusa smanjuje ovu vrstu greške prije nego što preraste u verzioni haos.

---

## 3. Osnovni princip politike statusa

Glavno pravilo glasi:

> svaki dokument mora jasno pokazivati koliko je stabilan, koliko je obavezujući i kako se smije mijenjati.

To znači da status dokumenta mora odgovarati stvarnom stanju, a ne optimističnoj želji da dokument izgleda završenije nego što jeste.

Ako je dokument još otvoren za ozbiljne korekcije, ne smije nositi status koji sugeriše kanonsku stabilnost.

---

## 4. Šta status dokumenta jeste

Status dokumenta treba da kaže najmanje tri stvari:

* koliko je dokument stabilan
* koliko je obavezujući za dalji rad
* koliko strogu reviziju traži prije izmjene

---

## 5. Šta status dokumenta nije

Status dokumenta nije:

* estetska oznaka bez posljedice
* nagrada za trud uložen u pisanje
* zamjena za verziju dokumenta ili igre
* način da se prikrije da dokument nije dovoljno provjeren

Status mora pratiti stvarnost dokumenta, ne reputaciju dokumenta.

---

## 6. Obavezni statusi u projektu

U CoS repozitorijumu koriste se sljedeći osnovni statusi:

* **Draft/Nacrt**
* **Review/U provjeri**
* **Locked/Zaključano**
* **Deprecated/Zastarjelo**

Po potrebi se kasnije može uvesti i dodatni status, ali samo ako ima jasnu funkciju i ne duplira značenje postojećih statusa.

---

## 7. Draft / Nacrt

### 7.1. Definicija

**Draft/Nacrt** znači da je dokument aktivan, ali još nije dovoljno stabilan da se tretira kao čvrsta osnova bez opreza.

### 7.2. Kada se koristi

Koristi se kada:

* dokument je tek napravljen
* očekuju se veće dopune ili korekcije
* još nije dovoljno provjeren kroz povezane dokumente ili workflow
* sadržaj je funkcionalan, ali još nije zaključan

### 7.3. Šta to znači za rad

* dokument se smije aktivno mijenjati
* drugi dokumenti mogu ga koristiti kao radni orijentir, ali ne kao potpuno čvrst izvor istine bez provjere
* ozbiljne zavisnosti prema njemu treba uvoditi oprezno

### 7.4. Šta Draft nije

**Draft/Nacrt** ne znači da je dokument loš ili neupotrebljiv. Znači samo da još nije dovoljno stabilizovan.

---

## 8. Review / U provjeri

### 8.1. Definicija

**Review/U provjeri** znači da je dokument sadržajno skoro stabilan, ali je u toku formalnija provjera dosljednosti, zavisnosti ili kanonske usklađenosti.

### 8.2. Kada se koristi

Koristi se kada:

* osnovni sadržaj dokumenta je postavljen
* glavne izmjene više nisu očekivane bez dobrog razloga
* dokument treba proći dependency check, cross-check ili finalnu sadržajnu reviziju

### 8.3. Šta to znači za rad

* dokument se i dalje može mijenjati
* ali izmjene treba da budu ciljanije i disciplinovanije nego u **Draft/Nacrt** fazi
* dobar je kandidat da uskoro postane **Locked/Zaključano** ako provjere prođu

### 8.4. Glavna opasnost

Najčešća greška je tretirati **Review/U provjeri** kao da je već potpuno zaključan dokument.
To nije tačno.

---

## 9. Locked / Zaključano

### 9.1. Definicija

**Locked/Zaključano** znači da je dokument trenutno stabilan, kanonski usklađen i da se koristi kao aktivna osnova za dalji rad.

### 9.2. Kada se koristi

Koristi se kada:

* sadržaj je dovoljno stabilan
* zavisni dokumenti su usklađeni koliko je potrebno
* nema otvorenih većih kontradikcija
* dokument trenutno služi kao važeći izvor istine za svoju temu

### 9.3. Šta to znači za rad

* dokument se ne mijenja olako
* svaka izmjena mora proći strožiji revision workflow
* drugi dokumenti se smiju oslanjati na njega kao na aktivnu kanonsku osnovu

### 9.4. Važno ograničenje

**Locked/Zaključano** ne znači “zauvijek završeno”.
Znači “trenutno dovoljno stabilno da bude aktivna osnova dok nova revizija ne bude pravilno odobrena”.

---

## 10. Deprecated / Zastarjelo

### 10.1. Definicija

**Deprecated/Zastarjelo** znači da dokument više nije aktivna osnova i ne smije se koristiti kao primarni izvor za dalji rad.

### 10.2. Kada se koristi

Koristi se kada:

* dokument je zamijenjen novijim ili boljim dokumentom
* verzija više nije aktivna
* sadržaj je zadržan samo radi istorijskog traga ili reference

### 10.3. Šta to znači za rad

* dokument se ne koristi kao aktivna osnova
* mora jasno upućivati na dokument koji ga je zamijenio, gdje je to moguće
* smije ostati u repozitorijumu samo ako njegov status ne može zbuniti korisnika

### 10.4. Glavna opasnost

Najveća greška je ostaviti zastarjeli dokument bez jasne oznake, pa da izgleda jednako važeće kao aktivni dokument.

---

## 11. Preporučeni životni ciklus dokumenta

Tipičan životni ciklus izgleda ovako:

1. **Draft/Nacrt**
2. **Review/U provjeri**
3. **Locked/Zaključano**
4. po potrebi kasnije **Deprecated/Zastarjelo**

Ne mora svaki dokument proći savršeno linearno kroz svaku fazu, ali to je zdrava osnovna logika.

---

## 12. Kada dokument ne smije biti Locked / Zaključano

Dokument ne smije nositi status **Locked/Zaključano** ako:

* još ima otvorene veće kontradikcije
* zavisni dokumenti se očigledno ne slažu s njim
* očekuje se veća sistemska promjena u kratkom roku
* dokument još nije dovoljno provjeren u kontekstu verzije
* status bi samo stvarao lažan osjećaj stabilnosti

Ovo je posebno važno za systems i rules dokumente.

---

## 13. Status i verzija nisu ista stvar

Ovo mora biti potpuno jasno:

* **Status** = koliko je dokument stabilan i obavezujući
* **Verzija** = na koju iteraciju igre se dokument odnosi

Primjer:

* dokument može biti **Draft/Nacrt** i ipak biti za **v2.7**
* dokument može biti **Locked/Zaključano** i ipak kasnije postati **Deprecated/Zastarjelo** kada dođe **v2.8**

Miješanje ove dvije stvari stvara veliku konfuziju.

---

## 14. Status i folder nisu ista stvar

To što je dokument u `systems/` ili `rules/` folderu ne znači da je automatski stabilniji od onog u `visuals/` ili `playtests/`.

Status mora biti napisan u samom dokumentu.
Folder daje funkciju, a status daje stabilnost.

---

## 15. Pravilo promjene statusa

Promjena statusa ne smije biti nasumična.

### Iz Draft u Review

Kad:

* sadržaj je uglavnom kompletan
* najveće rupe su zatvorene
* dokument je spreman za ozbiljniju provjeru

### Iz Review u Locked

Kad:

* provjere i usklađivanja su dovoljno prošle
* dokument trenutno može služiti kao aktivni izvor istine

### Iz Locked u Deprecated

Kad:

* dokument je zamijenjen ili više nije aktivna osnova

Promjena statusa treba da ima razlog, a ne samo želju da repo izgleda “zrelije”.

---

## 16. Pravilo statusa i changelog traga

Za sitne editorial promjene nije nužno svaki put mijenjati globalni `CHANGELOG.md`.

Ali za promjene koje:

* mijenjaju status važnog dokumenta
* mijenjaju kanonsku osnovu
* uvode novi **Locked/Zaključano** systems ili rules dokument
* depreciraju važan aktivni dokument

potrebno je ostaviti jasan trag kroz odgovarajuću revizionu logiku i po potrebi changelog.

---

## 17. Pravilo statusa i dependency logike

Kad dokument promijeni status, treba provjeriti kako to utiče na zavisne dokumente.

Primjeri:

* ako systems dokument postane **Locked/Zaključano**, content i components dokumenti koji se oslanjaju na njega mogu dobiti veću stabilnost
* ako rules dokument postane **Deprecated/Zastarjelo**, aid i setup dokumenti možda moraju promijeniti reference

Status nije izolovana oznaka. On utiče na mrežu dokumenata.

---

## 18. Pravilo opreza kod Deprecated / Zastarjelo

Ako dokument postaje **Deprecated/Zastarjelo**, treba jasno navesti:

* da više nije aktivan
* šta ga zamjenjuje, ako postoji zamjena
* da li ostaje samo radi istorijskog traga

Ne treba ostaviti zastarjeli dokument bez putokaza.
To stvara repozitorijumsku zamku za budući rad.

---

## 19. Najčešće greške u radu sa statusima

* držati sve kao **Draft/Nacrt** i nikad ne zaključavati ništa
* prerano dati **Locked/Zaključano** status
* koristiti **Review/U provjeri** predugo, bez odluke
* ne označiti zastarjeli dokument kao **Deprecated/Zastarjelo**
* tretirati status kao dekorativnu formalnost umjesto radnog signala

---

## 20. Workflow pravilo za novi dokument

Kada se pravi novi dokument, po pravilu treba krenuti sa statusom:

* **Draft/Nacrt**

Izuzetak postoji samo ako je dokument mehanički vrlo jednostavan i samo prenosi već potpuno zaključanu logiku bez stvarnih otvorenih pitanja.

Čak i tada, treba biti oprezan sa preranim zaključavanjem.

---

## 21. Workflow pravilo za status pregled repozitorijuma

Povremeno treba uraditi status provjeru repozitorijuma i pitati:

* koji dokumenti su i dalje stvarno **Draft/Nacrt**
* koji su spremni za **Review/U provjeri**
* koji su dovoljno stabilni za **Locked/Zaključano**
* koji više ne smiju ostati bez **Deprecated/Zastarjelo** oznake

Ovo je važno jer statusi koji se nikad ne ažuriraju postaju neupotrebljivi.

---

## 22. Pravilo protiv status inflacije

Ne treba uvoditi previše različitih statusa samo zato što zvuči preciznije.

Previše statusa često znači:

* više konfuzije
* manje dosljednosti
* više sivih zona

Bolje je imati mali broj statusa koji se koriste strogo i tačno, nego veliki broj statusa koji niko ne razlikuje kako treba.

---

## 23. Veza sa revision workflow dokumentom

`docs/revision-workflow.md` govori kako izmjena prolazi kroz proces.

`docs/document-status-policy.md` govori kakvo je trenutno stanje dokumenta u tom procesu.

Jedan dokument opisuje tok promjene.
Drugi opisuje stabilnost rezultata tog toka.

Ta dva dokumenta moraju uvijek ostati usklađena.

---

## 24. Veza sa repository structure dokumentom

`docs/repository-structure.md` određuje gdje dokument pripada.

`docs/document-status-policy.md` određuje koliko je taj dokument stabilan i kako se s njim smije postupati.

Folder organizacija i status politika zajedno čine osnovu repozitorijumske discipline.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li statusi ostaju jasni i operativni?
2. da li nova pravila smanjuju ili povećavaju konfuziju?
3. da li pomažu verzionoj disciplini?
4. da li ostaju dovoljno jednostavna za stvarnu upotrebu?
5. da li čuvaju razliku između stabilnosti dokumenta i verzije igre?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `docs/revision-workflow.md`
* `docs/repository-structure.md`
* `docs/version-status.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `gdd/canonical-decisions.md`
* `GLOSSARY.md`

---

## 27. Završna napomena

**Document Status Policy / Politika statusa dokumenata** mora ostati jedan od glavnih infrastrukturnih dokumenata repozitorijuma.

Ako radi dobro:

* odmah je jasno šta je stabilno
* odmah je jasno šta je još otvoreno
* manje se miješaju aktivni i zastarjeli dokumenti
* revizije su sigurnije
* a cijeli projekat djeluje mnogo urednije i profesionalnije

Ako radi loše:

* statusi ne znače ništa
* dokumenti djeluju jednako važeće i kada nisu
* verziona disciplina slabi
* a repo počinje da vara i autore i buduće saradnike

Zato ovaj dokument mora ostati strog, jasan i potpuno usklađen sa kanonskom logikom **v2.7**.
