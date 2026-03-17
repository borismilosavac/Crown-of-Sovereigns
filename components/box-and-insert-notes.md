# box-and-insert-notes.md

# Crown of Sovereigns v2.7 — Box and Insert Notes / Bilješke za kutiju i insert

## Status dokumenta

* **Dokument:** `components/box-and-insert-notes.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati funkcionalne zahtjeve, logističke prioritete i produkcijske granice za **Box/Kutiju** i **Insert/Insert** sistem igre
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Box/Kutija**, **Insert/Insert**, **Setup/Setup**
* **Povezani dokumenti:** `components/tokens-spec.md`, `components/cards-spec.md`, `components/units-and-markers-spec.md`, `components/board-spec.md`, `components/player-board-spec.md`, `rules/setup-guide.md`, `ux/player-aid-system.md`, `docs/release-readiness-checklist.md`, `GLOSSARY.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* definiše kako **Box/Kutija** i **Insert/Insert** treba da podrže stvarnu upotrebu igre
* spriječi da pakovanje bude tretirano kao čisto estetski dodatak bez logističke funkcije
* poveže broj i tip komponenti sa realnim potrebama skladištenja, sortiranja i pripreme partije
* pomogne da setup i teardown ostanu disciplinovani u skladu sa identitetom **v2.7**
* pripremi osnov za kasniji produkcijski i manufacturability pregled

Ovo nije finalni industrijski packaging dokument.
Ovo je funkcionalna specifikacija i skup guardrail-a za budući packaging rad.

---

## 2. Zašto su kutija i insert kritični

Kod složenijih strateških igara problemi često ne počinju tek kad igra krene, nego i ranije:

* otvaranje kutije je haotično
* komponente nisu logično razvrstane
* setup traje duže nego što bi morao
* teardown je spor i frustrirajući
* dijelovi se oštećuju ili miješaju između sesija

Ako **Box/Kutija** i **Insert/Insert** rade loše:

* igra djeluje većom i težom nego što jeste
* i dobar UX na tabli i aid-u gubi dio vrijednosti
* playtest i release spremnost pate kroz čistu logistiku

Zato pakovanje nije sporedna stvar. Ono je produžetak upotrebljivosti sistema.

---

## 3. Osnovni princip dizajna pakovanja

Glavno pravilo glasi:

> kutija i insert moraju prvenstveno smanjivati logistički teret igre, a ne dodavati proizvodni luksuz bez funkcionalnog povrata.

To znači:

* unutrašnja organizacija mora pratiti kako se igra stvarno postavlja i koristi
* prioritet imaju brz pristup i jasno sortiranje
* dekorativna rješenja ne smiju otežati otvaranje, vraćanje i zaštitu komponenti

Ako je rješenje lijepo, ali nepraktično, nije dobro rješenje za CoS.

---

## 4. Šta ovaj dokument jeste

Ovaj dokument treba da bude:

* funkcionalni packaging vodič
* osnova za buduće procjene box volumena i insert logike
* filter protiv logističkog i produkcijskog bloata
* most između komponentne specifikacije i fizičke spremnosti proizvoda

---

## 5. Šta ovaj dokument nije

Ovaj dokument nije:

* finalni manufacturing blueprint
* art brief za spoljašnji box cover
* luksuzni unboxing koncept
* izgovor da se prije vremena zaključavaju skupi produkcijski detalji

Ovdje je fokus na funkciji, ne na prestige pakovanju.

---

## 6. Glavne funkcije kutije i inserta

**Box/Kutija** i **Insert/Insert** sistem treba da rade najmanje sljedeće:

1. štite komponente
2. održavaju logičan raspored sadržaja
3. ubrzavaju **Setup/Setup** i **Teardown/Raspremanje**
4. smanjuju miješanje karti, tokena, jedinica i markera
5. ostanu produkcijski razumni u odnosu na stvarni opseg igre

Ako rade samo prvu stvar, ali ne i drugu, treću i četvrtu, logistika partije ostaje preskupa.

---

## 7. Osnovne klase sadržaja koje box sistem mora podržati

Kutija i insert moraju uzeti u obzir najmanje ove klase sadržaja:

### 7.1. Board Components / Komponente table

* glavna **Board/Tabla**
* **Player Boards/Table igrača**
* aid elementi

### 7.2. Cards / Karte

* **Treaty Cards/Karte sporazuma**
* **Event Cards/Karte događaja**
* **Crisis Cards/Karte kriza**
* eventualne coronation ili druge reference kartice

### 7.3. Tokens / Tokeni

Svi definisani **Tokens/Tokeni** elementi.

### 7.4. Units and Markers / Jedinice i markeri

Mapne jedinice, markeri kontrole, osporavanja, stabilnosti i ostali relevantni markeri.

### 7.5. Documentation / Dokumentacija

* rulebook ili rules reference
* quickstart ili first game materijal
* aid sažeci gdje je primjenjivo

Insert logika mora pratiti ove grupe dovoljno jasno da se ne miješaju bez razloga.

