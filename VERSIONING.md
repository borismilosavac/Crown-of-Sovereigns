# VERSIONING.md

# Crown of Sovereigns — Pravila verzionisanja

## Status dokumenta

* **Dokument:** VERSIONING.md
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Locked
* **Svrha:** definisati kako se verzije igre označavaju, kako se tretiraju aktivne i arhivske verzije, i kako se vodi revizioni trag kroz budući razvoj

---

## 1. Zašto ovaj dokument postoji

Versioning nije kozmetika.
On postoji da bi se jasno znalo:

* koja verzija je aktivna
* koja verzija je kanonska
* koje promjene su samo tuning
* koje promjene su strukturalne
* kada treba otvoriti novu glavnu verziju
* koji dokumenti moraju biti ažurirani kada se verzija promijeni

Ako versioning nije jasan, projekat vrlo brzo upada u haos:

* paralelna pravila
* različite interpretacije iste verzije
* nejasni playtest buildovi
* konfuzni grafički handoff
* loš trag promjena

---

## 2. Osnovni princip

Crown of Sovereigns koristi **kanonski verzioni sistem**.

To znači:

* u svakom trenutku postoji samo **jedna aktivna kanonska verzija**
* sve starije verzije ostaju sačuvane, ali nisu aktivna baza
* nova verzija postaje aktivna tek kada je eksplicitno zaključana

Trenutno pravilo glasi:

> **Crown of Sovereigns v2.7** je jedina kanonska i relevantna osnova za dalji razvoj.

Sve starije verzije:

* **v2.6.1**
* **v2.6**
* **v2.5.x**
* i ranije

smatraju se **arhivom**, osim ako se koriste za istorijsku analizu ili poređenje.

---

## 3. Struktura brojeva verzije

Koristi se format:

```text
vMAJOR.MINOR.PATCH
```

Primjeri:

* `v2.7`
* `v2.7.1`
* `v2.7.2`
* `v2.8`
* `v3.0`

### Značenje nivoa

* **MAJOR** — veliki identitetski ili razvojni skok
* **MINOR** — nova kanonska iteracija sa važnim promjenama
* **PATCH** — tuning, clarity ili playtest korekcija bez promjene osnovnog identiteta

---

## 4. Šta znači svaka vrsta verzije

## 4.1. PATCH verzija

Primjeri:

* `v2.7.1`
* `v2.7.2`

PATCH se koristi kada:

* se podešavaju brojevi
* se popravljaju wording nejasnoće
* se fino podešava balans
* se smanjuje downtime
* se poboljšava onboarding
* se koriguje 2P / 3P / 4P ponašanje
* se poboljšava player aid ili rules clarity

PATCH ne smije:

* rušiti identitet igre
* uvoditi potpuno nove glavne podsisteme
* mijenjati osnovnu fantaziju igre
* pretvarati verziju u novi dizajnerski pravac

Drugim riječima:

> PATCH popravlja kako sistem radi, ali ne redefiniše šta sistem jeste.

---

## 4.2. MINOR verzija

Primjeri:

* `v2.7`
* `v2.8`

MINOR se koristi kada:

* se zaključava nova kanonska iteracija
* se uvodi važna nova dizajnerska odluka
* se više povezanih sistema pomjera zajedno
* se mijenja struktura tempa, toka ili glavne završnice
* se uvodi novi zaključani razvojni paket koji utiče na više zona igre

MINOR verzija smije:

* mijenjati ključne odnose među sistemima
* restrukturirati tok igre
* mijenjati glavne putanje do pobjede
* uvoditi novi veliki sistem ako je identity-safe i opravdan

Ali i dalje ne bi trebala:

* potpuno razbiti identitet igre
* tražiti da se projekat tretira kao novi naslov

Drugim riječima:

> MINOR je nova kanonska faza iste igre.

---

## 4.3. MAJOR verzija

Primjeri:

* `v3.0`
* `v4.0`

MAJOR se koristi samo kada se desi stvarni razvojni lom, kao što je:

* promjena osnovne fantazije igre
* promjena glavnog core loopa
* promjena žanrovskog identiteta
* promjena ciljne publike
* potpuni redesign glavnih sistema
* prelazak u produkcijski ili izdavački okvir koji traži novi status cijelog projekta

MAJOR verzija znači:

> više nije riječ o istoj razvojnoj fazi, nego o novoj generaciji dizajna.

