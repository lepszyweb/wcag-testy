MONITOROWANIE I BADANIA DOSTĘPNOŚCI SERWISU
Ocena dostępności stron internetowych

# Monitorowanie i badania dostępności serwisu 
 
Zapoznaj się z nieoficjalnym tłumaczeniem jednej z pierwszych wersji dokumentu Evaluation of Web Content Accessibility. Dokument przedstawia ogólne procedury i wskazówki pomocne dla przeprowadzania testów dostępności w czasie tworzenia witryny oraz monitorowania już istniejących stron internetowych.

**Uwaga**: Ten dokument pochodzi sprzed 15 lat. Publikujemy go głównie w celach edukacyjnych. Jakkolwiek może dostarczać pewnych wskazówek dotyczących oceniania dostępności stron internetowych, to trudno byłoby dziś polecać przedstawione w nim rozwiązania.

## 1. Wstęp
Dokument ten zarysowuje problematykę wstępnego przeglądu dostępności witryny internetowej oraz oceny zgodności z WCAG 1.0. Chociaż nie prezentuje technik testowania punkt po punkcie, zawiera ogólne procedury i wskazówki pomocne dla przeprowadzania testów podczas tworzenia stron internetowych oraz monitorowania istniejących stron. Inne dokumenty zostaną stworzone do dogłębnego/szczegółowego testowania zgodności. Opisane tu środki mają być w zamierzeniu wsparciem dla już używanych procedur zarządzania zawartością i kontroli jakości na stronach internetowych. Powody, dla których dostępność stron internetowych jest ważna, wymienione są we Wprowadzeniach do Zasobów WAI.

Istnieje wielka rozmaitość narzędzi i podejść do oceny dostępności stron internetowych. Jak dotąd żadne pojedyncze narzędzie sprawdzające nie zapewnia wyczerpujących informacji ani nie wychwytuje wszystkich problemów związanych z dostępnością strony internetowej; dlatego też na ocenianie składa się kombinacja metod. Cele oceny stron internetowych są różne i wymagają różnych podejść, aby osiągnąć te cele:

- Wstępny przegląd dostępności może:
  - Rozpoznać ogólne rodzaje barier na stronie internetowej.
- Ocena zgodności może:
  - wychwywycić główne problemy podczas fazy projektowania i tworzenia nowej strony internetowej;
  - określić poziom zgodności istniejącej witryny z WCAG 1.0;
  - wykazać, że strona internetowa odpowiada danemu poziomowi zgodności WCAG 1.0.
- Ocena zgodności i dodatkowo przegląd procedur dla bieżącego monitorowania może:
  - pomóc w zapewnieniu, że witryna utrzyma określony poziom zgodności w przyszłości.

**Uwaga**: Ten dokument może być regularnie uaktualniany, aby odzwierciedlić wyjaśnienia lub udoskonalania metodyki oceny, wynikające z rosnącej roli półautomatycznych narzędzi oceny, ponieważ możliwości takich narzędzi poprawiają się, i powiązaną z tym redukcję kroków ręcznego testowania; tak samo jak włączenie bardziej precyzyjnych technik testowania punktów kontrolnych, w miarę jak stają się one dostępne. Przyszłe wersje tego dokumentu mogą zawierać listę kontrolną oceny i / lub być publikowane jako Notatka W3C. Data wersji i informacje o tym, gdzie należy przesyłać uwagi, jest umieszczona na końcu dokumentu. Wymienienie w tym dokumencie konkretnych narzędzi oceny nie stanowi poparcia ze strony W3C. Ani użycie wstępnego przeglądu, ani metod sprawdzania poprawności nie gwarantuje zgodności z prawem lub prawnymi regulacjami jakiegoś konkretnego rządu.

## 2. Przegląd wstępny
Przegląd wstępny może pomóc w szybkiej identyfikacji zakresu problemów na stronie internetowej. Jednakże nie wychwyci wszystkich problemów i nie powinien być wykorzystywany do określenia poziomu zgodności. Przegląd wstępnyani nie bierze pod uwagę zróżnicowania problemów, jakie napotykają niepełnosprawni użytkownicy, ani nie obejmuje i nie sprawdza wszystkich aspektów witryny.

