---
title: 4. Treść powtarzalna


sidebar: testy_sidebar
permalink: ICT-04-tresc-powtarzalna
folder: testy/itc
---
# 4. Treść powtarzalna

## Wymagania dostępności
- {% include ks/2-4-1.md %}  
- {% include ks/3-2-3.md %}  
- {% include ks/3-2-4.md %}

## Uzasadnienie metody badania
Aby umożliwić równe korzystanie ze strony przez użytkowników osbługujących ją wyłącznie z klawiatury, musi istnieć metoda umożliwiająca obejście powtarzających się treści bez konieczności użycia dodatkowych narzędzi. Powszechnie stosowaną metodą omijania powtarzalnych treści są łącza wewnętrzne (do miejsc na tej samej stronie), ale inne metody, takie jak ukrywanie menu i drzewo nawigacji, są dopuszczalne. Powtarzane treści są również oceniane pod kątem konsekwentnej kolejności względnej.

## Ograniczenia, założenia lub wyjątki
- Małe sekcje, takie jak powtarzające się pojedyncze słowa, zwroty lub pojedyncze łącza, nie są uważane za bloki w sensie używanym w tym wymaganiu.
- Większość przeglądarek internetowych udostępnia skróty klawiaturowe, które przenoszą uwagę użytkownika na górę strony lub przeglądarki, dlatego umieszczenie łącza „pomijającego” może być zbędne, jeśli zestaw łączy nawigacyjnych znajduje się na dole strony internetowej.
- [Taka sama kolejność względna](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-locations.html#samerelorderdef) jest definiowana jako taka sama pozycja względem innych elementów. **Uwaga**: Uznaje się, że pozycje posiadają taką samą względną kolejność, nawet jeśli inne elementy zostały dodane lub usunięte z kolejności oryginalnej. Przykładowo, rozszerzenie menu nawigacji może wyświetlić dodatkowy poziom szczegółów, lub też druga sekcja nawigacji może zostać dodana do kolejności czytania.
- Spójne alternatywy tekstowe dla komponentów interfejsu, które spełniają tę samą funkcję, nie zawsze są naprawdę „identyczne”. Jest to dopuszczalne, jeśli mają one spójny format. Na przykład, w przypadku użycia strzałki graficznej na dole strony internetowej, która odsyła do następnej strony, alternatywą tekstową może być: „Przejdź do strony 4.” Jednak ten sam obrazek strzałki na następnej stronie powinien zawierać jako alternatywę napis „Przejdź do strony 5.”
- „Mechanizmy nawigacyjne”, o których mowa w KS 3.2.3, obejmują zarówno interaktywne, jak i nieinteraktywne komponenty powtarzane na stronach. Spójna prezentacja i układ są korzystne dla użytkowników, którzy wchodzą w interakcję z powtarzającymi się treściami w obrębie zestawu stron internetowych i muszą znajdować określone informacje lub funkcje częściej niż jeden raz.

## Procedura testu dla KS 2.4.1 Możliwość pominięcia bloków

### Identyfikacja treści
Bloki treści, które powtarzają się na wielu stronach, w tym zestawy łączy nawigacyjnych, nagłówki stron i banery.

### Instrukcja testowania
1.  Użyj standardowych poleceń klawiatury, aby przechodzić do przodu do powtarzalnych bloków treści. Niektóre funkcje obejścia mogą być niewidoczne, dopóki nie uzyskają fokusa.
2.  Sprawdź, czy dostępna jest metoda umożliwiająca pomijanie powtarzających się treści przy użyciu klawiatury.
3.  Użyj klawiatury, aby aktywować metodę obejścia i sprawdzić działanie funkcji obejścia.
4.  Sprawdź, czy metoda działa zgodnie z przeznaczeniem. Na przykład:
    -   Blok powtarzanej treści jest ukrywany, zamykany lub pomijany.
    -   Jeśli metoda ma na celu pominięcie, sprawdź, czy fokus jest przesunięty poza powtarzalną treść. Treści, które nie są powtarzalne, nie należy pomijać. Jeśli jest tylko tekst/brak elementu interaktywnego, który ma odbierać przesunięcie fokusa, może nie być oczywiste, że nastąpiło przesunięcie fokusa.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.1 oraz wymaganie podstawowe nr 4 kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.3 Konsekwentna nawigacja

### Identyfikacja treści
Mechanizmy nawigacyjne powtarzane na wielu stronach (które mogą, ale nie muszą być zawarte w bloku treści).

### Instrukcja testowania
1. Przejrzyj wiele stron internetowych. Nie inicjuj zmian treści.
2. Sprawdź, czy każdy powtarzany mechanizm nawigacyjny występuje w tej samej kolejności względnej, co inne powtarzające się elementy interfejsu na każdej stronie internetowej, na której się pojawia.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.2.3 oraz wymaganie podstawowe nr 4 kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.4 Konsekwentna identyfikacja

### Identyfikacja treści
Komponenty, które mają tę samą funkcjonalność w zestawie stron internetowych.

### Instrukcja testowania
1.  Sprawdź, czy powiązany tekst (np. etykieta, nazwa lub tekst alternatywny) dla określenia treści jest identyczny dla każdego przypadku, w którym pełnią tę samą funkcję.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.2.4 oraz wymaganie podstawowe nr 4 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

-   Niektóre metody pomijania mogą wymagać określonego skrótu klawiaturowego (np. domyślnie do nawigacji między ramkami jest to klawisz F6 ).
-   Jeśli podano metodę obejścia, ale nie można jej aktywować za pomocą klawiatury, jest to również defekt wymagania podstawowego 1. Dostęp z klawiatury.
-   Jeśli metoda obejścia jest w porządku tabbulacji, ale nie jest widoczna, gdy ustawiany jest fokus klawiatury, jest to defekt wymagania podstawowego 2. Widoczny fokus.
-   Jeśli na jednej stronie istnieje potrzeba zastosowania wielu metod obejścia, każda z nich musi opisywać swoje przeznaczenie, aby spełnić wymagania wymaganie podstawowe 14. Linki. Na przykład strona z powtarzającymi się linkami powinna mieć opisową metodę obejścia. Jeśli istnieje również blok powtarzalnych treści, powinien on posiadać oddzielnie opisaną metodę obejścia.

## Techniki WCAG 2.1
Ten test podstawowy obejmuje metody obejścia, które działają tylko z klawiaturą. Nie uwzględniono następujących wystarczających technik WCAG, które wymagają dodatkowych narzędzi pomocniczych do działania jako metody obejścia:

- {% include techniki/H69.md %}
-   [Używanie punktów orientacyjnych ARIA do określenia istotnych obszarów strony](https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA11.html)

Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G1.md %}
- {% include techniki/G123.md %}
- {% include techniki/G124.md %}
- {% include techniki/SCR28.md %}
- {% include techniki/G202.md %}
- {% include techniki/H70.md %} ORAZ {% include techniki/H64.md %}
- {% include techniki/G61.md %}
- {% include techniki/G197.md %}
- {% include techniki/F31.md %}