To ne smije biti rutinska odluka.

---

## 5. Pravilo jedne kanonske verzije

U svakom trenutku smije postojati samo jedna verzija sa statusom:

* **active canonical base**
* odnosno jedina relevantna za dalji razvoj

Sve ostale verzije moraju biti označene kao:

* **archived**
* **deprecated**
* ili istorijske reference

Kritično pravilo:

> Ne smiju postojati dvije paralelne “aktivne” verzije.

Ako se to desi, cijeli repozitorijum gubi jasnoću izvora istine.

---

## 6. Kada se otvara nova verzija

Nova verzija se otvara samo kada postoji jasan razlog.

### PATCH otvaraš kada:

* su promjene tuning prirode
* popravljaju postojeće probleme
* ne mijenjaju identitet
* ne traže novi GDD iz temelja

### MINOR otvaraš kada:

* set promjena mijenja više povezanih sistema
* moraš ažurirati GDD kao novu kanonsku bazu
* postoji novi zaključani repair / redesign paket
* želiš jasno odvojiti novu stabilnu fazu razvoja od stare

### MAJOR otvaraš kada:

* se igra konceptualno preslaže
* mijenja se osnovni model iskustva
* staro ime verzije više ne opisuje pošteno novi dizajn

---

## 7. Primjena na Crown of Sovereigns

### Dosadašnja logika

* `v2.5` — ranija zaključana kanonska baza
* `v2.6` — repair i koherencijski upgrade
* `v2.6.1` — dijagnostički i tuning korak
* `v2.7` — nova kanonska baza nakon primjene repair paketa i novih zaključanih sistema

### Aktivna logika od sada

* **v2.7** = jedina kanonska osnova
* **v2.7.1** = naredni tuning pass nakon playtest nalaza
* **v2.7.2** = dodatni clarity / balance pass ako bude potreban
* **v2.8** = naredna veća kanonska iteracija samo ako se više sistema istovremeno zaključano pomjeri

---

## 8. Kako se dokumenti ponašaju pri promjeni verzije

Kada se aktivna verzija promijeni, nisu svi dokumenti jednako pogođeni.

### 8.1. Dokumenti koji se uvijek moraju ažurirati

Kada verzija pređe u novu kanonsku fazu, obavezno ažurirati:

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `docs/version-status.md`
* `gdd/crown-of-sovereigns-vX.X-gdd.md`
* `revision/document-status-matrix.md`

### 8.2. Dokumenti koji se ažuriraju po dependency mapi

Ako se pravilo stvarno mijenja, onda po potrebi ažurirati:

* rules dokumente
* systems dokumente
* content dokumente
* components dokumente
* UX dokumente
* visuals dokumente

### 8.3. Dokumenti koji mogu ostati netaknuti

Ako promjena verzije ne utiče na njihovu temu, dokument ostaje isti, ali njegov status se i dalje provjerava.

---

## 9. Pravila imenovanja verzionih fajlova

### Aktivni dokumenti

Aktivni dokumenti za verziju mogu imati eksplicitnu verziju u imenu kad je to važno.

Primjer:

* `crown-of-sovereigns-v2.7-gdd.md`
* `rules-reference-v2.7.md`
* `playtest-plan-v2.7.md`

### Neutralni dokumenti

Dokumenti koji opisuju trajni sistem repozitorija mogu ostati bez verzije u imenu.

Primjer:

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `CONTRIBUTING.md`

### Zabranjeno

Ne koristiti:

* `final-v2-last.md`
* `latest-rules-real-final.md`
* `gdd-updated-newest.md`

Nazivi moraju ostati čisti i predvidivi.

---

## 10. Pravila promjene statusa dokumenta

Svaki dokument ima status:

* **Draft**
* **Review**
* **Locked**
* **Deprecated**
* **Archived**

### Kada dokument ide u Locked

Dokument ide u **Locked** kada:

* sadržaj je provjeren
* usklađen je sa source-of-truth dokumentom
* nema otvorenih kontradikcija
* spreman je da služi kao aktivna osnova

### Kada dokument ide u Deprecated

Kad postoji noviji aktivni dokument za istu temu.

### Kada dokument ide u Archived

Kad više nije operativno koristan osim kao istorijska referenca.

---

## 11. Pravilo promjene verzije u praksi