Przegląd wstępny jest połączeniem ręcznego sprawdzania reprezentatywnych stron witryny z wykorzystaniem kilku półautomatycznych narzędzi oceniających dostępność. Osoby przeprowadzający taki przegląd (recenzenci) nie muszą znać języka znaczników internetowych, ale powinny być w stanie pobrać oprogramowanie i zapoznać się z niektórymi narzędziami online oraz zmienić pewne ustawienia w swojej przeglądarce.

Aby przeprowadzić wstępny przegląd, należy wykonać wszystkie pięć poniższych kroków.

1. Wybierz do przeglądu reprezentatywną próbkę różnych rodzajów stron z witryny; próbka musi zawierać wszystkie strony, na które prawdopodobnie trafią goście („strony powitalne” itd.)

**Uwaga**: na stronach z zawartością generowaną dynamicznie z baz danych, wygeneruj szeroką reprezentację próbek, zapisz je i testuj zapisane strony.

2. Użyj przeglądarki internetowej posiadającej graficzny interfejs użytkownika (GUI), takiej jak Mozilla Firefox, Chrome, Internet Explorer lub Opera, i sprawdź wybrane strony, dostosowując ustawienia przeglądarki w następujący sposób.

  (**Uwaga**: jeżeli przegląd dokonywany jest przez osoby z niepełnosprawnościami, w niektórych czynnościach muszą asystować im ludzie, którzy nie posiadają takich samych niepełnosprawności.)
  (**Uwaga**: Niektóre z tych ręcznych testów mogą być wykonywane poprzez zmianę ustawień lub preferencji w przeglądarce, inne mogą wymagać zmiany ustawień systemu operacyjnego, a niektóre mogą wymagać dodatkowego oprogramowania.)

  1. Wyłącz obrazy i sprawdź, czy dostępny jest odpowiedni tekst alternatywny.
  2. Wyłącz dźwięk i upewnij się, czy zawartość audio jest nadal dostępna poprzez odpowiedniki tekstowe.
  3. Użyj elementów sterujących przeglądarki, aby zmienić rozmiar czcionki: sprawdź, czy rozmiar czcionki zmienia się odpowiednio na ekranie; i czy strona może być nadal używana przy większych rozmiarach czcionki.
  4. Sprawdź w różnych rozdzielczościach ekranowych i/oraz zmieniając rozmiary okna aplikacji do mniejszego niż maksymalne, upewnij się, czy nie jest potrzebne przewijanie w poziomie(**Uwaga**: sprawdź w różnych przeglądarkach lub przetestuj kod dla rozmiaru bezwzględnego, żeby upewnić się, że to jest problem zawartości a nie przeglądarki)
  5. Zmień kolor wyświetlania na skalę szarości (albo obejrzyj stronę na wydruku czarno-białym lub w skali szarości) i sprawdź, czy kontrast kolorów jest wystarczający.
  6. Bez użycia myszy przemieszczaj się pomiędzy odsyłaczami i polami formularza, upewniając się, że możesz uzyskać dostęp do wszystkich odsyłaczy i pól formularza oraz że teksty odsyłaczy wyraźnie wskazują, do czego prowadzą.
3. Użyj przeglądarki głosowej (takiej jak Home Page Reader) lub tekstowej (takiej jak Lynx) i zapoznaj się ze stroną internetową odpowiadając na poniższe pytania.
  (**Uwaga**: doświadczeni użytkownicy czytników ekranu mogą zastąpić czytnik ekranu przeglądarką głosową lub tekstową, ale jeśli są niewidomi mogą potrzebować widzącego partnera, żeby porównać informacje dostępne wizualnie; jeśli nie są niewidomi, powinni słuchać tego z zamkniętymi oczami, a potem z otwartymi oczami sprawdzić, czy informacje są równoważne).
  1. czy informacje dostępne za pośrednictwem przeglądarki głosowej lub tekstowej są równoważne informacjom dostępnym za pośrednictwem przeglądarki GUI?
  2. czy informacje czytane sekwencyjnie są przedstawiane w logicznym (znaczącym) porządku?
