---
title: UWEM 1.2
summary: "UEWM jest pierwszą kompleksową metodologią badania dostępności cyfrowej stron internetowych opracowaną w ramach trzech europejskich projektów badawczych 6.&nbsp;Ramowego programu badań w&nbsp;zakresie technologii społeczeństwa informacyjnego. Odnosi się do WCAG 1.0."

sidebar: metoda_sidebar
permalink: met-uwem
folder: metoda
---

## Jednolita metodologia oceniania dostepności

UWEM jest skrótem tytułu <span lang="en">Unified Web Evaluation Methodology</span>, co można przetłumaczyć na język polski jako „jednolita metodologia oceny dostępności internetowej”.   

Metodologia powstała w wyniku prac prowadzonych w ramach trzech europejskich projektów badawczych 6.&nbsp;Ramowego programu badań w&nbsp;zakresie technologii społeczeństwa informacyjnego (Sixth Framework Programme Information Society Technologies) zgrupowanych w&nbsp;ramach klastra Web Accessibility Benchmarking (wzorcowe testy dostępności Sieci).

Celem projektów było wypracowanie metodologii, która byłaby podstawą oceny i certyfikacji dostępności Sieci w&nbsp;Europie.

Pierwsza wersja została opublikowana w listopadzie 2006 roku.

