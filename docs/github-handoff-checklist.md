# github-handoff-checklist.md

# Crown of Sovereigns v2.7 — GitHub Handoff Checklist / Checklist za GitHub handoff

## Status dokumenta

* **Dokument:** `docs/github-handoff-checklist.md`
* **Aktivna verzija igre:** **v2.7**
* **Status dokumenta:** Draft
* **Svrha:** definisati obaveznu checklistu prije predaje, objave ili internog zaključavanja dokumentacije na GitHub-u
* **Pravilo jezika:** svi ključni termini pišu se dvojezično, npr. **Handoff/Predaja**, **Checklist/Checklista**, **Dependency/Zavisnost**
* **Povezani dokumenti:** `docs/repository-structure.md`, `docs/revision-workflow.md`, `docs/document-status-policy.md`, `docs/version-status.md`, `VERSIONING.md`, `CHANGELOG.md`, `GLOSSARY.md`, `gdd/canonical-decisions.md`

---

## 1. Svrha ovog dokumenta

Ovaj dokument služi da:

* uvede jasan završni pregled prije nego što dokument ili paket dokumenata bude predat na GitHub kao aktivna radna baza
* spriječi da u repo uđu polovično usklađeni, terminološki nečisti ili verziono zbunjujući dokumenti
* pomogne da svaki handoff bude pregledan, revizijski siguran i spreman za dalji rad
* smanji rizik da se poslije predaje tek otkriju osnovne greške u statusu, zavisnostima i strukturi

Ovo nije samo formalna kontrolna lista.
Ovo je završni filter prije nego što dokumentacija postane stvarno operativna u repozitorijumu.

---

## 2. Zašto je GitHub handoff checklist kritična

Bez završne checkliste vrlo brzo nastaju problemi:

* dokument izgleda gotov, ali nema ispravan status
* verzija u dokumentu nije usklađena sa aktivnom bazom
* povezani dokumenti nisu ažurirani
* terminologija nije dosljedna
* fajl je na pogrešnom mjestu ili se preklapa sa postojećim dokumentom
* patch ili revizija nema trag gdje bi trebala imati

Dobra handoff checklista hvata ove greške prije nego što postanu dio radne baze.

---

## 3. Osnovni princip handoffa

Glavno pravilo glasi:

> dokument nije spreman za GitHub handoff samo zato što je napisan; spreman je tek kada je sadržajno, verziono i strukturno usklađen sa ostatkom repozitorijuma.

To znači da handoff mora provjeriti najmanje:

* sadržaj
* status
* verziju
* folder
* ime fajla
* zavisnosti
* terminologiju
* revizioni trag gdje je potreban

---

## 4. Šta ova checklista jeste

Ova checklista treba da bude:

* završni pregled prije predaje
* alat za samoprovjeru
* alat za internu provjeru kvaliteta repozitorijuma
* sigurnosna mreža protiv brzih i tihih grešaka

---

## 5. Šta ova checklista nije

Ova checklista nije:

* zamjena za revision workflow
* zamjena za changelog
* zamjena za playtest validaciju
* izgovor da dokument izgleda spreman i kad nije

Ona je zadnji pregled, ne cijeli proces razvoja.

---

## 6. Kada se koristi GitHub handoff checklist

Checklistu treba koristiti najmanje u ovim situacijama:

* kada se dodaje novi važan dokument u repo
* kada se set postojećih dokumenata ažurira u okviru jedne revizije
* kada se patch dokumentacija zaključava za novu test seriju
* kada se aktivna verzija ili njen status formalno ažurira
* kada se priprema paket za grafički, UX ili playtest handoff

Ne treba je preskakati samo zato što promjene “djeluju male”, ako realno mogu zbuniti stanje repozitorijuma.

---

## 7. Glavne kategorije provjere

Checklistu treba organizovati kroz ove glavne kategorije:

1. **Version Check/Provjera verzije**
2. **Document Status Check/Provjera statusa dokumenta**
3. **Naming and Placement Check/Provjera imena i smještaja**
4. **Dependency Check/Provjera zavisnosti**
5. **Terminology Check/Provjera terminologije**
6. **Cross-Document Consistency Check/Provjera dosljednosti između dokumenata**
7. **Revision Trace Check/Provjera revizionog traga**
8. **Readiness Check/Provjera spremnosti za upotrebu**

Ovaj redoslijed treba ostati isti jer ide od osnovnog identiteta dokumenta ka njegovoj operativnoj spremnosti.

---

## 8. Version Check / Provjera verzije

Prvo treba provjeriti:

* da li dokument navodi tačnu aktivnu verziju igre
* da li je verzija u skladu sa `docs/version-status.md`
* da li dokument slučajno sadrži ostatke starije verzije u naslovima, primjerima ili formulacijama
* da li ime fajla treba ili ne treba verzijsku oznaku po pravilima iz `VERSIONING.md`

