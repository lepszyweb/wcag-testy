---
title: 4. Dostęp z klawiatury i fokus


sidebar: testy_sidebar
permalink: tz-04-klawiatura
folder: testy/tz
---
## Cel procedury testowej


Celem tej procedury jest ustalenie, czy użytkownicy mogą skorzystać ze wszystkich informacji na stronie internetowej i ze wszystkich funkcji, jeśli posługują się tylko klawiaturą. Krócej, celem tej procedury jest ustalenie, czy użytkownicy mają dostęp do treści strony, jeśli posługują się tylko klawiaturą. 

Ponadto, celem jest ustalenie, czy kolejność, w jakiej użytkownik dociera do elementów strony internetowej podczas nawigacji za pomocą klawiatury, jest logiczna. Logiczny porządek poruszania się podczas nawigacji po stronie zapewnia, że użytkownicy mają pełny dostęp do funkcjonalności strony w sposób, który nie jest mylący.

Dostęp do treści strony internetowej tylko za pomocą klawiatury jest niezbędny dla osób niewidomych, a także dla osób z ograniczonymi możliwościami ruchu i manipulacji oraz osób, które nie mogą korzystać z innych urządzeń wskazujących takich, jak mysz czy dotyk. Osoby te mogą, ale nie muszą korzystać z technologii pomocniczych, takich jak czytniki ekranu. 

Celem jest również sprawdzenie, czy na stronie stosowane są widoczne wskaźniki fokusa, czyli oznaczenia miejsca, które aktualnie oczekuje na sygnały wprowadzane przez użytkownika za pomocą klawiatury (naciśnięcia klawiszy). Widoczny wskaźnik fokusa zapewnia, że użytkownicy klawiatury,  mogą się w każdym momencie zorientować, w którym  miejscu strony się znajdują. Wyraźne wskaźniki fokusa są szczególnie ważne dla osób słabowidzących oraz dla osób z problemami poznawczymi, z trudnościami koncentracji uwagi, bo pozwalają im na takie same możliwości orientowania się na stronie, jakie mają osoby korzystające z urządzeń wskazujących.    


Testy zostały zgrupowane w jeden zestaw, ponieważ wszystkie wymagają ręcznej kontroli w celu ustalenia, czy treść spełnia wymagania dostępu za pomocą klawiatury.


Do wykonania testów dostępu z klawiatury i widoczności fokusa klawiatury nie są potrzebne żadne narzędzia testowe.

Procedura testowa „Dostęp z klawiatury i fokus” obejmuje osiem testów:

- Test 4.A - 2.1.1-dostęp z klawiatury
- Test 4.B - 2.1.1-bez-czasu-nacisniecia-klawiszy
- Test 4.C - 2.1.2-bez-pułapki-na-klawiaturę 
- Test 4.D - 2.4.7-widoczny-fokus
- Test 4.E - 3.2.1-po-oznaczeniu-fokusem
- Test 4.F - 2.4.3-kolejnosc-fokusa
- Test 4.G - 2.4.3-fokus-do-tresci-odkrytej
- Test 4.H - 2.4.3-powrot-fokusa-do-porządku


## Dostęp z klawiatury

### Test 4.A 2.1.1-dostep-z-klawiatury 

| Nazwa testu             | ID testu | Warunek testowy |
|----------------|------|-------------------------------------------------------------------|
| 2.1.1-dostep-z-klawiatury | 4.A     | Wszystkie funkcje i wszystkie informacje, które są niezbędne lub wymagane do wykonania danej czynności, mogą być dostępne i wykonywane wyłącznie za pomocą klawiatury. |

### Cel testu
Celem tego testu jest ustalenie, czy wszystkie działania na stronie internetowej i wszystkie informacje niezbędne lub wymagane do ukończenia działania są dostępne i mogą być wykonywane przez osoby, które mogą się posługiwać tylko klawiaturą, wyłącznie za pomocą klawiatury bez potrzeby użycia innych interfejsów. 


Niektóre osoby (w tym osoby niewidome, z ograniczeniami wzroku, z ograniczeniami sprawności ruchowej) mogą nie być w stanie korzystać z myszy lub innego urządzenia wskazującego. Zamiast tego do nawigacji po stronach, wybierania i uruchamiania elementów funkcjonalnych, uzyskiwania informacji umożliwiających zrozumienie treści strony i wykonywania niezbędnych czynności używają klawiatury lub innego urządzenia. Każda funkcjonalność, którą można „wybrać” lub jest dostępna dla osoby używającej myszy, musi być również dostępna dla użytkowników klawiatury. Obejmuje to elementy menu rozwijanego, łącza, przyciski, podpowiedzi, podstawowe informacje w atrybucie `title` i ikony, aby wymienić tylko kilka.

**Uwaga**:
- Informacje w atrybucie `title` są uważane za niezbędne lub wymagane, gdy są niezbędne do wykonania działania lub zrozumienia informacji i relacji.
- Informacje w atrybucie `title` pojawiają się często jako podpowiedzi po najechaniu na element wskaźnikiem myszy. W większości przeglądarek informacje w atrybucie `title` nie są dostępne dla użytkowników korzystających wyłącznie z klawiatury, jeśli nie zastosowano dodatkowego kodowania, które je odsłania.

