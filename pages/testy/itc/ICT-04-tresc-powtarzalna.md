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

## Objaśnienie metody badania
Aby umożliwić równe korzystanie ze strony przez użytkowników obsługujących ją wyłącznie z klawiatury, musi istnieć metoda umożliwiająca obejście powtarzających się treści bez konieczności użycia dodatkowych narzędzi. Powszechnie stosowaną metodą omijania powtarzalnych treści są łącza wewnętrzne (do miejsc na tej samej stronie), ale inne metody, takie jak ukrywanie menu i drzewo nawigacji, są dopuszczalne. Powtarzające się treści są również oceniane pod kątem spójnej kolejności względnej.

## Ograniczenia, założenia lub wyjątki
- Małe sekcje, takie jak powtarzające się pojedyncze słowa, frazy lub pojedyncze łącza, nie są uważane za bloki w sensie używanym w tym wymaganiu.
- Większość przeglądarek internetowych udostępnia skróty klawiaturowe, które przenoszą fokus użytkownika na górę strony lub przeglądarki, dlatego umieszczenie łącza „pomijającego” może być zbędne, jeśli zestaw łączy nawigacyjnych znajduje się na dole strony internetowej.
- [Taka sama kolejność względna](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-locations.html#samerelorderdef) to takie samo położenie względem innych elementów. **Uwaga**: Uznaje się, że elementy mają taką samą względną kolejność, nawet jeśli inne elementy zostały dodane lub usunięte z kolejności oryginalnej. Przykładowo, rozszerzenie menu nawigacji może wyświetlić dodatkowy poziom szczegółowości, lub też drugorzędna sekcja nawigacji może zostać dodana do kolejności czytania.
- Spójne alternatywy tekstowe dla komponentów interfejsu, pełnią tę samą funkcję, nie zawsze są naprawdę „identyczne”. Jest to dopuszczalne, jeśli mają one spójny format. Na przykład, w przypadku użycia strzałki graficznej na dole strony internetowej, która odsyła do następnej strony, alternatywą tekstową może być: „Przejdź do strony 4.” Jednak ten sam obrazek strzałki na następnej stronie powinien zawierać jako alternatywę napis „Przejdź do strony 5.”
- „Mechanizmy nawigacyjne”, o których mowa w KS 3.2.3, obejmują zarówno interaktywne, jak i nieinteraktywne komponenty powtarzające się na stronach. Spójna prezentacja i układ są korzystne dla użytkowników, którzy wchodzą w interakcję z powtarzającymi się treściami w obrębie zestawu stron internetowych i muszą znajdować określone informacje lub funkcje częściej niż raz.
- Ten test podstawowy obejmuje metody obejścia, które działają tylko przy użyciu klawiatury. Nie uwzględniono następujących wystarczających technik WCAG, które wymagają dodatkowych narzędzi wspomagających, aby działały jako metody obejścia:
  - {% include techniki/ARIA11.md %}
  - {% include techniki/H69.md %}

## Procedura testu dla KS 2.4.1 Możliwość pominięcia bloków
Identyfikator testu podstawowego: *4.A-BypassBlocks*
### Identyfikacja treści
Bloki treści, które powtarzają się na wielu stronach, w tym zestawy łączy nawigacyjnych, nagłówki stron i banery.

### Instrukcja testowania
1.  Użyj standardowych poleceń klawiaturowych, aby przechodzić do przodu do powtarzających się bloków treści. Niektóre funkcje obejścia mogą nie być widoczne, dopóki nie uzyskają fokusu.
2.  Sprawdź, czy istnieje metoda umożliwiająca pomijanie powtarzających się treści przy użyciu klawiatury.
3.  Użyj klawiatury, aby aktywować metodę obejścia i sprawdzić działanie funkcji obejścia.
4.  Sprawdź, czy metoda działa zgodnie z przeznaczeniem. Na przykład:
    -   Blok powtarzającej się treści jest ukrywany, zamykany lub pomijany.
    -   Jeśli metoda ma na celu pominięcie, sprawdź, czy fokus jest przesunięty poza powtarzającą się treść. Treści, które się nie powtarzają, nie powinny być pomijane. Jeśli jest tylko tekst (nie ma elementu interaktywnego, który ma odbierać fokusu, może nie być oczywiste, że nastąpiło przeniesienie fokusu.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test podstawowy *4.A-BypassBlocks* kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.3 Spójna nawigacja
Identyfikator testu podstawowego: *4.B-ConsistentNavigation*

### Identyfikacja treści
Mechanizmy nawigacyjne, które powtarzają się na wielu stronach (które mogą, ale nie muszą być zawarte w bloku treści).

### Instrukcja testowania
1. Przejrzyj wiele stron internetowych. Nie inicjuj zmian treści.
2. Sprawdź, czy każdy powtarzający się mechanizm nawigacyjny występuje w tej samej kolejności względnej, co inne powtarzające się komponenty interfejsu na każdej stronie internetowej, na której się pojawia.

### Wynik testów
Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy *4.B-ConsistentNavigation* kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.4 Spójna identyfikacja
Identyfikator testu podstawowego: *4.C-ConsistentIdentification*
### Identyfikacja treści
Komponenty, które mają te same funkcje w zestawie stron internetowych.

### Instrukcja testowania
1.  Sprawdź, czy powiązany tekst (np. etykieta, nazwa lub tekst alternatywny) dla oznaczonej treści jest identyczny dla każdego wystąpienia, w którym pełnią one tę samą funkcję.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy *4.C-ConsistentIdentification* kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Niektóre metody pomijania bloków mogą wymagać określonego skrótu klawiaturowego (np. domyślnie do nawigacji między ramkami jest to klawisz F6 ).
-   Jeśli istnieje metodę pomijania, ale nie można jej aktywować za pomocą klawiatury, jest to również błąd wymagania podstawowego 1. Dostęp z klawiatury (Test 1.A).
-   Jeśli metoda pomijania jest w porządku tabulacji, ale nie jest widoczna, gdy ustawiany jest fokus klawiatury, jest to błąd wymagania podstawowego 2. Widoczny fokus.
-   Jeśli na jednej stronie istnieje potrzeba zastosowania wielu metod obejścia, każda z nich musi opisywać swoje przeznaczenie, aby spełnić wymagania wymaganie podstawowe 14.A. Na przykład strona z powtarzającymi się łączami powinna mieć opisową metodę obejścia. Jeśli istnieje również blok powtarzającej się treści, powinien on mieć oddzielnie opisaną metodę obejścia.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/F31.md %}
- {% include techniki/G1.md %}
- {% include techniki/G61.md %}
- {% include techniki/G123.md %}
- {% include techniki/G124.md %}
- {% include techniki/G197.md %}
- {% include techniki/G202.md %}
- {% include techniki/H70.md %} ORAZ {% include techniki/H64.md %}
- {% include techniki/SCR28.md %}

