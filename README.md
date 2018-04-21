# ZUS Edu
 Projekt na predmet Objektovo orientované programovanie
 
 autor: Patrik Honíšek
 
 IDE: Eclipse
 
 Jazyk: Java
 
 UI : JavaFX
 
 ak. rok: 2017/2018
 
 prednášajúci: V. Vranić
 
 
## Stručný popis programu:
Program slúži ako informačný systém pre základné umelecké školy. Používatelia sú rozdelení do troch kategórií: žiaci, rodičia, učitelia.
Každá skupina má špeciálny prístup k jednotlivým funkcionalitám. Program poskytuje prehľad vyučovaných predmetov, zobrazenie a prácu 
so známkami, platenie školného, prezeranie výučbových materiálov a posielanie správ medzi používateľmi.

## Sprievodca používaním:
Tento sprievodca by Vám mal lepšie priblížiť čo všetko program dokáže a ako používať jednotlivé funkcionality.

### Login
Loginové okno je prvé, ktoré sa otvorí po spustení programu a je jediné, z ktorého je možné program (správne) ukončiť použitím [x]
Jeho použitie je jednoduché proste zadajte prihlasovacie údaje do príslušných políčok (cheetsheet s údajmi je v PrihlasovacieUdaje.txt)

---

### Menu
Menu okno Vám poskytne náhľad základných sekcií programu, ktoré budú bližšie priblížené nižšie

---

### Hodiny
Prvá možnosť, ktorú ponúka Menu Vám poskytne prístup k predmetom, v novom okne sú k dispozícii dve možnosti:
- **Prihlasovanie hodín**  - táto možnosť je prístupná **len pre žiakov**, môžete sa v nich prihlásiť a odhlásiť z jednotlivých predmetov
- **Moje hodiny** - táto možnosť zobrazí v prípade žiaka hodiny, na ktoré je prihlásený, v prípade rodiča hodiny, na ktoré je prihlásené
jeho dieťa a v prípade učiteľa hodiny, ktoré vyučuje

---

### Známky  
Druhá možnosť, ktorú ponúka Menu Vám poskytne prístup k známkam, v novom okne sa zobrazia predmety, ktoré navštevujete/vyučujete
- **Žiak (Rodič)** - ako žiakovi (aj rodičovi) sa Vám po kliknutí na konkrétny predmet otvorí okno so známkami, ktoré ste dostali z daného
predmetu
- **Učiteľ** - ako učiteľovi sa Vám po kliknutí na konkrétny predmet otvorí okno s novvými možnosťami, ktoré predstavujú jednotliví žiaci
daného predmetu, následne po odkliknutí konkrétneho žiaka sa zobrazia jeho známky a je tam možnosť pridať, odobrať nejakú známku ale aj možnosť vypočítať aritmetický priemer známok

---

### Platby
Tretia možnosť, ktorú ponúka Menu, Vám poskytne prístup a informácie o platbách, táto funkcia je prístupná **len pre rodičov**, ktorým sa
po otvorení v okne zobrazí prehľad, aká suma bola zaplatená a koľko treba mesiacov ešte zaplatiť
- **Uskutočnenie platby** - platba sa vykoná tak, že zvolíte počet mesiacov (ak už nijaké neostávajú program vás na to upozorní už pri 
otvorení okna platieb) a následne zvolíte spôsob platby
- **Platba kartou** - možnosť platby kartou sa líši od zvyšných dvoch pretože jediná vyžaduje Vašu interakciu, je potrebné zadať údaje
o karte, pre úspešné pokračovanie platbov ďalej treba vyplniť všetky údaje, po úspešnom zadaní údajov o karte bude program od Vás žiadať ešte SMS verifikáciu a to kódom, ktorý príde na telefónne číslo, ktoré je zadané pri danom bankovom účte (momentálne tam stačí zadať hocičo), po úspešnom zadaní prebehne platba

---

### Materiály
Štvrtá možnosť, ktorú ponúka Menu, Vám umožňuje prácu s vyvesenými materiálmi, ak prvé sa otvorí zoznam predmetov, po kliknutí na vybraný
predmet sa otvorí list s materiálmi pridanými pre daný predmet
- **Otvoriť** - jednoducho otvorí príslušný materiál, je to spustiteľné pre akomkoľvek type súboru
- **Tlačiť** - táto možnosť je platná **len pre dokumenty s príponami .pdf, .txt** alebo **.docx**
- **Pridať** - táto možnosť je **len pre učiteľov**, umožňuje pridať materiál na základe názvu a aj nastaviť jeho menovku v programe,
program následne už sám pri vypisovaní materiálov vyhodnotí či daný materiál existuje alebo nie, takže používateľ nebude upozornení hneď
ale neskôr sa na chýbajúci súbor ukáže

---

### Správy
Piata možnosť, ktorú ponúka Menu, Vám umožňuje komunikáciu s ostatnými používateľmi:
- **Napísať novú správu** - táto možnosť otvorí okno s formátom správy, adresáta si vyberáte z ponuky všetkých používateľov, ďalej je možnosť zadať predmet, ak do tohoto políčka nič nevpíšete správa sa odošle s implicitne nastaveným názvom premet *Bez predmetu*, ďalej nasleduje už samotný text správy, ten prázdny ostať nesmie, program Vás nepustí ak tam nebude **aspoň jeden znak**
- **Prijaté správy** - zobrazí zoznam prijatých správ od najnovších po najstaršie vo formáte: *Predmet*(*odosielateľ*), toto okno umožňuje
jednotlivé správy zobraziť a aj na ne odpovedať
- **Odoslané správy** - pracuje na rovnakom princípe ako prijaté správy akurát, že zobrazuje správy, ktoré boli odoslané Vami
- **Odpoveď na jednotlivú správu** - možnosť odpovede na správu je v prijatých aj v odoslaných správach, po jej zvolení sa otvorí okno, do
ktorého môžete napísať Vašu odpoveď (tu ešte nie je ošetrené aby musel byť v správe aspoň jeden znak), predmet aj adresát sú pevne daní, na
základe správy, na ktorú píšete odpoveď

---

### Odhlásenie
Posledná možnosť, ktorú ponúka Menu, zatvorí všetky existujúce okná programu a otvorí nové loginové okno

---

## Spustenie
Program je spustiteľný zatiaľ len vytvorením projektu v Eclipse a importovaním všetkých .java súborov do tohto projektu, metóda *main* sa 
nachádza v súbore PrihlasenieGUI.java