Wyniki tego testu pozwalają ustalić, czy spełnione jest [kryterium sukcesu 2.1.1 Klawiatura](https://wcag.lepszyweb.pl/#keyboard).


### Metody i narzędzia testowe 

1.	Kontrola ręczna

2.	ANDI: interaktywne > przycisk „atrybuty title”.

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

1. Użyj myszy lub innego urządzenia wskazującego, aby określić:
   - dostępne funkcje zapewniane przez elementy interaktywne (w tym menu rozwijane, pola formularzy, ujawnianie / ukrywanie treści, podpowiedzi ORAZ wszystkie elementy interfejsu interaktywnego),
   - elementy interaktywne, które dostarczają informacji niezbędnych lub wymaganych do ukończenia działania.

2.	ANDI: interaktywne > przycisk „atrybuty title”, aby wykryć elementy z atrybutami `title` i ich treść.
   - Jeśli nie ma przycisku „atrybuty title”, to znaczy, że na stronie nie ma atrybutów `title`.
   - Ustal przypadki, w których atrybut `title` zawiera informacje niezbędne do zrozumienia lub obsługi treści strony.

**Uwaga**:

-   Kryterium sukcesu WCAG 2.1.1 nie dotyczy funkcji, które wymagają danych wejściowych zależnych od ścieżki ruchu użytkownika, a nie tylko punktów końcowych. W przypadku tego procesu testowego, tester nie ma obowiązku identyfikacji i pominięcia tego typu funkcji. Tester powinien uwzględnić wszystkie funkcje, które odpowiadają opisowi w części Identyfikacja treści. <!-- W przypadku niektórych funkcji można zastosować wyjątek określony w sekcji 508, jednak jest to poza zakresem procesu testowego.-->

Dane wejściowe zależne od ścieżki wymagają wprowadzenia danych za pomocą ruchu użytkownika wykonanego wskaźnikiem po ścieżce. Tego rodzaju dane wejściowe to niewielka klasa akcji „myszy”, których nie można wykonać z klawiatury bez konieczności wykonania dodatkowych ruchów. Obejmuje to między innymi używanie myszy do rysowania odręcznego, malowania lub poruszania się po torze przeszkód.

Czynności takie jak rysowanie linii prostych, regularnych kształtów geometrycznych, zmiana rozmiaru okien i przeciąganie obiektów w wybrane miejsce (gdy ścieżka do tego miejsca nie jest istotna) nie wymagają wprowadzania danych zależnych od ścieżki.

Ponieważ różnica pomiędzy tymi funkcjami może być trudna do określenia, testerzy nie są zobowiązani do określania, czy funkcje zależą od ścieżki ruchu użytkownika. Przetestuj wszystkie funkcje. <!-- a jeśli z powodu funkcji zależnej od ścieżki dojdzie do defektu dostępności klawiatury, koordynator sekcji 508 może uznać wyjątek dotyczący zmiany fundamentalnej.-->

### Zastosowanie

Test 4.A 2.1.1-dostep-z-klawiatury **nie ma zastosowania**, jeśli na stronie nie ma interaktywnych elementów treści, na których można ustawić fokus klawiatury.

**Uwaga**
Jeśli na stronie nie ma interaktywnych elementów treści, na których można ustawić fokus klawiatury, przeprowadzanie kolejnych testów z tej procedury nie jest możliwe. Odnotuj jako wynik testów **nie ma zastosowania** przy wszystkich testach z tego zestawu, a więc:

- 4.A - 2.1.1-dostęp z klawiatury
- 4.B - 2.1.1-bez-czasu-nacisniecia-klawiszy
- 4.C - 2.1.2-bez-pułapki-na-klawiaturę 
- 4.D - 2.4.7-widoczny-fokus
- 4.E - 3.2.1-po-oznaczeniu-fokusem
- 4.F - 2.4.3-kolejnosc-fokusa
- 4.G - 2.4.3-fokus-do-tresci-odkrytej
- 4.H - 2.4.3-powrot-fokusa-do-porządku

### Jak testować

1.  Użyj myszy, aby zidentyfikować funkcjonalności i niezbędne informacje dostarczane przez elementy interaktywne.

    1.  Funkcja ANDI: interaktywne > „atrybuty title” może pomóc zidentyfikować wszelkie istotne informacje zawarte w atrybutach `title`.
	
	   - Jeśli nie ma przycisku „atrybuty title”, to znaczy, że na stronie nie ma atrybutów `title`.
	   - Ustal przypadki, w których atrybut `title` zawiera informacje niezbędne do zrozumienia lub obsługi treści strony.

2.  Użyj klawiatury, aby obsługiwać konkretną funkcjonalność i uzyskać dostęp do niezbędnych informacji:   klawiszem Tab uzyskaj dostęp do elementu i uruchom funkcjonalność (np. naciśnij klawisz Enter).

    1.  W przypadku elementów interaktywnych z atrybutami `title` umieść fokus klawiatury na elemencie. Jeśli w ciągu dwóch sekund nie pojawi się podpowiedź, fokus klawiatury nie ujawnia informacji z atrybutu `title`.

    **Uwaga**: Jeśli na stronie wystąpią jakiekolwiek automatyczne zmiany funkcjonalności (takie jak wyświetlenie powiadomienia o przekroczeniu limitu czasu, aby umożliwić Ci zażądanie więcej czasu), należy je tutaj przetestować.
	
	Jeśli na stronie wystąpią jakiekolwiek zmiany w wyniku z interakcji ze stroną (takie jak ujawnienie dodatkowych pól formularza), należy je tutaj przetestować.

3.  Jeśli element interaktywny nie ma dostępu do klawiatury, sprawdź, czy na stronie dostępna jest inna metoda dostępna za pomocą klawiatury, która zapewnia tę samą funkcjonalność, np. jedna z dwóch podanych metod  drukowania jest dostępna za pomocą klawiatury itp. Aby uzyskać szczegółowe informacje, zobacz [Zgodna wersja alternatywna](tz-01-alternatywne.md)

4.  Jeśli element interaktywny nie zapewnia dostępu do istotnych informacji za pomocą interakcji klawiatury, sprawdź, czy informacje są dostępne w innym miejscu strony (np. jako tekst).

**Uwaga:** Nie wszystkie przeglądarki wyświetlają wizualnie atrybut `title` jako etykietkę narzędzia, gdy element uzyskuje fokus klawiatury.



### Ocena wyników

Jeśli **wszystkie** poniższe twierdzenia są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 2.1.1:

1.  Za pomocą klawiatury można uzyskać dostęp do wszystkich funkcjonalności i uruchomić je **oraz**

2.  Dostęp do wszystkich niezbędnych informacji można uzyskać za pomocą klawiatury **lub** informacje istnieją w innym miejscu strony.


### Uwaga: 

-   W tym teście należy uwzględnić wszelkie zmiany funkcji, które nastąpią automatycznie lub w wyniku interakcji ze stroną.
-   Informacje uważa się za niezbędne lub wymagane, gdy są one niezbędne do wykonania działania lub zrozumienia informacji i relacji.
-   Informacje w atrybucie `title` lub podpowiedzi (tooltip), które nie są niezbędne, nie wymagają dostępu do klawiatury.

## Czas naciśnięcia klawiszy

### Test 4.B 2.1.1-bez-czasu-nacisniecia

| Nazwa testu               | ID testu | Warunek testowy  |
|----------------|------|-------------------------------------------------------------------|
| 2.1.1-bez-czasu-nacisniecia-klawisza | 4.B | Poszczególne naciśnięcia klawiszy nie wymagają określonego czasu aktywacji funkcji. |

Celem tego testu jest sprawdzenie, czy na stronie istnieje jakakolwiek funkcjonalność, która wymaga od użytkownika wykonania naciśnięcia pewnych klawiszy w określonym czasie lub z zachowaniem określonego czasu między naciśnięciami klawiszy. Na przykład, czy istnieją sytuacje, w których użytkownik musi powtórzyć lub wykonać wiele naciśnięć klawiszy w krótkim czasie lub gdy klawisz musi być przytrzymany przez dłuższy czas, aby wywołać działanie.   

Wymóg naciskania klawiszy przez określony czas lub z zachowaniem określonego czasu przerw między naciśnięciami klawiszy stanowi poważne utrudnienie dla osób z ograniczonymi możliwościami ruchu i manipulacji.

**Uwaga**: Wymóg naciskania klawiszy przez określony czas występuje często w grach (naciskanie spacji, aby strzelać, gdy cel znajduje się w celowniku) lub w symulacjach aktywności (przesuwanie bloku po stole za pomocą klawiszy strzałek).

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.1.1 Klawiatura](https://wcag.lepszyweb.pl/#keyboard).


### Metody i narzędzia testowe

1.	Kontrola ręczna

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

Sprawdzasz wszystkie elementy interaktywne i wszystkie funkcjonalności zidentyfikowane w teście 4.A (2.1.1-dostęp z klawiatury). W teście 4.A sprawdzaliśmy, czy wszystkie elementy interaktywne i funkcjonalności są dostępne wyłącznie za pomocą klawiatury. Teraz ustalamy, czy skorzystanie z którejkolwiek z tych funkcjonalności nie wymaga od użytkownika określonego czasu przytrzymywania klawiszy albo naciskania klawiszy w określonych odstępach czasu.  

**Uwaga**. Ten test nie wymaga oceniania, czy funkcjonalności nie podlegają temu wymogowi ze na funkcję wymagającą danych wejściowych zależną od ścieżki ruchu użytkownika. 

### Zastosowanie

Test 4.B 2.1.1-bez-czasu-nacisniecia **nie ma zastosowania**, jeśli na stronie nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.A 2-1-1 został oznaczony jako **nie ma zastosowania**, to test 4.B 2.1.1-bez-czasu-nacisniecia również **nie ma zastosowania**.


### Jak testować

1.  Kontynuuj test 4.A.

2.  Ustal, czy istnieją przypadki, w których wymagany jest określony czas naciśnięcia klawiszy, aby aktywować element, np. szybkość wpisywania hasła jest częścią uwierzytelniania hasła.

    1. Poszukaj instrukcji wskazujących, że klawisz musi być przytrzymany przez określony czas lub że przydzielono określoną ilość czasu na wykonanie serii naciśnięć klawiszy.
	
	2. Poszukaj komunikatów wskazujących, że nie można aktywować funkcji, ponieważ akcja nie została ukończona w wyznaczonym czasie.
	
	**Uwaga**: Testowana jest wszelka treść, która wymaga wyczucia czasu naciśnięcia klawisza, nawet jeśli wydaje się, że funkcja może zależeć od ścieżki ruchu użytkownika, a nie tylko punktów końcowych.

3.  Jeśli istnieje funkcja zależna od czasu, sprawdź, czy na stronie istnieje inna metoda wykonania zadania za pomocą klawiatury, która nie wymaga określonego czasu.

#### Ocena wyników

Jeśli poniższe stwierdzenie jest prawdziwe, treść (strona) **spełnia** wymóg testowy, jest **zgodna** z KS 2.1.1

1.  Istnieje metoda, która umożliwia aktywację każdej funkcji za pomocą klawiatury, nie wymagając od użytkowników określonego czasu aktywacji (czasu naciskania klawiszy).


## Bez pułapki na klawiaturę

### Test 4.C 2.1.2-bez-pulapki-na-klawiature

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.1.2-bez-pulapki-na-klawiature | 4.C     | Nie ma pułapki na klawiaturę. |

### Cel testu
Celem tego testu jest sprawdzenie, czy użytkownicy są w przenosić fokus klawiatury z elementów interaktywnych, które otrzymały fokus klawiatury na poprzednie i następne elementy interaktywne, jeśli istnieją. Jeśli nie jest to możliwe, mówimy, że na stronie istnieje „pułapka na klawiaturę”.

Pułapka na klawiaturę zdarza się często wtedy, gdy na stronie znajduje się wiele połączonych wtyczek lub osadzonych aplikacji.

Test dotyczy wszystkich elementów strony, także sekcji, które są ujawniane (odkrywane) w wyniku interakcji z elementem strony (np. przyciskiem, zakładką karty, itp.). Jeśli użytkownik przejdzie do takiej treści, konieczna jest również metoda opuszczenia tego obszaru. 

Jeśli do opuszczenia takiego obszaru lub jakiegokolwiek elementu interaktywnego konieczna jest niestandardowa metoda (inna niż naciśnięcie klawisza Tab lub klawiszy strzałek), użytkownik musi zostać poinformowany o tej metodzie. 

Pułapka na klawiaturę może zakłócać zdolność użytkownika do korzystania z całej strony. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.1.2 Bez pułapki na klawiaturę](https://wcag.lepszyweb.pl/#no-keyboard-trap).


### Metody i narzędzia testowe

1.	Kontrola ręczna

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

Nawiguj tabulatorem po elementach interaktywnych strony (odkrytych w teście 4.A), aby ustalić, czy klawiatura (i użytkownicy) nie zostanie uwięziona w jakimś elemencie strony albo obszarze na stronie odkrytym w efekcie interakcji z komponentem strony.

### Zastosowanie

Test 4.C 2.1.2-bez-pulapki-na-klawiature **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.A 2-1-1 został oznaczony jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.C 2.1.2-bez-pulapki-na-klawiature **nie ma zastosowania**.


#### Jak testować

1.  Nawiguj tabulatorem między wszystkimi komponentami strony, na których można ustawić fokus klawiatury.
2.  Ustal, czy istnieją przypadki, w których nawigacja klawiaturą jest zablokowana:

   1.  Użytkownicy klawiatury nie mogą wyjść z elementu, np. za pomocą klawisza TAB lub klawiszy strzałek albo klawisza ESC
   2.  Dostęp z klawiatury jest ograniczony do niewielkiej części strony, bez możliwości wyjścia z „pętli” do innych interaktywnych komponentów strony.

2.  Jeśli znaleziono pułapkę na klawiaturę::

    1.  Sprawdź wszelką pomoc (kontekstową, pomoc aplikacji) i dokumentację pod kątem powiadomień o alternatywnych poleceniach klawiaturowych (np. niestandardowe sterowanie klawiaturą, klawisze dostępu, klawisze skrótów), które pozwalają wyjść z pułapki na klawiaturę.
    2.  Sprawdź, czy polecenia alternatywne działają.

**Uwaga**: W przypadku wystąpienia pułapki na klawiaturę kontynuuj testowanie interaktywnych elementów za „pułapką”, używając do omijania pułapki myszy lub odświeżając stronę i używając klawiatury do nawigowania wstecz po stronie.

### Ocena wyników 
Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.1.1

1.  Fokus klawiatury można przenieść z każdego komponentu strony za pomocą:

    1.  Standardowych klawiszy nawigacyjnych (tab, klawisze strzałek) 
    2.  Niestandardowych naciśnięć klawiszy (które są udokumentowane i dostępne dla użytkowników w aplikacji).

**oraz**

2.  Fokus klawiatury można przenieść z każdego zawierającego komponenty interaktywne obszaru strony do innego obszaru za pomocą:

    1.  Standardowych klawiszy nawigacyjnych
    2.  Niestandardowych naciśnięć klawiszy (które są udokumentowane i dostępne dla użytkowników w aplikacji).

### Uwaga:

W przypadku wystąpienia pułapki na klawiaturę kontynuuj testowanie interaktywnych elementów poza „pułapką”, używając do omijania pułapki myszy lub odświeżając stronę i używając klawiatury do nawigowania wstecz po stronie.

## Fokus klawiatury 

### Test 4.D 2.4.7-widoczny-fokus 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.7-widoczny-fokus | 4.D     | Graficzny wskaźnik fokusa jest wyświetlany, gdy fokus znajduje się na komponencie interfejsu.|

### Cel testu 

Celem tego testu jest ustalenie, czy wszystkie komponenty interfejsu dostępne z klawiatury mają w stanie gotowości na odbieranie zdarzeń związanych z naciskaniem klawiatury widoczne oznaki fokusa.

### Dlaczego to jest ważne?
Osoby, które obsługują stronę internetową tylko za pomocą klawiatury muszą wiedzieć, który z elementów interaktywnych na stronie jest aktualnie w stanie gotowości na odbieranie zdarzeń związanych z naciskaniem klawiatury. Taki stan nazywa się *skupieniem*, *punktem uwagi* albo z angielskiego *fokusem*. W otwartym oknie strony lub aplikacji tylko jeden element w danym momencie może się znajdować w stanie skupienia. 

Wizualny sygnał stanu skupienia jest również bardzo pomocny osobom z ograniczeniami uwagi, pamięci krótkotrwałej, zręczności, procesów wykonawczych.

Skupienie można przenosić z jednego elementu na następny za pomocą klawiszy Tab oraz Shift+Tab, a wewnątrz złożonych elementów za pomocą klawiszy strzałek.

Elementy mogą się znaleźć w stanie skupienia także w wyniku kliknięcia myszą, ale w reakcji na kliknięcie wykonują zwykle jeszcze dodatkowe funkcje.

Wskaźnik skupienia może przybierać różne formy: obramowania elementu, migającego kursora (karetka) w polu tekstowym, wizualnej zmiany wyglądu przycisku. 

Twórcy stron i aplikacji mogą umożliwiać i wyłączać możliwość otrzymywania skupienia przez elementy strony, a także zmieniać kolejność przenoszenia skupienia, korzystając z atrybutu `tabindex` oraz ze skryptów.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.4.6 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible).