Kad odlučiš da pređeš sa npr. `v2.7` na `v2.7.1`, idi ovim redom:

### Korak 1 — potvrdi opseg promjene

Odredi da li je promjena:

* PATCH
* MINOR
* ili MAJOR

### Korak 2 — ažuriraj source of truth

Prvo promijeni glavni dokument za pogođenu temu.

### Korak 3 — propagiraj zavisnosti

Prema dependency mapi ažuriraj sve izvedene dokumente.

### Korak 4 — upiši promjenu

Zabilježi u:

* `CHANGELOG.md`
* revision log dokumenta
* eventualno `canonical-decisions.md` ako je odluka važna

### Korak 5 — zaključaj novu istinu

Nakon provjere status se vraća na **Locked**.

---

## 12. Kako razlikovati tuning od structural rewrite-a

Ovo je najvažnija praktična razlika.

### PATCH / tuning

Ako radiš nešto poput:

* mijenjanja broja bodova
* smanjenja ili povećanja troška
* pojačavanja 2P pressure-a
* skraćivanja pregovaračkih prozora
* čišćenja player aid wording-a

onda je to uglavnom PATCH.

### Structural rewrite

Ako radiš nešto poput:

* uvođenja novog završnog core sistema
* promjene kako dvor generiše akcije
* promjene osnovne ekonomije
* promjene kako stabilnost radi na nivou cijele partije
* potpunog redizajna diplomatije

onda vjerovatno više nije riječ o običnom patchu.

---

## 13. Pravilo za playtest buildove

Playtest buildovi ne smiju zamijeniti kanonske verzije.

To znači:

* build može biti označen kao `v2.7-test-A`
* ali aktivna verzija i dalje ostaje `v2.7` dok se nova iteracija ne zaključa

Drugim riječima:

> test build nije automatski nova kanonska verzija.

---

## 14. Pravilo za grafičke fajlove

Grafički fajlovi moraju biti vezani za kanonsku verziju koja je zaključana.

Primjer:

* ako je aktivna baza `v2.7`, grafički handoff mora koristiti `v2.7` spec
* ako se kasnije promijeni sistem u `v2.7.1`, mora se jasno znati da li grafika ostaje kompatibilna ili traži novi handoff

Ovo sprečava da grafika bude zasnovana na zastarjeloj logici.

---

## 15. Minimalna verziona disciplina za budući rad

Za svaku buduću promjenu obavezno odgovoriti na 5 pitanja:

1. Da li je ovo PATCH, MINOR ili MAJOR promjena?
2. Koji je source-of-truth dokument pogođen?
3. Koji drugi dokumenti zavise od te promjene?
4. Da li se mijenja kanonski status verzije?
5. Da li je promjena upisana u changelog i revision log?

Ako nema odgovora na tih 5 pitanja, promjena nije dovoljno disciplinovana.

---

## 16. Primjer zdrave verzione putanje za CoS

Realističan naredni tok može izgledati ovako:

* **v2.7** — zaključana kanonska baza
* **v2.7.1** — tuning na osnovu prvog većeg playtest kruga
* **v2.7.2** — dodatni clarity / balance pass
* **v2.8** — novi veći zaključani paket ako više sistema mora biti promijenjeno zajedno
* **v3.0** — samo ako se desi ozbiljan konceptualni lom ili produkcijski redefinisana generacija igre

---

## 17. Brutalno iskrena napomena

Najčešća greška nije da ljudi nemaju verzije.
Greška je da imaju previše nejasnih verzija.

To vodi ka tome da:

* niko ne zna koja pravila su aktivna
* playtest podaci više nisu pouzdani
* grafički tim radi po pogrešnoj bazi
* promjene se više ne mogu pratiti
* povjerenje u projekat opada

Zato Crown of Sovereigns mora ostati disciplinovan:

> jedna aktivna verzija, jasan trag promjena, jasna razlika između patcha i nove kanonske faze.

---

## 18. Završna definicija

Od ove tačke važi:

* **Crown of Sovereigns v2.7** je jedina aktivna kanonska verzija
* naredne manje izmjene vode se kao **v2.7.x**
* nova velika stabilna iteracija ide u **v2.8**
* starije verzije ostaju u arhivi i ne koriste se kao aktivna baza

Ovaj dokument služi da ta logika ostane stabilna kroz cijeli naredni razvoj projekta.
