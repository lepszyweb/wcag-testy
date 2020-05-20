---
title: Automatyczne testy dostępności
Summary: "Czym są testy automatyczne? Zalety testów automatycznych. Ograniczenia testów automatycznych. "

sidebar: metoda_sidebar
permalink: met_testy-automatyczne
folder: metoda
---

## Co to są testy automatyczne

Automatyczne testowanie dostępności polega na używaniu serii skryptów, które badają obecność lub brak określonych warunków w kodzie. Skrypty mogą być uruchamiane za pomocą aplikacji komputerowej lub internetowej albo usługi internetowa, dodatku do przeglądarki, wtyczki w zintegrowanym środowisku programistycznym (IDE).  

Nowoczesne strony i aplikacje internetowe to często bardzo skomplikowane tworzy, zudowane z tysięcy linii kodu, przyjmujące setki różnych stanów, umożliwiajace skomplikowane interakcje. Byłoby absurdem oczekiwać, że człowiek lub zespół ludzi jest w stanie skontrolować wszystkie możliwe usterki, braki, operacje na stronie czy w aplikacji, wszystkie   

Nowoczesne strony internetowe i aplikacje internetowe to skomplikowane rzeczy, które obejmują setki stanów, tysiące linii kodu i skomplikowane interakcje na wielu ekranach. Byłoby absurdem oczekiwać człowiekiem (lub zespół ludzi) na myśl cały kod kontrolowania wszelkich możliwych permutacji w miejscu, nie mówiąc już o takich rzeczach regresji , oprogramowania zgniliznę i A / B testów .
Automatyzacja naprawdę świeci tutaj. Może wielokrotnie i niestrudzenie wylewać te szczegóły z doskonałą pamięcią, w tempie znacznie szybszym niż jakikolwiek człowiek.




Automatyczne testowanie dostępności to proces, w którym używasz serii skryptów do testowania obecności lub braku określonych warunków w kodzie. Warunki te są podyktowane Wytycznymi dotyczącymi dostępności treści internetowych (WCAG) , standardem W3C, który określa, w jaki sposób udostępnić wrażenia cyfrowe.Przejdź do spisu treści ↬


Automatyczne testowanie dostępności polega na użyciu aplikacji komputerowej lub internetowej albo usługi internetowej, wtyczki do przeglądarki lub wtyczki IDE, która może uzyskać dostęp do źródła testowanej strony internetowej. Źródło jest następnie oceniane na podstawie wbudowanych przez producenta narzędzia testów heurystycznych  w celu ustalenia, czy istnieją jakieś błędy.



Co mogę znaleźć? Zautomatyzowane testowanie umożliwia ostateczne przetestowanie około 25% najlepszych praktyk dotyczących dostępności. Kolejne około 35% może być sprawdzone przez testowanie maszynowe, ale wyniki wymagają weryfikacji przez człowieka. Wiele z automatycznie Wiele z automatycznie wykrywanych problemów ma duży wpływ na dostępność
Czego będzie mi brakowało? W przybliżeniu 40% najlepszych praktyk dotyczących dostępności nie można w ogóle przetestować za pomocą narzędzia do automatycznego testowania, ponieważ są one albo zbyt subiektywne, albo zbyt skomplikowane, aby testować je automatycznie.
Ile to kosztuje? Tyle, ile narzędzie i czas testera na jego użycie i wykrycie problemów oraz ich segregację.
Mimo że duża liczba najlepszych praktyk w zakresie dostępności nie może być automatycznie przetestowana, faktem jest, że w ujęciu ilościowym można automatycznie znaleźć dużą liczbę błędów dostępności.
Z moich danych wynika, że średnio na witrynach organizacji rozpoczynającej pracę nad dostępnością występuje około 40 błędów na stronie, które można wykryć za pomocą testów automatycznych. Jeśli narzędzie, którego używasz, ma możliwość mapowania strony i przekazywania znalezisk za pomocą odniesień do kodu, automatyczne testowanie będzie zdecydowanie najbardziej wydajnym sposobem gromadzenia danych dotyczących dostępności.


Zalety i ograniczenia automatycznego testowania
Zautomatyzowane testowanie zasobów sieciowych pod kątem standardów dostępności i najlepszych praktyk jest kluczowe dla większości procesów opracowywania, testowania i monitorowania. Zautomatyzowane testowanie samo w sobie nie jest jednak kompletnym rozwiązaniem (w dającej się przewidzieć przyszłości). Podczas gdy dalsze ręczne testowanie ma kluczowe znaczenie dla potwierdzenia dostępności i włączenia produktu lub witryny, testy automatyczne pozostają tylko jednym z elementów większego wysiłku w zakresie aktywnych działań, które organizacje muszą podjąć, aby dostosować się do przepisów i zapewnić dostęp osobom niepełnosprawnym.