### Metody i narzędzia testowe

1. Kontrola ręczna
2. Inspekcja wzrokowa

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

Użyj klawiatury, aby poruszać się po wszystkich komponentach interfejsu dostępnych z klawiatury **oraz** wszystkich interaktywnych komponentów interfejsu (łącza, przyciski, przełączniki, pola formularzy, rozwijane menu, treść odkrywana/ukrywana itd.). 

### Zastosowanie

Test 4.D 2.4.7-widoczny-fokus **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.A 2-1-1 został oznaczony jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.D 2.4.7-widoczny-fokus **nie ma zastosowania**.


#### Jak testować

1.  Kontynuuj test 4.C.

2.  Ustal, czy na elemencie, który ma fokus klawiatury, widoczny jest graficzny wskaźnik fokusa.

    1.  Gdy fokus klawiatury jest ustawiony na ramce, niektóre przeglądarki wyświetlają graficzny wskaźnik fokusa, a inne nie. Jeśli graficzny wskaźnik fokusa nie jest widoczny na ramce, zignoruj ten fakt, **nie jest** to defekt treści internetowej.	

    **Uwaga**: Aby potwierdzić, że niewidoczny fokus klawiatury znajduje się na ramce, użyj kombinacji klawiszy Tab i Shift+Tab, aby wydedukować, że fokus klawiatury jest na ramce. Będąc na ramce, naciśnij tabulator, aby przenieść fokus na pierwszy element, który można ustawić za pomocą klawiatury w ramce. Tam naciśnij klawisze Shift+Tab, aby wrócić do ramki, i kolejny raz Shift+Tab, aby przenieść fokus na element interaktywny przed ramką. Tylko ramka może nie mieć widocznego fokusa. Upewnij się, że to ramka nie ma widocznego fokusa, a nie inny element.

    Wizualny wskaźnik fokusa może przyjmować różną formę, taką jak kropkowany kontur, wyróżnienie kolorem, podświetlenie, pionowy pasek (kursor, karetka) w polu tekstowym. 

    Odczucie jasności fokusa jest subiektywne, ale tester powinien być w stanie zidentyfikować zmianę wizualną elementu, który ma fokus klawiatury lub otrzymuje fokus.

    W niektórych przypadkach może być konieczne nawigowanie po całej stronie zarówno do tyłu, jak i do przodu, aby ustalić, czy określony element interfejsu zapewnia wizualne wskazanie fokusa. Należy jednak pamiętać, że kolejność ustawiania fokusa jest testowana osobno. 


