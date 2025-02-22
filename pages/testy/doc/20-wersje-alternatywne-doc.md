---
title: 20. Zgodna wersja alternatywna (dokumenty)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 20-wersje-alternatywne-doc
folder: testy/doc
---

## Wymagania dostępności
-   [Wymagania zgodności: Zgodna wersja alternatywna](https://wcag.irdpl.pl/understanding/zgodnosc#conforming-alt-versions): Wersja alternatywna zapewniająca zgodność - Poziom AA: w przypadku zgodności z poziomem AA, treść spełnia wszystkie kryteria sukcesu na poziomie A i poziomie AA lub zapewniona jest wersja alternatywna zgodna z poziomem AA („zgodna wersja alternatywna”). Wymóg zgodności \#1 pozwala na włączenie w zakres zgodności stron niezgodnych, o ile mają one „zgodną wersję alternatywną", czyli wersję tej samej treści, która:
    1.  spełnia wszystkie kryteria sukcesu na wyznaczonym poziomie **oraz**
	2.  zawiera równoważne informacje i funkcje w tym samym ludzkim języku, **oraz**
    3.  jest tak samo aktualna jak wersja niezgodna, **oraz**
    4.  spełnia przynajmniej jeden z poniższych warunków:
        -  wersja zgodna jest osiągalna z wersji niezgodnej za pomocą mechanizmu obsługującego dostępność **lub**
        -  wersja niezgodna jest osiągalna tylko z wersji zgodnej, **lub**
        -  wersja niezgodna może być osiągalna tylko z wersji zgodnej, która zawiera również mechanizm umożliwiający dostęp do wersji zgodnej.

## Uzasadnienie metody testowej
Zgodna wersja alternatywna musi spełniać wszystkie części definicji, aby uznać ją za „wersję zapewniająca zgodność” („zgodną wersję alternatywną”).

## Ograniczenia, założenia lub wyjątki

-  Uwagi z definicji zgodnej wersji alternatywnej:
    -   Uwaga 1: W tej definicji „jest osiągalna tylko” („można uzyskać tylko dostęp”) oznacza, że istnieje jakiś mechanizm, jak na przykład przekierowanie warunkowe, który uchroni użytkownika przed „dotarciem” (załadowaniem) niezgodnej wersji, chyba że użytkownik przeszedł właśnie z wersji zgodnej.
    -   Uwaga 2: Zgodna wersja alternatywna nie musi być identyczna z podstawową co do liczby stron (np. zgodna wersja alternatywna może składać się z wielu stron).
    -   Uwaga 3: Jeżeli istnieje wiele wersji językowych, to dla każdego oferowanego języka wymagane są zgodne wersje alternatywne.
    -   Uwaga 4: Zgodne wersje alternatywne mogą być zapewniane dla różnych  środowisk technologicznych lub grup odbiorców. Każda wersja powinna być zgodna w jak najwyższym stopniu. Co najmniej jedna wersja musi być w pełni zgodna na wskazanym poziomie, aby spełnić Wymóg zgodności nr 1.
    -   Uwaga 5: Zgodna wersja alternatywna nie musi znajdować się w „zakresie zgodności” (zestawie stron, których dotyczy deklaracja zgodności), ani nawet w tej samej witrynie internetowej, o ile jest równie łatwo osiągalna, jak wersja niezgodna.
    -   Uwaga 6: Zgodna wersja alternatywna nie powinna być mylona z treściami uzupełniającymi, która mają wspierać i rozszerzać wersję podstawową oraz poprawiać zrozumienie.
    -   Uwaga 7: Ustawienie w preferencjach użytkownika, które pozwala na osiągnięcie zgodnej wersji alternatywnej jest akceptowalnym mechanizmem dla osiągnięcia innej wersji, o ile mechanizm ustawień obsługuje dostępność.
-   Zgodnie z [Objaśnieniem alternatywnej wersji zgodnej w WCAG 2.2](https://wcag.irdpl.pl/understanding/zgodnosc), twórcy polegający na zgodnych wersjach alternatywnych muszą uświadomić użytkownikom, że istnieje zgodna wersja alternatywna. Można to osiągnąć, podając łącze do bardziej dostępnej wersji, wyraźnie oznaczonej tekstem łącza. Alternatywnie można podać łącze do instrukcji, która dokumentuje, jak uzyskać dostęp do bardziej dostępnej wersji, a także konkretne sposoby, dzięki którym alternatywna wersja jest bardziej dostępna (np. „wersja o wysokim kontraście”).	
-   Zapewnienie zgodnej wersji alternatywnej nie jest wymogiem WCAG. Ten test sprawdza tylko, czy istnieje zgodna wersja alternatywna. Jeśli nie ma zgodnej wersji alternatywnej, wynikiem tego testu podstawowego jest **Nie dotyczy**. (Brak zgodnej wersji alternatywnej nie jest defektem, nie narusza żadnego kryterium sukcesu.)
-   Aby spełnić Wymóg zgodności 1 dla poziomu AA, strona internetowa musi spełniać wszystkie kryteria sukcesu poziomu A i poziomu AA albo istnieje jest alternatywna wersja zgodna z poziomem AA.


## 20.A Procedura testowania Zgodnej wersji alternatywnej
Identyfikator testu bazowego: _20.A-ConformingAltVersion_

### Identyfikacja treści
Wiele wersji tej samej treści.

### Instrukcja testowania
1.  Sprawdź, czy zgodna wersja alternatywna zawiera te same informacje i funkcje w tym samym języku użytkownika. 
2.  Sprawdź, czy zgodna wersja alternatywna jest tak samo aktualna, jak wersja niezgodna.
3.  Sprawdź, czy zgodna wersja alternatywna przeszła wszystkie inne testy podstawowe.
4.  Sprawdź, czy spełniony jest co najmniej jeden z poniższych warunków:
    -  z wersji niezgodnej można uzyskać dostęp do zgodnej wersji alternatywnej za pomocą mechanizmu obsługiwanego przez funkcje dostępności, **lub**
    -  do wersji niezgodnej można uzyskać dostęp tylko ze zgodnej wersji alternatywnej, **lub**
    -  dostęp do wersji niezgodnej można uzyskać tylko ze zgodnej wersji alternatywnej, która zapewnia również mechanizm dostępu do wersji alternatywnej.
5.	Sprawdź, czy treść wskazuje, że istnieje zgodna wersja alternatywna. 
	
### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas nie istnieje **zgodna wersja alternatywna**, a wymaganie podstawowe _20.A-ConformingAltVersion_ NIE MA ZASTOSOWANIA (wynikiem testu jest **NIE DOTYCZY**).


##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Jeśli zapewniona jest zgodna wersja alternatywna, to niezgodne wersje tej treści są testowane tylko pod kątem [Wymagania zgodności 5 Bez zakłóceń](03-bez-zaklocen-doc.md). Nie jest konieczne wykonywanie innych testów podstawowych na wersjach niezgodnych.
-   Jeśli istnieją zgodne wersje alternatywne, należy podjąć decyzję, czy wersja niezgodna wymaga przetestowania i w jakim zakresie. Aby zaoszczędzić czas i wysiłek, zaleca się, aby był to jeden z pierwszych testów.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G136.md %}
- {% include techniki/G190.md %}
