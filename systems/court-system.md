# court-system.md

# Crown of Sovereigns v2.7 — Court System / Sistem dvora

## Status dokumenta

* **Dokument:** `systems/court-system.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** detaljno objasniti kako funkcioniše **Court/Dvor** kao glavni motor odluka u igri
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Cleric/Klerik**
* **Povezani dokumenti:** `gdd/crown-of-sovereigns-v2.7-gdd.md`, `rules/rules-reference-v2.7.md`, `rules/turn-structure.md`, `systems/diplomacy-and-treaties.md`, `systems/stability-and-unrest.md`, `content/court-roles.md`, `ux/player-aid-system.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument objašnjava:

* šta je **Court/Dvor** u sistemu igre
* zašto je **Court/Dvor** glavni identitetski stub
* kako se dvorske uloge koriste u toku runde
* kako **Court/Dvor** stvara agency, tempo i političku težinu
* kako se sistem čuva od prevelikog **downtime/usporenja** i rules bloata

Ovo nije samo opis dvorskih kartica ili uloga.
Ovo je sistemski dokument koji definiše kako cijeli motor odluka radi.

---

## 2. Zašto Court/Dvor postoji

**Court/Dvor** postoji zato što Crown of Sovereigns ne želi da bude samo:

* mapa sa jedinicama
* ekonomska tabela sa resursima
* ili skup nepovezanih akcija

**Court/Dvor** je tu da svaku rundu pretvori u pitanje državničkog prioriteta:

* šta je ovoj kruni sada najvažnije?
* vojni pritisak?
* politički sporazumi?
* trgovački razvoj?
* unutrašnja stabilizacija?
* prikriveno podrivanje protivnika?

Zato **Court/Dvor** nije sporedni podsistem.
On je glavni okvir kroz koji igrač doživljava da vodi državu.

---

## 3. Osnovna dizajnerska funkcija Court/Dvor sistema

**Court/Dvor** mora raditi 5 stvari odjednom:

1. dati igraču smislen izbor prioriteta
2. učiniti svaki potez tematski čitljivim
3. povezati mapu, ekonomiju, diplomatiju i stabilnost
4. ograničiti akcioni haos kroz jasan okvir
5. graditi politički identitet partije

Ako **Court/Dvor** ne radi ove stvari, igra lako sklizne ili u apstraktni euro-flow ili u čisti vojni pritisak.

---

## 4. Šta Court/Dvor nije

Da bi sistem ostao čist, važno je definisati šta **Court/Dvor** nije:

* nije kozmetički “layer” preko običnih akcija
* nije samo izbor bonusa
* nije zasebna mini-igra odvojena od ostatka sistema
* nije administrativni filter koji usporava partiju bez vrijednosti
* nije skup uloga koje svi koriste isto i bez identitetske težine

Ako bi postao bilo šta od ovoga, gubio bi razlog da postoji.

---

## 5. Glavna struktura Court/Dvor sistema

U v2.7 **Court/Dvor** se oslanja na sljedeći okvir:

1. postoji ograničen set glavnih **Court Roles/Dvorskih uloga**
2. igrači kroz reveal / izbor strukturu određuju prioritete runde
3. u akcijskoj fazi vrijedi princip:

> **one core court action per turn / jedna glavna dvorska akcija po potezu**

4. dodatni efekti su mogući samo kada su kratki, eksplicitni i sistemski opravdani
5. dvorske uloge ne zamjenjuju ostatak igre, nego ga fokusiraju

---

## 6. Kanonske Court Roles / Dvorske uloge

Glavne zaključane dvorske uloge u v2.7 su:

* **Marshal/Maršal**
* **Diplomat/Diplomata**
* **Merchant/Trgovac**
* **Cleric/Klerik**
* **Spy/Špijun**

Kritično pravilo:

> ovi nazivi su zaključani.
> ne uvoditi alternativne prevode ili paralelne termine bez eksplicitne verzione odluke.

---

## 7. Uloga svake dvorske funkcije

### 7.1. **Marshal/Maršal**

Predstavlja vojni i teritorijalni fokus vlasti.
Njegova uloga je da otvori:

* mobilizaciju
* pritisak na mapi
* sukob
* odbrambenu ili prijeteću poziciju

### 7.2. **Diplomat/Diplomata**

Predstavlja političko-posrednički fokus vlasti.
Otvara:

* **Treaty/Sporazum** rad
* politički leverage
* diplomatsku vrijednost
* formalne odnose među krunama

### 7.3. **Merchant/Trgovac**

Predstavlja trgovinski i razvojni fokus.
Otvara:

* **Goods/Roba** napredak
* ekonomski tempo
* prihodnu stabilnost
* trgovačku putanju razvoja