---

## 8. Box / Kutija — osnovni zahtjevi

Kutija mora biti:

* dovoljno velika da primi sadržaj bez nasilnog sabijanja
* dovoljno disciplinovana da ne pravi lažni premium volumen bez potrebe
* dovoljno čvrsta za ponovljenu upotrebu i transport
* dovoljno logična da insert i sadržaj u njoj imaju stabilan raspored

Važno pravilo:

* box size ne treba projektovati po idealizovanom maksimumu “za svaki slučaj”, nego po realnom obimu **v2.7** + razumnom prostoru za zaštitu i organizaciju.

---

## 9. Insert / Insert — osnovni zahtjevi

Insert mora biti:

* funkcionalan
* intuitivan
* dovoljno robustan za ponovljeno vraćanje komponenti
* usklađen sa realnim setup redoslijedom

Insert ne smije biti:

* previše granularan bez potrebe
* toliko osjetljiv da igrač mora slagati komponente savršeno da bi kutija mogla da se zatvori
* rješenje koje radi samo bez sleeve-ova ili samo sa njima, ako to nije unaprijed odlučeno

---

## 10. Setup-driven logika inserta

Insert treba pratiti kako se igra stvarno postavlja.

To znači da najprirodnije odvojene cjeline treba da budu:

* brzo dostupne pri setupu
* lako vraćene nakon partije
* grupisane prema načinu korištenja, ne samo prema materijalu

Primjer zdrave logike:

* mape i table zajedno
* kartični paketi logično odvojeni
* tokeni i markeri grupisani po stvarnoj upotrebi
* lične komponente organizovane tako da se mogu brzo podijeliti igračima

---

## 11. Teardown-driven logika inserta

Jednako važno kao setup je i raspremanje.

Dobro rješenje mora omogućiti da poslije partije:

* komponente imaju očigledno mjesto povratka
* vraćanje ne traži dug lookup “šta ide gdje”
* osjetljive karte i kartonski elementi ne budu sabijeni između tvrđih dijelova

Ako insert izgleda uredno, ali je spor za vraćanje sadržaja, realno nije dovoljno dobar.

---

## 12. Kartični prostor u insertu

Kartama treba posvetiti poseban prostor jer su među najosjetljivijim i najčešće korištenim komponentama.

Insert mora uzeti u obzir:

* odvojene kartične grupe
* dovoljno jasan pristup za sortiranje i uzimanje
* zaštitu od savijanja i pritiskanja
* potencijalnu potrebu za sleeve tolerancijom, ako se to želi podržati

Ako kartični prostor postane preuzak ili prenapet, to direktno smanjuje kvalitet upotrebe i trajnost proizvoda.

---

## 13. Token i marker prostor u insertu

**Tokens/Tokeni**, **Markers/Markeri** i manje jedinice moraju biti organizovani tako da:

* se ne miješaju bez razloga
* mogu brzo u setup ući kao odvojene logične grupe
* ne traže beskrajno kopanje po kutiji

Previše sitnih odjeljaka može biti jednako loše kao i premalo.

Dobro pravilo:

* grupisati po stvarnoj stolnoj funkciji, ne po opsesivnoj mikro-klasifikaciji.

---

## 14. Player kit logika

Ako igra koristi jasan lični set po igraču, insert treba gdje god je moguće podržati logiku “uzmi svoj paket i kreni”.

To znači:

* dijelovi vezani za jednog igrača treba da se mogu brzo razdvojiti
* ne treba da budu rasuti kroz pet različitih odjeljaka ako to usporava setup

Ovo je posebno korisno za:

* **Player Boards/Table igrača**
* lične markere
* lične jedinice ili početne resurse, ako su dio seta

---

## 15. Board and large components prostor

Velike komponente kao što su:

* glavna tabla
* table igrača
* veći aid ili reference listovi

moraju imati stabilan i siguran raspored koji:

* ne savija rubove
* ne prelama kartonske elemente
* ne stvara pritisak na karte ili manje plastične/drvene dijelove ispod njih

Veliki elementi često izgledaju “jednostavni za smjestiti”, ali loš raspored ovdje lako ošteti ostatak sadržaja.

---

## 16. Documentation slot / Slot za dokumentaciju

Pravila, quickstart i aid dokumenti ne smiju biti tretirani kao višak koji se samo “nekako ugura”.

Treba predvidjeti mjesto za:

* rules reference
* quickstart ili first game pomoćni materijal
* eventualni scenario ili setup list ako postoji

To mjesto mora biti:

* lako dostupno
* dovoljno ravno
* bez pritiska koji gužva papir ili tanji karton

---

## 17. Insert i komponentni budžet

Insert ne smije tiho podsticati komponentni bloat.

To znači:

* ne praviti prazne komplikovane zone za komponente koje još nemaju opravdanje
* ne širiti box footprint samo da bi insert izgledao impresivnije
* insert mora odgovarati realnom budžetu komponenti **v2.7**, a ne fantaziji o budućem “možda” sadržaju

