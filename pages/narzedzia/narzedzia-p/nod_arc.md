---
title: ARC Toolkit
tags: [rozszerzenia_przeglądarek,narzędzia_oceny_dostępności]

sidebar: narzedzia-sidebar
permalink: nod_arc
folder: narzedzia-p
---

## ARC Toolkit - wyśmienity pomocnik testera dostępności

W ramach Światowego Dnia Świadomości Dostępności 2019 programiści z Pacciello Group - firma Vispero udostępnili wyśmienite, a przy tym bezpłatne narzędzie do testowania dostępności – ARC Toolkit.
ARC Toolkit jest rozszerzeniem dla przeglądarki Chrome. Szybko i skutecznie testuje pojedyncze strony pod kątem dostępności i wskazuje niezgodności z kryteriami sukcesu na poziomie A i AA wytycznych WCAG 2.1 bądź sytuacje, które wymagają dodatkowej weryfikacji przez człowieka.
Narzędzie można polecić:
-	twórcom stron i programistom do wykorzystania w procesie projektowania stron,
-	testerom i audytorom dostępności, dla których będzie ogromną pomocą w badaniu wyselekcjonowanej do oceny próbki typowych i kluczowych stron serwisu,
-	wszystkim, których zadaniem jest dbałość o dostępność stron internetowych – wydawcom,  administratorom, redaktorom, autorom, koordynatorom ds. dostępności.   

