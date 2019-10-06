# Testy zgodności z WCAG

## Co to jest?


## Wprowadzenie
W literaturze polskiej istnieją aktualnie dwa systematyczne opracowania poświęcone ocenianiu dostępności:

- [Metodologia badania dostępności strony www](http://www.pad.widzialni.org/index.php?p=new&idg=mg,12&id=637) dla osób niepełnosprawnych, starszych i innych narażonych na wykluczenie cyfrowe w oparciu o WCAG 2.0
- [Badanie dostępności strony internetowej w oparciu o WCAG](http://www.widzialni.org/badanie-dostepnosci-strony-www-w-oparciu-o-wcag,new,mg,5,254)

Ten skromny zestaw został wzbogacony tłumaczeniem na język polski francuskiej metodyki badania dostępności:

- [RGAA - Francuska metodyka badania dostępności](https://www.gov.pl/web/dostepnosc-cyfrowa/francuska-metodyka-badania-dostepnosci-rgaa)

### Metodologia, podstawy, zarys, wstęp?

[Metodologia badania dostępności strony www](http://www.pad.widzialni.org/index.php?p=new&idg=mg,12&id=637) to licząca 30 stron publikacja elektroniczna opracowana w 2013 roku wysiłkiem Fundacji Widzialni we współpracy z Uniwersytetem Śląskim przez zespół w składzie: dr Izabela Mrochen (UŚl) oraz Przemysław Marcinkowski, Marcin Luboń i Artur Marcinkowski (Fundacje Widzialni). 

W skrótowej formie, wręcz lapidarnie autorzy sygnalizują problemy i hipotezy, metody, technik i strategie, organizację i przebieg audytu oraz kwestie raportowania i interpretacji wyników audytu. 

Proponowana „metodologia badań dostepności” autorzy opierają na metodzie analizy realizowanej w dwóch etapach badania – **analizie eksperckiej** i **badania z użytkownikami**. 

Na etapie analizy eksperckiej proponują zastosowanie czterech metod: 

- **metoda I** – sprawdzanie zgodności ze standardami HTML lub XHTML z wykorzystaniem usługi internetowej udostępnionej przez W3C pod adresem http://validator.w3.org/
- **metoda II** – sprawdzanie zgodności CSS ze standardami określonymi przez W3C z wykorzystaniem usługi internetowej udostępnionej pod adresem http://jigsaw.w3.org/css-validator/  
- **metoda III problemowa** – sprawdzenie zgodności z WCAG 2.0 z wykorzystaniem swego rodzaju list kontrolnych zestawionych w 13 tabelach, zbierających wskazówki do audytu według kryterium zasad i wytycznych zdefiniowanych w WCAG.
- **metoda IV** – analiza kontrastu z użyciem narzędzia Contrast Analyzer oferowanego przez PacielloGroup oraz trybu wysokiego kontrastu w systemie operacyjnym MS Windows.      

Charakterystyka metod sprowadza się zestawionych w 13 tabelkach zwięzłych 1-3 zdaniowych wskazówek, co należy poddać badaniu i z rzadka, jakiego użyć narzędzia.

Na etapie badania z użytkownikiem autorzy proponują obserwację uczestniczącą realizacji przez kilku użytkowników z niepełnosprawnościami zestawu  trzech do pięciu zadań, których dobór zależy od charakteru i celów strony, np. założenie swojego konta na stronie, odnalezienie numeru telefonu kontaktowego, odnalezienie informacji przy pomocy wyszukiwarki, zamówienie towaru w sklepie internetowym.

Druga pozycja - [Badanie dostępności strony internetowej w oparciu o WCAG](http://www.widzialni.org/badanie-dostepnosci-strony-www-w-oparciu-o-wcag,new,mg,5,254) jest opracowanym przez Artura Marcinkowskiego rozwinięciem pierwszej, z nieco wzbogaconymi wskazówkami dotyczącymi sposobu oceniania zgodności z poszczególnymi kryteriami sukcesu WCAG oraz o obszerną, blisko 50-stronicową prezentację narzędzi do badnia i oceniania dostępności autorstwa Sebastiana Depty. 

Jeśli przyjąć choćby za Wikipedią, że [metodologia](https://pl.wikipedia.org/wiki/Metodologia) to „nauka o metodach badań naukowych, ich skuteczności i wartości poznawczej”, omówione opracowanie, nie umniejszając w najmniejszym stopniu jego znaczenia, trudno byłoby nawet uznać za wstęp, zarys czy nawet szkic do metodologii. 

Tym bardziej nie jest to rzecz, którą można by nazwać „polską metodologią”. Określenie to w założeniu sugeruje, że wypracowana została jakaś oryginalna **polska** metodologia badania i oceniania zgodności z WCAG, czy szerzej dostępności cyfrowej. Żadna z przedstawionych w broszurze metod nie jest oryginalna, żadna nie postuluje niczego nowego, czego wcześniej nie prezentowano w dość już bogatej w 2013 roku anglojęzycznej literaturze przedmiotu.

Obie pozycje można traktować co najwyżej jako dobry początek drogi do opracowania, **niekoniecznie polskiej**, ale **po polsku**metodologii, a raczej podstaw metodologii badania dostepności cyfrowej, która oby jak najszybciej stała się przedmiotem systematycznych dociekań naukowych.

### O metodyce RGAA
[RGAA](https://www.gov.pl/web/dostepnosc-cyfrowa/francuska-metodyka-badania-dostepnosci-rgaa) to kompleksowa propozycją systemu oceniania zgodności stron internetowych z wymogami dostępności zdefiniowanymi w WCAG 2.0. 

Początki metodyce RGAA dało francuskie stowarzyszenie [BraileNet](https://www.braillenet.org/), które już w 2003 roku opracowało i opublikowałło pod nazwą [AccessiWeb](https://www.braillenet.org/accessibilite-numerique/cadre-technique/), aby zapewnić ujednolicone podejście do kontroli zgodności usług sieciowych dla WCAG. Ta metoda została szeroko rozpowszechniona zastosowana we Francji oraz w świecie francuskojęzycznym.

W 2009 roku francuska administracja rządowa opublikowała pierwszą wersję „ogólnych wytycznych dostępności dla administracji” („Référentiel Général d'Accessibilité des Administrations”, w skrócie RGAA). Wytyczne były adaptacją WCAG 2.0 na potrzeby administracji francuskiej, wzbogaconą o szczegółowe instrukcje oceniania zgodności. W wytycznych wykorzystano dorobek stowarzyszenia BraileNet.

W 2014 roku stowarzyszenie BraileNet z grupą firm wygrało przetarg na aktualizację RGAA, w wyniku którego zostało wykonawca tego rządowego zamówienia. 29 kwietnia 2015 roku udostępniono wersję 3.0 RGAA, kktóra w dużej mierze korzysta z repozytorium AccessiWeb HTML5/ARIA.   

W swej istocie RGAA to nie są tylko „ogólne wytyczne”, jak można by wnosić z nazwy. Jest to bogaty zasób cyfrowy, dostarczający precyzyjnych sposobów badania i oceniania dostępności stron internetowych.

Całe repozytorium składa się z 6 sekcji:

1. Kryteria i testy - uporządkowane w 13 kategorii - tematów,
2. Słownik - definiujący i ujednoznaczniający stosowane terminy,
3. Przypadki szczególne - prezentacja odstępstw od wymogów zdefiniowanych w kryteriach,
4. Uwagi techniczne - wyjaśnienia dotyczące obsługi niektórych elementów HTML5,
5. Baza referencyjna - kombinacje technologii, systemów operacyjnych i przeglądarek, które pozwalają stwierdzić, że oprogramowanie oparte na HTML5/ARIA „wspiera dostępność”, jak zdefiniowano w WCAG 2.0.
6. Referencje - lista wykorzystanych źródeł i referencji

#### Polskie tłumaczenie RGAA 

W 2018 roku tłumaczenie RGAA wykonane przez pracowników Ministerstwa Cyfryzacji udostępniono na stronie [Dostępność cyfrowa](https://www.gov.pl/web/dostepnosc-cyfrowa/francuska-metodyka-badania-dostepnosci-rgaa). Dzięki temu polskie zasoby poświęcone dostępności cyfrowej wzbogaciły się o niezwykle cenne i jedyne w takim wymiarze źródło metodyki oceniania dostępności.

Specyfikacja RGAA zawiera ogółem blisko 280 testów dla 133 kryteriów uporządkowanych w 13 kategorii. RGAA stosuje wprawdzie własne kryteria sukcesu, ale każde z nich jest zmapowane z odpowiednimi kryetriami sukcesu oraz technikami WCAG, cco powoduje, że RGAA jest **w pełni zgodne** z WCAG. Nie znaczy to - oczywiscie - że odwrotne stwierdzenie jest prawdziwe. WCAG nie są w pełni zgodne z RGAA.

Na podstawie tłumaczenia udostępnionego przez Ministerstwo Cyfryzacji Pracownia Dostępności Cyfrowej LepszyWeb.pl przygotowała i opublikowała [internetową wersję RGAA](https://rgaa.lepszyweb.pl) systematycznie poprawianą.
   