### Ocena wyników 
Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.7

1.  Gdy komponent interfejsu otrzymuje fokus klawiatury, widoczny jest graficzny wskaźnik fokusa.

## Po oznaczeniu fokusem 

### Test 4.E 3.2.1-po-oznaczeniu-fokusem 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 3.2.1-po-oznaczeniu-fokusem| 4.E     | Przeniesienie fokusa na element interaktywny nie inicjuje zmiany kontekstu |

## Cel testu
Celem tego testu jest sprawdzenie, czy komponenty interfejsu, które otrzymują fokus, nie inicjują nieoczekiwanej zmianę kontekstu w wyniku samego faktu przeniesienia fokusa na element. Takie zachowanie zapewnia przewidywanie zachowania się elementów funkcjonalnych strony. Żaden element interfejsu, który jest w stanie wyzwolić zdarzenie po otrzymaniu fokusa, nie może zmieniać kontekstu.

Zmiana kontekstu to poważna zmiana treści, która może dezorientować użytkowników, zwłaszcza, jeśli nie są w stanie wyświetlić całej strony równocześnie. 

Przykłady nieoczekiwanych zmian kontekstu obejmują:

-	otwieranie nowego okna przeglądarki,
-	przeniesienie fokusa na inny komponent interfejsu na stronie,
-	automatyczne przesłanie formularza,
-	przejście na inną stronę internetową lub do innego okna,
-	znacząca zmiana treści strony.

