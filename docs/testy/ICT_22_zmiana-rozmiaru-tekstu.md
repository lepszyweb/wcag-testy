# 22. Zmiana rozmiaru tekstu

## Wymagania dostępności

-   [KS WCAG 1.4.4 Zmiana rozmiaru tekstu](https://wcag.lepszyweb.pl/#resize-text) -- Oprócz napisów rozszerzonych oraz tekstu w postaci grafiki, rozmiar tekstu może zostać powiększony do 200% bez użycia technologii wspomagających oraz bez utraty treści lub funkcjonalności.

## Uzasadnienie metody badania
Ten test podstawowy wymaga oceny wizualnej treści i funkcjonalności po zmianie rozmiaru tekstu.

## Ograniczenia, założenia lub wyjątki

-   Wyjątek: Napisy obrazy tekstu nie są uwzględniane w teście.

## Procedura testu dla 1.4.4 Zmiana rozmiaru tekstu


### Identyfikacja treści
Cały tekst na stronie.

### Instrukcja testowania
1.  Sprawdź, czy istnieje mechanizm zmiany rozmiaru, skalowania lub powiększania zawartości co najmniej do 200% oryginalnego rozmiaru. Znane rozwiązania obejmują:
    -   funkcja powiększania w przeglądarce,
	-   funkcje dostępności zapewniane przez platformę lub system operacyjny,
    -   Kontrolki do zmiany rozmiaru tekstu. (Jeśli funkcja powiększenia przeglądarki, systemu operacyjnego lub platformy nie jest obsługiwana przez stronę, strona musi zawierać mechanizm zmiany rozmiaru).
2.  Zmodyfikuj rozmiar czcionki, aby zwiększyć dwukrotnie szerokość i wysokość lub zwiększyć ją o 200%.
3.  Sprawdź wszystkie następujące elementy:
    -   tekst nie jest skracany, obcinany ani zasłaniany
    -   tekst wprowadzany w polach formularza również zmienia rozmiar
    -   cała funkcjonalność jest dostępna
    -   cała zawartość jest dostępna

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.4.4  oraz Wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Wskazówki dotyczące usprawniania procesu testów
brak

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G178: Zapewnienie na stronie internetowej przełączników, która pozwalają użytkownikom na przyrostową zmianę rozmiaru całego tekstu na stronie do 200 procent](https://www.w3.org/TR/WCAG20-TECHS/G178.html)
-   [G179: Zapewnienie, że nie dojdzie do utraty treści lub funkcjonalności, gdy zmianie ulegnie rozmiar tekstu albo obszar przeznaczony na tekst](https://www.w3.org/TR/WCAG20-TECHS/G179.html)
-   [F69: Niespełnienie kryterium sukcesu 1.4.4 podczas zmiany rozmiaru wizualnie renderowanego tekstu do 200 procent powoduje przycięcie, przycięcie lub zasłonięcie tekstu, obrazu lub formantów](https://www.w3.org/TR/WCAG20-TECHS/F69.html)
-   [F80: Niespełnienie kryterium sukcesu 1.4.4, gdy formanty formularza tekstowego nie zmieniają rozmiaru, gdy wizualnie renderowany tekst jest zmieniany do 200%](https://www.w3.org/TR/WCAG20-TECHS/F80.html)
-   [F94: Niespełnienie kryterium sukcesu 1.4.4 z powodu nieprawidłowego użycia jednostek rozmiaru obszaru operacyjnego (viewport) do zmiany rozmiaru tekstu](https://www.w3.org/TR/WCAG20-TECHS/F80.html)


----------------------------------------
[Początek/Wprowadzenie](testy/ICT_00_wprowadzenie.md) | [Poprzedni &gt; Limity czasu](testy/ICT_21_limity-czasu.md) | [Następny &gt; Wiele dróg](testy/ICT_23_wiele-drog.md)
