# 2. Widoczny fokus

## Wymagania dostępności
-   [KS WCAG: 2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible) -- Każdy interfejs możliwy do nawigacji za pomocą klawiatury, posiada widoczny wskaźnik fokusa klawiatury.

## Uzasadnienie metody badania
Ręczna nawigacja lub sterowanie interfejsem tylko za pomocą klawiatury umożliwi testerowi rozpoznanie, kiedy nie ma wizualnego rozróżnienia między elementem posiadajacym fokus a resztą interfejsu lub zawartości.

## Ograniczenia, założenia lub wyjątki
-   Niektóre elementy interfejsu (np. tekst na ekranie do instrukcji wypełniania formularzy), które nie są zwykle uważane za interaktywne, mogą być w kolejności tabulacji. Takie komponenty interfejsu powinny otrzymywać widoczny fokus, gdy użytkownik nawiguje do nich za pomocą klawiatury.
-   Częścią tego testu jest widoczność fokusa na łączach pomijających.
-   Przełączanie fokusa na odkrywane treści nie jest tutaj testowane. Zobacz [5. Treść zmienna](testy/ICT_05_tresc-zmienna.md)
-   Utrata widocznego fokusa nie powinna wystąpić podczas ręcznego przesuwania fokusa przez stronę (za pomocą TAB lub klawiszy strzałek). Jednak po uruchomieniu funkcji, która przemieszcza fokus (np. odsłonięcie wewnętrznego łącza strony lub ukrytej zawartości), może być konieczne ręczne przesunięcie fokusa za pomocą klawiatury, zanim fokus stanie się ponownie widoczny. To nie jest uważane za defekt.

## Procedura testu dla KS 2.4.7 Widoczny fokus

### Identyfikacja treści

Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes).

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się między poszczególnymi elementami interfejsu.
2.  Sprawdź, czy widoczne jest wskazanie fokusa, gdy fokus znajduje się na elemencie interfejsu.

### Wynik testów
-   Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.7 oraz wymaganie podstawowe nr 2 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

-   Wyrazistość widocznego fokusa jest subiektywna, a minimalnym poziomem jest domyślne ustawienie wyświetlacza przeglądarki (lub platformy systemu operacyjnego) do wskazywania fokusa. Przeglądarki mogą również inaczej przedstawiać fokus w określonych sytuacjach.
-   Wskaźnik fokusa może przybierać różne formy: obramowania elementu, migającego kursora w polu tekstowym, wizualnej zmiany wyglądu przycisku. 
-   Ten test można przeprowadzić równocześnie z testem [1. Dostęp z klawiatury](testy/ICT_01_klawiatura.md).
-   Podczas testowania nie należy włączać żadnych modyfikacji fokusa w środowisku testowym. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus. Chociaż narzędzia testujące mogą pomóc testerom w śledzeniu fokusa, żadne znaczniki dostarczone przez narzędzie testujące nie powinny być używane jako wskaźnik widocznego fokusa dla spełnienia tego wymagania.
-   Biorąc pod uwagę zmienność sposobu, w jaki przeglądarki mogą prezentować fokus w określonych sytuacjach, raporty z testów powinny zawierać szczegółowe informacje na temat środowiska testowego, w tym przeglądarki i wersji.


## Techniki WCAG 2.1
-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
    -   [G149: Korzystanie z komponentów interfejsu użytkownika, które są wyróżniane przez aplikację klienta, gdy otrzymują fokus.](http://www.w3.org/TR/WCAG20-TECHS/G149.html)
    -   [G165: Korzystanie z domyślnego dla platformy oznaczenia fokusa, dzięki czemu będą one przenoszone na inne platformy](https://www.w3.org/TR/WCAG20-TECHS/G165.html)
    -   [G195: Korzystanie z dobrze widocznego wskaźnika fokusa dostarczonego przez autora](https://www.w3.org/TR/WCAG20-TECHS/G195.html)

----------------------------------------
[Początek/Wprowadzenie](testy/ICT_00_wprowadzenie.md) | [Poprzedni &gt; Klawiatura](testy/ICT_01_klawiatura.md) | [Następny &gt; Kolejność fokusa](testy/ICT_03_kolejnosc-fokusa.md)