### Instalacja
ARC Toolkit instalujemy jak każde inne rozszerzenie przeglądarki Chrome.
1.	[Przejdź na stronę sklepu Chrome](https://chrome.google.com/webstore/detail/arc-toolkit/chdkkkccnlfncngelccgbgfmjebmkmce).
2.	Wybierz przycisk **Dodaj do Chrome**.

![Opcja Dodaj do Chrome w sklepie Chrome](/images/arc_toolkit_dodaj-do-chrome.png)

3.	Po zainstalowaniu, otwórz w Chrome menu Ustawienia i wybierz opcję **Więcej narzędzi > Narzędzia dla deweloperów** albo użyj klawiszy F12 lub kombinacji Ctrl+Shift+ I w Windows, a w Mac – Option + CMD + I. Możesz również wskazać myszką dowolny element na badanej  stronie i wybrać z menu kontekstowego polecenie **Zbadaj element**.
4.	Na pasku narzędzi programisty wybierz ARC Toolkit.

![Opcja ARC Toolkit na pasku narzędzi dewelopera](/images/arc-toolkit_na-pasku-dewelopera.png)

*Uwaga*: Po zainstalowaniu w Chrome ARC Toolkit jest włączony z domyślnymi ustawieniami. Nie wymaga dodatkowych czynności konfiguracyjnych. Jeśli będziesz zmieniać ustawienia domyślne, w grupie opcji Dostęp do stron pozostaw włączoną opcję **We wszystkich witrynach**.  
*Uwaga 2*: Możesz zmieniać miejsce, w którym osadzone są Narzędzia programisty. Jeśli dysponujesz dwoma ekranami, to najlepszym wyborem będzie wyświetlenie narzędzi programisty w odrębnym oknie.

### Testowanie strony
Aby rozpocząć testowanie strony internetowej, naciśnij na pasku przycisk _Run Tests_ (Uruchom testy).

![Opcja Urudhom testy](/images/arc_toolkit-uruchom-test.png)

Po chwili otrzymamy wyniki. Przyjrzyjmy się bliżej funkcjom oferowanym przez ARC Toolkit.
Narzędzie składa się z dwóch obszarów: paska bocznego i głównego okna. Pasek boczny zawiera tabelę ze statystyką wyników.
Oceniane reguły silnika ARC są zorganizowane w kategorie i podkategorie:
-	**Media**: Obrazy (*Images*), Obrazy tła (*BG Images*), Bogate media (*Rich Media*);
-	**Struktura** (*Structure*): Nagłówki (*Headings*), Punkty orientacyjne (*Landmarks*), Listy (*Lists)*, Akapity (*Paragraph*), Treśc generowana (*Pseudo Content*), Tabele (*Tables*), Formularze (*Forms)*, Ramki (*Frames*), Tytuły (*Title*), Wyróżnianie tekstu (*Text Formating*), Języki (*Languages*);
-	**Klawiatura** (Keyboard): Łącza (*Links*), Łącza wewnętrzne (*Internal Links*), Przyciski (*Buttons*), Klawisze dostępu (*Access Key*), Indeks tabulacji (*Tabindex*), Porządek tabulacji (*Tab Order*);
-	**ARIA**: ARIA w komponentach interfejsu użytkownika (*ARIA UI*), ARIA zawartości modyfikowanej dynamicznie (*ARIA Live*), Stosowanie ARIA (*ARIA Usage*), ARIA ukrywająca elementy (*ARIA Hidden*);
-	**Kolor** (*Color*): Kontrast koloru (*Color Contrast*)
-	**Identyfikatory** (*IDs*).
Nazwy kategorii i podkategorii są nagłówkami wierszy tabeli, prezentującej wyniki w sześciu kolumnach.
Kolumny w tabeli wyników pokazują liczbę widocznych i niewidocznych wystąpień, w tym błędów i ostrzeżeń. Nagłówkami kolumn są ikony symbolizujące kolejno:

![Nagłówki kolumn w tabeli w pasku bocznym](/images/arc-toolkit-nglowki-kolumn.png)

1.	Widoczne wystąpienia (*Visible Instance*)
2.	Błędy widoczne (*Visible Errors*)
3.	Ostrzeżenia widoczne (*Visible Warnings*)
4.	Ukryte wystąpienia (*Hidden Instances*)
5.	Ukryte błędy (*Hidden Errors*)
6.	Ukryte ostrzeżenia (*Hidden Warnings*)
Elementy ukryte to elementy niewidoczne w przeglądarkach, ale istniejące w kodzie strony, widoczne m.in. dla technologii wspomagających.  Ostrzeżenia dotyczą sytuacji, które mogą być problemami, ale wymaga to oceny człowieka.
Po wykonaniu testów w oknie głównym wyświetlana jest tabela wyników prezentowanych w czterech kolumnach. W pierwszej znajdziemy systemowy opis testu (reguły ARC), w drugiej liczbę błędów, w trzeciej liczbę ostrzeżeń, a w czwartej nazwę kategorii błędu lub ostrzeżenia.  

![Interejs ARC Toolkit. Pasek boczny i główne okno](/images/arc-toolkit-okno.png)

Wybranie podkategorii na pasku bocznym ograniczy wyniki w głównym oknie do problemów określonego typu, takich jak związane z obrazami lub nagłówkami, przy czym domyślnie uwzględnione są tylko elementy widoczne w przeglądarkach. Aby wyświetlić także informacje o elementach ukrytych, należy zaznaczyć w pasku menu w oknie głównym opcję: Ukryte (*Hidden*). Pozostałe trzy opcje ograniczają wyświetlanie wyników do błędów (*Errors*), ostrzeżeń (Warnings) i aktualnie wybranego węzła (*Limit to Selected Node*).

### Definicje wyników
Szczegółowe wyniki testów sklasyfikowane są jako:

![Oznaczenia wyników](/images/arc_klasyfikacja.png)

-	**Zaliczone** – wyniki testów, w przypadku których nie stwierdzono żadnych problemów z dostępnością.
-	**Błędy** – wyniki, w przypadku których stwierdzono problemy z dostępnością.
-	**Ostrzeżenia** - potencjalne problemy, które wymagają ręcznej weryfikacji.
-	**Ukryte** – wyniki, które nie są widoczne w przeglądarce, ale mogą mieć wpływ na użytkowników technologii wspomagających.

### Analiza wyników
Aby przeanalizować wyniki, w tabeli w pasku bocznym wybierz podkategorię (np. Images).
Wszystkie wykryte wystąpienia zostaną oznaczone na stronie czerwoną przerywaną linią i znacznikiem IMG.
W oknie głównym ARC zostaną wyświetlone szczegółowe wyniki. Każde z wystąpień opatrzone jest numerem porządkowym i ikoną (OK, WARN, ERR, HIDDEN). Obok znajdują się objaśnienia i ewentualne wskazówki. Dodatkowo wyświetlana jest także miniatura obrazu. W przypadku obrazów podawany jest kod osadzający obrazek oraz obok treść tekstu alternatywnego, jeśli istnieje, bądź wartość NIL (pusty), jeśli istnieje atrybut alt.
Gdy ARC wykryje błąd lub możliwy błąd (ERR bądź WARN), w informacji o wystąpieniu znajduje się zwięzły opis problemu i zalecone działanie.

![Wyniki szczegółowe](/images/arc-toolkit-szczegolowe.png)

Informacje te wyświetlane są w języku angielskim. W razie potrzeby można je skopiować i przetłumaczyć za pomocą translatora internetowego (Google, Deepl i inne).

### Lokalizacja problemów w kodzie strony
Dzięki integracji z narzędziami programisty ARC umożliwia łatwą lokalizację każdego  błędu w kontekście wynikowego kodu strony .
Aby zobaczyć problematyczny kod w kontekście źródłowego kodu strony, kliknij w głównym panelu w wynikach testu cytowany fragment kodu.
ARC przeniesie cię na kartę Elementy w oknie narzędzi programisty. Wskazany fragment kodu będzie wyróżniony i wyświetlony w kontekście.
 

### Inne właściwości
ARC Toolkit posiada ponadto kilka innych cennych funkcji, które wspomagają proces ręcznego testowania dostępności.

#### Porządek tabulacji
Gdy wybierzesz w bocznym pasku tę podkategorię, ARC Toolkit natychmiast wyświetli na stronie graficzną reprezentację porządku tabulacji. Wszystkie punkty interaktywne zostaną wyróżnione czerwonymi kółeczkami i ponumerowane liczbami wskazującymi kolejność tabulacji oraz połączone odcinkami. Wśród narzędzi oferujących tę funkcję ARC jest niewątpliwym liderem.

![Graficzna reprezentacja porządku tabulacji](/images/arc-toolkit-tab-order.png)

#### Wzmocnienie fokusa
Zaznacz opcję **Show and Track Focus** (Pokaż i śledź skupienie) i wybierz w pasku bocznym podkategorię Tabindex (Indeks tabulatora). Następnie użyj klawisza Tab, by nawigować po stronie. Elementy, które uzyskują skupienie, zostaną wyróżnione wzmocnionym czerwonym obramowaniem. Jest to szczególnie pomocne narzędzie,  gdy projektant strony zmodyfikuje style tak, że fokus będzie niewidoczny lub nawet ukryty przed użytkownikiem.
#### Przewijanie ekranu
Włączenie funkcji **Check Page Reflow** (Wlej zawartość ponownie) spowoduje przeładowanie strony, powiększenie jej zawartości do 400% i ponowne wlanie do jednej kolumny dopasowanej do szerokości okna (rzutni). Funkcja ta pozwala sprawdzić zgodność z nowym w WCAG 2.1 kryterium sukcesu 1.4.10 Przewijanie tekstu. Tester może sprawdzić, czy użytkownik może przewijać i przeglądać zawartość pionowo lub poziomo, w jednym wymiarze bez konieczności przewijania w dwóch wymiarach (z wyjątkiem przypadków szczególnych). Równocześnie sprawdzamy, czy kolejność odczytu jest poprawna (logiczna).
#### Odstępy w tekście
Funkcja **Check Text Spacing** (Sprawdź odstępy w tekście) służy do testów zgodności z nowym WCAG 2.1 kryterium sukcesu 1.4.12. Gdy włączysz tę opcję, zostaną zwiększone odstępy między znakami co najmniej do wielkości równej 0,12 rozmiaru czcionki, między wyrazami do 0,16 rozmiaru czcionki, między wierszami do 1,5 rozmiaru czcionki. Aby zaliczyć test, zmiana ta nie powinna spowodować trudności w czytaniu (nakładania się znaków i wierszy na siebie, oddzielania znaków diakrytycznych od znaków, itp.).
#### Skróty do walidatora HTML
Wygodną dla testerów funkcją są również przyciski **Send DOM to Validator **(Prześlij DOM do walidatora) oraz **Send URL to Validator** (Prześlij URL do walidatora). Oba przyciski przesyłają dane do walidatora Nu Html Checker, który sprawdza poprawność kodu HTML i XHTML. 

