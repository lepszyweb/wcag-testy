---
title: 2. Widoczny fokus


sidebar: testy_sidebar
permalink: ICT-02-widoczny-fokus
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-4-7.md %}  

## Uzasadnienie metody badania
Ręczna nawigacja lub sterowanie interfejsem tylko za pomocą klawiatury umożliwi testerowi rozpoznanie, kiedy nie ma wizualnego rozróżnienia między elementem posiadajacym fokus a resztą interfejsu lub zawartości.

## Ograniczenia, założenia lub wyjątki
-   W porządku tabulacji mogą być niektóre elementy interfejsu, które nie są zwykle uważane za interaktywne (np. tekst instrukcji wypełniania formularzy). Takie komponenty interfejsu powinny otrzymywać widoczny fokus, gdy użytkownik nawiguje do nich za pomocą klawiatury.
-   Częścią tego testu jest widoczność fokusu na łączach pomijających.
-   Przełączanie fokusu na odkrywane treści nie jest tutaj testowane. Zobacz [5. Treść zmienna](testy/ICT_05_tresc-zmienna)
-   Podczas ręcznego przesuwania fokusu przez stronę (za pomocą <kbd>Tab</kbd> lub klawiszy strzałek) nie powinno wystąpić zniknięcie fokusu. Jednak po uruchomieniu funkcji, która przemieszcza fokus (np. odsłonięcie wewnętrznego łącza strony lub ukrytej zawartości), może być konieczne ręczne przesunięcie fokusu za pomocą klawiatury, zanim fokus stanie się ponownie widoczny. To nie jest uważane za defekt.

## Procedura testu dla KS 2.4.7 Widoczny fokus

### Identyfikacja treści

Komponenty interfejsu dostępne dla klawiatury (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes).

### Instrukcja testowania
1.  Użyj klawiatury, aby poruszać się między poszczególnymi elementami interfejsu.
2.  Sprawdź, czy widoczne jest wskazanie fokusu, gdy fokus znajduje się na elemencie interfejsu.

### Wynik testów
-   Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.7 oraz wymaganie podstawowe nr 2 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

-   Wyrazistość widocznego fokusu jest subiektywna, a minimalnym poziomem jest domyślne ustawienie wyświetlacza przeglądarki (lub platformy systemu operacyjnego) do wskazywania fokusu. Przeglądarki mogą również inaczej przedstawiać fokus w określonych sytuacjach.
-   Wskaźnik fokusu może przybierać różne formy: obramowania elementu, migającego kursora w polu tekstowym, wizualnej zmiany wyglądu przycisku.
-   Ten test można przeprowadzić równocześnie z testem [1. Dostęp z klawiatury](testy/ICT_01_klawiatura.md).
-   Podczas testowania nie należy włączać żadnych modyfikacji fokusu w środowisku testowym. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus. Chociaż narzędzia testujące mogą pomóc testerom w śledzeniu fokusu, żadne znaczniki dostarczone przez narzędzie testujące nie powinny być używane jako wskaźnik widocznego fokusu dla spełnienia tego wymagania.
-   Biorąc pod uwagę zmienność sposobu, w jaki przeglądarki mogą prezentować fokus w określonych sytuacjach, raporty z testów powinny zawierać szczegółowe informacje na temat środowiska testowego, w tym przeglądarki i wersji.


## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G149.md %}
- {% include techniki/G165.md %}
- {% include techniki/G195.md %}
