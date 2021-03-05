---
title: Dostęp do klawiatury i widoczny fokus
tags: nawigacja

sidebar: testy_sidebar

permalink: 06-P-klawiatura
folder: testy/latwe
---

## Dostęp do klawiatury i widoczny fokus

Wiele osób nie może korzystać z myszy i w&nbsp;interakcjach z&nbsp;internetem musi polegać na klawiaturze.

Osoby niewidome i&nbsp;słabowidzące, a&nbsp;także osoby z&nbsp;ograniczonymi możliwościami ruchu i&nbsp;manipulacji oraz osoby, które nie mogą korzystać z&nbsp;innych urządzeń wskazujących takich, jak mysz czy dotyk, polegają na klawiaturze lub technologiach wspomagających i&nbsp;strategiach adaptacyjnych, które opierają się na poleceniach klawiaturowych wprowadzanych za pomocą skrótów klawiaturowych lub poleceń głosowych.

Dla takich osób strony są dostępne tylko wówczas, gdy umożliwiają przeglądanie wszystkich treści i obsługę wszystkich funkcji – łączy, formularzy, odtwarzaczy mediów itp. – za pomocą klawiatury. Takie osoby mogą, ale nie muszą korzystać z&nbsp;technologii wspomagających, takich jak czytniki ekranu.

Dla osób słabowidzących niezbędna jest również widoczność wskaźnika fokusu, czyli oznaczenia miejsca, które aktualnie oczekuje na sygnały wprowadzane przez użytkownika za pomocą klawiatury (naciśnięcia klawiszy). Fokus pokazuje, na którym elemencie w&nbsp;danej chwili w&nbsp;programie użytkownika skupiona jest uwaga odbiornika sygnałów z&nbsp;klawiatury, czyli który z&nbsp;interaktywnych elementów strony jest aktualnie wybrany i&nbsp;gotowy, by wykonać działanie żądane przez użytkownika.

Widoczny wskaźnik fokusu zapewnia, że użytkownicy klawiatury mogą się w&nbsp;każdym momencie zorientować, w&nbsp;którym miejscu strony się znajdują. Wyraźne wskaźniki fokusu są szczególnie ważne dla osób słabowidzących oraz dla osób z&nbsp;problemami poznawczymi, z&nbsp;trudnościami koncentracji uwagi, bo pozwalają im na takie same możliwości orientowania się na stronie, jakie mają osoby korzystające z&nbsp;urządzeń wskazujących.

Podczas nawigacji klawiaturą po stronie, nazywanej nawigacją sekwencyjną, fokus powinien się przemieszczać sensownie zgodnie z&nbsp;logiczną kolejnością elementów strony.

Aby zapewnić widoczność fokusu, twórcy stron mogą posłużyć się różnymi wskaźnikami, np. obramowaniem lub podkreśleniem elementu, który uzyskał fokus, odwróceniem (inwersją) kolorów elementu – wyświetleniem jasnego tekstu na ciemnym tle lub odwrotnie. W&nbsp;polach formularzy domyślnym wskaźnikiem fokusu jest migający kursor. Autorzy stron są zachęcani, by wzmocnić widoczność fokusu, który jest użyteczny dla wszystkich, a&nbsp;niezbędny dla osób z&nbsp;niepełnosprawnościami wzroku i&nbsp;ruchu.  


![Kontur wokół środkowego łacza](images/andi/06_P_fokus-linki.png)

Rysunek 1. Zwróć uwagę na kontur wokół środkowego łącza

![Przycisk bez fokusu po lewej stronie i z fokusem po prawej stronie. Zastosowano inwersję kolorów](images/andi/06_P_fokus-przycisk.png)

Rysunek 2. Porównaj ten sam przycisk bez fokusu (po prawej – fioletowy napis na białym obramowanym tle) i&nbsp;z&nbsp;fokusem (po prawej – biały napis na fioletowym tle i&nbsp;obramowanie).


### Co robić
W przeglądarkach, która obsługują nawigację za pomocą klawiatury za pomocą klawisza <kbd>Tab</kbd> (na przykład, Firefox, IE, Chrome i Safari):
-	W systemie Mac trzeba włączyć nawigację za pomocą klawiatury. W tym celu:
	- W nowszych przeglądarkach: wybierz **Preferencje systemowe > Klawiatura > Skróty**, a następnie wybierz przycisk opcji **Wszystkie elementy sterujące**.
	- W starszych przeglądarkach: wybierz **Preferencje systemowe > Klawiatura > Skróty klawiaturowe**, a następnie w sekcji **Pełny dostęp z klawiatury** zaznacz **Wszystkie kontrolki**.
-	Kliknij w pasku adresu, a następnie odłóż na bok mysz i nie używaj jej podczas testowania.
-	Naciskaj na klawiaturze klawisz <kbd>Tab</kbd>, aby przejść przez elementy na stronie. Można naciskać kombinację klawiszy <kbd>Shift+Tab</kbd>, aby poruszać się do tyłu.
-	Aby poruszać się w obrębie elementów, takich jak listy rozwijane, paski menu, harmonijki, naciskaj klawisze strzałek.
-	Aby wybrać konkretną pozycję w obrębie listy rozwijanej:
	- Przejdź klawiszem <kbd>Tab</kbd> do listy rozwijanej,
	- za pomocą klawiszy strzałek przenoś fokus między elementami listy,
	- naciśnij <kbd>Enter</kbd>, gdy fokus znajdzie się na elemencie, który chcesz wybrać.

