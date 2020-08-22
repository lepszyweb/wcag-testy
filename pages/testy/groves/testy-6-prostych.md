---
title: 6 prostych testów według Karla Grovesa
summary: "Te testy może przeprowadzić każdy, bez żadnej wiedzy na temat dostępności i wiedzy na temat projektowania stron."
sidebar: testy_sidebar
permalink: testy-6-prostych
folder: testy
toc: false
---


{% include callout.html content="Publikacja jest tłumaczeniem:<br/>**Źródło**: [Karl Groves: The 6 Simplest Web Accessibility Tests Anyone Can Do](https://karlgroves.com/2013/09/05/the-6-simplest-web-accessibility-tests-anyone-can-do), opublikowane 5 września 2013, tłumaczenie i publikacja za zgodą autora, Karla Grovesa - Stefan Wajda " type="success" %}

{% include callout.html content="**Od tłumacza**: Moim celem nie było wierne przetłumaczenie artykułu K. Grovesa, ale wierne zrealizowanie celu, któremu służył jego artykuł. Stąd drobne uzupełnienia w niektórych partiach, np. objaśniających, jak skonfigurować współczesne przeglądarki, aby wykonać test (Stefan Wajda)." type="primary" %}

## 6 najprostszych testów dostępności internetowej, które może wykonać każdy
A gdybym ci powiedział, że wydrukowana rekomendacja WCAG 2.0 W3C to 36 stron? Dodatkowo, „Jak spełnić WCAG 2.0” to 44 strony, a „Zrozumieć WCAG 2.0” to 230 stron. A do tego towarzyszące im „Techniki dla WCAG 2.0” to 780 stron druku. Istnieje około 400 technik i błędów. Wszystko to jest wspaniałym zbiorem informacji stworzonych przez jednych z najbardziej kompetentnych ludzi zajmujących się dostępnością. Niestety stanowi rodzaj bariery wejścia dla osób, które naprawdę chcą wiedzieć, co muszą zrobić, aby zwiększyć  dostępność. Ta bariera działa w obie strony: nie należy zakładać, że jest to łatwe. Nie można po prostu użyć przełącznika, by mieć dostępną stronę internetową. Aby w pełni zrozumieć dostępność i tworzenie dostępnych stron internetowych, wymagana jest dogłębna znajomość HTML, CSS, JavaScript, DOM (Obiektowy Model Dokumentu – Document Object Model) i BOM (Obiektowy Model Przeglądarki - Browser Object Model), interfejsów API dostępności, technologii asystujących oraz tego, jak osoby niepełnosprawne korzystają z komputerów. Poświęciłem temu swoją karierę i dowiaduję się, im więcej wiem, tym mniej rozumiem.

A co z tymi, dla których dostępność nie jest ich wyborem zawodowym? A co z tymi, którzy nie chcą wiedzieć takich rzeczy, jak skomplikowana interakcja między znacznikami, interfejsami DOM i mapowaniem ról API dostępności? Co z ludźmi, którzy chcą wiedzieć: Jak działa moja strona internetowa dla osób niepełnosprawnych?

Proszę bardzo. 6 testów, które każdy może wykonać bez żadnej wiedzy na temat projektowania.

### 1. Odłącz mysz i wyłącz panel dotykowy
Prawdopodobnie najszybszym i najłatwiejszym sposobem przetestowania dostępności witryny jest odłączenie myszy i  - w laptopie przykrycie lub wyłączenie panelu dotykowego. W naturalny sposób w takim przypadku będziesz zmuszony do interakcji ze stron wyłącznie za pomocą klawiatury.

**Proces testowania jest prosty**: Działaj na stronie – poruszaj się, uaktywniaj łącza i kontrolki tylko klawiaturą. Klawisz [Tab] pozwoli Ci przechodzić do przodu w kolejności tabulacji. Równoczesne naciskanie klawiszy [Shift] i [Tab] spowoduje przechodzenie w kolejności tabulacji do tyłu. Naciśnięcie [Enter] spowoduje przejście do miejsc wskazywanych  przez łącza. Naciśnięcie spacji uaktywnia przyciski. Gdy znajdziesz się wewnątrz złożonego komponentu strony, np. menu rozwijanego, rozwijanej harmonijki ukrywającej treści, kalendarzyka wydarzeń, powinno być możliwe przemieszczanie się między pozycjami w tym komponencie za pomocą strzałek w lewo, w prawo, w dół, w górę.