Ako verzija nije čista, dokument nije spreman za handoff.

---

## 9. Document Status Check / Provjera statusa dokumenta

Treba provjeriti:

* da li dokument ima jasno naveden status
* da li je taj status realan
* da li je status usklađen sa `docs/document-status-policy.md`
* da li dokument možda izgleda kao **Locked/Zaključano**, a zapravo je još **Draft/Nacrt** ili **Review/U provjeri**

Status ne smije biti optimistična maska. Mora biti stvarno stanje dokumenta.

---

## 10. Naming and Placement Check / Provjera imena i smještaja

Treba provjeriti:

* da li ime fajla koristi `kebab-case`
* da li ime fajla jasno opisuje funkciju dokumenta
* da li se fajl nalazi u pravom folderu prema `docs/repository-structure.md`
* da li već postoji sličan dokument koji ovaj treba dopuniti umjesto duplirati

Ako ime ili folder nisu pravilni, to treba ispraviti prije handoffa, ne kasnije.

---

## 11. Dependency Check / Provjera zavisnosti

Treba provjeriti:

* da li su **Povezani dokumenti** lista relevantna i potpuna
* da li **Dependency notes** postoje gdje su potrebni
* da li promjene u ovom dokumentu traže promjene u drugim dokumentima
* da li su ti drugi dokumenti već ažurirani ili barem eksplicitno označeni za naknadnu reviziju

Ovo je jedan od najvažnijih koraka jer hvata tihi raspad dosljednosti.

---

## 12. Terminology Check / Provjera terminologije

Treba provjeriti:

* da li su svi ključni termini u skladu sa `GLOSSARY.md`
* da li su dvojezični formati dosljedni
* da li se koristi isti redoslijed **English/Srpski**
* da li se koristi standardni separator `/`
* da li postoje paralelni nazivi koji ne bi smjeli postojati

Ako terminologija nije čista, dokument nije spreman za ozbiljan rad u repozitorijumu.

---

## 13. Cross-Document Consistency Check / Provjera dosljednosti između dokumenata

Treba provjeriti:

* da li dokument kontradiktira systems, rules ili content bazu
* da li koristi iste klase, statuse i nazive kao povezani dokumenti
* da li opisuje isti proces ili sistem drugačije od već zaključanog dokumenta bez jasne revizije
* da li se u primjerima i objašnjenjima zadržava ista logika verzije **v2.7**

Ovaj korak je posebno važan za dokumente koji povezuju više slojeva repo-a.

---

## 14. Revision Trace Check / Provjera revizionog traga

Treba provjeriti:

* da li promjena traži unos u `CHANGELOG.md`
* da li promjena traži ažuriranje `docs/version-status.md`
* da li promjena traži novu stavku u `gdd/canonical-decisions.md`
* da li je revizija usklađena sa `docs/revision-workflow.md`

Ne treba svaka mala korekcija globalni trag, ali svaka značajna promjena mora ostaviti pravi zapis na pravom mjestu.

---

## 15. Readiness Check / Provjera spremnosti za upotrebu

Na kraju treba provjeriti:

* da li dokument može odmah služiti svojoj svrsi
* da li je dovoljno jasan za naredni korak procesa
* da li bi novi saradnik ili budući ti mogao razumjeti kako se koristi
* da li dokument ima previše otvorenih rupa da bi bio stvarno upotrebljiv

Ovo je završna procjena: da li dokument stvarno radi, ne samo da li formalno postoji.

---

## 16. Minimalna obavezna checklist forma

Prije handoffa preporučeni minimalni format provjere je:

* **Version Check/Provjera verzije:** pass / fail
* **Status Check/Provjera statusa:** pass / fail
* **Naming & Placement/ime i smještaj:** pass / fail
* **Dependencies/Zavisnosti:** pass / fail
* **Terminology/Terminologija:** pass / fail
* **Consistency/Dosljednost:** pass / fail
* **Revision Trace/Revizioni trag:** pass / fail / not needed
* **Ready for Handoff/Spremno za handoff:** yes / no

Ako ijedna važna stavka padne, handoff ne treba tretirati kao završen.

---

## 17. Preporučena dodatna pitanja prije handoffa

Pored formalne checkliste, korisno je pitati:

* da li ovaj dokument smanjuje ili povećava mogućnost zabune?
* da li uvodi novi pojam bez dovoljno razloga?
* da li izgleda više zaključano nego što stvarno jeste?
* da li sam ostavio nešto “da se poslije sredi”, a zapravo je temeljno za upotrebu?
* da li je ovo pravi trenutak za handoff ili dokument još traži jednu reviziju?

Ova pitanja pomažu protiv prerane predaje.

