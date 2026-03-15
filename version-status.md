# version-status.md

# Crown of Sovereigns — Version Status

## Status dokumenta

* **Dokument:** `docs/version-status.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Locked
* **Svrha:** jasno definisati koja je verzija aktivna, koje verzije su arhiva i kako se trenutni projekat mora tretirati u svim budućim dokumentima i revizijama
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Cleric/Klerik**

---

## 1. Svrha ovog dokumenta

Ovaj dokument postoji da bi u svakom trenutku bilo potpuno jasno:

* koja verzija igre je aktivna
* koja verzija je kanonska
* koje verzije više nisu operativna baza
* koju verziju svi dokumenti moraju pratiti
* kako razlikovati aktivni razvoj od arhive

Ovo nije pomoćna napomena.
Ovo je dokument koji sprečava najskuplju grešku u razvoju:

> miješanje verzija.

Ako se verzije pomiješaju, posljedice su brze i skupe:

* GDD i rules počnu govoriti različitim jezikom
* playtest feedback postaje nepouzdan
* grafička izrada krene po zastarjeloj logici
* komponente više ne odgovaraju pravilima
* revizije se ne mogu pratiti precizno

---

## 2. Aktivni status projekta

### Aktivna kanonska baza

> **Crown of Sovereigns v2.7** je jedina aktivna, kanonska i relevantna osnova za dalji razvoj.

To znači da se svi budući dokumenti, izmjene, playtest planovi, komponentne specifikacije i grafički handoff dokumenti moraju oslanjati na **v2.7** kao jedini **source of truth/izvor istine** na nivou verzije.

### Šta to praktično znači

Sve buduće reference moraju polaziti od:

* **GDD-a za v2.7**
* **rules** dokumenata za v2.7
* sistemskih dokumenata koji su usklađeni sa v2.7
* dvojezične terminologije zaključane za v2.7

Ako neki dokument koristi stariju verziju kao osnovu, taj dokument nije usklađen i mora se revidirati.

---

## 3. Trenutni status verzija

| Verzija         | Status                             | Kako se tretira                | Napomena                                                    |
| --------------- | ---------------------------------- | ------------------------------ | ----------------------------------------------------------- |
| **v2.7**        | **Locked / Active Canonical Base** | aktivna osnova za dalji razvoj | jedina relevantna verzija                                   |
| **v2.6.1**      | Archived transitional repair layer | istorijska referenca           | važna za razumijevanje repair logike, ali nije aktivna baza |
| **v2.6**        | Archived former canonical base     | istorijska referenca           | prethodna kanonska iteracija                                |
| **v2.5.x**      | Archived historical base           | istorijska referenca           | važna za identitetski temelj, ali nije aktivna baza         |
| starije verzije | Archived                           | arhiva                         | samo za poređenje i istorijsku analizu                      |

---

## 4. Zašto je v2.7 aktivna baza

Verzija **v2.7** je aktivna baza zato što predstavlja najkoherentniji i najstabilniji do sada definisani oblik igre.

U njoj su zaključane sljedeće ključne stvari:

* **Court/Dvor** ostaje glavni motor odluka
* **Goods/Roba** ostaje razvojna i identitetska osovina
* **Stability/Stabilnost** ostaje stvarna cijena moći
* **Structured Diplomacy/Strukturisana diplomatija** ostaje pun i mjerljiv sistem
* **Condensed Warfare/Kratak rat** ostaje važan, ali ne dominantan
* **Coronation Attempt/Pokušaj krunisanja** postaje glavni sistemski wow vrhunac
* 2P dobija lider-targetirani **Crown Pressure/Pritisak krune**
* **Balanced Path/Balansirani put** i **Diplomatic Path/Diplomatski put** više nisu samo teorijski, nego podržani kao realni putevi do pobjede
* **Player Aid/Pomoćni igrački vodič** i onboarding dobijaju veću težinu
* wow arhitektura se gradi iz sistema, ne iz čistog haosa

Drugim riječima, v2.7 nije samo još jedan numerički korak.
To je verzija u kojoj su raniji repair zaključci pretvoreni u stabilniju, čišću bazu za dalji rad.

---

## 5. Šta više nije dozvoljeno od ove tačke

Od ove tačke nije dozvoljeno:

* koristiti **v2.6.1** kao operativnu bazu za nova pravila
* koristiti **v2.6** kao glavni referentni dokument za sistemsku logiku
* vraćati se na **v2.5** wording kao da je aktivan source-of-truth
* pisati nove dokumente koji miješaju rješenja iz više verzija bez eksplicitne verzione odluke
* uvoditi wording ili komponente iz starijih verzija bez revizionog traga

Ako se bilo šta iz starijih verzija koristi, to mora biti:

* označeno kao istorijska referenca
* provjereno protiv v2.7
* i eksplicitno prihvaćeno u novom dokumentu

---

## 6. Pravilo za sve buduće GitHub dokumente

Svi budući GitHub dokumenti za projekat moraju poštovati sljedeće:

### 6.1. Verzijska usklađenost

Dokument mora jasno pokazivati da radi sa **v2.7**.

### 6.2. Nema miješanja starih pravila

Ako postoji konflikt između starijeg dokumenta i v2.7 dokumenta, prednost ima v2.7 dokument.

### 6.3. Dvojezična terminologija je obavezna

Svi ključni termini pišu se u formatu:

* **English/Srpski**

Primjeri:

* **Court/Dvor**
* **Goods/Roba**
* **Marshal/Maršal**
* **Diplomat/Diplomata**
* **Cleric/Klerik**
* **Spy/Špijun**
* **Influence/Uticaj**
* **Stability/Stabilnost**

### 6.4. Source-of-truth logika ostaje obavezna

Ako se piše novi dokument, mora biti jasno:

* da li je to glavni dokument za temu
* ili izvedeni dokument koji referencira glavni izvor

---

## 7. Kako koristiti starije verzije bez pravljenja haosa

Starije verzije nisu zabranjene kao istorijski materijal. One su i dalje korisne za:

* razumijevanje evolucije dizajna
* praćenje zašto je neka odluka donesena
* poređenje prije / poslije
* identifikaciju starih problema koji se možda vraćaju

Ali njihova upotreba ima stroga pravila:

### Dozvoljeno

* koristiti ih za analizu
* koristiti ih za istorijsko poređenje
* koristiti ih za referencu u changelog-u ili canonical-decisions dokumentu

### Nije dozvoljeno

* tretirati ih kao aktivna pravila
* kopirati njihove formulacije bez provjere usklađenosti sa v2.7
* koristiti ih kao bazu za nove komponente ili grafiku

---

## 8. Kada se mijenja ovaj dokument

Ovaj dokument se ažurira samo kada se desi jedna od sljedećih stvari:

* nova verzija postane kanonska baza
* aktivna verzija promijeni status
* promijeni se pravilo kako se arhiva tretira
* promijeni se režim rada sa verzijama u repozitoriju

Ovaj dokument se ne mijenja zbog sitnih balans korekcija ako one ne utiču na aktivni status verzije.

---

## 9. Veza sa ostalim ključnim dokumentima

Ovaj dokument je direktno povezan sa:

* `README.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `gdd/crown-of-sovereigns-v2.7-gdd.md`
* `gdd/canonical-decisions.md`
* `revision/document-status-matrix.md`

