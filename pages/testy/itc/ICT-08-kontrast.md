---
title: 8. Kontrast


sidebar: testy_sidebar
permalink: ICT-08-kontrast
folder: testy/itc
---


## Wymagania dostępności
- {% include ks/1-4-3.md %}  

## Opis metody testowej
Ten test jest przeprowadzany w celu oceny równego dostępu do informacji dla wszystkich użytkowników, w tym tych, którzy mogą mieć trudności z rozróżnieniem elementów o niskim kontraście.

## Ograniczenia, założenia lub wyjątki

-   **Wyjątki:** następujące typy tekstu i obrazów tekstu nie są uwzględnione w tym teście:
    -   Logotypy: logo lub nazwa marki
    -   Nieaktywne (wyłączone) komponenty interfejsu użytkownika
    -   Czysto dekoracyjne i nie znaczące, nie mające żadnej funkcji
    -   Zawarte na obrazie, który zawiera inne istotne treści wizualne
-   Testowanie zmian w kontraście tekstu obejmuje zmiany wynikające z najechania myszą i stanu zaznaczenia.
-   Wyłączone pola formularza nie otrzymują fokusu klawiatury, nie można ich wybrać ani modyfikować. Nie są one uwzględniane w testach kontrastu. **Uwaga:** Komponenty interfejsu *tylko do odczytu* i wyłączone to nie to samo. Wyłączone komponenty interfejsu można uznać za nieaktywne komponenty interfejsu; komponenty interfejsu *tylko do odczytu* są aktywnymi elementami interfejsu i muszą spełniać wymagania dotyczące współczynnika kontrastu.
-   Duży tekst to tekst co najmniej 18-punktowy lub tekst pogrubiony 14-punktowy.


## 8.A Procedura testowania kontrastu (minimum)
Identyfikator testu podstawowego: _8.A-ContrastMinimum_

### Identyfikacja treści
Cały widoczny tekst **ORAZ** obrazy tekstu (z wyjątkiem wymienionych w sekcji Ograniczenia, założenia lub wyjątki powyżej).

### Instrukcja testowania
1.  Określ  [współczynnik kontrastu](https://www.w3.org/TR/2008/REC-WCAG20-20081211/#contrast-ratiodef) tekstu (pierwszego planu) i tła.
2.  Sprawdź, czy współczynnik kontrastu wynosi co najmniej 4.5:1.
3.  Jeśli współczynnik kontrastu jest mniejszy niż 4.5:1, sprawdź, czy współczynnik wynosi co najmniej 3:1  ORAZ czy czcionka spełnia jedno z następujących kryteriów:
    -   ma rozmiar co najmniej 18 punktów (23,94 pikseli)
    -   ma rozmiar co najmniej 14 punktów  (18.62 pikseli) ORAZ pogrubienie (wagę co najmniej 700)

### Wynik testów
Jeśli oba powyższe testy zakończą się niepowodzeniem, test podstawowy _8.A-ContrastMinimum_ kończy się niepowodzeniem.



##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Istnieje wiele narzędzi do badania kontrastu kolorów, które mogą wykonać algorytmy niezbędne do określenia kontrastu. Zobacz technikę [G18: Zapewnienie, że istnieje kontrast wynoszący co najmniej 4,5:1 między tekstem (i obrazami tekstu) a tłem za tekstem](https://www.w3.org/TR/WCAG20-TECHS/G18.html), aby uzyskać informacje na temat możliwych narzędzi testujących, które wykorzystują odpowiedni algorytm.
-   Używaj narzędzi oceny kontrastu, które nie zaokrąglają wartości. Stosunek 4,499:1 nie spełniłby progu 4,5:1.
-   [WCAG 2.2 - Objaśnienie KS 1.4.3. Kontrast (minimum)](https://wcag.irdpl.pl/understanding/kontrast-minimum.html): sugeruje, aby oceniając to kryterium sukcesu, uzyskiwać rozmiar czcionki w punktach z programu użytkownika lub obliczyć na podstawie wskaźników czcionki w taki sam sposób, w jaki robią to programy użytkownika, a nie z badania tekstu przedstawionego na ekranie.
-   Chociaż tekst zawarty w logo renderowanym jako obrazy jest zwolniony z tego wymogu, obraz musi nadal zapewniać tekst alternatywny (np. w postaci atrybutu alt).

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:


- {% include techniki/G18.md %}
- {% include techniki/G145.md %}
- {% include techniki/F83.md %}