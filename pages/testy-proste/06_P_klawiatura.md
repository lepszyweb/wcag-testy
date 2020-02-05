---
title: Dostęp do klawiatury i widoczny fokus
tags: nawigacja

sidebar: testy-proste_sidebar

permalink: 06_P_klawiatura
folder: testy-proste
---

## Dostęp do klawiatury i widoczny fokus

Wiele osób nie może korzystać z myszy i w interakcjach z internetem musi polegać na klawiaturze. Osoby niewidome i słabo widzące oraz osoby słabowidzące z ograniczeniami ruchu polegają na klawiaturze lub technologiach i strategiach wspomagających, które opierają się na poleceniach klawiaturowych wprowadzanych za pomocą skrótów klawiszowych lub poleceń głosowych. Dla takich osób strony są dostępne tylko wówczas, gdy umożliwiają przeglądanie wszystkich treści i obsługę wszystkich funkcji - łączy, formularzy, odtwarzaczy mediów itp. – za pomocą klawiatury.

Dla osób słabowidzących niezbędna jest również widoczność wskaźnika klawiatury, który nazywamy fokusem. Fokus pokazuje, na którym elemencie w danej chwili skupiona jest uwaga odbiornika sygnałów z klawiatury w programie użytkownika, czyli który z&nbsp;interaktywnych elementów strony jest aktualnie wybrany, który jest gotowy, by wykonać działanie żądane przez użytkownika. 
Podczas nawigacji klawiaturą po stronie, nazywanej nawigacją sekwencyjną, fokus powinien się przemieszczać sensownie zgodnie z&nbsp;logiczną kolejnością elementów strony. 

Aby zapewnić widoczność fokusa, twórcy stron mogą posłużyć się różnymi wskaźnikami, np. obramowaniem lub podkreśleniem elementu, który uzyskał fokus, odwróceniem (inwersją) kolorów elementu – wyświetleniem jasnego tekstu na ciemnym tle lub odwrotnie. W&nbsp;polach formularzy domyślnym wskaźnikiem fokusa jest migający kursor. Autorzy stron są zachęcani, by wzmocnić widoczność fokusa, który jest użyteczny dla wszystkich, a niezbędny dla osób z niepełnosprawnościami wzroku i ruchu.  

![Kontur wokół środkowego łacza](images/andi/06_P_fokus-linki.png)
Rysunek: Zwróć uwagę na kontur wokół środkowego łącza

![Przycisk bez fokusa po lewej stronie i z fokusem po prawej stronie](images/andi/06_P_fokus-przycisk.png)
Rysunek: Porównaj ten sam przycisk bez fokusa (po prawej - fioletowy napis na białym obramowanym tle) i z fokusem (po prawej - biały napis na fioletowym tle i otoczka)


### Co robić
W przeglądarkach, która obsługują nawigację za pomocą klawiatury za pomocą klawisza Tab (na przykład, Firefox, IE, Chrome i Safari):
-	W systemie Mac trzeba włączyć nawigację za pomocą klawiatury. W tym celu:
	- W nowszych przeglądarkach: Wybierz Preferencje systemowe > Klawiatura > Skróty, a następnie wybierz przycisk opcji Wszystkie elementy sterujące.
	- W starszych przeglądarkach: Wybierz Preferencje systemowe > Klawiatura > Skróty klawiaturowe, a następnie w sekcji „Pełny dostęp z klawiatury” zaznacz „Wszystkie kontrolki”.
-	Kliknij w pasku adresu, a następnie odłóż na bok mysz i nie używaj jej podczas testowania.
-	Naciskaj na klawiaturze klawisz Tab, aby przejść przez elementy na stronie. Można naciskać kombinację klawiszy „Shift-Tab”, aby poruszać się do tyłu.
-	Aby poruszać się w obrębie elementów, takich jak listy rozwijane, paski menu, harmonijki, naciskaj klawisze strzałek.
-	Aby wybrać konkretną pozycję w obrębie listy rozwijanej:
	- Przejdź klawiszem Tab do listy rozwijanej,
	- za pomocą klawiszy strzałek przenoś fokus między elementami listy,
	- naciśnij Enter, gdy fokus znajdzie się na elemencie, który chcesz wybrać.

