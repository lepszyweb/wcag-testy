---
title: Określenie języka

sidebar: testy_sidebar
permalink: H4-01-identyfikacja-jezyka
folder: testy/jbt
---


## Określenie języka

### Metoda badania:
Kontrola wzrokowa. Inspekcja kodu HTML.

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [3.1.1 Język strony](https://wcag.lepszyweb.pl/#language-of-page), kryterium sukcesu: [3.1.2 Język części](https://wcag.lepszyweb.pl/#language-of-parts).

- Element `<html>` zawiera atrybut języka `lang`, a określony w nim język pasuje języka strony głównej treści strony.
- Treść w innych językach ma odpowiednio zdefiniowany atrybut językowy na elemencie obejmującym fragment innojęzyczny.

### Procedura testowania:
1.	Przeglądając treść strony, określ domyślny naturalny język strony. Domyślnym jest język, w którym prezentowana jest główna treść strony.
2.	Zobacz źródło strony i sprawdź, czy w znaczniku `<html>` zdefiniowany jest atrybut `lang`.
3.	Sprawdź, czy wartość atrybutu `lang` odpowiada domyślnemu językowi strony.
4.	Przejrzyj ponownie stronę i sprawdź, czy istnieją na stronie pojedyncze słowa lub grupy słów w innych językach, niż domyślny język strony..
5.	Korzystając z funkcji Zbadaj element w przeglądarce, sprawdź, czy każdy znaleziony innojęzyczny element strony został objęty odpowiednim znacznikiem z poprawną wartością atrybutu `lang`.


### Zasoby

#### Pomocne narzędzia:
- skryptozakładka [Lang Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access
- opcja *struktura* w skryptozakładce ANDI  https://lepszyweb.pl/andi/help/install.html

#### Wykorzystanie skryptozkładki ANDI
![Testowanie języka strony za pomocą skryptozkładki ANDI](/images/andi/andi_lang.png)

1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *struktura*.
2.	Wybierz z menu poziomego opcję  *więcej szczegółów*.
3.	Wybierz z rozwijanej listy opcję *język strony*.
4.	Sprawdź w oknie dialogowym, czy domyślny język strony  został określony poprawnie.

#### Techniki WCAG 2.1
-   [H57: Używanie atrybutu lang dla elementu html](https://www.w3.org/WAI/WCAG21/Techniques/html/H57.html)
-   [H58: Używanie atrybutu lang do wskazywania zmian w języku naturalnym](https://www.w3.org/WAI/WCAG21/Techniques/html/H58.html)
-   [FLASH13: Użycie atrybutów lang HTML w celu określenia języka treści we Flashu](https://www.w3.org/WAI/WCAG21/Techniques/flash/FLASH13.html)

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