Zmiany treści **nie zawsze** są zmianami kontekstu. Zmiany treści mogą polegać na rozszerzeniu konturu, odsłonięciu treści ukrytych bądź ukrycie odsłoniętych, uzyskaniu dostępu do pozycji dynamicznego menu. Takie zmiany nie zmieniają ani kontekstu.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 3.2.1 Po oznaczeniu fokusem](https://wcag.lepszyweb.pl/#on-focus).


### Metody i narzędzia testowe

1. Kontrola ręczna
2. Inspekcja wzrokowa

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

Użyj klawiatury, aby poruszać się po wszystkich komponentach interfejsu dostępnych z klawiatury **oraz** wszystkich interaktywnych komponentów interfejsu (łącza, przyciski, przełączniki, pola formularzy, rozwijane menu, treść odkrywana/ukrywana itd.). 
### Zastosowanie

Test 4.E 3.2.1-po-oznaczeniu-fokusem **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.A 2-1-1 został oznaczony jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.E 3.2.1-po-oznaczeniu-fokusem **nie ma zastosowania**.


### Jak testować

1.  Kontynuuj test 4.D.

2.  Gdy na element interfejsu zostanie przeniesiony  fokus, oceń, czy nastąpi nieoczekiwana zmiana kontekstu, np. uruchomione zostanie nowe okno lub fokus zostanie przeniesiony na inny element interfejsu.

Pamiętaj, że sprawdzasz poprawność tego, co się dzieje, gdy komponent otrzymuje fokus. Podczas tego testu nie uruchamiasz komponentu np. naciskając klawisze Enter lub Spacja, aby aktywować przycisk „prześlij” czy „rozwinąć” menu. Podczas tego testu oceniasz jedynie, co się dzieje, gdy fokus wyląduje na elemencie.

### Ocena wyników
Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 3.2.1

1.  Gdy komponent interfejsu otrzymuje fokus, nie jest inicjowana żadna zmiana niespodziewana kontekstu.

## Kolejność tabulacji


### Test 4.F 2.4.3-kolejnosc-fokusa 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-kolejnosc-fokusa  | 4.F     | Kolejność ustawiania fokusa zachowuje znaczenie i użyteczność strony. |

### Cel testu

Celem tego testu jest upewnienie się, że użytkownicy klawiatury poruszający się sekwencyjnie po stronie internetowej napotykają informacje w kolejności zgodnej ze znaczeniem treści. Wskaźnik fokusa powinien poruszać się po elementach strony w logicznej kolejności, a gdy sekwencja nawigacyjna wpływa na znaczenie lub działanie, komponenty, na których można ustawić fokus, powinny otrzymywać fokus w kolejności, która zachowuje to znaczenie. Kolejność ustawiania fokusa może nie być identyczna z ustaloną programowo lub wizualną kolejnością czytania, o ile użytkownik nadal może zrozumieć i obsługiwać stronę internetową. 

Ten test dotyczy tylko elementów, które otrzymują fokus klawiatury. 

Kolejność tabulacji ma szczególne znaczenie dla osób, które obsługują stronę tylko za pomocą klawiatury. 
Osoby te spodziewają się, że porządek tabulacji będzie intuicyjny, zgodny ze znaczeniem treści, logiczny i dostosowany do porządku czytania.  

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.4.3 Kolejność fokusa](https://wcag.lepszyweb.pl/#focus-order).

### Metody i narzędzia testowe

1. Kontrola ręczna
2. Inspekcja wzrokowa

### Identyfikacja treści
Wszystkie interaktywne elementy treści.


Użyj klawiatury, aby poruszać się po wszystkich komponentach interfejsu dostępnych z klawiatury **oraz** wszystkich interaktywnych komponentów interfejsu (łącza, przyciski, przełączniki, pola formularzy, rozwijane menu, treść odkrywana/ukrywana itd.). 

### Zastosowanie

Test 4.F 2.4.3-kolejnosc-fokusa  **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.F 2.4.3-kolejnosc-fokusa jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.F 2.4.3-kolejnosc-fokusa **nie ma zastosowania**.

### Jak testować

1.  Ustaw kursor w pasku adresu przeglądarki, a następnie użyj klawisza Tab, aby przemieszczać się do kolejnych interaktywnych elementów strony (łącza, przyciski, przełączniki, pola formularzy, itd.).  Nie używaj myszy.

2.  Oceń, czy kolejność przemieszczania się fokusa wpływa na znaczenie i użyteczność (funkcjonalność)  strony (np. pola przeznaczone na adres otrzymują fokus w logicznej kolejności - zgodnej z budową adresu).

    1.  Najczęściej można zauważyć, że kolejność przemieszczania się fokusa nie jest zgodna z wizualnym porządkiem elementów i logiczną kolejnością działania (zwykle od lewej do prawej, z góry na dół)


    2.  W przypadku modalnych okien dialogowych fokus powinien pozostać w oknie, dopóki nie zostanie ono zamknięte. Modalne okno dialogowe wymaga interakcji użytkownika, aby powrócić do aplikacji.

    3.  Pomocne może być uruchomienie ANDI: interaktywne i wybranie przycisku porządek tabulacji.

### Ocena wyniku
Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.2

1.  Kolejność ustawiania fokusa zachowuje znaczenie treści **oraz**

2.  Kolejność ustawienia fokusa zachowuje funkcjonalności strony.

### Uwaga:

-   Znaczniki kolejności tabulatorów ANDI mogą się nieznacznie różnić od rzeczywistej kolejności tabulatorów klawiatury w niektórych przeglądarkach. Zawsze oceniaj wyniki z kolejności tabulacji klawiatury.

## Powrót fokusa

### Test 4.G 2.4.3-fokus-do-tresci-odkrytej 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-fokus-do-tresci-odkrytej | 4.G     | Fokus jest przenoszony na odkryte treści. |

### Cel testu 
Celem tego testu jest sprawdzenie, czy po ujawnieniu ukrytej treści na tej samej stronie fokus jest przenoszony do ujawnionej treści albo natychmiast, albo po jednym naciśnięciu klawisza. 

Ujawnianie treści to np. rozwijanie pozycji menu, otwieranie okna modalnego, odkrywanie treści ukrytej w harmonijce.

Ten test jest ściśle związany z poprzednim 4.F 2.4.3-kolejnosc-fokusa. Oba testy łącznie sprawdzają, czy kolejność fokusa jest logiczna, gdy użytkownik wchodzi w interakcję z treścią strony.
 
Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.4.3 Kolejność fokusa](https://wcag.lepszyweb.pl/#focus-order).

### Metody i narzędzia testowe

1. Kontrola ręczna
2. Inspekcja wzrokowa

### Identyfikacja treści
Wszystkie interaktywne elementy treści.


Użyj klawiatury, aby poruszać się po wszystkich komponentach interfejsu dostępnych z klawiatury **oraz** wszystkich interaktywnych komponentów interfejsu (łącza, przyciski, przełączniki, pola formularzy, rozwijane menu, treść odkrywana/ukrywana itd.). 

### Zastosowanie
Test 4.G 2.4.3-fokus-do-tresci-odkrytej  **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.G 2.4.3-fokus-do-tresci-odkrytej jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.G 2.4.3-fokus-do-tresci-odkrytej  **nie ma zastosowania**.

**Uwaga**: Ten test **nie jest stosowany**, gdy element interaktywny otwiera całkowicie nową stronę treści, na przykład gdy łącze prowadzi użytkownika do nowej strony internetowej.


#### Jak testować

1. Użyj klawiatury, aby aktywować elementy sterujące, które ujawniają ukrytą treść (np. menu, okna dialogowe, modalne okna dialogowe).

   1. W przypadku modalnych okien dialogowych, widoczny fokus powinien pozostać w oknie do momentu jego zamknięcia. (Jest to uwzględnione w teście 4.F.)
   
   2. Ujawniona treść nie zawiera informacji, które pojawiają się jak część atrybutu `title` podpowiedzi (tooltipa).

2. Przemieszczaj fokus poprzez ujawnioną treść za pomocą klawisza TAB.

   1.  Widoczny fokus może nie przechodzić do ujawnionej treści, jeśli nie zawiera ona elementów, które mogą otrzymać fokus lub jeśli  nie można ustawić fokusa na całej ujawnionej treści.

### Ocena wyników
Jeśli którekolwiek z poniższych twierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.3

1.  Fokus klawiatury przenosi się bezpośrednio na ujawnioną treść **albo**

2.  Jedno dodatkowe naciśnięcie klawisza przenosi fokus na ujawnioną treść.


### Test 4.H 2.4.3-powrot-fokusa-do-porządku 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-powrot-fokusa-do-porządku | 4.H     | Fokus powraca do logicznej sekwencji |

## Cel testu

Celem tego testu jest sprawdzenie, czy użytkownik powraca do logicznej sekwencji fokusa sprzed ujawnienia treści. Ten test dotyczy tego, na jaki element interfejsu przechodzi fokus po opuszczeniu obszaru z ujawnioną treścią, jeśli został do tego obszaru przeniesiony. Po  

Po zakończeniu interakcji użytkownika z ujawnioną treścią fokus powinien powrócić do elementu, który zainicjował akcję, lub przejść do następnego elementu w logicznym porządku tabulacji, aby umożliwić użytkownikowi kontynuowanie nawigacji po stronie internetowej. 

Ten test jest ściśle związany z poprzednim 4.G 2.4.3-fokus-do-tresci-odkrytej, ponieważ oba testy łącznie weryfikują, czy kolejność fokusa jest logiczna, gdy użytkownik wchodzi w interakcję z treścią strony.
 
Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu 2.4.3 Kolejność fokusa](https://wcag.lepszyweb.pl/#focus-order).

### Metody i narzędzia testowe

1. Kontrola ręczna
2. Inspekcja wzrokowa

### Identyfikacja treści
Wszystkie interaktywne elementy treści.

Użyj klawiatury, aby poruszać się po wszystkich komponentach interfejsu dostępnych z klawiatury **oraz** wszystkich interaktywnych komponentów interfejsu (łącza, przyciski, przełączniki, pola formularzy, rozwijane menu, treść odkrywana/ukrywana itd.). 

### Zastosowanie
Test 4.H 2.4.3-powrot-fokusa-do-porządku **nie ma zastosowania**, jeśli na stronie nie ma komponentów, na których można ustawić fokus klawiatury, czyli nie ma funkcji aktywowanych przez użytkownika (takie sytuacje są raczej niespotykane, ale możliwe).

**Uwaga**: Jeśli test 4.H 2.4.3-powrot-fokusa-do-porządku jako **nie ma zastosowania**, to wszystkie inne testy z tej procedury testowej, a więc także test 4.H 2.4.3-powrot-fokusa-do-porządku **nie ma zastosowania**.

### Jak testować

1.  Kontynuuj test 4.G

2.  Jeśli to możliwe, aby zamknąć/ukryć lub odrzucić ujawnianą treść, użyj klawiatury, aby zamknąć / ukryć i / lub przenieść fokus z ujawnionej treści.

3.  Zidentyfikuj element, który ma fokus klawiatury.

    1.  Konieczne może być naciśnięcie klawiszy Shift + Tab lub klawisza strzałki, aby przesunąć fokus do tyłu.

3.  Porównaj położenie elementu, który po otrzymaniu fokusa ujawnił ukrytą treść, z miejscem, w ktróym znajduje się fokus po opuszczeniu obszaru z ujawnioną treścią. Jeśli fokus nie powróci do elementu wyzwalającego ukrytą treść, sprawdź, czy elementem, do którego zostanie przeniesiony, jest następny element interaktywny na stronie, czy żaden interaktywny element nie zostanie pominięty w porządku tabulacji.


### Ocena wyników

Jeśli którekolwiek z poniższych twierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.3

1.  Fokus klawiatury automatycznie powraca do logicznej sekwencji kolejności fokusa sprzed ujawnienia treści **albo**

2.  Jedna dodatkowe naciśnięcie klawisza lub kombinacji klawiszy przywraca fokus do logicznej sekwencji kolejności fokusa sprzed ujawnienia treści.

**Uwaga**: Sekwencja logiczna oznacza, że znaczenie i użyteczność strony są zachowane. Dopuszczalne jest, jeśli fokus nie wraca dokładnie do miejsca sprzed ujawnienia treści, o ile sekwencja jest logiczna. Może się to zdarzyć w przypadku elementów takich jak menu; zamknięcie opcji menu może spowodować przeniesienie użytkownika do następnego elementu w kolejności fokusu. Może to nadal utrzymywać logiczną sekwencję.


### Obowiązujące normy


{% include ks/2-1-1.md %}

{% include ks/2-1-2.md %} 

[1. Dostęp z klawiatury](ICT-01-klawiatura) 

{% include ks/2-4-7.md %}

[2. Widoczny fokus](ICT-02-widoczny-fokus)

| {% include ks/2-4-3.md %}

{% include ks/3-2-1.md %}

[3. Kolejność fokusa](ICT-03-kolejnosc-fokusa)