3. Użyj dwóch ogólnych narzędzi oceny dostępności i odnotuj wszelkie problemy wskazane przez te narzędzia.
5. Podsumuj rezultaty
  1. Podsumuj rodzaje napotkanych problemów, jak również najlepsze praktyki, które powinny być zastosowane lub rozwinięte na witrynie.
  2. Wskaż metody, za pomocą których zidentyfikowano problemy i wyraźnie oświadcz, że nie była to pełna ocena zgodności.
  3. Zarekomenduj kroki, jakie należy podjąć, w tym pełną ocenę zgodności, która obejmie walidację kodu i inne testy oraz sposoby rozwiązania wszelkich zidentyfikowanych problemów.


## 3. Ocena zgodności z WCAG 1.0
Wszechstronna ocena jest połączeniem wielu metod testowania aspektów dostępności: półautomatycznych, ręcznych oraz testów z udziałem użytkowników z niepełnosprawnościami. Przeprowadzenie kompleksowej oceny wymaga znajomości używanych w Internecie języków znaczników; uprzedniego pobrania oprogramowania i/lub szkolenia w zakresie różnych narzędzi i podejść do oceny, konfiguracji ustawień przeglądarki oraz koordynacji z przeprowadzającymi testy z użytkownikami reprezentującymi różne niepełnosprawności. Ocena z użytkownikami jest ważna, ponieważ pomaga identyfikować problemy w stosowaniu technologii wspomagających.

Prawidłowo przeprowadzona kompleksowa ocena może zidentyfikować potencjalnie poważne problemy na etapie rozwoju nowej witryny; określić jaki witryna ma poziom zgodności z WCAG; i/lub zapewnić, że utrzyma go w przyszłości.

Wszechstronna ocena obejmuje wszystkie poniższe kroki z wyjątkiem tych, które w wyraźny sposób określone są jako opcjonalne.
(**Uwaga**: podczas identyfikowania wybór stron jest pierwszym krokiem, a podsumowanie i raportowanie rezultatów sprawdzenia jest logiczną konkluzją, kolejność etapów następujących pomiędzy nimi nie ma znaczenia).

1. Określ i opisz zakres, w jakim witryna ma być sprawdzona i docelowy poziom zgodności

  (**Uwaga**: informacja ta jest do użytku wewnętrznego na czas testów; jeśli zgodność jest deklarowana publicznie, powinno się ją publicznie ogłosić (np. na witrynie)):

  1. określ i zadeklaruj docelowy stopień zgodności z WCAG 1.0.
  2. określ i zadeklaruj taki wybór stron do testowania ręcznego i z udziałem użytkownika, taki, aby zawierał przynajmniej jedną z każdego typu stron witryny, i wszystkie strony, na które użytkownicy najprawdopodobniej trafią.
  
  **Uwaga**: w specyficzny sposób należy potraktować strony z zawartością dynamicznie generowaną przy pomocy bazy danych

  3. określ i zadeklaruj całą witrynę, włączając w to wszystkie strony na bazowym URL do automatycznej i półautomatycznej oceny;
  
  **Uwaga**: jeśli sprawdzenie całej strony jest niewykonalne (np. ze względu na jej duży rozmiar lub dynamiczny charakter), określ rozszerzony wybór stron, należy to w wyraźny sposób wyjaśnić i zdeklarować na witrynie. Ten poszerzony wybór stron powinien zawierać: strony z różnych części witryny, strony reprezentujące odmienny wygląd; strony reprezentujące różne narzędzia i procesy programistyczne, w tym narzędzia generowane z baz danych; strony stworzone według różnych wytycznych; strony „skontaktuj się z nami”; strony kluczowe dla Twojej firmy; itp. Jeśli jakikolwiek obszar witryny jest wykluczony z oceny, należy ujawnić te informacje.