Dyskusje i dalsze prace nad UWEM 1.0 doprowadziły do opublikowania we wrześniu 2007 roku finalnej wersji [Unified Web Evaluation Methodology (UWEM) 1.2](http://www.wabcluster.org/uwem1_2/).

UWEM jest metodologią oceny zgodności stron internetowych z [WCAG 1.0](https://www.w3.org/TR/WAI-WEBCONTENT/) opublikowanymi przez World Wide Web Consortium (W3C) w&nbsp;1999 roku.

Metodologia UWEM obejmowała:
- określenie podstawowych założeń,
- opis procedur oceniania,
- zalecenia dotyczące zakresu oceny i pobierania próbek zasobów do oceny,
- testy dla punktów kontrolnych WCAG 1.0 na poziomie priorytetu 1 i 2,
- zalecenia dotyczące raportowania wyników oceny,
- szablony i definicje danych.
- słownik terminów.

## Definicja metodologii
UWEM definiuje metodologię oceniania dostępności jako _system zasad i praktyk dla ekspertów i&nbsp;automatycznej oceny dostępności stron internetowych przez ludzi i interfejsy maszyn_.

## Założenia metodologii
UWEM została zaprojektowana tak, aby była zgodna z priorytetami 1 i&nbsp;2 punktów kontrolnych WCAG 1.0 w&nbsp;odniesieniu do kryteriów technicznych. Celem UWEM było _zwiększenie wartości ocen poprzez oparcie ich na wspólnej interpretacji WCAG 1.0 i&nbsp;zestawie testów, które są wystarczająco solidne, aby dać zainteresowanym stronom zaufanie do wyników_.

UWEM została opracowana w taki sposób, aby spełniała następujące wymagania:
- zgodność techniczna z istniejącymi dokumentami Web Accessibility Initiative (WAI),
- niezależność narzędzi i przeglądarek.
- jednoznaczność (unikalna interpretacja): opisy powinny być interpretowane tylko w&nbsp;jeden sposób
- replikacyjność: te same testy na tej samej stronie wykonane przez różnych oceniających powinny przynosić te same wyniki.
- zgodność z rozporządzeniem (WE) nr 808/2004 Parlamentu Europejskiego i&nbsp;Rady dotyczącym statystyk Wspólnoty w sprawie społeczeństwa informacyjnego.

## Proces oceny
UWEM zdefiniowała trzy główne scenariusze zastosowania, zależne od celów oceny:
- zastosowanie w celu potwierdzenia zgodności z WCAG,
- zastosowanie w celu oceny, jak strona lub witryna spełnia wymagania WCAG (ale nie w&nbsp;celu stwierdzenia zgodności),
- zastosowanie w celu monitorowania dostępności dużej liczby stron internetowych.

## Procedury
UWEM wskazuje na trzy zasadnicze procedury testowania dostepności:
- testowanie automatyczne,
- badanie eksperckie,
- testy użyteczności z udziałem użytkowników z niepełnosprawnościami.   

Każda z tych procedur ma swoje mocne i słabe strony. Żadna nie jest kompletna i wyczerpująca.

Najlepszym sposobem zapewnienia rzetelnej i warygodnej oceny dostępności i&nbsp;zgodności z&nbsp;normami jest zastosowanie podejścia łączonego, obejmującego wszystkie metody oceny: ocenę automatyczną, ocenę ekspercką i testowanie z udziałem użytkowników z niepełnosprawnościami.


## Zakres i pobieranie próbek zasobów
W metodologii UWEM stwierdzenia dotyczące zgodności i inne raporty oceniające muszą odnosić się do listy zasobów ocenianych w&nbsp;ramach strony internetowej (stron internetowych).

## Procedura wyznaczania zakresu ocenianych zasobów
Dla celów UWEM witrynę internetową definiuje się jako dowolny zbiór połączonych hiperłaczami zasobów internetowych, z których każdy jest określany zgodnie z procedurą opisaną w sekcji definiującej.  

Celem UWEM jest wspieranie powtarzalności wyników. Z tego powodu jednoznaczna identyfikacja ocenianych zasobów ma zasadnicze znaczenie dla agregacji i porównywania wyników. Stwierdzenia ogólne, takie jak: "http://przyklad.org/ jest zgodna z normą UWEM 1.2 Poziom 1" są nie do przyjęcia w oświadczeniach o zgodności z normą UWEM 1.2. Takie oświadczenie sugerowałoby, że zestaw zasobów został przeszukany do końca zgodnie z pewnymi wcześniej ustalonymi limitami lub ograniczeniami. Biorąc jednak pod uwagę szeroką gamę istniejących skanerów i różne stosowane przez nie technologie, nie można zweryfikować wiarygodności tych stwierdzeń. Ponadto różne RFC związane z nazwami domen pozostawiają otwarte pole do interpretacji w odniesieniu do koncepcji poddomeny i jej rozdzielczości.

Dlatego w przypadku deklaracji zgodności UWEM 1.2 zakres witryny MUSI być wyrażony w formie listy zasobów.

### Procedury wyboru próbek do oceny
Testowanie wszystkich zasobow witryny pod kątem wszystkich kryteriów oceny nie jest praktyczne. W zwiazku z tym, po ustaleniu listy zasobów do oceny oraz celów oceny, można wybrać podzbiór lub „próbkę” zasobów do oceny.    

UWEM określa dwie procedury generowania probek do oceny:
- **próbka losowa**, wygenerowana automatycznie przez narzędzie; jeżeli ocena musi być powtarzalna i umożliwiać porównania synchroniczne lub asynchroniczne (np. monitorowanie), próbka do oceny musi być wygenerowana w drodze jednolitej procedury losowej.
- **próbka nielosowa**, wybierana przez eksperta, jeśli powtarzalność wyników nie jest kluczowa.


#### Pobieranie próbek nielosowych: Lista zasobów podstawowych

Lista zasobów podstawowych (ang. <span lang="en">Core Resource List</span>) stanowi zbiór zasobow kluczowych dla oceny użyteczności i dostepnpości strony. Lista zasobow podstawowych stanowi zatem zbiór zasobów, które powinny być objęte każdą oceną dostępności witryny dokonywaną przez ekspertów. Lista zasobów podstawowych nie może, ogólnie rzecz biorąc, być określona automatycznie, ale wymaga wyboru zasobów na podstawie osądu ludzkiego.Lista zasobów podstawowych powinna składać się z jak największej liczby następujących zasobów, które mają zastosowanie:

- Zasób „Strona główna”.
- Zasób „Informacje kontaktowe” (jeśli istnieje).
- Zasób „Pomoc” (jeśli istnieje).
- Zasób „Mapa witryny” (jeśli istnieje).
- Zasoby składające się na usługę „podstawowe przeszukiwanie stron” (jeśli istnieje). Obejmuje to co najmniej jeden zasób, w którym można rozpocząć wyszukiwanie i co najmniej jeden zasób pokazujący wyniki przykładowego wyszukiwania.
- Zasoby opisujące funkcje dostępności i/lub politykę dostępności strony (jeśli istnieją).
- Przykłady zasobów reprezentatywnych dla głównych zastosowań witryny (jeśli są możliwe do określenia).
- Jeżeli witryna świadczy usługi, w których użytkownik systematycznie przechodzi przez sekwencję zasobów (np. wielostronicowy formularz lub transakcję), wówczas należy uwzględnić reprezentatywne zasoby dostępne na każdym etapie każdego z takich kluczowych scenariuszy (w stosownych przypadkach i tylko w zakresie).
- Zasoby reprezentatywne dla każdej kategorii zasobów o zasadniczo odmiennym „wyglądzie i stylu” ([Look and feel](https://en.wikipedia.org/wiki/Look_and_feel)) (zazwyczaj reprezentujące odrębne „szablony” witryny) (jeśli można je zidentyfikować).
- Zasoby reprezentatywne dla każdej z następujących odrębnych technologii internetowych (jeśli są wykorzystywane):
  - formularze,
  - ramki,
  - tabele danych,
  - skrypty po stronie klienta,
  - kaskadowe arkusze stylów,
  - aplety, wtyczki, multimedia itp.

Jeśli próbka ewaluacyjna jest tworzona ręcznie, musi zawierać listę zasobów podstawowych.

Jeśli lista zasobów podstawowych zawiera mniej stron niż wymagana wielkość próbki, należy dodać dodatkowe zasoby z następujących kategorii:

- Zasoby reprezentatywne dla głównych zamierzonych zastosowań witryny (jeśli są możliwe do określenia).
- Jeżeli witryna świadczy usługi, w których użytkownik systematycznie przechodzi przez sekwencję zasobów (np. wielostronicowy formularz lub transakcję), wówczas należy uwzględnić reprezentatywne zasoby dostępne na każdym etapie każdego z takich kluczowych scenariuszy (w stosownych przypadkach i tylko w zakresie).
- Zasoby reprezentatywne dla każdej kategorii zasobów o zasadniczo odmiennym „wyglądzie i stylu” ([Look and feel](https://en.wikipedia.org/wiki/Look_and_feel)) (zazwyczaj reprezentujące odrębne „szablony” witryny) (jeśli można je zidentyfikować).
- Zasoby reprezentatywne dla każdej z następujących odrębnych technologii internetowych (jeśli są wykorzystywane):
  - formularze,
  - ramki,
  - tabele danych,
  - skrypty po stronie klienta,
  - kaskadowe arkusze stylów,
  - aplety, wtyczki, multimedia itp.
Jeśli próbka ewaluacyjna jest tworzona ręcznie, musi zawierać listę zasobów podstawowych.

Oczywiście, każdy pojedynczy zasób może należeć do więcej niż jednej z powyższych kategorii: wymogiem jest po prostu to, że lista zasobów podstawowych jako całość powinna, w miarę możliwości, wspólnie zająć się wszystkimi stosownymi celami próbkowania.

Każdy konkretny zasób powinien pojawić się tylko raz w próbie ewaluacyjnej.


#### Losowe pobieranie próbek

W przypadku ocen ukierunkowanych na porównywalność wyników, np. monitorowania oraz porównań synchronicznych lub asynchronicznych, należy zastosować próbę losową. Należy pamiętać, że w pełni losowa próbka nie może zostać wygenerowana bez narzędzia.

Aby wygenerować reprezentatywną i bezstronną próbkę ewaluacyjną, wymagany jest jednolity losowy wybór z zestawu wszystkich zasobów należących do strony internetowej.

Istnieją różne sposoby określenia listy wszystkich zasobów należących do strony internetowej. W niektórych przypadkach lista zasobów jest znana wcześniej, np. dlatego, że jest dostarczana przez właściciela strony zlecającego ocenę. Jeśli lista zasobów jest nieznana, witryna musi zostać zbadana przed dokonaniem oceny. Zazwyczaj wykorzystywany jest do tego celu [robot internetowy](https://pl.wikipedia.org/wiki/Robot_internetowy), automatycznie przeglądający witrynę za pomocą linków. Indeksowanie rozpoczyna się od jednego lub więcej „zasobów początkowych”, np. strony głównej.

Jeśli strona internetowa jest bardzo duża lub jeśli duża liczba stron internetowych została uwzględniona w monitoringu, określenie pełnej listy zasobów należących do danej strony internetowej może być niewykonalne. W takim przypadku oceniający może zdecydować o przerwaniu procesu indeksowania, gdy zostanie zidentyfikowana wystarczająco duża liczba zasobów.

Próbkę do oceny wybiera się z listy zasobów należących do strony internetowej, stosując jednolite losowe próbkowanie  bez zastępowania.

Należy pamiętać, że zarówno zastosowany algorytm indeksowania, jak i próbkowania oraz wszelkie dalsze ograniczenia ograniczające lub zniekształcające wynik, w tym między innymi poniższe ograniczenia, powinny zostać wyraźnie ujawnione w każdym raporcie z oceny:
- ograniczenie do stron bez formularzy interakcyjnych,
- ograniczenie według rodzaju treści (np. bez JavaScript / Flash / PDF),
- ograniczenie przez głębokość połączeń z dowolnego zasobu źródłowego,
- ograniczenie przez protokół robots.txt,
- ograniczenie konkretnych wykorzystanych zasobów początkowych,
- ograniczenie całkowitej liczby zasobów na liście zasobów.

## Wielkość próbek do oceny
W przypadku oceny eksperckiej minimalna liczba zasobów w próbie zależy od szacowanej wielkości strony internetowej. Minimalna wielkość próby składa się z 30 unikalnych zasobów (jeśli są dostępne), dodając 2 unikalne zasoby na 1000 dostępnych zasobów do maksymalnie 50 zasobów w próbie oceniającej.

Jeżeli wyniki oceny mają być przedstawione w formie raportu karty wyników, można zastosować **adaptacyjną strategię doboru próby**, która kończy się po osiągnięciu wymaganej dokładności.

Zaczynając od minimalnej liczebności próby 30 zasobów, należy kontynuować dobór próby aż do momentu, gdy średni wynik strony internetowej znajdzie się w granicach danego marginesu błędu m dla danego poziomu zaufania (wiarygodności). Należy zwrócić uwagę, że UWEM wymaga ujawnienia marginesu błędu i przedziału wiarygodności próby.

## Raportowanie wyników oceny

Wynik oceny dostępności w ramach UWEM można przedstawić na wiele sposobów, w zależności od rodzaju ewaluacji i potrzeb organizacji zlecających i/lub przeprowadzających ewaluację.

W przypadku ocen dostępności stron internetowych przeprowadzanych przez eksperta istnieją trzy opcje raportowania.

Jeśli wynik testu jest pozytywny, tzn. wszystkie istotne testy przeszły pozytywnie, można go przedstawić jako oświadczenie o zgodności na wybranym poziomie. Aby zapewnić więcej szczegółów oceny dostępności, ekspert wybiera pomiędzy raportem opartym na szablonie tekstowym a raportem nadającym się do odczytu maszynowego w formacie EARL.

W celu zautomatyzowanego monitorowania sytuacji dostępności dużej liczby stron internetowych , wyniki mogą być przedstawione w formie raportu w postaci karty wyników. Ten rodzaj raportu oferuje wysoki poziom agregacji. Dla każdej strony internetowej obliczana jest jedna liczba - wynik UWEM - aby umożliwić porównanie z innymi stronami internetowymi oraz z poprzednimi wersjami tej samej strony. Poza raportem przeglądowym w karcie wyników wyniki automatycznej oceny dostępności mogą być również prezentowane w szczegółowym raporcie odczytywanym maszynowo w formacie EARL.

Należy pamiętać, że wszystkie trzy rodzaje raportów przeznaczonych dla pojedynczych stron internetowych (deklaracja zgodności, raport tekstowy, raport do odczytu maszynowego) wymagają podania listy zasobów objętych próbą w formacie RDF. Jeżeli próbka do oceny jest generowana przez narzędzie, łatwo jest utworzyć listę RDF. Raport karty wyników nie wymaga szczegółowego wykazu zasobów objętych próbą.