### 7.4. **Cleric/Klerik**

Predstavlja legitimacijski i stabilizacioni fokus.
Otvara:

* oporavak ili održavanje **Stability/Stabilnost**
* političku vjerodostojnost
* određene krizne odgovore
* pomoć u očuvanju unutrašnjeg reda

### 7.5. **Spy/Špijun**

Predstavlja prikrivenu i destabilizacionu moć.
Otvara:

* contest elemente
* političko podrivanje
* ciljano kvarenje planova protivnika
* informacijski i taktički pritisak

---

## 8. Zašto je ovih 5 uloga dovoljno

Broj uloga nije slučajan.
Pet uloga je dovoljno da igra:

* ima jasan identitet
* obuhvati glavne državničke sfere
* ne postane preširoka i nečitljiva
* zadrži jasan vizuelni i UX okvir

Dodavanje novih glavnih dvorskih uloga bez vrlo jakog razloga vjerovatno bi povećalo:

* rules overhead
* component bloat
* onboarding težinu
* i vizuelnu konfuziju

---

## 9. Reveal / prioritet struktura

### 9.1. Svrha reveal faze

Reveal ili prioritet dvora postoji da igrač ne ulazi u rundu bez identiteta.
Prije akcione faze mora biti jasno:

* koji je njegov fokus
* kako ta fokusna logika utiče na njegov potez
* gdje će pokušati napraviti tempo ili političku prednost

### 9.2. Zahtjev čitljivosti

Sve relevantno u vezi sa **Court/Dvor** stanjem mora biti:

* javno
* čitljivo
* lako pratljivo sa svih pozicija za stolom

### 9.3. UX pravilo

Ako drugi igrači ne mogu procijeniti nečiji dvorski fokus, politička čitljivost partije pada.

---

## 10. Jedna glavna dvorska akcija po potezu

Ovo je jedno od najvažnijih zaključanih pravila v2.7.

### 10.1. Šta znači

Na svom potezu igrač radi jednu glavnu akciju vezanu za **Court/Dvor** okvir.

### 10.2. Zašto ovo postoji

Ovo pravilo je uvedeno da bi se:

* smanjio **downtime/usporenje**
* smanjio chain combo haos
* povećala čitljivost poteza
* zadržao osjećaj da je svaka odluka važna

### 10.3. Šta ne znači

To ne znači da igra postaje plitka ili da nema interakcije.
To znači da je osnovni tok poteza disciplinovan.

### 10.4. Bonus efekti

Bonus efekti su dozvoljeni samo ako su:

* kratki
* jasno zapisani
* ne traže novu veliku proceduralnu granu
* dio većeg sistema koji je već internalizovan

---

## 11. Kako Court/Dvor povezuje ostatak igre

### 11.1. Court/Dvor + Provinces/Provincije

Dvor određuje kako pristupaš mapi.
Mapa određuje gdje tvoj dvorski plan ima smisla.

### 11.2. Court/Dvor + Goods/Roba

**Merchant/Trgovac** i ekonomski fokus omogućavaju da goods sistem bude aktivna putanja, ne pasivna pozadina.

### 11.3. Court/Dvor + Stability/Stabilnost

**Cleric/Klerik** i određeni dvorski izbori određuju koliko daleko igrač može gurati rizik prije unutrašnjeg loma.

### 11.4. Court/Dvor + Diplomacy/Diplomatija

**Diplomat/Diplomata** pretvara politički layer u formalnu i pobjednički relevantnu putanju.

### 11.5. Court/Dvor + Combat/Borba

**Marshal/Maršal** omogućava sukob, ali ga ne smije učiniti automatski dominantnim.

### 11.6. Court/Dvor + Wow

Veliki wow trenuci u CoS često kreću iz dvorskih odluka, jer one otvaraju:

* rat
* izdaju
* političke obrte
* stabilnost lom
* završni **Coronation Attempt/Pokušaj krunisanja**

---

## 12. Psihološki efekat Court/Dvor sistema

Dobar **Court/Dvor** sistem mora proizvoditi sljedeći osjećaj:

* svaki potez ima političku ličnost
* izbor prioriteta ima cijenu
* nije sve moguće u istoj rundi
* vlast mora birati na šta se oslanja

Ako igrač osjeća da može “raditi sve”, **Court/Dvor** je preslab.
Ako osjeća da je sistem previše stegnut i guši agency, **Court/Dvor** je prekrut.

---

## 13. Balansni ciljevi Court/Dvor sistema

**Court/Dvor** mora pomoći da sljedeće stvari ostanu žive:

