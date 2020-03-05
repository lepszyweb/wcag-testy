---
title: Tytuł strony
tags: [nawigacja]
sidebar: testy_sidebar
permalink: 01-P-tytul-strony
folder: testy/latwe
---

## Tytuł strony
Wszystkie strony internetowe i dokumenty powinny mieć tytuły opisujące ich temat, funkcję lub cel.

W witrynach internetowych tytuł każdej strony powinien zawierać temat strony i nazwę witryny.

Tytuły stron są:
-	wyświetlane na kartach przeglądarek,
-	wyświetlane w wynikach wyszukiwania,
-	wykorzystywane do tworzenia ulubionych zakładek w przeglądarce,
-	odczytywane przez czytniki ekranu.

### Dlaczego tytuł strony jest ważny?
Dzięki tytułom identyfikujemy wszelkie utwory, a więc strony internetowe również. Tytuł jest nazwą strony. Bez tytułu trudno byłoby się do strony odwołać.

Zwięzłe, unikalne tytuły stron pomagają użytkownikom zrozumieć treść i cel strony internetowej. Dzięki tytułom użytkownicy mogą łatwo ustalić, czy są zainteresowani treścią strony.

Dobre tytuły stron sprawiają, że różne sposoby wyszukiwania w Internecie potrzebnych treści stają się bardziej wydajne i skuteczne.

Tytuły są użyteczne dla wszystkich, ale szczególnie przydatne są dla osób niewidomych, ponieważ są zawsze pierwszym elementem strony ogłaszanym przez oprogramowanie do odczytywania ekranu.

Krótko mówiąc, tytuły są ważne nie tylko ze względu na dostępność.

### Tytuł strony w kodzie HTML
W kodzie strony tytuł strony określony jest za pomocą znacznika `<title>` umieszczanego na początku sekcji `<head>`. Może wyglądać np. tak:

```html
<title>Dostępny tytuł strony internetowej | Lepszy Web</title>
```

**Uwaga**: Znacznik elementu TITLE, znajdujący się w sekcji HEAD kodu HTML strony internetowej, nie powinien być mylony z atrybutem TITLE, który można zastosować do większości elementów HTML.

### Nadawanie tytułów stronom w systemach zarządzania treścią
W systemach do zarządzania treścią stron internetowych, a także w wielu generatorach witryn statycznych tworzenie tytułów stron jest zwykle zautomatyzowane.

Sposób generowania tytułów stron zależy od przyjętego przez twórców programu rozwiązania projektowego. Zazwyczaj źródłem tytułu konkretnej strony jest tytuł umieszczonej na tej stronie głównej zawartości, np. tytuł artykułu. W&nbsp;niektórych systemach można zdefiniować tytuły stron w opcjach pozycji menu, np. dla stron z&nbsp;przeglądami artykułów czy produktów w kategorii.

Ogólną zasadę generowania tytułu można często określić w sekcji globalnej konfiguracji witryny.  Na przykład w&nbsp;Joomla można zdecydować, czy do tytułów stron dodawać nazwę witryny oraz czy umieszczać ją przed, czy za tytułem.    

### Dobre praktyki

Tytuł strony powinien być:
-	**zwięzły**, aby go łatwo zapamiętać – nie więcej niż 60-70 znaków (tyle wyświetla Google),
-	**wyjątkowy**, aby odróżniał stronę od innych,
-	**odpowiedni**, aby precyzyjnie opisywał treść strony, jej główny temat,
-	**sensowny**, aby przekazywał przemyślaną, racjonalną informację, a nie dekoracje.

Dobrą praktyką jest, aby tytuł strony internetowej na witrynie składał się z dwóch części:
-	unikatowego tematu strony i
-	nazwy witryny.

Anglojęzyczni specjaliści dostępności podkreślają, że tytuły stron powinny być „front-loaded”, czyli żeby ważne i unikatowe informacje identyfikujące stronę znajdowały się z przodu, a nazwa witryny czy nazwa wydawcy za unikatowym tytułem.

#### Zasady pisowni
Według zasad pisowni polskiej po tytułach, śródtytułach i wyrażeniach hasłowych nie stawiamy kropki. Reguła ta odnosi się również do tytułów stron internetowych. Na końcu tytułu kropki nie stawiamy. Ale inne znaki interpunkcyjne – wykrzykniki i pytajniki – stawiamy. Gdy jednak pytanie w tytule jest pozbawione tonu pytającego, to można znak zapytania pominąć.

W tytułach kilkuczęściowych, np. złożonych z tematu strony i nazwy witryny, potrzebny jest jakiś znak interpunkcyjny jako separator części składowych. Nie ma jasno zdefiniowanej reguły dotyczących stosowania znaków interpunkcyjnych jako separatorów tytułów. Mogą to być myślniki. Często jest to znak pionowej kreski „|”  (nazywany „pipe”). Można też użyć kropki.  
Nie należy natomiast używać w tytułach znaków interpunkcyjnych do celów dekoracyjnych, na przykład ":: Tytuł ::" lub "... == Tytuł == ...".  Każdy taki znak jest odczytywany przez czytniki ekranu, co sprawia, że odsłuchanie tytułów staje się uciążliwe.

