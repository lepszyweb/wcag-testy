---
title: 24. Parsowanie


sidebar: testy-itc_sidebar
permalink: ICT_24_parsowanie
folder: testy-itc
---

## Wymogi dostępności

-   [KS WCAG 4.1.1 Parsowanie](https://wcag.lepszyweb.pl/#parsing) -- W treści wprowadzonej przy użyciu języka znaczników, elementy posiadają pełne znaczniki początkowe i końcowe, elementy są zagnieżdżane według swoich specyfikacji, elementy nie posiadają zduplikowanych atrybutów oraz wszystkie ID są unikalne, za wyjątkiem przypadków, kiedy specyfikacja zezwala na wyżej wymienione cechy.

## Uzasadnienie metody badania
Ten test podstawowy wymaga, aby treść nie zawierała błędów w składni elementów i atrybutów oraz zapewniała prawidłowo zagnieżdżone znaczniki początku/końca, aby uniknąć błędów, które uniemożliwiają programom użytkowników niezawodne przetwarzanie zawartości. Jeśli treści nie można przetworzyć w strukturę danych, wówczas różne programy użytkownika, w tym technologie wspomagające, mogą ją prezentować  odmiennie lub w ogóle nie potrafią jej przetworzyć.



## Ograniczenia, założenia lub wyjątki

-   *Uwaga*: Znaczniki początkowe i końcowe, w których brakuje znaku kluczowego, takiego jak zamykający nawias kątowy lub właściwy cudzysłów wartości atrybutu, nie są kompletne.
- Znaczniki nie zawsze są osiągalne dla technologii wspomagających lub dla wybranych przez użytkownika programów użytkownika, takich jak przeglądarki. Niekiedy oprogramowanie wykorzystuje wewnętrzne (własne) języki znaczników, aby zachować spójność interfejsu użytkownika oprogramowania w sposób, w którym znaczniki nigdy nie są dostępne dla technologii wspomagającej (bezpośrednio lub poprzez obietowy model dokumentu (DOM)),lub klienta użytkownika (np. przeglądarki).  W takich przypadkach zgodność z tym wymogiem nie miałaby wpływu na dostępność, ponieważ może mieć to wpływ na treści internetowe, w których są one udostępniane.
-    Jak stwierdzono w języku wymagań, niektóre specyfikacje mogą zezwalać na powielanie identyfikatorów. Na przykład niektóre języki znaczników mogą zezwalać na powielanie identyfikatorów, pod warunkiem że identyfikatory te są niepowtarzalne dla elementów równorzędnych w ramach tego samego elementu nadrzędnego.


## Procedura testu dla KS 4.1.1 Parsowanie

### Identyfikacja treści
Wszystkie strony internetowe

### Instrukcja testowania
1.  Sprawdź, czy (z wyjątkiem przypadków, w których specyfikacje dopuszczają takie cechy)
    1.  elementy mają pełne znaczniki początkowe i końcowe,
    2.  elementy są zagnieżdżone zgodnie z ich specyfikacjami,
    3.  elementy nie zawierają powtarzających się atrybutów; oraz
    4.  wszelkie identyfikatory są niepowtarzalne.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 4.1.1  oraz Wymaganie podstawowe nr 24 kończy się niepowodzeniem.

## Porada: Wskazówki dotyczące usprawniania procesu testów

Chociaż walidatory mogą być świetnym narzędziem do wychwytywania błędów, nie mogą określać, które z nich są wyłącznie błędami parsowania, ani nie wychwytują wszystkich przypadkó, w których zawartość nie jest w pełni zgodna ze specyfikacją.


## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G134: Sprawdzanie poprawności kodu stron internetowych (walidacja)](https://www.w3.org/TR/WCAG20-TECHS/G134.html)
-   [G192: Pełna zgodność ze specyfikacjami](https://www.w3.org/TR/WCAG20-TECHS/G192.html)
-   [H88: Używanie HTML zgodnie ze specyfikacją](https://www.w3.org/TR/WCAG20-TECHS/H88.html)
-   [H74: Zapewnienie, że znaczniki otwierające i zamykające są używane zgodnie ze specyfikacją](https://www.w3.org/TR/WCAG20-TECHS/H74.html) ORAZ [H93: Zapewnienie, że atrybuty id są unikalne](https://www.w3.org/TR/WCAG20-TECHS/H93.html) AND [H94: Zapewnienie, że elementy nie zawierają zduplikowanych atrybutów](https://www.w3.org/TR/WCAG20-TECHS/H94.html)