- Czy możesz obsłużyć wszystkie elementy sterujące, łącza i menu za pomocą samej klawiatury?
- Czy widzisz w każdym momencie, na którym elemencie strony znajduje się punkt uwagi (wskaźnik fokusu)?  
- Czy kolejność przenoszenia fokusu jest zgodna z logiczna kolejnością interakcji?
- Czy fokus pozostaje w punkcie, do którego został przeniesiony, nie powodując zmiany kontekstu?

Jeśli nie możesz odpowiedzieć „Tak” na wszystkie powyższe pytania, wówczas strona wymaga naprawy, aby była dostępna.

#### Jakie to ma znaczenie?
Duża liczba osób z niepełnosprawnościami nie może używać myszy w pracy z komputerem.
Użytkownicy niewidomi nie widzą wskaźnika myszy. Użytkownicy słabowidzący mogą preferować klawiaturę. Użytkownicy z zaburzeniami motoryki mogą nie być w stanie używać myszy, a dla osób z chronicznym bólem korzystanie z myszy może być bolesne.
Dostępność z klawiatury jest wymagana dla użytkowników niewidomych, słabowidzących lub z zaburzeniami motoryki. Należy pamiętać: widoczność wskaźnika fokusu jest szczególnie ważne dla ogólnej użyteczności, a krytyczna dla użytkowników słabowidzących lub cierpiących na zaburzenia motoryki. Nie wszyscy użytkownicy niepełnosprawni są niewidomi!

### 2. Włącz tryb wysokiego kontrastu
W systemie operacyjnym Windows, tryb wysokiego kontrastu umożliwia użytkownikom o słabym wzroku, użytkownikom wrażliwym na światło (światłowstręt), a czasem także użytkownikom z dysleksją w wygodny sposób poprawić zdolności skutecznego korzystania z komputera. Tryb wysokiego kontrastu w systemie Windows zmienia kolory pierwszego planu i tła, aby uzyskać wyższy kontrast. Kolory na stronie internetowej są zasadniczo całkowicie usuwane. Całe tło jest czarne, a cały tekst na pierwszym planie ma znacznie jaśniejszy kolor, taki jak biały lub żółty (użytkownicy mogą go dostosować).

Włącz tryb wysokiego kontrastu w Windows (Alt + lewy Shift + Print) i zbadaj:

- Czy na stronie widoczne jest wszystko, co było widoczne w zwykłym trybie?
- Czy potrafisz odróżnić łącza, przyciski i inne elementy interaktywne?
- Czy ważne informacje przekazywane za pomocą obrazów są nadal widoczne?

Następnie sprawdź dokładniej:

- Czy na stronie były obrazy w tle, które już nie są widoczne? Czy były to obrazy wyłącznie dekoracyjne, czy też  przekazywały informacje lub służyły celom instruktażowym lub jako kontrolki (np. łącza, przyciski)?
- Co dzieje się z innymi obrazami? Co z obrazami zawierającymi tekst? Czy obrazy też zmieniły kolory? Jeśli ich kolory się zmieniły, czy są czytelne, z odpowiednim kontrastem? Jeśli ich kolory nie zmieniły się, czy osoby  potrzebujące wysokiego kontrastu, z łatwością zrozumieją treść obrazów?

Jeśli okaże się, że ważne informacje zostaną ukryte albo będą nieczytelne lub trudne do rozróżnienia i odczytania, jeśli jakieś elementy sterujące (interaktywne) nie będą już widoczne lub zrozumiałe albo po włączeniu trybu wysokiego kontrastu wizualna reprezentacja strony w ogóle nie zostanie zmieniona, to najprawdopodobniej spora grupa osób z niepełnosprawnością wzrokową i z problemami poznawczymi nie będą mogli skutecznie korzystać ze strony, strona wymaga poprawy dostępności.

#### Jakie to ma znaczenie?
Nie ma wiarygodnych badań, które mówią, jak duża grupa osób potrzebuje trybu wysokiego kontrastu i korzysta z niego. W odpowiedzi na ankietę przeprowadzoną swego czasu przez WebAIM 30% użytkowników słabowidzących twierdzi, że korzystało z trybów wysokiego kontrastu. Osób słabowidzących, z różnymi schorzeniami wzroku, dla których tryb wysokiego kontrastu może podnosić komfort korzystania ze strony albo być niezbędny, jest znacznie więcej niż osób całkowicie niewidomych. Jeśli więc Twoja strategia dostępności opiera się na założeniu, że wystarczy zapewnić dobre działanie witryny z czytnikami ekranu,  zrewiduj swoje podejście.
Więcej informacji o trybie wysokiego kontrastu znajdziesz w artykułach:

