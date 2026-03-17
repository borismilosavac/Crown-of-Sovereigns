# crown-of-sovereigns-v2.7-gdd.md

# Crown of Sovereigns v2.7 — Game Design Document / Dokument dizajna igre

## Status dokumenta

* **Dokument:** `gdd/crown-of-sovereigns-v2.7-gdd.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** objediniti kanonsku bazu verzije **v2.7** u jedan glavni GDD dokument koji povezuje identitet igre, ciljeve dizajna, osnovne sisteme, strukturu partije, komponente, UX i razvojne guardrail-e
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Court/Dvor**, **Goods/Roba**, **Stability/Stabilnost**, **Treaty/Sporazum**, **Coronation Attempt/Pokušaj krunisanja**
* **Povezani dokumenti:** `gdd/canonical-decisions.md`, `docs/version-status.md`, `rules/rules-reference-v2.7.md`, `rules/setup-guide.md`, `rules/turn-structure.md`, `rules/scoring-reference.md`, `systems/win-paths.md`, `systems/coronation-system.md`, `components/component-manifest.md`, `GLOSSARY.md`

---

# 1. Executive Summary / Izvršni sažetak

**Crown of Sovereigns** je **kompetitivna strateška board game igra upravljanja kraljevstvom** (*competitive kingdom-management strategy board game*) smještena u istorijski inspirisanu Evropu oko 1350. godine.

U srcu igre nije samo rat, niti samo ekonomija.
Srce igre je:

* **Court/Dvor** kao upravni i politički motor
* mapa i **Provinces/Provincije** kao stvarni prostor moći
* **Goods/Roba** i razvoj kao dugoročna snaga države
* **Stability/Stabilnost** kao cijena ambicije
* formalna **Diplomacy/Diplomatija** kroz **Treaty/Sporazum** sistem
* završni politički i legitimacijski pritisak kroz **Coronation Attempt/Pokušaj krunisanja**

Cilj dizajna nije da igra djeluje kao čisti **wargame** ili kao suhi **euro**.
Cilj je da igrač ima osjećaj da zaista vodi kraljevstvo pod pritiskom.

---

# 2. Core Identity / Jezgro identiteta

## 2.1. Jednorečenični identitet

**Crown of Sovereigns** je igra u kojoj igrači vode kraljevstva kroz **Court/Dvor**, teritoriju, **Goods/Robu**, **Stability/Stabilnost** i formalnu **Diplomacy/Diplomatiju**, pokušavajući da do kraja partije pretvore izgrađenu moć u legitimnu pobjedu.

## 2.2. Šta igra mora osjećajno isporučiti

Igra mora davati osjećaj:

* državničkog pritiska
* političke težine odluka
* prostorne napetosti na mapi
* cijene moći
* zaslužene završne kulminacije

## 2.3. Šta igra ne smije postati

Igra ne smije skliznuti u:

* čisti **wargame** bez državne dubine
* čisti **euro** sa mapom kao dekoracijom
* diplomatski “free talk” bez formalne težine
* završnicu koja briše cijelu partiju kroz nezasluženi swing

---

# 3. Product Definition / Definicija proizvoda

## 3.1. Format

* **Tip:** kompetitivna strateška board game igra
* **Broj igrača:** 1–4
* **Najbolje iskustvo:** 3–4
* **2P cilj:** ozbiljno podržan, ali ne glavni prodajni profil
* **Trajanje:** približno 90–150 minuta
* **Ciljna težina:** oko BGG 3.6–3.7

## 3.2. Komercijalni profil

Igra cilja publiku koja voli:

* strateške igre srednje više težine
* političku interakciju
* mapni pritisak
* višestruke puteve do pobjede
* igre koje daju osjećaj narativne partije, a ne samo matematičke optimizacije

## 3.3. Referentni benchmark prostor

Primarni benchmark prostor čine:

* **Dune: Imperium – Uprising**
* **Scythe**
* **Inis**
* **Brian Boru**
* **Oath**
* **Hegemony**

CoS ne pokušava biti kopija nijedne od tih igara.
Njegov cilj je da zauzme vlastitu nišu u prostoru **statecraft/state management** dizajna.

---

# 4. Design Pillars / Dizajnerski stubovi

## 4.1. Court/Dvor is central / Court-Dvor je centralan

**Court/Dvor** nije bonus modul.
On je glavni političko-upravni motor koji govori gdje je fokus države u toj rundi.

## 4.2. Map matters / Mapa je stvarno važna

**Board/Tabla** i **Provinces/Provincije** moraju biti stvarna osovina moći.
Teritorija nije dekorativna.

## 4.3. Goods/Roba drive state quality / Goods-Roba grade kvalitet države

**Goods/Roba** i razvoj nisu samo resursna ekonomija.
Oni predstavljaju rast, kapacitet i dugoročnu državnu snagu.

## 4.4. Stability/Stabilnost is the cost of power / Stabilnost je cijena moći

Igrač može gurati ambiciju, ali država mora izdržati posljedice.
**Stability/Stabilnost** mora biti i kazna i pokazatelj kvaliteta države.

## 4.5. Diplomacy/Diplomatija is formal / Diplomatija je formalna

Pregovor nije samo društvena improvizacija.
**Treaty/Sporazum** sistem mora nositi pravila, obaveze i stvarnu pobjedničku relevantnost.

## 4.6. Endgame must be sharp / Završnica mora biti oštra

Partija mora završiti kao politička i legitimacijska kulminacija, ne kao troma računica ni kao haotični reset.

---

# 5. Player Fantasy / Fantazija igrača

Igrač ne igra generičnog vladara.
Igrač vodi državu kroz konflikte između:

* ekspanzije i održivosti
* ambicije i stabilnosti
* saveza i izdaje
* razvoja i vojnog pritiska
* kratkoročnog dobitka i završne legitimnosti

Najvažniji osjećaj koji igra mora isporučiti je:

> “Moje kraljevstvo je moćno, ali da li zaista može izdržati i završiti kao legitimni pobjednik?”

---

# 6. Intended Experience / Namjeravano iskustvo

## 6.1. Početak partije

Rani dio partije treba dati osjećaj otvaranja prostora:

* upoznavanje sa mapom
* prvi politički odnosi
* prvi signal dvora
* rano pozicioniranje goods i stabilnosti

## 6.2. Sredina partije

Sredina partije treba donijeti:

* rast napetosti
* jače političke blokove i raskide
* jasniji konflikt interesa
* prve ozbiljne cijene nestabilnosti
* sve konkretniji oblik svakog **Win Path/Puta do pobjede**

## 6.3. Kraj partije

Kraj partije mora donijeti:

* osjećaj da se sve izgrađeno sada testira
* pojačanu relevantnost legitimiteta, završnog pritiska i coronation logike
* mogućnost foto-finiš završnice bez jeftinog reset osjećaja

---

# 7. Player Counts and Modes / Broj igrača i modovi

## 7.1. 2P

2P mora biti:

* napet
* čitljiv
* podržan dodatnim korektivima kao što je **Crown Pressure/Pritisak krune**
* zaštićen od prebrzog runaway obrasca

## 7.2. 3P

3P je jedan od najvažnijih ciljnih modova.
Treba biti:

* politički najčitljiviji
* dovoljno otvoren za diplomatiju
* dovoljno kompaktan da ostane pod kontrolom u teachu i downtime-u

## 7.3. 4P

4P treba biti najbogatiji mod.
Mora dati:

* najviše političke gustine
* najviše mogućih savezničkih i izdajničkih obrta
* najviše stolne energije

Ali ne smije skliznuti u pregovarački mulj ili proceduralni zastoj.

## 7.4. Solo/Automa

**Automa/Automa** postoji kao podrška za:

* solo učenje
* sistemski trening
* funkcionalan solo izazov

Ali solo nije centralni identitetski stub proizvoda.

---

# 8. Win Condition / Uslov pobjede

Pobjeda ne dolazi iz jedne osovine.
Pobjeda dolazi iz toga da igrač:

* izgradi dovoljno jaku teritorijalnu i političku osnovu
* razvije državu kroz **Goods/Robu** i druge razvojne alate
* održi ili iskontroliše **Stability/Stabilnost** i **Unrest/Nemire**
* dođe u završnicu sa dovoljno moći i legitimiteta
* prođe završni **Coronation Attempt/Pokušaj krunisanja** i povezani contest jače od ostalih

---

# 9. Macro System Overview / Pregled glavnih sistema

Glavni sistemi igre su:

1. **Court System/Sistem dvora**
2. **Province and Map System/Sistem provincija i mape**
3. **Goods and Development/Sistem robe i razvoja**
4. **Stability and Unrest/Sistem stabilnosti i nemira**
5. **Diplomacy and Treaties/Sistem diplomatije i sporazuma**
6. **Combat System/Sistem borbe**
7. **Event and Crisis System/Sistem događaja i kriza**
8. **Catch-up and Runaway Control/Sistem povratka i kontrole runaway lidera**
9. **Scaling 2P-3P-4P/Sistem skaliranja 2P-3P-4P**
10. **Coronation System/Sistem krunisanja**

Ovaj GDD daje zajednički okvir za sve njih, dok pojedinačni systems dokumenti nose detalje.

---

# 10. Court System / Sistem dvora

## 10.1. Uloga sistema

**Court/Dvor** je političko-upravni motor igre.
On pokazuje gdje igrač ulaže fokus svoje države.

## 10.2. Dizajnerski cilj

Dvor mora:

* osjećajno nositi državu
* biti relevantan svake runde
* uticati na glavni akcioni tok
* dati identitetski signal igračevom stilu

## 10.3. Rizik koji sistem rješava

Bez jakog **Court/Dvor** sistema, CoS bi previše lako skliznuo u mapnu ili ekonomsku igru bez državničkog centra.

---

# 11. Province and Map System / Sistem provincija i mape

## 11.1. Uloga sistema

Mapa i **Provinces/Provincije** predstavljaju prostor moći, pritiska i konflikta.

## 11.2. Dizajnerski cilj

Mapa mora:

* biti stvarna, ne dekorativna
* nositi teritorijalnu vrijednost
* proizvoditi contested situacije
* hraniti i političke i vojne odluke

## 11.3. Ključna razlika

**Presence/Prisutnost** i **Control/Kontrola** nisu uvijek isto.
To je važno za političku i državničku teksturu igre.

---

# 12. Goods and Development / Roba i razvoj

## 12.1. Uloga sistema

**Goods/Roba** i razvoj grade dugoročnu državu, ne samo kratkoročni gain.

## 12.2. Dizajnerski cilj

Ovaj sistem mora omogućiti da:

* ekonomski pristup bude stvarno pobjednički relevantan
* goods imaju identitet, ne samo funkciju resursa
* razvoj ulazi u završnu jednačinu moći i legitimiteta

## 12.3. Ključni rizik

Ako goods daju samo “dobra podešavanja” bez stvarne završne težine, **Economic Path/Ekonomski put** djeluje pametno, ali ne pobjednički.

---

# 13. Stability and Unrest / Stabilnost i nemiri

## 13.1. Uloga sistema

**Stability/Stabilnost** i **Unrest/Nemiri** predstavljaju unutrašnju održivost kraljevstva.

## 13.2. Dizajnerski cilj

Sistem mora:

* učiniti da moć ima cijenu
* razlikuje zdravu i prenapregnutu državu
* bude završno relevantan
* biti dovoljno jasan da ga igrač osjeti, ne samo vidi kao broj

## 13.3. Ključni rizik

Ako sistem postane samo kaznen, gubi stratešku eleganciju.
Ako postane preslab, gubi identitetsku funkciju.

---

# 14. Diplomacy and Treaties / Diplomatija i sporazumi

## 14.1. Uloga sistema

Diplomatija daje formalni politički prostor između igrača.

## 14.2. Dizajnerski cilj

**Treaty/Sporazum** sistem mora:

* biti javan i čitljiv
* davati stvarne benefite i obaveze
* proizvoditi politički leverage
* podržati stvaran **Diplomatic Path/Diplomatski put** do pobjede

## 14.3. Ključni rizik

Ako diplomatija bude samo socijalni sloj bez završne težine, jedan od glavnih diferencijatora igre propada.

---

# 15. Combat System / Sistem borbe

## 15.1. Uloga sistema

Borba postoji da presiječe važne mapne i političke situacije.

## 15.2. Dizajnerski cilj

Borba mora biti:

* kratka
* jasna
* skupa
* važna
* ali ne dominantna nad ostatkom igre

## 15.3. Ključni rizik

Ako borba preuzme previše pažnje, igra prestaje biti prvenstveno državnička.
Ako je preslaba, mapa i pritisak gube zube.

---

# 16. Event and Crisis System / Događaji i krize

## 16.1. Uloga sistema

**Event/Događaj** i **Crisis/Kriza** sistem daje zajednički ritamski pritisak partiji.

## 16.2. Dizajnerski cilj

Ovaj sistem mora:

* postaviti zajednički kontekst runde
* mijenjati prioritete bez oduzimanja agency-ja
* pojačavati sredinu i kraj partije

## 16.3. Ključni rizik

Ako događaji i krize postanu previše skriptovani ili previše swingy, igra gubi osjećaj zasluženosti.

---

# 17. Catch-up and Runaway Control / Povratak i kontrola runaway lidera

## 17.1. Uloga sistema

Sistem mora omogućiti da partija ostane otvorena dovoljno dugo, bez kažnjavanja lidera na nepošten način.

## 17.2. Dizajnerski cilj

Potrebno je:

* držati agresivni snowball pod kontrolom
* otvoriti povratne prozore
* sačuvati zasluženost vodstva

## 17.3. Ključni rizik

Ako catch-up postane prejak, igra djeluje nepošteno.
Ako je preslab, završnica postaje lažno napeta ili zatvorena prerano.

---

# 18. Scaling / Skaliranje

## 18.1. Uloga sistema

Skaliranje omogućava da isti identitet igre radi u 2P, 3P i 4P bez raspada uloge pojedinih sistema.

## 18.2. Dizajnerski cilj

Skaliranje mora:

* održati političku relevantnost u 3P i 4P
* zadržati 2P pod kontrolom kroz posebne korektive
* ne praviti potpuno drugu igru po player count-u

---

# 19. Coronation System / Sistem krunisanja

## 19.1. Uloga sistema

**Coronation Attempt/Pokušaj krunisanja** je završni politički i legitimacijski test partije.

## 19.2. Dizajnerski cilj

Sistem mora:

* pojačati završnicu
* biti dovoljno snažan da završni contest bude stvaran
* biti dovoljno pošten da ne briše cijelu partiju
* osjećajno djelovati kao kulminacija državne borbe

## 19.3. Ključni rizik

Ako je coronation preblag, završnica je ceremonialna.
Ako je prejak, završnica djeluje kao reset i ruši pravičnost.

---

# 20. Round Structure / Struktura runde

Kanonska runda u v2.7 sastoji se od:

1. **Event/Crisis Phase/Faza događaja i krize**
2. **Diplomatic Window/Diplomatski prozor**
3. **Court Reveal and Order/Otkrivanje dvora i redoslijed**
4. **Action Phase/Faza akcija**
5. **Conflict Resolution/Rješavanje sukoba**
6. **Income and Development/Prihod i razvoj**
7. **Stability and Unrest Update/Ažuriranje stabilnosti i nemira**
8. **Round End Check/Završna provjera runde**

Ovaj redoslijed je proceduralna kičma igre.

---

# 21. Scoring Logic / Logika bodovanja

Bodovni okvir se dijeli na:

* **Ongoing Value/Tekuća vrijednost**
* **Triggered Scoring/Okidano bodovanje**
* **Endgame Scoring/Završno bodovanje**

Glavne osovine koje hrane pobjedu su:

* **Territorial Value/Teritorijalna vrijednost**
* **Political and Treaty Value/Politička i sporazumska vrijednost**
* **Goods and Development Value/Vrijednost robe i razvoja**
* **Stability and State Quality/Vrijednost stabilnosti i kvaliteta države**
* **Endgame and Coronation Pressure/Završna i coronation vrijednost**

---

# 22. Main Win Paths / Glavni putevi do pobjede

Kanonski glavni stilovi koje igra mora podržati su:

* **Aggro/Aggro**
* **Balanced Path/Balansirani put**
* **Diplomatic Path/Diplomatski put**
* **Economic Path/Ekonomski put**
* plus ponašajni profili kao **Opportunist/Oportunista** i **Defender/Branilac**

Ključno pravilo:
ni jedan od glavnih puteva ne smije biti samo teorijski prisutan.
Svaki mora imati realan završni domet.

---

# 23. Components Overview / Pregled komponenti

Glavne komponente v2.7 su:

* glavna **Board/Tabla**
* **Player Boards/Table igrača**
* **Treaty Cards/Karte sporazuma**
* **Event Cards/Karte događaja**
* **Crisis Cards/Karte kriza**
* završne referentne komponente gdje su potrebne
* **Tokens/Tokeni**
* **Units/Jedinice**
* **Markers/Markeri**
* aid i onboarding materijali

Sve komponente moraju biti vođene funkcijom, ne viškom dekorativnog ili produkcijskog tereta.

---

# 24. UX Principles / UX principi

## 24.1. Prva partija mora biti lakša od pune dubine igre

To znači:

* jak **Quickstart/Brzi vodič**
* jasan **Setup/Setup** vodič
* čista **Round Spine/Kičma runde** logika
* snažan **Player Aid/Pomoćni igrački vodič**

## 24.2. Informacijska hijerarhija mora biti brutalno jasna

Na tabli i tablama igrača mora biti jasno:

* šta je zajednički kontekst
* šta je lično stanje
* šta je prostorni status
* šta je završna prijetnja

## 24.3. Fizička čitljivost ima prioritet nad ukrasom

Komponentni sistem mora služiti brzom čitanju partije.

---

# 25. Art and Visual Direction Constraints / Ograničenja art i vizuelnog smjera

Iako puni vizuelni dokumenti stoje odvojeno, ovaj GDD zaključava nekoliko guardrail-a:

* tabla i komponente moraju biti čitljive prije nego dekorativne
* vizuelni sistem mora podržati političku i državničku ozbiljnost
* završni i coronation signali moraju biti vizuelno važni, ali ne smiju jesti ostatak table
* karta i marker sistem ne smiju postati ornamentalno teški na račun UX-a

---

# 26. Playtest Priorities / Prioriteti playtesta

Najvažniji test fokusi za v2.7 su:

* zdravlje **2P** moda
* realna snaga **Balanced Path/Balansirani put**
* realna završna relevantnost **Diplomatic Path/Diplomatski put**
* goods i razvoj kao stvaran završni motor
* pravi balans između wow i pravičnosti u **Coronation Attempt/Pokušaj krunisanja** sistemu
* kontrola downtime-a, posebno u **4P**

---

# 27. Production Guardrails / Produkcijski guardrail-i

## 27.1. Nema komponentnog bloata bez stvarnog povrata

Novi token, marker, kartična klasa ili packaging sloj mora opravdati svoj logistički i produkcijski trošak.

## 27.2. Nema “premium” rješenja bez funkcije

CoS ne smije izgledati raskošnije nego što je praktično održivo.

## 27.3. Box, insert i setup moraju služiti brzini ulaza

Pakovanje je dio UX-a, ne samo dio prezentacije.

---

# 28. Main Risks / Glavni rizici verzije

Glavni razvojni rizici v2.7 su:

* prevelik teach teret za prvu partiju
* proceduralna magla između političkih i akcionih faza
* diplomatski leverage bez dovoljno finishing power-a
* goods i razvoj koji djeluju važnije nego što se stvarno prevode u pobjedu
* 2P runaway rizik
* 4P pregovarački downtime
* završnica koja može skliznuti ili u ceremonijalnost ili u prejak swing

---

# 29. Success Conditions / Uslovi uspjeha verzije

Verzija v2.7 se može smatrati uspješnom ako:

* nova grupa poslije prve dvije runde razumije centralnu fantaziju igre
* **Court/Dvor**, mapa, **Goods/Roba**, **Stability/Stabilnost** i diplomatija svi djeluju stvarno važni
* glavni **Win Paths/Putanje do pobjede** izgledaju živo
* završnica djeluje oštro, pošteno i pamtljivo
* igra djeluje kao država pod pritiskom, a ne kao skup odvojenih mini-sistema

---

# 30. Role in Repository / Uloga u repozitorijumu

Ovaj GDD dokument služi kao:

* glavni krovni dizajnerski dokument verzije **v2.7**
* sažeti kanonski pregled za nove saradnike
* orijentir za rules, systems, content, components, UX i playtest slojeve

On nije zamjena za pojedinačne dokumente, ali jeste njihova zajednička osovina.

---

# 31. Dependency Notes / Napomene o zavisnostima

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `gdd/canonical-decisions.md`
* `docs/version-status.md`
* `rules/rules-reference-v2.7.md`
* `rules/setup-guide.md`
* `rules/turn-structure.md`
* `rules/scoring-reference.md`
* `systems/win-paths.md`
* `systems/coronation-system.md`
* `components/component-manifest.md`
* `GLOSSARY.md`

---

# 32. Završna napomena

**Crown of Sovereigns v2.7 GDD / Dokument dizajna igre** mora ostati glavni krovni dokument koji odgovara na pitanje:

> šta je ova igra, šta pokušava da bude i po kojim pravilima razvoja čuva svoj identitet?

Ako ovaj dokument radi dobro:

* cijeli repo djeluje povezanije
* novi dokumenti lakše nalaze svoje mjesto
* verzione promjene se manje miješaju
* a svi budući handoff-i imaju mnogo jači zajednički temelj

Ako radi loše:

* systems dokumenti djeluju kao izolovana ostrva
* pitch i dizajnerski identitet se razdvajaju
* a repo izgleda bogatije nego što je stvarno koherentan

Zato ovaj dokument mora ostati jasan, detaljan i potpuno usklađen sa kanonskom logikom **v2.7**.
