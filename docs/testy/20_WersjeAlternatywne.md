# 20. Zgodność z wersją alternatywną

## Wymogi dostępności
---------------------
-   [WCAG: Wersja alternatywna zapewniająca zgodność](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conforming-alt-versions-head): Wersja alternatywna zapewniająca zgodność - Poziom AA: w przypadku zgodności z poziomem AA, \[treść\] spełnia wszystkie kryteria powodzenia poziomu A i poziomu AA lub dostarczana jest wersja alternatywna zgodna z poziomem AA. Wymóg zgodności \#1 pozwala na włączenie stron niezgodnych ze sobą w zakres zgodności tak długo, jak długo istnieje „Wersja alternatywna zapewniająca zgodność”, która
    1.  jest zgodna z określonym poziomem oraz
    2.  zapewnia te same informacje i funkcjonalności w tym samym języku oraz
    3.  jest tak samo aktualna jak wersja niezgodna oraz
    4.  dla której przynajmniej jeden z poniższych warunków jest spełniony:
        1.  wersja zgodna jest osiągalna z wersji niezgodnej za pomocą mechanizmu wspierającego dostępność lub
        2.  niezgodna wersja jest osiągalna jedynie z wersji zgodnej lub
        3.  wersja niezgodna może być osiągalna tylko z wersji zgodnej, o ile zawiera mechanizm osiągnięcia wersji zgodnej.

## Uzasadnienie metody badania
------------------------------
Wersja alternatywna musi spełniać wszystkie części definicji, aby uznać ją za „wersję zapewniająca zgodność”.


## Ograniczenia, założenia lub wyjątki

-  Uwagi do definicji wersji alternatywnej zapewniającej zgodność:
    -   Uwaga 1: W tej definicji „może być osiągalna tylko” oznacza, że zapewniony jest jakiś mechanizm, jak na przykład warunkowe przekierowanie, który uchroni użytkownika przed „osiągnięciem” (załadowaniem) niezgodnej wersji, dopóki nie przejdzie z wersji zgodnej.
    -   Uwaga 2: Alternatywna wersja nie musi być identyczna, co do ilości stron z podstawową (np. może się składać z kilku podstron).
    -   Uwaga 3: Jeżeli dostępne są różne wersje językowe serwisu, to dla każdej powinny być zapewnione zgodne wersje.
    -   Uwaga 4: Alternatywne wersje mogą być zapewniane dla różnych technologii lub grup odbiorców. Każda wersja powinna być zgodna w jak najwyższym stopniu. Jedna wersja powinna być w pełni zgodna, aby uzyskać Wymóg zgodności nr 1.
    -   Uwaga 5: Zgodna wersja alternatywna nie musi znajdować się w zakresie zgodności, ani nawet w tym samym serwisie internetowym, jeżeli jest równie łatwo dostępna, jak jej wersja niezgodna.
    -   Uwaga 6: Alternatywna wersja nie powinna być mylona z treścią uzupełniającą, która ma wspierać i rozszerzać wersję podstawową.
    -   Uwaga 7: Ustawienie w preferencjach użytkownika, które pozwala na uzyskanie zgodnej wersji jest akceptowalnym mechanizmem dla osiągnięcia innej wersji, o ile mechanizm ustawień wspiera dostępność.
-   Dostarczenie wersji alternatywnej zapewniającej zgodność nie jest wymogiem WCAG. Ten test sprawdza tylko, czy obecna jest wersja alternatywna zapewniająca zgodność. Jeśli nie istnieje wersja alternatywna zapewniająca zgodność, wynikiem tego testu podstawowego jest „Nie dotyczy”. (Brak wersji alternatywnej zapewniającej zgodność nie jest defektem)
-   Aby spełnić Wymóg zgodności 1 dla stwierdzenia zgodności z poziomem AA, strona internetowa musi spełniać wszystkie kryteria sukcesu na poziomach A i  AA albo dostępna jest wersja alternatywna zapewniająca zgodność z poziomem AA.

## Procedura testowania dla Wersja alternatywna zapewniająca zgodność

### Identyfikacja treści
Inne wersje tej samej treści.

### Instrukcja testowania
1.  Sprawdź, czy wersja alternatywna zawiera wszystkie te same informacje i te sam funkcje w tym samym języku naturalnym..
2.  Sprawdź, czy wersja alternatywna jest tak samo aktualna, jak treść w wersji niedostępnej.
3.  Sprawdź, czy wersja alternatywna przechodzi wszystkie inne testy podstawowe.
4.  Sprawdź, czy spełniony jest przynajmniej jeden z poniższych warunków:
    1.  wersję zapewniająca zgodność można uzyskać z wersji niezgodnej za pośrednictwem mechanizmu obsługiwanego przez dostępność LUB
    2.  wersję niezgodną można uzyskać tylko z wersji alternatywnej zapewniającej zgodność, LUB
    3.  wersję niezgodną można uzyskać tylko z wersji alternatywnej zapewniającej zgodność, która zapewnia również mechanizm umożliwiający przejście do wersji alternatywnej.

### Wynik testów
Jeżeli którakolwiek z powyższych próbzakończy się niepowodzeniem, wówczas nie istnieje zgodna **wersja alternatywna**  i Wymaganiem podstawowe nr 20 NIE MA ZASTOSOWANIA.

## Porada: Wskazówki dotyczące usprawniania procesu testów

-   Jeśli zapewniona jest wersja alternatywna zapewniająca zgodność, niezgodne wersje tej treści są testowane tylko pod kątem [Wymagania zgodności nr 5 Brak zakłóceń](25BrakZaklocen.md). Nie jest konieczne testowanie wykonywanie innych testów podstawowych dla wersji niezgodnych.
-   Jeśli istnieją wersje alternatywne zapewniające zgodność, należy podjąć decyzję, czy i w jakim zakresie wersja niezgodna wymaga przetestowania. Aby zaoszczędzić czas i wysiłek, zaleca się, aby był to jeden z pierwszych testów.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G136: Zapewnienie linku na początku niezgodnej strony internetowej, która wskazuje na alternatywną wersję zgodną z wymaganiami](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/G136)
-   [G190: Zapewnienie łącza sąsiadującego lub powiązanego z niezgodnym obiektem, który łączy się z odpowiednią wersją alternatywną](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/G190)
-   [C29: Używanie przełącznika stylu do zapewnienia zgodnej wersji alternatywnej (CSS)](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/C29)

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](19Ramki.md) | [[Następny]](21LimityCzasu.md)
