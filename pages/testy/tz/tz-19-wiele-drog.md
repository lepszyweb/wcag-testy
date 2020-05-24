---
title: 19. Wiele dróg


sidebar: testy_sidebar
permalink: tz-19-wiele-drog
folder: testy/tz
---


## Dostęp do strony internetowej

Celem tej procedury testowej jest sprawdzenie, czy udostępniono użytkownikom co najmniej dwie metody zlokalizowania treści, aby mogli wybrać metodę, która jest dla nich łatwiejsza i bardziej zrozumiała.

Procedura testowa Wiele dróg obejmuje jeden test:
- Test 19.A  2.4.5-wiele-drog

### Test 19.A  2.4.5-wiele-drog

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.4.5-wiele-drog | 19.A    | Istnieją dwa lub więcej sposobów na zlokalizowanie strony internetowej w ramach jednego zestawu stron internetowych. |

### Cel testu 19.A  2.4.5-wiele-drog

Celem tego testu jest ustalenie, czy istnieje więcej niż jeden sposób na zlokalizowanie strony internetowej w zestawie stron. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 2-4-5 Wiele dróg](https://wcag.lepszyweb.pl/#multiple-ways).

### Identyfikacja treści

Wszystkie strony internetowe w zestawie stron (witrynie).

**Wyłączenia**: strony internetowe, które są wynikiem lub krokiem w procesie, takim jak formularz potwierdzenia zamówienia.

### Zastosowanie:

Test 19.A 2.4.5-wiele-drog **nie ma zastosowania**, jeśli zachodzi którakolwiek z poniższych sytuacji:

- strona nie jest częścią zestawu powiązanych stron internetowych (witryny),
- strona internetowa jest wynikiem albo krokiem w procesie i nie ma innego sposobu uzyskania dostępu do tych treści, dopóki nie zostanie wykonane inne działanie. Może to dotyczyć:
   - strony rejestracji, potwierzenia zamowienia, transakcji finansowej lub ukończenia kursu
   - strony wynikow wyszukiwania wyświetlanej na podstawie danych wprowadzonych prrzez użytkownika   
### Jak testować:

1.  Ustal, czy istnieją *dwa lub więcej* sposobów zlokalizowania określonej strony internetowej w zestawie stron internetowych; mogą one obejmować (ale nie wyłącznie) techniki takie jak:
    1.  mapy witryny
    2.  wyszukiwarka
    3.  spis treści
    4.  menu nawigacyjne lub menu rozwijane
    5.  drzewa nawigacyjne
    6.  łącza między stronami (poprzednia - następna)
	
	** Uwaga **: Oprócz wymienionych mogą istnieć inne sposoby lokalizacji stron w witrynie internetowej.

2.  Sprawdź, czy zidentyfikowane techniki działają poprawnie i prowadzą do strony internetowej w&nbsp;witrynie, na przykład:
   1. Łącza/menu prowadzą do odpowiednich stron witryny.
   2. Formularz wyszukiwania prowadzi do strony, która zawiera wyszukiwane hasło.


### Ocena wyników
Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.5:

1.  Istnieją co najmniej dwie techniki zlokalizowania strony internetowej w witrynie **oraz**

2.  Techniki te działają poprawnie, dzięki czemu prowadzą do właściwej strony internetowej.

## Obowiązujące normy

- {% include ks/2-4-5.md %}
- [23. Wiele dróg](ICT-23-wiele-drog)                                                                                         