# 5. Treść zmienna

## Wymogi dostępności
-   [KS WCAG: 4.1.2 Nazwa, rola, wartość](https://www.w3.org/TR/UNDERSTANDING-WCAG20/ensure-compat-rsv.html): Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
Celem tego testu podstawowego jest identyfikacja zmian wizualnych w treści i stanach komponentów, które występują bez odświeżania strony oraz skorelowanie tych zmian z równoważnymi informacjami programowymi i/lub tekstowymi. Użytkownicy technologii wspomagajacych powinni uzyskać powiadomienie o takich zmianach.
-   Zmiany treści mogą obejmować zmiany stanu komponentów (np. zamknięte/otwarte sekcje, kolejność sortowania, zwinięte/rozwinięte menu), wartości dynamiczne i/lub obliczane (np. „Pozostało 34 znaki”) oraz automatyczne aktualizowanie treści (np. ceny akcji).
-   Treść, która zmienia się w trakcie interakcji użytkownika z treścią (w tym między innymi zmiany w tekście, stanach komponentów, strukturze, relacjach lub funkcjonalnościach) musi zapewniać środki, za pomocą których zmianę treści można określić programowo lub w inny sposób dostępny w tekście.

## Ograniczenia, założenia lub wyjątki
- Stan elementów formularza (zaznaczone, niezaznaczone itp.) są uwzględnione w tym teście podstawowym.
- W tym teście uwzględniono zmiany inicjowane przez użytkownika i automatyczne aktualizacje.


## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość

### Identyfikacja treści
Zidentyfikuj zmiany w prezentowanej treści (zarówno wywołane przez użytkownika, jak i automatyczne). Przykłady obejmują zmiany w obrazach, drzewach nawigacji, kontrolkach sortowania tabeli danych, automatycznych aktualizacjach informacji, elementach formularza, treści odkrywanej itp.
- Może być konieczne użycie myszy, aby ustalić, czy zmiany stanu występują po najechaniu myszą czy kliknięciu.
- Zależnie od komponentu zmiana stanu może zostać wywołana przez różne działania, takie jak zmiana wartości lub stanów innych komponentów, przełączanie funkcji, wprowadzanie danych do komponentu, najechanie myszą itp.

### Instrukcja testowania
1. Sprawdź, czy strona programowo powiadamia o zmianie treści.
   - Powiadomienia o zdarzeniach programowych obejmują okna dialogowe z alertami, przeniesienie fokusa na zmienioną treść oraz aktywne (*live*) regiony ARIA.
1. Przy każdej zmianie treści sprawdź, czy kombinacja nazwy, roli, stanu i wartości zmienionej treści jest odpowiednia.
    - Nazwa: nazwa jest odpowiednia po zmianie. 
        - Zastosuj [accessible name and description computation](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation), jeśli zmiana nazwy miała miejsce. 
    - Rola: rola dokładnie opisuje cel elementu po zmianie, jeśli ma to zastosowanie.
        - Rozważ role ARIA, typ elementu i inny opisowy tekst.
    - Rola: rola dokładnie opisuje cel elementu po zmianie, jeżeli ma zastosowanie. 
        - Oceń ARIA i atrybuty specyficzne dla elementu (np. `<option selected=”true”>`)
    - Wartość: wartość jest aktualizowana po zmianie, jeżeli ma zastosowanie.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 4.1.2 oraz wymaganie podstawowe nr 5 kończy się niepowodzeniem.

## Porada: Wskazówki dotyczące usprawniania procesu testów
-   Zmiana treści może również obejmować zmiany koloru w celu przekazania informacji. Jeśli tak, ten test powinien sprawdzić, czy nazwa została zaktualizowana, aby odzwierciedlić znaczenie zmienionego koloru. Jeśli kolor zostanie użyty jako jedyny wizualny sposób przekazywania informacji (lub zmian informacji), wówczas treść nie spełnia wymagań KS 1.4.1 Uzycie koloru (omówione w punkcie 7 [Właściwości zmysłowe](07WlasciwościZmyslowe.md)).
-   Liczba powiadomień o zdarzeniach może być bardzo duża; jeśli liczba zmian w elemencie jest nieznana lub bardzo duża, konieczne może być zastosowanie próbkowania.

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](04TrescPowtarzalna.md) | [[Następny]](06Obrazy.md)