2. Półautomatyczna i automatyczna ocena
  1. Sprawdź poprawność kodu, włączając w to składnię i arkusze stylów, przy użyciu wszystkich odpowiednich walidatorów na wybranych stronach. Uruchom przynajmniej jedno narzędzie sprawdzające kompleksowo całą witrynę
   - HTML Validation service
   - HTML Tidy Online
   - CSS Validation service
   - MathML Validator
  2. Użyj przynajmniej dwóch narzędzi oceny dostępności na wybranych stronach i przynajmniej jednego na całej witrynie. Wynotuj wszystkie problemy odnalezione przez narzędzia. Lista narzędzi jest dostępna na Web Accessibility Evaluation Tools List.
3. Ocena ręczna
  1. Przetestuj wybrane strony, używając odpowiednich punktów kontrolnych z Listy punktów kontrolnych dotyczących Web Content Accessibility Guidelines 1.0. **Uwaga**: Odpowiednich może oznaczać: punkty kontrolne, których nie można ocenić za pomocą narzędzi automatycznych lub półautomatycznych; punkty kontrolne, które faktycznie dotyczą witryny (np. jeśli witryna nie zawiera treści audio, pomiń je); oraz, jako minimum, te punkty kontrolne, które odnoszą się do poziomu zgodności, który oceniasz.
  2. Przetestuj wybrane strony za pomocą przeglądarek posiadających graficzny interfejs użytkownika (GUI); wybierz co najmniej trzy różne konfiguracje spośród następujących zmiennych: różne przeglądarki GUI (Internet Explorer, Netscape, Opera), w różnych wersjach (najnowsze, starsze), na różnych platformach (Windows. Linux, Mac) i mające następujące ustawienia (**Uwaga**: dla niepełnosprawnych testerów niektóre kroki muszą być zrobione z inną osobą, która nie ma tej niepełnosprawności.):
    1. wyłącz obrazy i sprawdź, czy dostępny jest adekwatny tekst alternatywny.
    2. wyłącz dźwięk i upewnij się, że zawartość audio jest nadal dostępna w formie tekstowych odpowiedników.
    3. użyj kontrolek przeglądarki do zmiany wielkości czcionki: sprawdź, czy rozmiar czcionki zmienia się odpowiednio na ekranie i czy przy większych rozmiarach czcionki strona jest nadal funkcjonalna.
    4. przetestuj z różnymi rozdzielczościami ekranu, i/lub zmieniając rozmiar okna aplikacji do mniejszego od maksymalnego, upewnij się, czy nie jest wymagane przewijanie w poziomie (**Uwaga**: przetestuj z różnymi przeglądarkami lub sprawdź kod dla rozmiaru bezwzględnego, aby upewnić się, że jest to problem zawartości, a nie problem z przeglądarką)
    5. zmień kolor wyświetlania na skalę szarości (albo obejrzyj stronę na wydruku czarno-białym lub w skali szarości) i sprawdź, czy kontrast kolorów jest wystarczający.
    6. bez użycia myszy przemieszczaj się pomiędzy odsyłaczami i polami formularza, upewniając się, że możesz uzyskać dostęp do wszystkich odsyłaczy i pól formularza oraz że linki wyraźnie wskazują, do czego prowadzą.
    7. sprawdź również stronę z niezaładowanymi skryptami, arkuszami stylów i apletami.
  3. Sprawdź wybrane strony z jedną przeglądarką tekstową (taką jak Lynx) ORAZ jedną przeglądarką głosową (taką jak Home Page Reader), i odpowiedz na następujące pytania:
    1. Z przeglądarką tekstową
       1. czy informacje lub funkcja dostępne za pośrednictwem przeglądarki tekstowej są równoważne informacjom dostępnym za pośrednictwem przeglądarki GUI?
       2. czy informacje czytane sekwencyjnie są przedstawiane w logicznym (znaczącym) porządku?
    2. Z przeglądarką głosową
       (**Uwaga**: W przypadku ustawień, w których istnieje ograniczony wybór technologii wspomagających, należy również przeprowadzić ręczną ocenę witryny, używając tych technologii wspomagających; na przykład JAWS jest jedynym czytnikiem ekranu przetłumaczonym na język duński, dlatego w Danii audytor powinien ocenić witrynę za pomocą JAWS.)
       - czy informacje lub funkcja dostępne za pośrednictwem przeglądarki głosowej są równoważne informacjom dostępnym za pośrednictwem przeglądarki GUI?
       - czy informacje czytane sekwencyjnie są przedstawiane w logicznym (znaczącym) porządku?
  4. Przejrzyj jeszcze raz tekst strony: czy jasny i prosty w stopniu odpowiednim dla celów strony internetowej? (W przypadku stron internetowych w języku angielskim należy rozważyć zastosowanie testu Clear and Appropriate Language and Design (CLAD).)
  [**Uwaga**: to pytanie należy również zadać ludziom biorącym udział w testach użyteczności funkcji dostępności].

