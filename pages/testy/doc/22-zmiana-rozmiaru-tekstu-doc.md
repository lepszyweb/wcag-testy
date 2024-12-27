---
title: 22. Zmiana rozmiaru tekstu (dokument)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 22-zmiana-rozmiaru-tekstu-doc
folder: testy/doc
---

# 22. Zmiana rozmiaru tekstu

## Wymagania dostępności
- {% include ks/1-4-4.md %}

## Uzasadnienie metody testowej
Ten test podstawowy wymaga oceny wizualnej treści i funkcjonalności po zmianie rozmiaru tekstu.

## Ograniczenia, założenia lub wyjątki

-   Wyjątek: Obrazy tekstu i napisy rozszerzone dla niesłyszących nie są uwzględniane w teście.

## 22.A Procedura testowa zmiany rozmiaru tekstu
Identyfikator testu podstawowego: _22.A-ResizeText_

### Identyfikacja treści
Cały tekst w dokumencie.

### Instrukcje testowe
1.  Sprawdź, czy istnieje mechanizm zmiany rozmiaru, skalowania lub powiększania treści co najmniej do 200% oryginalnego rozmiaru. Znane rozwiązania obejmują:
    -   funkcja powiększania treści lub funkcja zmiany rozmiaru tekstu w aplikacji (przeglądarce),
	-   funkcje dostępności zapewniane przez platformę lub system operacyjny,
    -   kontrolki do zmiany rozmiaru tekstu w dokumencie lub aplikacji.
2.  Zmodyfikuj rozmiar czcionki, aby podwoić szerokość i wysokość lub zwiększyć ją o 200%.
3.  Sprawdź, czy spełnione są wszystkie poniższe warunki [KS 1.4.4]:
    -   tekst nie jest przycinany, obcinany ani zasłonięty
    -   tekst wprowadzany w polach tekstowych formularza również w pełni zmienia rozmiar
    -   wszystkie funkcje są dostępne
    -   cała treść jest dostępna

### Wynik testów
<p id="d22aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _22.A-ResizeText_ również kończy się niepowodzeniem.</p>

## Poradnik: Wskazówki dotyczące usprawniania procesu testów
brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G178.md %}
- {% include techniki/G179.md %}
- {% include techniki/F69.md %}
- {% include techniki/F80.md %}
- {% include techniki/F94.md %}

