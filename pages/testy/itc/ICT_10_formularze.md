---
title: 10. Formularze


sidebar: testy_sidebar
permalink: ICT_10_formularze
folder: testy/itc
---

## Wymagania dostępności
---------------------
-   [WCAG: 1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships): Informacje, struktura oraz relacje pomiędzy treściami przedstawiane w treści mogą być odczytane przez program komputerowy lub są dostępne w postaci tekstu.
-   [WCAG: 2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels): Nagłówki i etykiety opisują temat lub cel treści.
-   [WCAG: 3.2.2 Podczas wprowadzania danych](https://wcag.lepszyweb.pl/#on-input): Zmiana ustawień jakiegokolwiek komponentu interfejsu użytkownika nie powoduje automatycznej zmiany kontekstu, chyba, że użytkownik został poinformowany o takim działaniu zanim zaczął korzystać z komponentu.
-   [WCAG: 3.3.1 Identyfikacja błędu](https://wcag.lepszyweb.pl/#error-identification): Jeśli przy wpisywaniu informacji, błąd zostanie wykryty automatycznie, system wskazuje błędny element, a użytkownik otrzymuje opis błędu w postaci tekstu.
-   [WCAG: 3.3.2 Etykiety lub instrukcje](https://wcag.lepszyweb.pl/#labels-or-instructions): Etykiety lub instrukcje pojawiają się w treści, kiedy wymagane jest wprowadzenie informacji przez użytkownika.
-   [WCAG: 3.3.3 Sugestie korekty błędów](https://wcag.lepszyweb.pl/#error-suggestion): Jeśli przy wpisywaniu informacji, błąd zostanie wykryty automatycznie i znane są sugestie korekty, wtedy użytkownik otrzymuje takie sugestie, chyba, że stanowiłoby to zagrożenie dla bezpieczeństwa treści lub zmieniłoby to cel treści.
-   [WCAG: 3.3.4 Zapobieganie błędom (kontekst prawny, finansowy, związany z podawaniem danych)](https://wcag.lepszyweb.pl/#error-prevention-legal-financial-data): Dla \[stron internetowych\], na których pojawiają się zobowiązania prawne lub transakcje finansowe, i w których użytkownik modyfikuje lub usuwa dane zawarte w systemach przechowywania danych, lub wprowadza testowe odpowiedzi, przynajmniej jedno z poniższych założeń jest prawdziwe::
    1.  **Odwracalność**: Wprowadzenie danych jest odwracalne..
    2.  **Sprawdzanie**: Dane wprowadzone przez użytkownika są sprawdzane pod kątem błędów, a użytkownik ma możliwość wprowadzenia poprawek.
    3.  **Potwierdzenie**: Dostępny jest mechanizm sprawdzania, potwierdzania oraz korekty informacji przed jej ostatecznym wysłaniem.
-   [WCAG: 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value): Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
------------------------------
Przejrzyj instrukcje formularza pod kątem kompletności i programowego powiązania z ich danymi wejściowymi. Wprowadź błędne dane wejściowe i przejrzyj powiadomienia o błędach dostarczone użytkownikowi.


## Ograniczenia, założenia lub wyjątki
--------------------------------------
-   Pola formularza tylko do odczytu (np. wstępnie wypełnione) otrzymują fokus klawiatury i można je wybierać, ale nie można ich modyfikować. Pola te muszą być oznaczone i [możliwe do odczytania przez program komputerowy](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable) oraz są testowane zgodnie z KS 1.3.1.
-   Wyłączone kontrolki nie otrzymują fokusa klawiatury, nie można ich wybrać ani modyfikować. Nie są one uwzględniane w tym teście.
-   Kliknięcie opcji lub zaznaczenie opcji w formularzu powinno wybrać opcję, ale nie powinno inicjować zmiany kontekstu.
-   [Zmiana kontekstu](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html#context-changedef) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po oznaczeniu fokusem](https://www.w3.org/TR/UNDERSTANDING-WCAG20/consistent-behavior-receive-focus.html) jako: znaczące zmiany treści \[strony internetowej\], które dokonywane bez świadomości użytkownika, mogą go dezorientować, jeżeli nie jest on w stanie oglądać całej strony jednocześnie. Zmiany kontekstu obejmują zmiany::
    1.  W programie użytkownika (przeglądarce, itp.)
    2.  Obszaru operacyjnego
    3.  Fokusa
    4.  Treści, która zmienia sens \[strony internetowej\].
-   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiana w treści, na przykład rozwinięcie drzewa, dynamicznego menu lub zakładki niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusa).
-   **Przykład zmiany kontekstu**: Otwarcie nowego okna, przeniesienie fokusa na inny obiekt, przejście na inną stronę internetową (włączając w to także każdą sytuację, kiedy użytkownikowi tylko wydaje się, że przechodzi na inną stronę internetową) lub znaczące przekształcenie wyglądu strony są przykładami zmiany kontekstu.


## Procedura testu dla KS 1.3.1 Informacje i relacje oraz 4.1.2 Nazwa, rola, wartość
------------------------------------------------------------------------------------
### Identyfikacja treści
1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania
1.  Sprawdź, czy kombinacja [dostępnej nazwy, dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) i innych powiązań programowych (np. powiązanie kolumny i wiersze tabeli) opisuje każdą kontrolkę i zawiera wszystkie niezbędne i odpowiednie instrukcje i wskazówki (tekstowe i graficzne). Odwołaj się do [Mapowania API dostępności HTML 1.0](https://www.w3.org/TR/html-aam-1.0/#input-type-text-input-type-password-input-type-search-input-type-tel-input-type-url-and-textarea-element),  aby uzyskać szczegółowe informacje na temat technik, które przyczyniają się do określenia dostępnej nazwy i dostępnego opisu.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.1, KS 4.1.2,  oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 2.4.6 Nagłówki i etykiety
---------------------------------------------------
### Identyfikacja treści
1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania
1.  Sprawdź, czy etykiety i/lub instrukcje dla każdej kontrolki zbierającej dane informują użytkowników, jakie dane wejściowe są oczekiwane i, w stosownych przypadkach, jaki format jest wymagany.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.6, KS 4.1.2,  oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 3.2.2 Podczas wprowadzania danych
-----------------------------------------------------------
### Identyfikacja treści
Wszystkie aktywne komponenty formularza.

### Instrukcja testowania
1.  Wprowadź dane w każdym polu formularza i opuść pole (klawiszem Tab).
2.  Zmień wybór lub wartości dla kontrolek formularza, takich jak przyciski opcji, pola wyboru, listy wyboru itp.
3.  Sprawdź, czy opuszczenie pola lub zmiana wyboru albo wartości w polu (np. wprowadzanie danych w polu tekstowym, zmiana wyboru przycisku opcji)  **NIE**  inicjuje zmiany kontekstu, chyba że użytkownik został poinformowany o takim zachowaniu przed użyciem komponentu. Przykłady zmiany kontekstu:
    -   Automatyczne przesłanie formularza po opuszczeniu pola,
    -   Automatyczne przesłanie formularza po opuszczeniu ostatniego pola w formularzu,
    -   Uruchamienie nowego okna, gdy zostanie zmienione zaznaczenie w grupie przycisków opcji
    -   Przeniesienie fokusa na inny komponent interfejsu po zaznaczeniu elementu na liśccie wyboru

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.2.2  oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 3.3.1 Identyfikacja błędu
----------------------------------------------------
### Identyfikacja treści
Pola zbierające dane z automatycznym wykrywaniem błędów i powiadomianiem.

### Instrukcja testowania
1.  Wprowadź nieprawidłowe wartości w polach zbierających dane, aby uruchomić automatyczne wykrywanie błędów, które powodują powiadomienia o błędach, np.:
    -   w polach oznaczonych jako wymagane
    -   w polach daty (format)
    -   w polach adresów internetowych (URL, e-mail)
    -   w polach przeznaczonych na hasło
2.  Jeśli błąd we wprowadzaniu danych zostanie wykryty automatycznie, sprawdź, czy powiadomienie o błędzie spełnia wszystkie poniższe warunki:
    -   użytkownik jest informowany o błędzie (albo natychmiast po opuszczeniu błędnie wypełnionego pola, albo przy próbie przesłania formularza) ORAZ
    -   błąd jest opisany w tekście, ORAZ
    -   element z błędem jest zidentyfikowany w tekście.


### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.3.1  oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 3.3.2 Etykiety lub instrukcje
-------------------------------------------------------
### Identyfikacja treści
1.  Znajdź wszystkie kontrolki formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne) związane z  kontrolkami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania
1.  Sprawdź, czy każdy komponent formularza zbierający dane ma etykietę(-y) lub instrukcje.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.3.2  oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 3.3.3 Sugestie korekty błędów
-------------------------------------------------------
### Identyfikacja treści
Pola zbierające dane z automatycznym wykrywaniem błędów i powiadomianiem.

### Instrukcja testowania
1.  Wprowadź nieprawidłowe wartości w polach zbierających dane, aby uruchomić automatyczne wykrywanie błędów, które powodują powiadomienia o błędach, np.:
    -   w polach oznaczonych jako wymagane
    -   w polach daty (format)
    -   w polach adresów internetowych (URL, e-mail)
    -   w polach przeznaczonych na hasło
2.  Przejrzyj wszystkie powiadomienia o błędach.
3.  Sprawdź, czy podano dodatkowe wskazówki, jak poprawić błędy w polach formularza, które nie zagroziłyby bezpieczeństwu ani przeznaczeniu treści (np. przykłady poprawnych danych, wskazówki, jak poprawić dane wprowadzone przez użytkownika).


### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.3.3 oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 3.3.4 Zapobieganie błędom (kontekst prawny, finansowy, związany z podawaniem danych
-------------------------------------------------------------------------------------------------------------
### Identyfikacja treści
Strony, które powodują powstanie zobowiązań prawnych użytkownika, strony transakcji finansowych, strony, za pomocą których użytkownik modyfikuje lub usuwa kontrolowane przez siebie dane w systemach przechowywania danych, strony, które przesyłają odpowiedzi użytkowników w testach (quizach).

### Instrukcja testowania
1.  Wypełnij pola formularza niezbędne do przesłania, wpisz błędne dane, poleć usunięcie istotnych danych.
2.  Sprawdź, czy przynajmniej jedno z poniższych założeń jest prawdziwe:
    1.  **Odwracalność**: Wprowadzenie danych jest odwracalne.
    2.  **Sprawdzanie**: Dane wprowadzone przez użytkownika są sprawdzane pod kątem błędów, a użytkownik ma możliwość wprowadzenia poprawek.
    3.  **Potwierdzenie**: Dostępny jest mechanizm sprawdzania, potwierdzania oraz korekty informacji przed jej ostatecznym wysłaniem.


### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 3.3.4 oraz wymaganie podstawowe nr 10 kończy się niepowodzeniem.

## Procedura testu dla KS 4.1.2 Nazwa, rola, wartość
----------------------------------------------------
Zobacz [5. Treść zmienna](testy/ICT_05_tresc-zmienna.md)

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------
-   W przypadku KS 3.3.1 dopuszczalne techniki obejmują: a) przeniesienie fokusa na komunikat o błędzie informujący użytkownika, że ​​poprzednie pole wymaga korekty i opisujące błąd, b) odświeżenie strony po przesłaniu formularza i wyświetlenie na górze strony opisów i lokalizacji błędów. **Uwaga**: Ponowne wyświetlenie formularza i wskazanie błędnych pól w formularzu jest niewystarczające, aby spełnić to wymaganie. Użytkownik nie powinien przeszukiwać formularza, aby dowiedzieć się, gdzie popełniono błędy.
-   W przypadku KS 3.3.4: ponieważ użytkownik może przejrzeć prosty, 1-stronicowy formularz przed naciśnięciem przycisku wysyłania na stronie, inny specjalny mechanizm weryfikacji poprawności nie jest wymagany.


## Techniki WCAG 2.1
---------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G115: Używanie znaczników semantycznych do oznaczania struktury](http://www.w3.org/TR/WCAG20-TECHS/G115.html) AND [H49: Używanie semantycznych znaczników do oznaczenia tekstu wyróżnionego lub specjalnego](http://www.w3.org/TR/WCAG20-TECHS/H49.html)
-   [G80: Zapewnienie przycisku przesyłania w celu zainicjowania zmiany kontekstu](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/G80)
-   [G13: Opisywanie, co się stanie, zanim nastąpi zmiana w formancie formularza, który powoduje zmianę kontekstu](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/G13)
-   [G131: Zapewnienie opisowych etykiet](http://www.w3.org/TR/WCAG20-TECHS/G131.html)
-   [H44: UUżywanie elementu label do kojarzenia etykiet tekstowych z formantami formularzy](http://www.w3.org/TR/WCAG20-TECHS/H44.html)
-   [H71: Zapewnienie opisu dla grup formantów formularzy przy użyciu elementów fieldset i legend](http://www.w3.org/TR/WCAG20-TECHS/H71.html)
-   [H65: Używanie atrybutu title do identyfikacji formantów formularzy, gdy nie można użyć elementu label](http://www.w3.org/TR/WCAG20-TECHS/H65.html)
-   [SCR19: Używanie zdarzenia onchange na wybranym elemencie bez powodowania zmiany kontekstu](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/SCR19)
-   [G83: Zapewnienie opisów tekstowych wskazujących wymagane pola, które nie zostały wypełnione](http://www.w3.org/TR/WCAG20-TECHS/G83.html)
-   [G85: Zapewnienie komunikatu tekstowego, gdy dane wprowadzane przez użytkownika nie mieszczą się w wymaganym formacie lub zakresie wartości](http://www.w3.org/TR/WCAG20-TECHS/G85.html)
-   [F36: Niespełnienie kryterium sukcesu 3.2.2 z powodu automatycznego przesłania formularza i prezentacji nowej treści bez uprzedniego ostrzeżenia, gdy ostatnie pole formularza ma wartość](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/F36)
-   [F37: Niespełnienie kryterium sukcesu 3.2.2 z powodu uruchomienia nowego okna bez uprzedniego ostrzeżenia po zmianie wyboru przycisku radiowego, pola wyboru lub listy wyboru](http://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/F37)