Chociaż automatyczne testowanie jest ważne, aby rozwiązać szybko wykrywalne problemy, należy uważać na wprowadzające w błąd twierdzenia dotyczące automatycznych rozwiązań testowych: nawet jeśli narzędzie może znaleźć połowę problemów z systemem, nie oznacza to, że połowa pracy została ukończona. Ograniczanie inicjatyw do zautomatyzowanych narzędzi nie „rozwiązuje” dostępności sieci. Chociaż zautomatyzowane narzędzia (w tym skanery, rozszerzenia przeglądarki, poprawki nakładek itp.) Są ważną częścią szerszego rozwiązania, nie mogą same zagwarantować dostępności, ani nie identyfikują wszystkich potencjalnych barier. Na przykład zautomatyzowane narzędzie może potwierdzić, że obraz ma alternatywny tekst - ale na razie nie jest w stanie samodzielnie stwierdzić, czy ten tekst ma znaczenie w kontekście.

Dlatego te zautomatyzowane rozwiązania, jeśli są stosowane poza bardziej kompleksową metodologią, narażają Twoją organizację na poważne ryzyko prawne. W Level Access automatyzacja odgrywa kluczową rolę w natychmiastowym wykrywaniu typowych i powszechnie zauważalnych problemów, jednocześnie ujawniając potencjalne problemy w bardziej złożonych obszarach, pozwalając zespołom zaoszczędzić cenny czas i lepiej skupić się na bardziej intensywnych, ręcznych kontrolach.

Level Access uważa również, że zautomatyzowane testowanie dostępności powinno zostać włączone do cyklu życia oprogramowania, aby wykryć i wyeliminować problemy w jak najwcześniejszym momencie. Skuteczne łączenie różnych rodzajów testów dostępności może zapewnić natychmiastową i ukierunkowaną informację zwrotną na temat wybranych problemów, a jednocześnie lepiej informować wysiłki na rzecz ogólnie bardziej wydajnego podejścia. Zautomatyzowane testowanie może pomóc użytkownikom w mądrzejszym testowaniu - w jaki sposób i co testują - zapewniając wystarczającą ilość informacji, aby podejmować bardziej inteligentne decyzje, a jednocześnie zwiększać wydajność w celu usprawnienia podróży do dostępnych treści.

Pierwsze kroki
Level Access udostępnia kilka bezpłatnych aplikacji Access Engine (naszej biblioteki testowej opartej na JavaScript) na stronie www.WebAccessibility.com . Te edycje społecznościowe naszych produktów zawierają rozszerzenia dla Firefoksa i Chrome, które umożliwiają szybką ocenę stron bezpośrednio z przeglądarki, a także kilka zestawów SDK dla Java i JavaScript przeznaczonych dla organizacji praktykujących CI w ich rozwoju. Zasoby te są doskonałym sposobem na rozpoczęcie pracy, a ich użycie do generowania natychmiastowych wyników może wprowadzić Twój zespół do ważnych koncepcji dostępności, umożliwiając jednocześnie identyfikację i naprawienie niektórych typowych przeszkód.


Automatyczne testowanie dostępności to proces, w którym używasz serii skryptów do testowania obecności lub braku określonych warunków w kodzie. Warunki te są podyktowane Wytycznymi dotyczącymi dostępności treści internetowych (WCAG) , standardem W3C, który określa, w jaki sposób udostępnić wrażenia cyfrowe.

Awarie mogą być następnie gromadzone i wykorzystywane do generowania raportów, które ujawniają liczbę i wagę problemów z dostępnością. Niektóre produkty zautomatyzowanej dostępności można również zintegrować jako narzędzie do ciągłej integracji lub ciągłego wdrażania (CI / CD), prezentując ostrzeżenia programistom w momencie, gdy próbują dodać kod do centralnego repozytorium.

Te zautomatyzowane programy to niesamowite zasoby. Nowoczesne strony internetowe i aplikacje internetowe to skomplikowane rzeczy, które obejmują setki stanów, tysiące linii kodu i skomplikowane interakcje na wielu ekranach. Byłoby absurdem oczekiwać człowiekiem (lub zespół ludzi) na myśl cały kod kontrolowania wszelkich możliwych permutacji w miejscu, nie mówiąc już o takich rzeczach regresji , oprogramowania zgniliznę i A / B testów .

Automatyzacja naprawdę świeci tutaj. Może wielokrotnie i niestrudzenie wylewać te szczegóły z doskonałą pamięcią, w tempie znacznie szybszym niż jakikolwiek człowiek.







Testy użyteczności to technika stosowana w projektowaniu interakcji zorientowanym na użytkownika w celu oceny produktu poprzez przetestowanie go na użytkownikach. Tradycyjnie wykonywane testy są metodą analizy poznawczej (Cognitive walkthrough) z wykorzystaniem  protokołu głośnego myślenia, chociaż istnieją również inne metody. W przypadku testów użyteczności pod kątem dostępności testy polegają na wykorzystaniu jako uczestników testu osób z niepełnosprawnościami .


Karl Groves
wszelkie testy dostępności, niezależnie od metodologii, muszą być ukierunkowane na jeden główny cel: zebranie danych niezbędnych do zrozumienia, co należy naprawić, aby ulepszyć system