* **Aggro/Aggro** da postoji, ali ne dominira
* **Balanced Path/Balansirani put** da bude stvaran
* **Diplomatic Path/Diplomatski put** da bude pun put do pobjede
* ekonomski razvoj da ne bude pasivan dodatak
* contest i politički odgovor da ostanu relevantni

Drugim riječima, **Court/Dvor** ne smije favorizovati samo jednu vrstu igrača.

---

## 14. Court/Dvor i tempo partije

### 14.1. Kako pomaže tempu

Ako radi dobro, **Court/Dvor**:

* skraćuje broj otvorenih opcija po potezu
* čini poteze čitljivijim
* pomaže drugim igračima da predvide smjer runde
* smanjuje paralelni proceduralni haos

### 14.2. Kako može pokvariti tempo

Ako je loše napisan, **Court/Dvor** može:

* dodati reveal bez stvarnog značenja
* učiniti svaki potez sporijim
* generisati previše rubnih izuzetaka
* pretvoriti igru u sporiji administrativni proces

Zato svaki novi dodatak **Court/Dvor** sistemu mora proći anti-bloat provjeru.

---

## 15. Court/Dvor u 2P, 3P i 4P modu

### 15.1. 2P

U 2P modu **Court/Dvor** mora ostati dovoljno bogat da igra ne postane predvidivi duel, ali dovoljno kontrolisan da ne pojača snowball.

### 15.2. 3P

U 3P modu dvorske odluke često postaju najčitljiviji politički signal za sto.

### 15.3. 4P

U 4P modu **Court/Dvor** mora ostati dovoljno jasan da veći broj političkih interakcija ne proizvede konfuziju.

---

## 16. Court/Dvor i First Game Mode / Mod prve partije

U onboarding modu **Court/Dvor** mora ostati potpuno prepoznatljiv, ali objašnjen jednostavnije.

To znači:

* isti identitet
* manje rubnih izuzetaka
* veći oslonac na **Player Aid/Pomoćni igrački vodič**
* fokus na razumijevanje funkcije svake uloge, ne na punu dubinu svih interakcija odmah

---

## 17. Najčešće greške sa Court/Dvor sistemom

* tretirati dvorske uloge kao obične akcione ikone bez identiteta
* koristiti više glavnih akcija u jednom potezu kroz pogrešno tumačenje bonus efekata
* ignorisati kako dvorski fokus signalizira namjeru drugima
* previše usitniti ulogu kroz dodatna mikro-pravila
* pustiti da **Marshal/Maršal** pojede ostatak dvora
* tretirati **Diplomat/Diplomata** kao “sporednu” ulogu

---

## 18. Pravila za buduće izmjene Court/Dvor sistema

Svaka buduća promjena mora proći ovu provjeru:

1. da li jača državnički osjećaj upravljanja?
2. da li čuva princip jedne glavne akcije po potezu?
3. da li smanjuje ili povećava **downtime/usporenje**?
4. da li jača više putanja do pobjede ili samo jednu?
5. da li uvodi component bloat?
6. da li komplikuje onboarding više nego što pomaže dubini?

Ako padne na ovim pitanjima, vjerovatno ne pripada v2.7.x tuning pravcu.

---

## 19. Veza sa grafičkom pripremom

**Court/Dvor** sistem direktno utiče na:

* raspored na player board-u
* ikonografiju dvorskih uloga
* player aid strukturu
* redoslijed prikaza toka runde
* vidljivost reveal / prioritet stanja

Zato ovaj dokument mora ostati potpuno usklađen sa budućim:

* `components/player-board-spec.md`
* `components/iconography-spec.md`
* `ux/player-aid-system.md`
* `visuals/visual-hierarchy.md`

---

## 20. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `rules/rules-reference-v2.7.md`
* `rules/turn-structure.md`
* `systems/diplomacy-and-treaties.md`
* `systems/goods-and-development.md`
* `systems/stability-and-unrest.md`
* `systems/combat-system.md`
* `systems/coronation-system.md`
* `content/court-roles.md`
* `ux/player-aid-system.md`
* `components/player-board-spec.md`
* `components/iconography-spec.md`

---

## 21. Završna napomena

**Court/Dvor** je najvažniji sistemski identitetski motor u **Crown of Sovereigns v2.7**.

Ako radi dobro:

* igra djeluje kao vođenje države
* odluke su politički obojene
* tempo ostaje zdrav
* više putanja do pobjede ostaje živo
* wow momenti imaju jači korijen u sistemu

Ako radi loše:

* igra ili postaje suviše apstraktna
* ili sklizne u vojni autopilot
* ili se uguši u proceduralnom trenju

Zato se ovaj sistem mora tretirati kao centralna osovina cijelog projekta.
