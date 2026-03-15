# canonical-decisions.md

# Crown of Sovereigns — Canonical Decisions

## Status dokumenta

* **Dokument:** `gdd/canonical-decisions.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Locked
* **Svrha:** čuvati listu svih ključnih zaključanih dizajnerskih odluka koje se više ne tretiraju kao otvorena pitanja, osim ako se eksplicitno ne otvori nova verziona odluka
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Cleric/Klerik**

---

## 1. Zašto ovaj dokument postoji

Tokom razvoja igre veliki broj stvari prolazi kroz faze:

* ideja
* hipoteza
* playtest pretpostavka
* privremena odluka
* zaključana odluka

Problem nastaje kada se zaključane odluke kasnije ponovo tretiraju kao da su otvorene, samo zato što nisu nigdje izdvojeno zapisane.

Ovaj dokument postoji da spriječi upravo to.

Njegova funkcija je da kaže:

* šta je u **v2.7** stvarno zaključano
* šta nije više tema za raspravu pri svakom novom dokumentu
* koje odluke čine identitet igre
* koje odluke su proizvod repair procesa i sad su sastavni dio kanonske baze

Kritično pravilo:

> Ako je odluka ovdje zaključana, ne otvara se ponovo usput.
> Može se promijeniti samo kroz novu eksplicitnu verzionu odluku.

---

## 2. Kako koristiti ovaj dokument

Ovaj dokument se koristi kada:

* pišeš novi rules dokument
* pišeš systems dokument
* pripremaš komponentne specifikacije
* provjeravaš da li novo rješenje ruši identitet
* odlučuješ da li je neka tema i dalje otvorena
* procjenjuješ da li nova promjena traži **PATCH**, **MINOR** ili veći razvojni korak

Ne koristi se kao zamjena za GDD.
GDD objašnjava cijeli dizajn.
Ovaj dokument čuva zaključane odluke u kratkoj, operativnoj formi.

---

## 3. Osnovne kanonske odluke o statusu projekta

### CD-001 — Aktivna verzija

**Odluka:** **Crown of Sovereigns v2.7** je jedina aktivna, kanonska i relevantna osnova za dalji razvoj.

**Status:** Locked
**Tip odluke:** projektni status
**Posljedica:** svi novi GitHub dokumenti, pravila i specifikacije moraju polaziti od v2.7.

### CD-002 — Status starijih verzija

**Odluka:** **v2.6.1**, **v2.6**, **v2.5.x** i starije verzije tretiraju se kao arhiva i istorija razvoja, ne kao aktivna baza.

**Status:** Locked
**Tip odluke:** projektni status
**Posljedica:** stare verzije se smiju koristiti samo kao istorijska referenca ili za poređenje.

### CD-003 — Dvojezični terminološki standard

**Odluka:** svi ključni termini u GitHub dokumentaciji koriste format **English/Srpski**, npr. **Goods/Roba**, **Court/Dvor**, **Cleric/Klerik**.

**Status:** Locked
**Tip odluke:** dokumentacioni standard
**Posljedica:** terminology drift više nije dozvoljen.

---

## 4. Osnovne kanonske odluke o identitetu igre

### CD-004 — Žanrovski identitet

**Odluka:** igra ostaje **kompetitivna strateška board game igra upravljanja kraljevstvom**.

**Status:** Locked
**Tip odluke:** identitet
**Posljedica:** igra se ne smije razvijati prema čistom **wargame** ili čistom suhom **euro** modelu.

### CD-005 — Centralna fantazija

**Odluka:** igrač mora imati osjećaj da vodi državu, a ne samo vojsku.

**Status:** Locked
**Tip odluke:** identitet
**Posljedica:** svi novi sistemi i popravke moraju podržavati državnički osjećaj upravljanja.

### CD-006 — Ključni identitetski stubovi

**Odluka:** sljedeći stubovi ostaju netaknuti kao osnova identiteta:

* **Court/Dvor**
* **Provinces/Provincije**
* **Goods/Roba**
* **Stability/Stabilnost**
* **Structured Diplomacy/Strukturisana diplomatija**
* **Condensed Warfare/Kratak rat**
* **Sharp Endgame/Oštra završnica**

**Status:** Locked
**Tip odluke:** identitet
**Posljedica:** nijedna buduća iteracija ne smije ih slučajno oslabiti kroz lokalni tuning.

### CD-007 — Istorijski okvir

**Odluka:** istorijski okvir ostaje Evropa oko 1350.

**Status:** Locked
**Tip odluke:** setting
**Posljedica:** ton, vizuelni pravac i narativna terminologija moraju ostati u tom okviru.

---

## 5. Kanonske odluke o strukturi partije

### CD-008 — Broj igrača

**Odluka:** igra ostaje projektovana za **1–4 igrača**.

**Status:** Locked
**Tip odluke:** opseg proizvoda
**Posljedica:** svi sistemi i dokumenti moraju tretirati 1–4 kao deklarisani raspon.

### CD-009 — Idealni broj igrača

**Odluka:** najbolje iskustvo ostaje na **3–4 igrača**.

**Status:** Locked
**Tip odluke:** iskustvo
**Posljedica:** 2P i solo se razvijaju ozbiljno, ali ne smiju redefinisati cijeli dizajn na štetu 3–4P jezgra.

### CD-010 — Trajanje partije

**Odluka:** ciljani raspon trajanja ostaje približno **90–150 minuta**.

**Status:** Locked
**Tip odluke:** proizvodni cilj
**Posljedica:** novi sistemi ne smiju nekontrolisano gurati partiju preko tog raspona.

### CD-011 — Ciljna težina

**Odluka:** ciljana težina ostaje približno **BGG 3.6–3.7**.

**Status:** Locked
**Tip odluke:** proizvodni cilj
**Posljedica:** tuning i repair ne smiju spašavati probleme tako što dižu kompleksnost izvan te zone bez veoma jakog razloga.

---

## 6. Kanonske odluke o mapi i teritoriji

### CD-012 — Mapa ostaje važna

**Odluka:** mapa nije dekoracija. **Provinces/Provincije** moraju ostati stvarno relevantne za pobjedu, pozicioniranje, goods ekonomiju i politički pritisak.

**Status:** Locked
**Tip odluke:** sistemski stub
**Posljedica:** buduće kompresije ne smiju svesti mapu na bodovni wallpaper.

### CD-013 — Broj provincija

**Odluka:** osnovna mapa koristi **24 Provinces/24 Provincije**.

**Status:** Locked
**Tip odluke:** komponentna / sistemska osnova
**Posljedica:** sve board, setup i component specifikacije moraju polaziti od tog broja dok se ne donese nova verziona odluka.

### CD-014 — Teritorija nije jedini put

**Odluka:** teritorijalna kontrola mora biti važna, ali ne smije biti jedini ili očigledno dominantan put do pobjede.

**Status:** Locked
**Tip odluke:** balansni princip
**Posljedica:** **Aggro/Aggro** ne smije ponovo postati autopilot meta.

---

## 7. Kanonske odluke o Court/Dvor sistemu

### CD-015 — Court/Dvor je glavni motor odluka

**Odluka:** **Court/Dvor** ostaje srce partije i primarni izvor agency-ja.

**Status:** Locked
**Tip odluke:** sistemski stub
**Posljedica:** igra se ne smije pomjeriti prema apstraktnom action soup modelu.

### CD-016 — Jedna glavna dvorska akcija po potezu

**Odluka:** u v2.7 se zaključava princip **one core court action per turn/jedna glavna dvorska akcija po potezu**.

**Status:** Locked
**Tip odluke:** tok i UX
**Posljedica:** smanjenje downtime-a i rules overhead-a ima prioritet nad lančanim mikro-aktivacijama.

### CD-017 — Dvorske uloge ostaju jezgro identiteta

**Odluka:** glavne dvorske uloge ostaju:

* **Marshal/Maršal**
* **Diplomat/Diplomata**
* **Merchant/Trgovac**
* **Cleric/Klerik**
* **Spy/Špijun**

**Status:** Locked
**Tip odluke:** identitet / terminologija
**Posljedica:** ne uvoditi alternativne nazive bez nove zaključane odluke.

---

## 8. Kanonske odluke o Goods/Roba i ekonomiji

### CD-018 — Goods/Roba su poseban sloj identiteta

**Odluka:** **Goods/Roba** nisu isto što i generički resursi; ostaju poseban razvojni i identitetski sistem.

**Status:** Locked
**Tip odluke:** sistemski stub
**Posljedica:** economic layer ne smije biti sveden na puki income tracker.

### CD-019 — Economic coherence je obavezna

**Odluka:** ekonomija mora ostati čitljiva, sistemska i direktno povezana sa razvojem, stabilnošću i strategijom.

**Status:** Locked
**Tip odluke:** dizajnerski princip
**Posljedica:** svaki future tuning mora čuvati osjećaj da Goods/Roba i Income/Prihod rade zajedno, ali nisu ista stvar.

### CD-020 — Balanced Path/Balansirani put mora biti stvaran

**Odluka:** **Balanced Path/Balansirani put** nije više samo teorijska ambicija, nego zaključani cilj koji mora ostati podržan kao realan put do pobjede.

**Status:** Locked
**Tip odluke:** balansni cilj
**Posljedica:** future tuning ne smije ga ponovo pretvoriti u “ispravnu ali presporu” opciju.

---

## 9. Kanonske odluke o Stability/Stabilnost i unutrašnjem pritisku

### CD-021 — Stability/Stabilnost je stvarna cijena moći

**Odluka:** **Stability/Stabilnost** ostaje jedna od glavnih osi dizajna i mora nositi stvarne posljedice za ambiciozne poteze.

**Status:** Locked
**Tip odluke:** sistemski stub
**Posljedica:** širenje, agresija i politički rizici moraju i dalje imati unutrašnju cijenu.

### CD-022 — Unrest/Nemiri ostaje vidljiv signal problema

**Odluka:** **Unrest/Nemiri** ostaju jasan indikator unutrašnjeg pritiska, a ne skrivena sekundarna statistika.

**Status:** Locked
**Tip odluke:** UX / sistem
**Posljedica:** player aid i board UI moraju ga učiniti lako čitljivim.

### CD-023 — Stability cliffs ostaju izvor zasluženog wow-a

**Odluka:** vrhunci partije smiju i trebaju nastajati kroz opasne **Stability/Stabilnost** odluke i njihove posljedice.

**Status:** Locked
**Tip odluke:** wow arhitektura
**Posljedica:** wow ne smije doći iz praznog spektakla kad već sistem ima jači izvor drame.

---

## 10. Kanonske odluke o diplomatiji

### CD-024 — Diplomacy/Diplomatija mora biti formalna

**Odluka:** **Diplomacy/Diplomatija** ostaje strukturisana, mjerljiva i pravilima omeđena.

**Status:** Locked
**Tip odluke:** sistemski stub
**Posljedica:** free-form table talk ne smije zamijeniti formalni sistem.

### CD-025 — Diplomatic windows su vremenski ograničeni

**Odluka:** pregovaranje u v2.7 ide kroz definisane prozore, ne kroz stalni drift preko cijele partije.

**Status:** Locked
**Tip odluke:** UX / flow
**Posljedica:** to je direktan alat za smanjenje downtime-a i održavanje tempa.

### CD-026 — Treaty/Sporazum mora imati zube

**Odluka:** svaki **Treaty/Sporazum** mora imati jasan benefit, ograničenje i posljedicu raskida.

**Status:** Locked
**Tip odluke:** sistemski kvalitet
**Posljedica:** diplomatija ne smije biti flavor-only sloj.

### CD-027 — Diplomatic Path/Diplomatski put je puni win path

**Odluka:** **Diplomatic Path/Diplomatski put** mora ostati realna i puna putanja do pobjede.

**Status:** Locked
**Tip odluke:** balans / identitet
**Posljedica:** future tuning ne smije ga vratiti na status sporednog value engine-a.

### CD-028 — Betrayal/Izdaja mora biti stvarna odluka

**Odluka:** **Betrayal/Izdaja** mora nositi stvarne posljedice i stvarati pamtljive političke obrate.

**Status:** Locked
**Tip odluke:** wow / identitet
**Posljedica:** izdaja ne smije biti jeftin trik bez sistemske težine.

---

## 11. Kanonske odluke o Combat/Borba sistemu

### CD-029 — Rat ostaje važan, ali ne dominantan

**Odluka:** **Condensed Warfare/Kratak rat** ostaje važan sloj, ali ne smije progutati ostatak igre.

**Status:** Locked
**Tip odluke:** identitet / balans
**Posljedica:** CoS ne smije skliznuti u čisti vojni dizajn.

### CD-030 — 3-step combat je zaključan standard

**Odluka:** borba se vodi kroz standard:

* **Declare/Objavi**
* **Modify/Izmijeni**
* **Resolve/Riješi**

**Status:** Locked
**Tip odluke:** flow / clarity
**Posljedica:** svaka nova borbena ideja mora stati unutar tog okvira ili tražiti novu odluku.

### CD-031 — Aggro/Aggro mora imati cijenu

**Odluka:** agresivna ekspanzija ostaje jaka, ali mora nositi dovoljno stabilnost i tempo troškova da ne postane dominantan autopilot.

**Status:** Locked
**Tip odluke:** balans
**Posljedica:** future tuning mora stalno pratiti da rat ostaje relevantan, ali ne previše isplativ.

---

## 12. Kanonske odluke o skaliranju i 2P modu

### CD-032 — 2P mora ostati ozbiljno podržan

**Odluka:** iako je najbolje iskustvo 3–4P, 2P ne smije biti formalno prisutan a dizajnerski zanemaren.

**Status:** Locked
**Tip odluke:** proizvodni cilj
**Posljedica:** 2P health ostaje obavezna playtest osovina.

### CD-033 — 2P Crown Pressure targetira lidera

**Odluka:** u 2P modu **Crown Pressure/Pritisak krune** je usmjeren na lidera, ne simetrično na oba igrača.

**Status:** Locked
**Tip odluke:** scaling / balans
**Posljedica:** to je glavni identity-safe odgovor na 2P snowball rizik.

### CD-034 — Skaliranje ne smije praviti tri različite igre

**Odluka:** 2P, 3P i 4P moraju ostati varijante istog prepoznatljivog jezgra, a ne tri odvojena dizajna.

**Status:** Locked
**Tip odluke:** proizvodna kohezija
**Posljedica:** skaliranje smije prilagođavati pritisak, ali ne smije razbiti identitet.

---

## 13. Kanonske odluke o wow arhitekturi

### CD-035 — Wow mora dolaziti iz sistema

**Odluka:** wow ne smije zavisiti od praznog spektakla, čistog RNG-a ili nezasluženog swinga.

**Status:** Locked
**Tip odluke:** wow princip
**Posljedica:** sve wow ideje moraju proći kroz filter agency-ja, rizika i posljedice.

### CD-036 — Coronation Attempt/Pokušaj krunisanja je glavni wow motor

**Odluka:** **Coronation Attempt/Pokušaj krunisanja** ostaje centralni sistemski vrhunac v2.7.

**Status:** Locked
**Tip odluke:** wow / endgame
**Posljedica:** završna arhitektura i politički pritisak moraju ga podržavati.

### CD-037 — Wow mora biti fer i pričljiv

**Odluka:** vrhunac mora biti:

* zaslužen
* javan
* contestable
* identitetski usklađen
* vrijedan post-game prepričavanja

**Status:** Locked
**Tip odluke:** wow kvalitativni standard
**Posljedica:** scripted chaos ili prazni cinematic dodaci nisu prihvatljivo rješenje.

### CD-038 — Late-crisis compression ostaje dio wow arhitekture

**Odluka:** kasne krize ostaju alat za kompresiju rezultata i stvaranje priče završnice, bez degeneracije u random haos.

**Status:** Locked
**Tip odluke:** endgame / wow
**Posljedica:** završnica mora ostati tijesna, ali poštena.

---

## 14. Kanonske odluke o UX-u i onboarding-u

### CD-039 — First Game Mode ostaje obavezan dio sistema

**Odluka:** **First Game Mode/Mod prve partije** nije pomoćna fusnota, nego zaključani onboarding alat projekta.

**Status:** Locked
**Tip odluke:** onboarding
**Posljedica:** sva buduća rules dokumentacija mora imati onboarding sloj, ne samo full reference.

### CD-040 — Player Aid/Pomoćni igrački vodič je sistemski alat

**Odluka:** **Player Aid/Pomoćni igrački vodič** nije kozmetika, nego ključni dio redukcije pitanja i downtime-a.

**Status:** Locked
**Tip odluke:** UX
**Posljedica:** aid mora biti projektovan zajedno sa pravilima, ne naknadno.

### CD-041 — Round Spine/Kičma runde mora biti čitljiva

**Odluka:** osnovni tok runde mora biti dovoljno jasan da igrač već u prvoj partiji internalizuje ritam igre.

**Status:** Locked
**Tip odluke:** flow / UX
**Posljedica:** future wording i phase design moraju čuvati preglednost runde.

---

## 15. Kanonske odluke o komponentama i produkciji

### CD-042 — Anti-bloat pravilo ostaje aktivno

**Odluka:** problemi se prvo rješavaju kroz wording kompresiju, faznu restrukturaciju, UX pomoć i numeric tuning, a tek onda kroz nove komponente.

**Status:** Locked
**Tip odluke:** produkcija / disciplina
**Posljedica:** component creep nije prihvatljiv default odgovor.

### CD-043 — Komponentna disciplina je dio identiteta projekta

**Odluka:** CoS treba da djeluje premium i ozbiljno, ali ne preglomazno i ne birokratski.

**Status:** Locked
**Tip odluke:** proizvodni identitet
**Posljedica:** graphic prep i production scope moraju ostati kontrolisani.

### CD-044 — Grafički handoff smije krenuti tek nakon zaključavanja ključnih spec dokumenata

**Odluka:** grafika ne smije početi prije nego što su zaključani rules, systems, terminology i components.

**Status:** Locked
**Tip odluke:** proces / produkcija
**Posljedica:** preuranjen visual polish nije dozvoljen ako source-of-truth nije stabilan.

---

## 16. Kanonske odluke o dokumentacionom sistemu

### CD-045 — Single Source of Truth ostaje obavezno pravilo

**Odluka:** za svaku temu postoji jedan glavni dokument koji ima prednost nad izvedenim dokumentima.

**Status:** Locked
**Tip odluke:** dokumentacioni standard
**Posljedica:** paralelne aktivne istine nisu dozvoljene.

### CD-046 — Svaki važan termin mora biti u GLOSSARY.md

**Odluka:** novi sistemski termini ne ulaze slobodno u dokumentaciju bez dodavanja u pojmovnik.

**Status:** Locked
**Tip odluke:** dokumentacioni standard
**Posljedica:** terminološki drift mora biti zaustavljen na ulazu.

### CD-047 — Svaka važna promjena mora ući u CHANGELOG.md

**Odluka:** nijedna važna sistemska promjena ne smatra se završenom dok nije zabilježena u changelog-u.

**Status:** Locked
**Tip odluke:** reviziona disciplina
**Posljedica:** projekat mora ostati auditabilan.

---

## 17. Odluke koje su svjesno odbačene

Ovaj dio postoji da se iste ideje ne vraćaju beskonačno.

### CD-R01 — Odbijena ideja: čisti free-talk diplomatski model

**Zašto odbačeno:** povećava downtime, smanjuje čitljivost i ruši strukturalni identitet diplomatije.

### CD-R02 — Odbijena ideja: proširenje kroz slobodno dodavanje novih podšpilova

**Zašto odbačeno:** rješava probleme kroz bloat umjesto kroz dizajnersku disciplinu.

### CD-R03 — Odbijena ideja: wow kroz nasumične spektakularne evente

**Zašto odbačeno:** daje kratkoročni efekat, ali ruši fer agency i identitetsku usklađenost.

### CD-R04 — Odbijena ideja: rješavanje 2P kroz skoro posebnu mini-igru

**Zašto odbačeno:** skaliranje ne smije pretvoriti 2P u odvojenu igru.

---

## 18. Kada se ovaj dokument smije mijenjati

Ovaj dokument se smije mijenjati samo kada:

* nova verziona odluka zaključava novu stvar
* neka zaključana odluka mora biti formalno zamijenjena
* postoji jasan razlog da se nešto iz otvorene teme prebaci u zaključanu temu
* stara zaključana odluka više nije poštena prema novoj kanonskoj verziji

Ne smije se mijenjati zbog:

* prolazne brainstorm ideje
* neprovjerenog osjećaja da bi nešto “možda bilo zanimljivo”
* lokalne wording preferencije

---

## 19. Brutalno iskrena napomena

Ako canonical decisions nisu jasno zapisane, tim se stalno vraća na iste rasprave.

To znači:

* sporiji razvoj
* više kontradikcija
* više nesigurnosti u dokumentaciji
* više mikrorazvoja bez stvarnog napretka

Zato ovaj dokument nije birokratija.
On je zaštita od zaborava i lutanja.

---

## 20. Završna definicija

Od ove tačke, sve zaključane odluke u ovom dokumentu tretiraju se kao sastavni dio kanonske baze **Crown of Sovereigns v2.7**.

Ako nova promjena želi da ih izmijeni, to više nije usputna korekcija.
To je nova verziona odluka.