3. Testowanie funkcjonalności ułatwień dostępu
   - Osoby z różnymi rodzajami niepełnosprawności, różnymi poziomami wiedzy technicznej i różnymi stopniami znajomości strony, korzystające z różnych technologii wspomagających i strategii adaptacyjnych, dokonują przeglądu wybranych stron i swobodnie nawigują na całej witrynie
   [**Uwaga**: Czasem jest to możliwe w warunkach laboratoryjnych, ale cenne może się okazać możliwość sprawdzenia witryny w środowisku typowym dla użytkowników. Różne poziomy doświadczenia technicznego użytkownika i znajomość strony są ważne i należy pamiętać, że będą się one zmieniać w miarę upływu czasu, w miarę jak ludzie biorą udział w przeglądaniu strony.]
   - Poproś testerów, aby spróbowali znaleźć odpowiedzi na najczęściej zadawane pytania, jakie mogą zadawać odwiedzający witrynę. Określ obszary, gdzie używanie witryny jest trudne lub niemożliwe.
4. Podsumowanie i późniejsze działania
   1. Podsumuj wszystkie napotkane problemy i najlepsze praktyki zidentyfikowane dla każdego typu stron oraz reprezentatywnego adresu URL, a także metody, za pomocą której zostały one zidentyfikowane.
   2. Zaleć kroki, jakie należy podjąć, potencjalnie włączając:
      - usunięcie barier dostępności zidentyfikowanych w procesie oceny zgodności.
      **Uwaga**: jeśli sprawdzenie dotyczyło „rozszerzonego wyboru stron” zamiast „całej witryny”, zastosuj to, czego nauczyłeś się na innych stronach
      - rozszerzenie najlepszych praktyk na witrynie
      - bieżące utrzymanie i monitoring witryny

## 4. Uwagi dotyczące specyficznych sytuacji

### Ocena w trakcie procesu rozwoju
Sprawdzanie w czasie rozwoju witryny ma zasadnicze znaczenie. Może czasem być trudne, ponieważ zatrudnieni w domu i pracujący na zlecenie twórcy internetowi czasami wolą ustalić wygląd strony i zademonstrować swoje możliwości/potencjał, zanim otrzymają zalecenia. Jednakże zagadnienia dostępności zidentyfikowane odpowiednio wcześnie są łatwiejsze do naprawienia i uniknięcia. Efektywne sprawdzanie podczas etapu projektowania może zawierać:

- ustalenie przejrzystych wymagań dotyczących oczekiwanego poziomu zgodności w zakresie dostępności
- współudział w spotkaniach roboczych mających na celu opracowanie planu witryny
- uzgodnienie harmonogramu przeglądu w trakcie procesu projektowania/tworzenia witryny
- udostępnienie informacji o metodyce oceniania tak, żeby programiści mogli przeprowadzić samodzielnie przynajmniej wstępne przeglądy

### Bieżące monitorowanie
Żeby zmaksymalizować prawdopodobieństwo, że witryna utrzyma dany stopień zgodności także w przyszłości, należy przedsięwziąć następujące kroki:

