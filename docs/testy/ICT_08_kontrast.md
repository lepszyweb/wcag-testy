# 8. Kontrast

## Wymagania dostępności
---------------------
-   [KS WCAG: 1.4.3 Kontrast (minimum)](https://wcag.lepszyweb.pl/#contrast-minimum) -- Wizualne przedstawienie tekstu, lub obrazu tekstu posiada kontrast wynoszący przynajmniej 4,5:1, poza następującymi wyjątkami:
    -   **Duży tekst**: Duży tekst oraz grafiki takiego tekstu posiadają kontrast przynajmniej 3:1.;
    -   **Przypadkowość**: Nie stosuje się wymogów minimalnego kontrastu dla tekstów lub obrazu tekstu, będących elementem nieużywanych części interfejsu użytkownika, mających cel czysto dekoracyjny, nie są widoczne lub też są częścią obrazu zawierającego inne istotne treści wizualne.
    -   **Logo**: Nie wymaga się minimalnego kontrastu dla tekstu, który jest częścią logo lub nazwy własnej produktu (marki)

## Uzasadnienie metody badania
------------------------------
Ten test jest przeprowadzany w celu oceny równego dostępu do informacji dla wszystkich użytkowników, w tym tych, którzy mogą mieć trudności z rozróżnieniem elementów o niskim kontraście.


## Ograniczenia, założenia lub wyjątki
--------------------------------------
-   **Wyjątki:** następujące typy tekstu i obrazy tekstu nie są uwzględnione w tym teście:
    -   Logotypy: logo lub nazwa marki
    -   Nieaktywne (wyłączone) komponenty interfejsu użytkownika
    -   Czysto dekoracyjne i nieistotne, bez żadnej funkcjonalności
    -   Zawarte w obrazach, które zawierają inną znaczącą treść wizualną
-   Testowanie zmian w kontraście tekstu obejmuje zmiany wynikające z najechania myszą i stanu zaznaczenia.
-   Wyłączone elementy wejściowe, które nie otrzymują fokusa klawiatury, których nie można ich wybrać ani modyfikować. Nie są one wymagane do spełnienia wymagań dotyczących kontrastu. **Uwaga:** Komponenty interfejsu *tylko do odczytu* i wyłączone to nie to samo. Wyłączone komponenty interfejsu można uznać za nieaktywne komponenty interfejsu; komponenty interfejsu *tylko do odczytu* są aktywnymi elementami interfejsu i muszą spełniać wymagania dotyczące współczynnika kontrastu.
-   Duży tekst to tekst co najmniej 18-punktowy lub tekst pogrubiony 14-punktowy.

## Procedura testu dla KS 1.4.3 Kontrast (minimum)
---------------------------------------------------
### Identyfikacja treści
Cały widoczny tekst ORAZ obrazy tekstu (z wyjątkiem tych wymienionych powyżej w sekcji Ograniczenia, założenia lub wyjątki).

### Instrukcja testowania
1.  Określ  [współczynnik kontrastu](https://www.w3.org/TR/2008/REC-WCAG20-20081211/#contrast-ratiodef) tekstu (pierwszego planu) i tła.
2.  Sprawdź, czy współczynnik kontrastu wynosi co najmniej 4.5:1.
3.  Jeśli współczynnik kontrastu jest mniejszy niż 4.5:1, sprawdź, czy współczynnik wynosi co najmniej 3:1  ORAZ czy czcionka spełnia jedno z następujących kryteriów:
    -   ma rozmiar co najmniej 18 punktów (23,94 pikseli)
    -   ma rozmiar co najmniej 14 punktów  (18.62 pikseli) ORAZ pogrubienie (wagę co najmniej 700)

### Wynik testów
Jeżeli OBIE powyższe próby zakończą się niepowodzeniem, wówczas test KS 1.4.3 oraz wymaganie podstawowe nr 8 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
-----------------------------------------------------------
-   Istnieje wiele narzędzi do kontrastu kolorów, które mogą wykonać algorytmy niezbędne do określenia kontrastu. Zobacz technike [G18: Zapewnienie, że istnieje kontrast wynoszący co najmniej 4,5:1 między tekstem (i obrazami tekstu) a tłem za tekstem](https://www.w3.org/TR/WCAG20-TECHS/G18.html), aby uzyskać informacje na temat możliwych narzędzi testujących, które wykorzystują odpowiedni algorytm.
-   Chociaż tekst zawarty w logo renderowanym jako obrazy jest zwolniony z tego wymogu, obraz musi nadal zapewniać tekst alternatywny (np. w postaci atrybutu alt).


## Techniki WCAG 2.1
--------------------
-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
    -   [G18: Zapewnienie, że istnieje kontrast wynoszący co najmniej 4,5:1 między tekstem (i obrazami tekstu) a tłem za tekstem](https://www.w3.org/TR/WCAG20-TECHS/G18.html)
    -   [G145: Zapewnienie, że kontrast między tekstem (i obrazami tekstu) a tłem pod tekstem wynosi co najmniej 3:1](http://www.w3.org/TR/WCAG20-TECHS/G145.html) (gdy tekst ma co najmniej 18 punktów, jeśli nie jest pogrubiony i co najmniej 14 punktów, jeśli jest pogrubiony).

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](ICT_07_wlasciwosci-zmyslowe.md) | [[Następny]](ICT_09_miganie.md)
