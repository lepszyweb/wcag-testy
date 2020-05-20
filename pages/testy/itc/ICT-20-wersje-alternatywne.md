---
title: 20. Wersja alternatywna zapewniająca zgodność


sidebar: testy_sidebar
permalink: ICT-20-wersje-alternatywne
folder: testy/itc
---

Według zdefiniownych w WCAG [wymogów zgodności](wcag21#5-zgodność") strona internetowa lub jej część może być uznana za zgodną z WCAG na określonym poziomie, jeśli spełnia wszystkie kryteria sukcesu na tym poziomie ALBO dostępna jest <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wersja_alternatywna_zapewniajaca_zgodnosc | strip_html | replace: '*', ''}}">wersja alternatywna zapewniająca zgodność</a> na tym poziomie **ORAZ** zostaną spełnione pozostałe cztery wymogi zgodności.    




## Wymagania dostępności
---------------------
-   [WCAG: Wersja alternatywna zapewniająca zgodność](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conforming-alt-versions-head): Wersja alternatywna zapewniająca zgodność - Poziom AA: w przypadku zgodności z poziomem AA, treść spełnia wszystkie kryteria sukcesu na poziomie A i poziomie AA lub zapewniona jest wersja alternatywna zgodna z poziomem AA („zgodna wersja alternatywna”). Wymóg zgodności \#1 pozwala na włączenie w zakres zgodności stron niezgodnych, jeżeli istnieje „wersja alternatywna zapewniająca zgodność”, czyli wersja tej samej treści, która:
    1.  spełnia wszystkie kryteria sukcesu na wyznaczonym poziomie **ORAZ**
	2.  zawiera równoważne informacje i funkcjonalności w tym samym języku, **ORAZ**
    3.  jest tak samo aktualna jak wersja niezgodna, **ORAZ**
    4.  spełnia przynajmniej jeden z poniższych warunków:
        1.  wersja zgodna może być osiągalna z wersji niezgodnej za pomocą mechanizmu obsługiwanego przez dostępność **LUB**
        2.  wersja niezgodna może być osiągalna tylko z wersji zgodnej, **LUB**
        3.  wersja niezgodna może być osiągalna tylko z wersji zgodnej, o ile wersja niezgodna zawiera również mechanizm osiągnięcia wersji zgodnej.

## Uzasadnienie metody badania
------------------------------
Wersja alternatywna musi spełniać wszystkie części definicji, aby uznać ją za „wersję zapewniająca zgodność” („zgodnę wersję alternatywną”).


## Ograniczenia, założenia lub wyjątki

-  Uwagi do definicji zgodnej wersji alternatywnej:
    -   Uwaga 1: W tej definicji „może być osiągalna tylko” oznacza, że zapewniony jest jakiś mechanizm, jak na przykład warunkowe przekierowanie, który uchroni użytkownika przed „osiągnięciem” (załadowaniem) niezgodnej wersji, dopóki nie przejdzie do niej z wersji zgodnej.
    -   Uwaga 2: Zgodna wersja alternatywna nie musi być identyczna z podstawową co do liczby stron (np. może się składać z kilku podstron).
    -   Uwaga 3: Jeżeli istnieją różne wersje językowe witryny, to dla każdej z nich powinny być zapewnione zgodne wersje alternatywne.
    -   Uwaga 4: Zgodne wersje alternatywne mogą być zapewniane dla różnych technologii lub grup odbiorców. Każda wersja powinna być zgodna w jak najwyższym stopniu. Co najmniej jedna wersja musi być w pełni zgodna na wskazanym poziomie, aby spełnić Wymóg zgodności nr 1.
    -   Uwaga 5: Zgodna wersja alternatywna nie musi znajdować się w „zakresie zgodności” (zestawie stron, których dotyczy oświadczenie o zgodności), ani nawet w tej samej witrynie internetowej, jeżeli jest równie łatwo osiągalna, jak wersja niezgodna.
    -   Uwaga 6: Zgodna wersja alternatywna nie powinna być mylona z treścią uzupełniającą, która ma wspierać i rozszerzać wersję podstawową.
    -   Uwaga 7: Ustawienie w preferencjach użytkownika, które pozwala na osiągnięcie zgodnej wersji alternatywnej jest akceptowalnym mechanizmem dla osiągnięcia innej wersji, o ile mechanizm ustawień wspiera dostępność.
-   Dostarczenie zgodnej wersji alternatywnej nie jest wymogiem WCAG. Ten test sprawdza tylko, czy istnieje wersja alternatywna zapewniająca zgodność. Jeśli zgodna wersja alternatywna nie istnieje, wynikiem tego testu podstawowego jest „Nie dotyczy”. (Brak zgodnej wersji alternatywnej nie jest defektem, nie narusza żadnego kryterium sukcesu.)
-   Aby spełnić Wymóg zgodności 1 dla stwierdzenia zgodności z poziomem AA, strona internetowa musi spełniać wszystkie kryteria sukcesu na poziomach A i  AA albo dostępna jest wersja alternatywna zapewniająca zgodność z poziomem AA.

## Procedura testowania Wersji alternatywnej zapewniającej zgodność

### Identyfikacja treści
Inne wersje tej samej treści.

### Instrukcja testowania
1.  Sprawdź, czy zgodna wersja alternatywna zawiera wszystkie równoważne informacje i równoważne  funkcjonalności w tym samym języku naturalnym, co wersja niezgodna (podstawowa). 
2.  Sprawdź, czy zgodna wersja alternatywna jest tak samo aktualna, jak wersja niezgodna.
3.  Sprawdź, czy zgodna wersja alternatywna przechodzi wszystkie inne testy podstawowe.
4.  Sprawdź, czy spełniony jest przynajmniej jeden z poniższych warunków:
    1.  zgodną wersję alternatywną można osiągnąć z wersji niezgodnej za pośrednictwem mechanizmu obsługiwanego przez dostępność **LUB**
    2.  niezgodną wersję można osiągnąć tylko ze zgodnej wersji alternatywnej, **LUB**
    3.  niezgodną wersję można osiągnąć tylko ze zgodnej wersji alternatywnej, o ile w zgodnej wersji alternatywnej również istnieje mechanizm umożliwiający przejście do wersji alternatywnej.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas nie istnieje zgodna **wersja alternatywna**  i Wymaganie podstawowe nr 20 NIE MA ZASTOSOWANIA (wynikiem testu jest **NIE DOTYCZY**.

##  Wskazówki dotyczące usprawniania procesu testowego

-   Jeśli zapewniona jest zgodna wersja alternatywna, to niezgodne wersje tej treści są testowane tylko pod kątem [Wymagania zgodności nr 5 Brak zakłóceń](25_BrakZaklocen.md). Nie jest konieczne wykonywanie innych testów podstawowych na wersjach niezgodnych.
-   Jeśli istnieją zgodne wersje alternatywne, należy podjąć decyzję, czy wersja niezgodna wymaga przetestowania i w jakim zakresie. Aby zaoszczędzić czas i wysiłek, zaleca się, aby był to jeden z pierwszych testów.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G136.md %}
- {% include techniki/G190.md %}
- {% include techniki/C29.md %}