- jasne określenie oczekiwanego poziomu zgodności i zakresu witryny, którego on dotyczy,
- wyraźne wyznaczenie osób odpowiedzialnych za monitorowanie witryny oraz określenie procedur, jakie należy zastosować w celu szybkiego naprawienia stron niezgodnych z wymogami,
- jasne określenie oczekiwań co do częstotliwości, metod i zakresu oceny,
- przeprowadzenie walidacji i oceny wszystkich zmienionych stron i nowych typów, zanim zostaną dodane do witryny,
- oprogramowanie ułatwiające ocenę,
- publikowanie adresu kontaktowego w celu uzyskania informacji zwrotnej na temat dostępności witryny
- automatyczne lub półautomatyczne testy mające na celu identyfikację problemów, jakie napotkano podczas wszechstronnego przeglądu,
  
  **Uwaga**: Pełna ocena zgodności nie jest koniecznie wymagana podczas każdego okresowego przeglądu. Kroki takie jak ponowne testowanie przez użytkownika mogą być wymagane tylko po wprowadzeniu istotnych zmian w szablonie lub treści.

### Ocena starszych witryn
Czasem witryny, które są „zamrożone” (stare; które nie są już aktywnie utrzymywane) mają poważne problemy z dostępnością. Trudno jest określić, w jaki sposób można się z nimi uporać. Pomóc w tym może:

   - określenie, kto jest aktualnym właścicielem;
   - ustalenie, czy istnieje jakikolwiek interes lub obowiązek w uczynieniu strony dostępną,
   - po sprawdzeniu strony; zarysuj właścicielowi zmiany, które byłyby wymagane, aby przystosować stronę do wymogów dostępności
   - rozpoznanie i szacunkowe przedstawienie, jakie środki będą niezbędne i ile czasu mogą zająć poszczególne etapy w procesie przebudowy witryny
   - publicznie ujawnienie problemów dostępności odnalezionych na witrynie.

### Sprawdzanie dynamicznie generowanych stron
Strony generowane dynamicznie składają się zwykle z jednego lub większej liczby szablonów, które zapewniają wspólne funkcje układu i narzędzia nawigacji oraz zawartość dostarczaną automatycznie z bazy danych lub innego systemu zarządzania treścią. Aby osiągnąć pełną zgodność z wymogami dostępności, należy ocenić zarówno dostępność szablonów, jak i wygenerowanej zawartości. Nie wystarczy ocenić tylko szablony: zawartość może także zawierać znaczniki lub może należy te znaczniki umieścić w celu zapewnienia dostępności. Powinno się rozważyć:

1. Szablony
   - sprawdź wszystkie szablony
   - jeśli szablony są generowane przez oprogramowanie do tworzenia stron, sprawdź zdolność tego oprogramowania w zakresie stosowania ułatwień dostępności (zobacz Selecting Web Accessibility Evaluation Tools, np.:
   - czy wygenerowany z szablonu porządek tabulacji pozwala na efektywne dostanie się do wygenerowanego tekstu?
2. Zawartość
   - jeśli cała dynamiczna zawartość nie może być sprawdzona, wygeneruj szeroki, reprezentatywny zakres próbki, zapisz zawartość i przetestuj ją;
   - sprawdź możliwości systemu zarządzania zawartością w zakresie przechowywania i generowania informacji w sposób spełniający wymogi dostępności (zobacz [Selecting Authoring Tools]);
   - czy obrazy są wzbogacone tekstami alternatywnymi, a jeśli jest to potrzebne także longdesc?
   - czy wygenerowane tabele danych posiadają ułatwienia dostępności (np. podpisy, id w <th>, komórki nagłówków, itp.)?
   - jeśli jest wygenerowane wideo, czy ma napisy?
   - jeśli wygenerowana jest narracja audio, czy dostępny jest tekstowy odpowiednik?
2. Szablony i zawartość razem wzięte
   - dla stron, które są wygenerowane w rezultacie przeszukiwania bazy danych, źródło wygenerowane jako strona jest wyświetlone powinno być zapisane i przetestowane w narzędziu sprawdzającym -- [może wymagać interwencji operatora] ;