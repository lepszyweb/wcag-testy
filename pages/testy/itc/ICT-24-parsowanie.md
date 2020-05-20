---
title: 24. Parsowanie


sidebar: testy_sidebar
permalink: ICT-24-parsowanie
folder: testy/itc
---

## Wymogi dostępności
- {% include ks/4-1-1.md %}

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

Chociaż walidatory mogą być świetnym narzędziem do wychwytywania błędów, nie mogą określać, które z nich są wyłącznie błędami parsowania, ani nie wychwytują wszystkich przypadków, w których zawartość nie jest w pełni zgodna ze specyfikacją.


## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G134.md %}
- {% include techniki/G192.md %}
- {% include techniki/H88.md %}
- {% include techniki/H74.md %} ORAZ {% include techniki/H93.md %}, ORAZ {% include techniki/H94.md %}