### Co sprawdzać
-	**Tab do wszystkich**: Sprawdź, czy klawiszem Tab można dotrzeć do wszystkich interaktywnych elementów na stronie, w tym linków, pól formularzy, przycisków i pokręteł odtwarzacza multimedialnego. (Częstym problemem jest to, że nie można tabulatorem do elementów sterujących odtwarzacza multimedialnego.)
-	**Tab ze wszystkich**: Sprawdź, czy za pomocą klawisza Tab można wyjść ze wszystkich elementów, do których można było przenieść fokus. (Częstym problemem jest zatrzymanie fokusa klawiatury przez kontrolki mediów albo utknięcie wewnątrz innego elementu osadzonego na stronie, np. mapie tak, że nie można się z nich wydostać bez użycia myszki. Nazywa się to „pułapką na klawiaturę”).
-	**Kolejność tabulacji**: Sprawdź, czy kolejność przemieszczania  następuje w logicznej kolejności czytania (np. od lewej do prawej, w przypadku języków, w których obowiązuje taki kierunek pisania,  z góry na dół).
-	**Widoczny fokus**: Sprawdź, czy fokus jest wyraźnie widoczny, gdy przemieszczasz się prze kolejne elementy, to znaczy, czy w każdym momencie umiesz powiedzieć, w którym miejscu znajduje się fokus, np. że łącze uzyskało dodatkowe wyróżnienie (uwaga, zniknięcie podkreślenia nie jest dodatkowym wyróżnieniem!), że przycisk zmienił kolorystykę, że wokół pola  formularza pojawił się obrys. Uwaga: Nie wszystkie elementy muszą uzyskiwać taki sam wskaźnik fokusa, ale wszystkie elementy pełniące podobne funkcje powinny być oznaczane fokusem w podobny sposób. 
-	**Wszystkie funkcje za pomocą klawiatury**: Sprawdź, czy za pomocą klawiatury można zrobić wszystko, to znaczy, że nie potrzebujesz myszy, aby aktywować akcje, opcje, widoczne zmiany i inne funkcje. (Częstym problemem jest to, że niektóre funkcje są dostępne tylko przy najechaniu myszą i nie są dostępne z ogniskowaniem na klawiaturze).
-	**Rozwijane listy**: Sprawdź, czy po przejściu tabulatorem do listy rozwijanej, można użyć klawiszy strzałek, aby przejść przez wszystkie opcje bez wywołania działania. (Częstym problemem w przypadku list rozwijanych używanych do nawigacji jest to, że gdy tylko strzałka przeniesie fokus na następną pozycję, to ta pozycja zostaje automatycznie wybrana i nie można już przejść do innych pozycji na liście albo następuje przekierowanie na inną stronę lub w inne miejsce strony. 
-	**Linki graficzne**: Sprawdź, gdy obrazy, które są łączami, mają wyraźnie widoczny fokus i czy łącza mogą być aktywowane za pomocą klawiatury (zwykle przez naciśnięcie klawisza Enter).

### Sprawdzenie widoczności fokusa na stronie demo PrzediPo  
Otwórz dostępną wersję strony Ankieta: https://przedipo.lepszyweb.pl/after/survey.html
Przejdź przez wszystkie elementy strony klawiszem Tab, a w obrębie złożonej grupy elementów poruszaj się strzałkami. Zwróć uwagę, 
-	że wiele elementów w chwili uzyskania fokusa otrzymuje zielone tło
-	że niektóre  elementy w chwili uzyskania fokusa są obrysowane przerywaną linią
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