Ako packaging logika unaprijed traži više komponenti nego što igra zaslužuje, to je loš signal.

---

## 18. Insert i produkcijski rizik

Rješenje za insert mora ostati razumno i po proizvodnom riziku.

Treba biti oprezan sa:

* previše složenim višespratnim insert logikama
* rješenjima koja traže vrlo precizne tolerancije
* luksuznim rješenjima koja znatno dižu cijenu bez jasnog UX povrata

CoS treba funkcionalno i disciplinovano rješenje, ne komplikovani prestige insert po svaku cijenu.

---

## 19. Insert i transport / skladištenje

Treba razmišljati i o tome da sadržaj kutije ostane dovoljno stabilan kada se:

* kutija uspravi
* pomjera
* nosi
* više puta otvara i zatvara

Ako komponente ispadaju iz logičnih grupa pri svakom pomjeranju, insert ne radi dovoljno dobro.

---

## 20. Odnos sa sleeve policy logikom

Ako se u budućnosti želi podrška za sleeve-ovane karte, to mora biti eksplicitno odlučeno.

Dobra packaging praksa traži da se rano zna:

* da li insert cilja raw cards ili sleeved cards
* da li tolerancija podržava bar umjeren sleeve scenario

Najgora opcija je neodlučna sredina gdje insert ne radi ni za jedno ni za drugo stanje dovoljno dobro.

---

## 21. Box and insert odnos prema onboarding-u

Pakovanje utiče i na onboarding više nego što djeluje na prvi pogled.

Ako je otvaranje kutije i prvo razvrstavanje haotično:

* prva partija djeluje težom
* setup stvara pogrešan prvi utisak
* pomoćni materijali kasnije spašavaju nešto što packaging nije podržao

Dobro pakovanje pomaže da igra već pri prvom otvaranju djeluje organizovano i razumljivo.

---

## 22. Veza sa components dokumentima

Ovaj dokument mora biti usklađen sa:

* `components/tokens-spec.md`
* `components/cards-spec.md`
* `components/units-and-markers-spec.md`
* `components/board-spec.md`
* `components/player-board-spec.md`

Ako packaging logika ne prati stvarni komponentni sistem, dobiće se lijep insert za pogrešan set potreba.

---

## 23. Veza sa setup i aid logikom

Ovaj dokument mora se čitati zajedno sa:

* `rules/setup-guide.md`
* `ux/player-aid-system.md`

Zašto?
Zato što insert nije neutralan. On direktno utiče na:

* redoslijed setupa
* brzinu prve partije
* koliko brzo igrači dolaze do pravih komponenti

Ako setup vodič i insert logika rade jedno protiv drugog, logistika pati.

---

## 24. Najčešće greške u box/insert radu

* kutija je prevelika bez potrebe
* insert izgleda impresivno, ali otežava vraćanje sadržaja
* kartični prostor je preuzak ili previše rascjepkan
* male komponente se previše miješaju
* lične komponente nisu grupisane logično
* dokumentacija nema siguran slot
* rješenje radi samo u idealno složenom stanju, ne i u stvarnoj upotrebi

---

## 25. Workflow pravilo za novo packaging rješenje

Ako se predlaže novo **Box/Kutija** ili **Insert/Insert** rješenje, treba provjeriti redom:

1. da li ubrzava ili usporava setup
2. da li ubrzava ili usporava teardown
3. da li bolje štiti komponente
4. da li povećava ili smanjuje produkcijski rizik
5. da li prati stvarne komponente i njihove grupe
6. da li dodaje luksuz bez dovoljno funkcionalnog povrata

Ako ne prolazi ova pitanja, rješenje nije dovoljno dobro za CoS.

---

## 26. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li pakovanje ostaje funkcionalno prije svega?
2. da li insert prati stvarni setup i teardown tok?
3. da li ostaje komponentno i produkcijski disciplinovano?
4. da li smanjuje ili povećava logistički teret?
5. da li ostaje usklađeno sa ostatkom komponentne dokumentacije?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 27. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `components/tokens-spec.md`
* `components/cards-spec.md`
* `components/units-and-markers-spec.md`
* `components/board-spec.md`
* `components/player-board-spec.md`
* `rules/setup-guide.md`
* `ux/player-aid-system.md`
* `docs/release-readiness-checklist.md`
* `GLOSSARY.md`

---

## 28. Završna napomena

**Box and Insert Notes / Bilješke za kutiju i insert** moraju ostati jedan od glavnih logističkih filtera u **Crown of Sovereigns v2.7**.

Ako rade dobro:

* setup je brži
* teardown je čišći
* komponente su zaštićenije
* igra djeluje organizovanije već pri prvom otvaranju
* a produkcijski okvir ostaje disciplinovan

Ako rade loše:

* čak i dobra igra djeluje napornije nego što treba
* logistika guši UX
* komponente se teže čuvaju i vraćaju
* a proizvod djeluje manje zreo nego što sistem zaslužuje

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
