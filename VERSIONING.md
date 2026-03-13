# Metodologija verzionisanja

Ovaj dokument definiše kako projekat **Crown of Sovereigns** koristi verzije tokom razvoja.

Cilj verzionisanja je da projekat ostane:

- pregledan
- jasan
- disciplinovan
- i lak za praćenje kroz više razvojnih faza

---

## 1. Osnovna logika

Projekat koristi strukturisani sistem verzija:

- **glavne radne verzije** → `v2.3`, `v2.4`, `v2.5`
- **manje revizije** → `v2.3.1`, `v2.3.2`, `v2.3.3`
- **privremeni interni buildovi** → opciono `v2.3.1-a`, `v2.3.1-b`

---

## 2. Šta je glavna verzija

**Glavna verzija** označava značajan razvojni korak.

Nova glavna verzija se uvodi kada se promijeni jedno ili više od sljedećeg:

- core loop
- onboarding model
- goods struktura
- stabilnost ili diplomatija na sistemskom nivou
- scaling logika
- tržišni hook i pozicioniranje
- psihološki ili proizvodni identitet igre
- rezultati velikog playtest ciklusa koji traže veći rebuild

### Primjeri
- **v2.2** → jači i čišći sistemski pravac
- **v2.3** → psihološko, replay i tržišno pojačanje

---

## 3. Šta je manja revizija

**Manja revizija** služi za tuning i fokusirane dorade.

Koristi se kada se mijenja:

- balans frakcija
- goods tuning
- event tuning
- UX / player aid poboljšanja
- scaling korekcije
- male rule korekcije
- wording i clarity popravke

### Primjeri
- `v2.3.1`
- `v2.3.2`

---

## 4. Privremeni buildovi

Ako je potrebno testirati više kratkih iteracija između dvije manje revizije, mogu se koristiti interni buildovi:

- `v2.3.1-a`
- `v2.3.1-b`

Oni služe samo za internu razvojnu disciplinu i kraće test faze.

Ne tretiraju se kao stabilne zaključane verzije.

---

## 5. Status oznake dokumenata i sistema

Svaki važan sistem ili dokument može imati jednu od sljedećih oznaka:

- **Locked**
- **Active**
- **Experimental**
- **Deprecated**

### Značenje

#### **Locked**
- sistem ili dokument se smatra stabilnim
- koristi se kao važeća osnova
- ne mijenja se bez jasnog razloga i zapisane promjene

#### **Active**
- sistem je u radu
- koristi se, ali nije finalno stabilan
- očekuju se korekcije

#### **Experimental**
- sistem je u test fazi
- nije još potvrđen
- ne smije se tretirati kao zaključani standard

#### **Deprecated**
- sistem ili dokument je napušten
- zadržava se samo radi arhive
- više nije aktivni dio razvoja

---

## 6. Glavno pravilo verzionisanja

Ništa se ne smatra dijelom stabilne verzije ako nije:

1. dokumentovano  
2. označeno verzijom  
3. evidentirano u `CHANGELOG.md`  
4. povezano sa playtest nalazom ili jasnom dizajnerskom odlukom  

To znači da:
- ideje iz razgovora nisu automatski pravila
- neupisane promjene nisu važeće
- i ništa ne smije ostati “samo u glavi”

---

## 7. Pravilo prelaska između verzija

### Iz `v2.3` u `v2.3.1`
Koristi se kada:
- radiš tuning
- ispravljaš balans
- popravljaš clarity i UX
- ne mijenjaš osnovni identitet igre

### Iz `v2.3.x` u `v2.4`
Koristi se kada:
- mijenjaš veliki razvojni sloj
- uvodiš novu potvrđenu strukturu
- završavaš veliki playtest ciklus
- ili prelaziš na novu razvojnu etapu

---

## 8. Branch metodologija

Preporučene grane:

- `main` → samo stabilne zaključane verzije
- `dev` → aktivni razvoj
- `feature/...` → fokusirane radne grane

### Primjeri
- `feature/factions-v2.3.1`
- `feature/player-aid`
- `feature/2p-scaling`
- `feature/events-tuning`
- `feature/solo-automa`

### Pravilo
Ništa ne ide direktno u `main` dok nije:
- dokumentovano
- zapisano u `CHANGELOG`
- i dovoljno provjereno za stabilnu bazu

---

## 9. Commit metodologija

Commit poruke treba da koriste prefikse radi preglednosti.

### Dozvoljeni prefiksi
- `[RULES]`
- `[BALANCE]`
- `[FACTION]`
- `[MAP]`
- `[UX]`
- `[PLAYTEST]`
- `[MARKET]`
- `[DOCS]`

### Primjeri
- `[RULES] Ažurirana struktura runde za v2.3`
- `[BALANCE] Smanjen ekonomski snowball Venecije`
- `[UX] Poboljšana hijerarhija na player aid-u`
- `[PLAYTEST] Dodat zapisnik 4p partije za v2.3`
- `[DOCS] Ažuriran README i status verzije`

---

## 10. Pravilo playtest verzionisanja

Svaki playtest zapis mora jasno navesti:

- verziju igre
- datum
- broj igrača
- korištene frakcije
- teach time
- ukupno trajanje
- pobjednika
- ključne probleme
- wow momente
- replay želju
- glavne zaključke

### Primjer naziva fajla
`2026-03-13_v2.3_4p_playtest.md`

Playtest feedback se nikad ne smije miješati između verzija bez jasne oznake.

---

## 11. Issue tracking pravilo

Svaki ozbiljan problem treba imati:

- **ID**
- **naziv**
- **opis**
- **kategoriju**
- **ozbiljnost**
- **status**
- **ciljnu verziju**

### Primjer
- `ISS-014`
- `Završnica nema dovoljno klimaktičnu napetost`
- kategorija: `psychology / pacing`
- ozbiljnost: `high`
- status: `active`
- target: `v2.3.1`

Issue tracking se može voditi:
- kroz `playtests/issues-tracker.md`
- i/ili kroz GitHub Issues

---

## 12. Preporučena razvojna disciplina

Uvijek koristi ovu logiku:

**ideja → dokumentacija → test → evaluacija → verzija → changelog**

Ne radi obrnutim redom.

Ne zaključavaj promjene:
- prije nego što su opisane
- prije nego što su testirane
- ili prije nego što znaš zašto postoje

---

## 13. Završno pravilo

Verzije u ovom projektu ne služe da zvuče profesionalno.

One služe da zaštite projekat od haosa.

Zato svaka verzija mora predstavljati:
- stvarni razvojni korak
- jasan skup promjena
- i stabilnu osnovu za naredni rad.