---

## 18. Kada handoff treba odbiti ili odgoditi

Handoff treba odgoditi ako:

* verzija nije čista
* status je nejasan ili pogrešan
* dokument kontradiktira aktivnu bazu
* ključne zavisnosti nisu ažurirane
* terminologija nije usklađena
* dokument još nije dovoljno upotrebljiv za svoju svrhu

Bolje je odgoditi predaju nego uvesti dokument koji kasnije pravi više štete nego koristi.

---

## 19. Pravilo za pakete dokumenata

Kad se ne predaje jedan dokument nego paket, treba dodatno provjeriti:

* da li svi dokumenti u paketu pripadaju istoj verzionoj osnovi
* da li im statusi imaju smisla kao grupa
* da li zajedno pokrivaju jednu cjelinu bez rupa i dupliranja
* da li jedan dokument u paketu ne kvari dosljednost ostalih

Handoff paketa je rizičniji od handoffa jednog dokumenta i zato traži strožiju provjeru.

---

## 20. Veza sa revision workflow dokumentom

`docs/revision-workflow.md` definiše kako promjena nastaje i prolazi kroz proces.

`docs/github-handoff-checklist.md` definiše završnu kontrolu prije nego što rezultat tog procesa postane operativno prisutan u repozitorijumu.

Jedan dokument vodi promjenu.
Drugi provjerava da li je spremna da uđe u radnu bazu bez kvarenja strukture.

---

## 21. Veza sa repository structure dokumentom

`docs/repository-structure.md` kaže gdje dokument treba da živi.

Ova checklista provjerava da li zaista živi na pravom mjestu, sa pravim imenom i pravim odnosom prema ostalim dokumentima.

To dvoje zajedno čine osnovu čistog handoffa.

---

## 22. Veza sa document status policy dokumentom

`docs/document-status-policy.md` definiše šta status znači.

Ova checklista provjerava da li je status konkretno dobro primijenjen na dokument koji ide u handoff.

To je važno jer je status jedna od najčešćih stvari koje izgledaju riješene, a zapravo nisu.

---

## 23. Najčešće greške pri GitHub handoffu

* dokument je dobar, ali verziono pogrešan
* dokument ima ispravan sadržaj, ali pogrešan status
* dokument je na pogrešnom mjestu u repo-u
* zavisni dokument nije ažuriran
* terminologija je “skoro ista”, ali ne dovoljno dosljedna
* revizioni trag nije ostavljen gdje treba
* paket dokumenata izgleda kompletno, ali krije jednu kontradikciju koja kasnije pravi haos

---

## 24. Workflow pravilo za korištenje checkliste

Kad se radi handoff, preporučeni redoslijed je:

1. provjeriti verziju i status
2. provjeriti ime i folder
3. provjeriti zavisnosti i dosljednost
4. provjeriti terminologiju
5. provjeriti revizioni trag
6. donijeti finalnu odluku: spremno / nije spremno

Ako se radi obrnuto, često se previše vremena troši na finese prije nego što se uhvate osnovne greške.

---

## 25. Pravila za buduće izmjene ovog dokumenta

Svaka buduća promjena mora proći ovu provjeru:

1. da li checklista ostaje praktična?
2. da li hvata stvarne greške prije handoffa?
3. da li ostaje kratka, ali dovoljno stroga?
4. da li pomaže verzionoj disciplini?
5. da li ostaje upotrebljiva i za pojedinačne dokumente i za pakete?

Ako promjena ne prolazi ova pitanja, vjerovatno nije dobar **v2.7.x** korak.

---

## 26. Dependency notes

Ako se ovaj dokument mijenja, obavezno provjeriti:

* `docs/repository-structure.md`
* `docs/revision-workflow.md`
* `docs/document-status-policy.md`
* `docs/version-status.md`
* `VERSIONING.md`
* `CHANGELOG.md`
* `GLOSSARY.md`
* `gdd/canonical-decisions.md`

---

## 27. Završna napomena

**GitHub Handoff Checklist / Checklista za GitHub handoff** mora ostati jedan od glavnih završnih filtera prije nego što dokument ili paket dokumenata postane operativan dio repozitorijuma.

Ako radi dobro:

* manje grešaka ulazi u repo
* verzije se manje miješaju
* dokumenti su čišći i upotrebljiviji
* revizije imaju manje naknadnih popravki
* a cijeli projekat djeluje sigurnije i profesionalnije

Ako radi loše:

* handoff postaje formalnost bez stvarne zaštite
* kontradikcije i greške ulaze u bazu
* kasnije korekcije postaju skuplje
* a repo počinje da izgleda stabilnije nego što zaista jeste

Zato ovaj dokument mora ostati strog, praktičan i potpuno usklađen sa logikom **v2.7**.
