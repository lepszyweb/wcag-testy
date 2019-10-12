# 14. Łącza i przyciski

## Wymagania dostępności
---------------------
-   [KS WCAG 2.4.4 Cel linku (w kontekście)](https://wcag.lepszyweb.pl/#link-purpose-in-context) -- Cel każdego linku może wynikać z samej treści linku, lub też z treści linku powiązanej z programistycznie określonym kontekstem, poza tymi przypadkami, kiedy cel łącza i tak byłby niejasny dla użytkowników.
-   [WCAG2 SC 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value) -- Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
------------------------------
Łącza i przyciski, w tym elementy skryptowe, muszą mieć znaczący tekst (powiązany bezpośrednio lub dostępny w kontekście) opisujący jego cel lub funkcję. Aby powiązany tekst był dostępny dla technologii wspomagających, informacje muszą być [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable).

## Ograniczenia, założenia lub wyjątki
--------------------------------------
-   [Z Objaśnienia UKS 2.4.4](https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-refs.html): Mogą zaistnieć sytuacje, w których cel połączenia ma być nieznany lub zasłonięty. Na przykład, gra może mieć linki oznaczone tylko jako drzwi \#2, drzwi nr \#2 i drzwi nr \#3. Ten tekst łącza byłby wystarczający, ponieważ celem jest stworzenie napięcia dla wszystkich użytkowników.
-   Ten test obejmuje przyciski. W Technikach wystarczających dla KS 2.4.4.4 znajduje się technika [FLASH27: Zapewnienie etykiet przycisków opisujących przeznaczenie przycisku](https://www.w3.org/WAI/WCAG21/Techniques/flash/FLASH27).


## Procedura testu dla KS 2.4.4 Cel linku (w kontekście)
--------------------------------------------------------
### Identyfikacja treści

Wszystkie łącza i przyciski, w tym te, które są elementami skryptowymi i którym przypisano rolę łącza (role="link")  i rolę przycisku (role="button").

### Instrukcja testowania

1.  Sprawdź, czy cel każdego linku i przycisku można określić na podstawie dowolnej kombinacji tekstu linku, [dostępnej nazwy, dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) lub poprzedzającego bezpośrednio kontekstu strony (ten sam akapit, lista lub komórka tabeli, w której znajduje się łącza lub komórka nagłówka tabeli, z którą jest powiązana komórka zawierająca łącze).

### Wynik testów

Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test 2.4.4, KS 4.1.2 oraz Wymaganie podstawowe nr 14 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------

-   W przypadku, gdy łącze / przycisk prowadzi do dokumentu lub aplikacji internetowej, nazwa dokumentu lub aplikacji internetowej wystarcza do opisania celu linku/przycisku (czyli odesłanie do dokumentu lub aplikacji internetowej).


## Techniki WCAG 2.1
--------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G91: Zapewnienie tekstu linku opisującego cel linku](https://www.w3.org/TR/WCAG20-TECHS/G91.html)
-   [G53: Określenie celu linku za pomocą tekstu linku w połączeniu z tekstem otaczającego zdania](https://www.w3.org/TR/WCAG20-TECHS/G53.html)
-   [ARIA7: Używanie atrybutu aria-labelledby, aby wskazać cel linku](https://www.w3.org/TR/WCAG20-TECHS/ARIA7.html)
-   [ARIA8: Używanie atrybutu aria-label, aby wskazać cel linku](https://www.w3.org/TR/WCAG20-TECHS/ARIA8.html)
-   [H77: Określenie celu łącza za pomocą tekstu linku w połączeniu z jego pozycją na liście](https://www.w3.org/TR/WCAG20-TECHS/H77.html)
-   [H79: Określenie celu łącza za pomocą tekstu linku w połączeniu z otaczającą go komórką tabeli i powiązanymi nagłówkami tabeli](https://www.w3.org/TR/WCAG20-TECHS/H79.html)
-   [F89: Niespełnienie kryterium sukcesu 2.4.4, 2.4.9 i 4.1.2 ze względu na brak podania dostępnej nazwy obrazu, który jest jedyną treścią w linku](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/F89)

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](ICT_13_struktura-tresci.md) | [[Następny]](ICT_15_jezyk.md)