### Co sprawdzać
-	**Tab do wszystkich**: Sprawdź, czy klawiszem <kbd>Tab</kbd> można dotrzeć do wszystkich interaktywnych elementów na stronie, w tym łączy, pól formularzy, przycisków i&nbsp;pokręteł odtwarzacza multimedialnego. (Częstym problemem jest to, że nie można dotrzeć tabulatorem do elementów sterujących odtwarzacza multimedialnego.)
-	**Tab ze wszystkich**: Sprawdź, czy za pomocą klawisza <kbd>Tab</kbd> można wyjść ze wszystkich elementów, do których można było przenieść fokus. (Częstym problemem jest zatrzymanie fokusu klawiatury przez kontrolki mediów albo utknięcie wewnątrz innego elementu osadzonego na stronie, np. mapie tak, że nie można się z nich wydostać bez użycia myszki. Nazywa się to „pułapką na klawiaturę”).
-	**Kolejność tabulacji**: Sprawdź, czy kolejność przemieszczania  następuje w&nbsp;logicznej kolejności czytania (np. od lewej do prawej, w&nbsp;przypadku języków, w&nbsp;których obowiązuje taki kierunek pisania,  z&nbsp;góry na dół).
-	**Widoczny fokus**: Sprawdź, czy fokus jest wyraźnie widoczny, gdy przemieszczasz się przez kolejne elementy, to znaczy, czy w każdym momencie umiesz powiedzieć, w którym miejscu znajduje się fokus, np. że łącze uzyskało dodatkowe wyróżnienie (uwaga, zniknięcie podkreślenia nie jest dodatkowym wyróżnieniem!), że przycisk zmienił kolorystykę, że wokół pola  formularza pojawił się obrys. Uwaga: Nie wszystkie elementy muszą uzyskiwać taki sam wskaźnik fokusu, ale wszystkie elementy pełniące podobne funkcje powinny być oznaczane fokusem w podobny sposób.
-	**Obsługa wszystkich funkcji klawiaturą**: Sprawdź, czy za pomocą klawiatury można zrobić wszystko, to znaczy, że nie potrzebujesz myszy, aby aktywować akcje, opcje, widoczne zmiany i inne funkcje. (Częstym problemem jest to, że niektóre funkcje są dostępne tylko przy najechaniu myszą i nie można ich aktywować  klawiaturą).
-	**Rozwijane listy**: Sprawdź, czy po przejściu tabulatorem do listy rozwijanej, można użyć klawiszy strzałek, aby przejść przez wszystkie opcje bez wywołania działania. (Częstym problemem w przypadku list rozwijanych używanych do nawigacji jest to, że gdy tylko strzałka przeniesie fokus na następną pozycję, to ta pozycja zostaje automatycznie wybrana i nie można już przejść do innych pozycji na liście albo następuje przekierowanie na inną stronę lub w inne miejsce strony.)
-	**Łącza graficzne**: Sprawdź, czy obrazy, które są łączami, mają wyraźnie widoczny fokus i czy możesz wywołać każde łącze klawiaturą (naciskając <kbd>Enter</kbd>).

### Sprawdzenie widoczności fokusu na stronie demo PrzediPo  
Otwórz dostępną wersję strony [Ankieta](https://przedipo.lepszyweb.pl/after/survey.html).
Przejdź przez wszystkie elementy strony klawiszem <kbd>Tab</kbd>, a w obrębie złożonej grupy elementów poruszaj się strzałkami. Zwróć uwagę,
-	że wiele elementów w chwili uzyskania fokusu otrzymuje zielone tło
-	że niektóre  elementy w chwili uzyskania fokusu są obrysowane przerywaną linią
-	że przyciski opcji są otaczane przerywanym obrysem i przenoszone jest do nich zaznaczenie (kropka)
-	że między opcjami w grupie opcji można się poruszać strzałkami
-	że pozycje na liście rozwijanej można wybierać strzałkami.   

### Dowiedz się więcej o dostępie za pomocą klawiatury  
-	[Funkcjonalność jest dostępna z klawiatury](http://www.w3.org/WAI/intro/people-use-web/principles#keyboard) - sekcja w Accessibility Principles; artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Przeglądanie stron internetowych za pomocą klawiatury](http://www.w3.org/WAI/users/browsing#keyboard) - sekcja na stronie Better Web Browsing: Tips for Customizing Your Computer; artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć Wytyczną 2.1 Dostępność z klawiatury](https://www.w3.org/WAI/WCAG21/Understanding/keyboard-accessible); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
	- [Zrozumieć Kryterium sukcesu 2.1.1 Klawiatura](https://www.w3.org/WAI/WCAG21/Understanding/keyboard.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
	- [Zrozumieć Kryterium sukcesu 2.1.2 Bez pułapki na klawiaturę](https://www.w3.org/WAI/WCAG21/Understanding/no-keyboard-trap.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć Sukces Kryterium 2.4.3 Kolejność zaznaczania](https://www.w3.org/WAI/WCAG21/Understanding/focus-order.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć Kryterium sukcesu 2.4.7 Widoczny fokus](https://www.w3.org/WAI/WCAG21/Understanding/focus-visible.html)(poziom AA); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.


--------------------
[&lt; Zmiana rozmiaru tekstu ](05-P-zmiana-rozmiaru-tekstu) | [Łatwe testy - spis treści](00-P-spis-tresci) | [Formularze, etykiety i błędy >](07-P-formularze)