#### Przykłady złych praktyk w tytułowaniu stron
````
Witamy na stronie głównej Pracowni Dostępności Cyfrowej LepszyWeb.pl
Pracownia Dostępności Cyfrowej LepszyWeb.pl | O nas
Pracownia Dostępności Cyfrowej LepszyWeb.pl – Usługi
Pracownia Dostępności Cyfrowej LepszyWeb.pl :: Skontaktuj się z nami
````

#### Przykłady dobrych praktyk
````
Strona główna | Pracownia Dostępności Cyfrowej LepszyWeb.pl
O nas | LepszyWeb.pl
Usługi | LepszyWeb.pl
Skontaktuj się z nami | LepszyWeb.pl
````

Zwróć uwagę, że pełna nazwa witryny w przykładach powyżej została zastosowana tylko na stronie głównej.

Obraz poniżej przedstawia tytuły trzech stron na zakładkach kart w przeglądarce Firefox. Zauważ, że w kartach wyświetlana jest tylko pierwsza część tytułu strony. Ale gdy otworzymy więcej kart, zakładki z&nbsp;tytułami mogą ulec tak dużemu zwężeniu, że będzie na nich widać jedynie ikonę witryny (favicon).
![Tytuły stron na zakładkach kart w przeglądarce Firefox](images/andi/01_P_tytul-strony-firefox.png)

Podobnie jest w przeglądarce Chrome.
![Tytuły stron na zakładkach kart w przeglądarce Chrome](images/andi/01_P_tytul-strony-chrome.png)
Jeśli jednak ustawisz kursor myszki nad zakładką, zobaczysz w dymku pełny tytuł witryny.

## Co robić:
-	Spójrz na tytuł głównej strony witryny lub odsłuchaj go, jeśli korzystasz z czytnika ekranu.
-	Zobacz tytuły co najmniej kilku innych stron w witrynie.

## Co sprawdzać:
-	Czy każda strona ma tytuł?
-	Czy tytuł każdej strony krótko i odpowiednio opisuje jej treść?
-	Czy tytuł każdej strony jest inny od pozostałych?
-	Czy tytuły nie zawierają zbędnej interpunkcji?
-	Czy tytuły zawierają nazwę witryny?

## Testowanie tytułów stron
Aby sprawdzić tytuły stron w różnych przeglądarkach:

-	Jeśli masz przeglądarkę, która domyślnie wyświetla tytuł strony na pasku tytułowym okna, użyj tej przeglądarki. W&nbsp;nowoczesnych przeglądarkach trudno spotkać tę opcje, ale być może wciąż używasz starszej wersji Firefoxa, Opery, czy Internet Explorer. Aktualnie  (2019 rok) z popularnych przeglądarek Safari wyświetla tytuły stron na pasku tytułowym okna.

![Tytuł strony na pasku tytułowym okna w przeglądarce Safari](images/andi/01_P_tytul-strony-safari.png)

- Jeśli twoja przeglądarka nie ma paska tytułu, możesz spróbować jednego z następujących sposobów:
  - Najedź wskaźnikiem myszy na zakładkę karty przeglądarki, aby zobaczyć tytuł strony tak, jak na ilustracji poniżej:

![Tytuł strony w okienku wyskakującym, wyświetlany po najechaniu myszką na zakładkę karty w przeglądarce Firefox](images/andi/01_P_tytul-strony-firefox.png)

  - Skorzystaj z funkcji **Dodaj zakładkę**, aby wyświetlić okno dialogowe, które zawiera tytuł strony. Aby wywołać okno dialogowe Dodaj zakładkę, możesz użyć w niektórych przeglądarkach systemu Windows skrótu klawiaturowego Ctrl + D, a&nbsp;w&nbsp;systemie Mac skrótu cmd + D. Ten sposób umożliwia skopiowanie tytułów badanych stron do raportu z&nbsp;przeglądu.

![Tytuł strony w oknie dialogowym Dodaj zakładkę w przeglądarce Chrome](images/andi/01_P_tytul-strony-okno-dialogowe.png)

  - Jeśli używasz przeglądarki Opera, skorzystaj z&nbsp;funkcji *Menu kart*, którą wywołasz skrótem Ctrl + M. Po uaktywnieniu menu kart wskaż kartę interesującej cię strony, a&nbsp;poniżej zobaczysz sporych rozmiarów podgląd strony z&nbsp;widocznym tytułem, jak na ilustracji poniżej:

![Tytuł strony na podglądzie strony w menu kart w przeglądarce Opera](images/andi/01_P_tytul-strony-opera.png)  

## Dowiedz się więcej o tytułach stron
- [Zrozumienie kryterium sukcesu 2.4.2 Tytuły stron w WCAG 2.1 (poziom A](https://www.w3.org/WAI/WCAG21/Understanding/page-titled.html) - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