- [Michał Dębiec: W krainie dużego kontrastu](http://www.moimioczami.pl/2012/02/w-krainie-duzego-kontrastu/)
- [Give yourself an accessibility test: turn on high contrast](https://www.boia.org/blog/give-yourself-an-accessibility-test-turn-on-high-contrast)
- [Terril Thompson: Windows High Contrast and Background Images](https://terrillthompson.com/182)

### 3. Wyłącz obrazy
Aby wyłączyć obrazy w programie Chrome przejdź do **Ustawienia > Zaawansowane  > Prywatność i bezpieczeństwo > Ustawienia witryn > Grafika**, a następnie odznacz opcję **Pokaż wszystkie (zalecane)**.

W programie Firefox  opcja wyłączania grafiki jest ukryta. Wpisz najpierw w pasku adresu przeglądarki **about:config**, następnie odszukaj ustawienie **permissions.default.image** i naciśnij Enter lub kliknij dwukrotnie, aby zmienić wartość w polu Wartość z 1 na 0.

Przeglądaj stronę z wyłączonymi obrazami.

- Czy treść ma sens?
- Czy treść jest nadal zrozumiała?
- Czy wszystkie istniejące wcześniej informacje są widoczne?
- Czy widoczne są wszystkie elementy interaktywne – łącza, przyciski i inne?

#### Jakie to ma znaczenie?
Obrazy są dobre zarówno dla użyteczności, jak i dostępności. Duże korzyści z połączenia obrazów i tekstu mogą odnieść zwłaszcza użytkownicy z zaburzeniami funkcji poznawczych. Ale generalnie obrazy wszystkim mogą pomóc w zrozumieniu informacji.

Mimo tego obrazy nie powinny być wymagane do zrozumienia treści strony i nie należy na nich polegać w przypadku istotnych elementów kontrolnych interfejsu użytkownika. Każdy tekst prezentowany na obrazach powinien być umieszczony w znaczniku, z wyjątkiem treści markowych, takich jak logo lub znaki towarowe Wszelkie obrazy przedstawiające ważną treść powinny otrzymać tekstową alternatywę, a niektóre obrazy najlepiej opisać bezpośrednio w treści strony.

Wszystkie obrazy przedstawiające ważną treść powinny otrzymać tekst alternatywny, a niektóre obrazy najlepiej opisać bezpośrednio w treści strony. Termin „opis alternatywny” oznacza przekazanie takich samych informacji, jakie niesie obraz, a nie wyglądu obrazu, choć niekiedy opis pewnych aspektów wyglądu również może mieć znaczenie. Teksty prezentowane na obrazach należy umieszczać w opisach alternatywnych (z wyjątkiem treści odnoszących się do marki, takich jak logo lub znaki towarowe).

### 4. Sprawdź napisy lub transkrypcje
OK, skłamałem, który z tych testów był najłatwiejszy. Ten jest łatwiejszy niż wszystkie inne. Jeśli masz na swojej witrynie multimedia, sprawdź napisy, transkrypcje i inne możliwe alternatywy. Gdziekolwiek masz media:

- Czy napisy znajdują się bezpośrednio na filmie lub czy w odtwarzaczu jest kontrolka, która włącza i wyłącza napisy?
- Czy w odtwarzaczu istnieje alternatywna wersja z opisem dźwiękowym (audiodeskrypcją) lub kontrolka, która włącza i wyłącza opis dźwiękowy?
- Czy w przypadku filmów z dużą ilością dialogów w pobliżu w pobliżu odtwarzacza wideo znajduje się transkrypcja tekstu lub link, który prowadzi do transkrypcji?

Prócz wymienionych powyżej istnieją inne wymagania odnoszące się do publikacji treści multimedialnych, w tym wideo bez dźwięku oraz nagrań dźwiękowych (tylko dźwięk), ale powyższe dotyczą większości  multimediów w większości witryn.

#### Jakie to ma znaczenie?
Łatwo jest przyjąć, że dostępność mediów ma wpływ tylko na użytkowników niewidomych i niesłyszących, ale w rzeczywistości dostępne alternatywy medialne przynoszą korzyści również użytkownikom słabowidzącym, niedosłyszącym i użytkownikom z zaburzeniami poznawczymi.

Transkrypcja tekstu jest dobra dla SEO, a także dla użytkowników, którzy chcą wyszukiwać określony fragment treści w mediach.

{% include note.html content="Uwaga: Nie tylko treść multimedialna powinna być dostępna, ale także odtwarzacz. " %}


### 5. Kliknij etykiety pól w formularzach
Formularze są najlepszą metodą interakcji ze stronami internetowymi i najlepszą metodą pomiaru konwersji. Niestety, problemy związane z dostępnością formularzy należą do najczęstszych.

Problemy z formularzami dzielą się na trzy główne kategorie: brakujące lub niekompletne etykiety, nieefektywna obsługa błędów i słaba widoczność fokusu. Jednym z najprostszych sposobów sprawdzenia istnienia etykiet formularzy jest po prostu kliknięcie etykiety tekstowej przylegającej do pola.

- Czy po kliknięciu etykiety obok pola kursor wchodzi w pole?
- Czy kliknięcie etykiety obok przycisku opcji lub pola wyboru zaznacza się opcja sąsiadująca z etykietą?
- Czy po kliknięciu etykiety obok elementu SELECT, fokus ustawia się na elemencie listy wyboru?

#### Jakie to ma znaczenie?
Między etykietą a powiązaną z nim kontrolką (polem, listą wyboru, opcjami) powinien istnieć bezpośredni związek zdefiniowany programowo. Ten prosty test pozwala sprawdzić, czy taki związek istnieje, bez badania kodu źródłowego. Może go wykonać każdy. Nieoznakowanie lub nieprawidłowe oznakowanie kontrolek musi być naprawione.
Rozważając dostępność formularzy, trzeba wziąć pod uwagę o wiele więcej kwestii, ale ten szybki test pozwala przynajmniej  stwierdzić, czy spełniony jest podstawowy warunek dostępności: właściwe etykietowanie formularzy. Bez poprawnego oznakowania pól formularzy żadna z pozostałych dobrych praktyk nie ma znaczenia.

### 6. Wyłącz CSS
Kaskadowe arkusze stylów są preferowaną metodą formowania układu graficznego i wizualnej prezentacji internetowych interfejsów użytkownika. Z punktu widzenia dostępności jest kilka kwestii, na które należy zwrócić uwagę.   

Jak wyłączyć CSS? Najprościej w przeglądarce Firefox. Otwórz menu (**Alt + P**), wybierz opcję **Widok > Styl strony -> Ignoruj style**. Podobnie w Internet Explorer. Użyj skrótu **Alt + P**, aby otworzyć pasek menu, następnie wybierz opcję **Widok > Styl strony > Brak stylu**. W ustawieniach Chrome nie ma możliwości wyłączenia stylów. Aby je wyłączać, zainstaluj dodatek Web Developer Tools. W pasku narzędziowym wybierz kartę CSS i zaznacz opcję **Disable All Styles** (Wyłącz wszystkie style).  

Po wyłączeniu stylów sprawdź:

- Czy zniknęły jakiekolwiek ważne treści, łącza, ikony lub inne elementy sterujące?
- Czy trudniej jest teraz zrozumieć takie elementy, jak komunikaty o błędach lub inne wcześniej wyraźnie widoczne wskazówki wizualne?
- Czy treść jest nadal wyświetlana w rozsądnej i łatwej do zrozumienia kolejności?
- Czy pozostaje jakikolwiek kolor, w tym kolor tła? (poza domyślnym niebieskim kolorem łączy nieodwiedzonych i filetowym łączy odwiedzonych)
- Czy pozostają jakieś style prezentacji tekstu?

#### Jakie to ma znaczenie?
Wyłączenie stylów CSS może obnażyć kilka istotnych problemów dostępności.

Po pierwsze, problemów z wykorzystaniem obrazów tła. Wyłączenie CSS powoduje m.in. wyłączenie obrazów tła. Jeśli w efekcie po wyłączeniu CSS znikają jakieś elementy sterujące, czy nawet treści (np. nagłówki), należy to naprawić.

Po drugie, problemów ze stosowaniem przestarzałych rozwiązań prezentacyjnego HTML. Jeśli po wyłączeniu stylów na stronie pozostaje jakiekolwiek formatowanie wizualne, również powinno to być naprawione, bo nie może być zastąpione przez użytkowników, którzy stworzyli własne style. Według ankiety przeprowadzonej przez WebAIM  19% użytkowników słabowidzących przegląda strony internetowe z „dostosowanymi kolorami stron lub niestandardowymi arkuszami stylów”.

{% include links.html %}