Ako se status verzije promijeni, svi gore navedeni dokumenti moraju biti provjereni i usklađeni.

---

## 10. Kako nova osoba treba da pročita repo

Ako nova osoba ulazi u projekat, čita redom:

1. `README.md`
2. `docs/version-status.md`
3. `VERSIONING.md`
4. glavni GDD za v2.7

To je minimalni ulaz da odmah shvati:

* šta je projekat
* koja je aktivna baza
* kako se verzije tretiraju
* gdje počinje pravi rad

---

## 11. Brza kontrolna lista za provjeru usklađenosti

Prije nego što se novi dokument smatra validnim, provjeri:

* da li eksplicitno radi sa **v2.7**
* da li koristi dvojezične termine
* da li referencira ispravan source-of-truth dokument
* da li ne vraća zastarjelu logiku iz v2.6.1 ili starije baze
* da li je u skladu sa identitetskim stubovima **Court/Dvor**, **Goods/Roba**, **Stability/Stabilnost**, **Structured Diplomacy/Strukturisana diplomatija**, **Condensed Warfare/Kratak rat**

Ako odgovor na bilo koju od tih tačaka nije jasan, dokument nije još spreman.

---

## 12. Brutalno iskrena napomena

Najbrži način da projekat postane konfuzan nije manjak kvaliteta, nego manjak verzijske discipline.

Ako se izgubi jasan status verzije, onda:

* playtest nalazi više nisu pouzdani
* dokumenti se međusobno sudaraju
* dizajn djeluje manje zreo nego što jeste
* grafička izrada će gotovo sigurno biti skuplja i haotičnija

Zato je ovaj dokument namjerno vrlo direktan:

> od ove tačke postoji samo jedna aktivna istina na nivou verzije — **v2.7**.

---

## 13. Završna definicija

Od sada važi:

* **Crown of Sovereigns v2.7** = jedina aktivna kanonska verzija
* svi novi dokumenti = v2.7 usklađeni
* starije verzije = arhiva i istorija razvoja
* svaka buduća promjena = ide kroz verzionu i revizionu disciplinu

Ovaj dokument služi da ta logika ostane jasna i neupitna kroz cijeli dalji razvoj projekta.
