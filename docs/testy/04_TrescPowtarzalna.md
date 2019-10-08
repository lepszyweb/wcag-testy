# 4. Treść powtarzalna

## Wymagania dostępności
-   [KS WCAG: 2.4.1 Możliwość pominięcia bloków](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-skip.html) -- Dostępny jest mechanizm, który umożliwia pominięcie bloków treści powtarzanych na wielu stronach internetowych.
-   [KS WCAG: 3.2.3 Konsekwentna nawigacja](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-locations.html) -- Mechanizmy nawigacji, które powtarzają się na wielu stronach w serwisie internetowym, w danym porządku względnym wobec siebie, za każdym razem pojawiają się w tym samym porządku, chyba, że użytkownik sam wprowadzi zmiany.
-   [KS WCAG: 3.2.4 Konsekwentna identyfikacja](http://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-consistent-functionality.html) -- Komponenty, które posiadają tę samą funkcjonalność w danym serwisie internetowym, są w taki sam sposób zidentyfikowane.

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

-   [H69: Zapewnienie nagłówków na początku każdej sekcji treści](http://www.w3.org/TR/WCAG20-TECHS/H69.html)
-   [Używanie punktów orientacyjnych ARIA do określenia istotnych obszarów strony](https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA11.html)

Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
 
-   [G1: Dodanie u góry każdej strony linku, który prowadzi bezpośrednio do głównego obszaru zawartości](http://www.w3.org/TR/WCAG20-TECHS/G1.html)
-   [G123: Dodanie linku na początku bloku powtarzanej treści, aby przejść do końca bloku](http://www.w3.org/TR/WCAG20-TECHS/G123.html)
-   [G124: Dodawanie linków u góry strony do każdego obszaru zawartości](http://www.w3.org/TR/WCAG20-TECHS/G124.html)
-   [SCR28: Korzystanie z rozwijanego i zwijanego menu w celu ominięcia bloku treści](http://www.w3.org/TR/WCAG20-TECHS/SCR28.html)
-   [G202: Zapewnienie sterowania klawiaturą dla wszystkich funkcji](http://www.w3.org/TR/WCAG20-TECHS/G202.html)
-   [H70: Używanie elementów ramek do grupowania bloków powtarzanego materiału](https://www.w3.org/TR/WCAG20-TECHS/H70.html) AND [H64: Używanie atrybutu title do tytułowania elementów frame i iframe](https://www.w3.org/TR/WCAG20-TECHS/H64.html)
-   [G61: Prezentowanie powtarzających się komponentów w tej samej kolejności, za każdym razem, gdy się pojawiają](https://www.w3.org/TR/WCAG20-TECHS/G61.html)
-   [G197: Używanie etykiet, nazw i alternatyw tekstowych w sposób spójny dla treści o takiej samej funkcjonalności](https://www.w3.org/TR/WCAG20-TECHS/G197.html)
-   [F31: Niespełnienie kryterium sukcesu 3.2.4 z powodu używania dwóch różnych etykiet dla tej samej funkcji na różnych stronach internetowych w zestawie stron internetowych](http://www.w3.org/TR/WCAG20-TECHS/F31.html)

-------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](03KolejnoscFokusa.md) | [[Następny]](05TrescZmienna.md)
