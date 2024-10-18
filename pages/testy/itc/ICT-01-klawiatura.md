---
title: 1. Dostęp z klawiatury


sidebar: testy_sidebar
permalink: ICT-01-klawiatura
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/2-1-1.md %}  
- {% include ks/2-1-2.md %}  

-   [Wymaganie zgodności: 5. Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Bez pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Pauza, zatrzymanie, ukrycie.


## Objaśnienie metody badawczej
To wymaganie opiera się na użyciu klawiatury, aby sprawdzić dostęp i możliwość sterowania wykonaniem wszystkich funkcji treści za pomocą samej klawiatury, korzystając ze standardowych poleceń klawiaturowych (TAB, Spacja, Enter, Escape, itp.). Jeśli interfejs wymaga korzystania z niestandardowych poleceń klawiatury, interfejs musi wyraźnie dokumentować te polecenia i informować użytkowników, że polecenia istnieją.

Dostęp i sterowanie za pomocą klawiatury obejmuje możliwość nawigowania do ORAZ z treści interaktywnych przy użyciu  samej klawiatury.

## Ograniczenia, założenia lub wyjątki
-   Ten test został napisany do wykonania na standardowej klawiaturze fizycznej dla komputera z systemem Windows. Chociaż można wykorzystywać emulatory klawiatury (takie jak klawiatury ekranowe, klawiatury alternatywne, wprowadzanie mowy itp.), instrukcje testowania mogą się różnić. Klawisze myszy (funkcja systemu Windows i Mac OS, która umożliwia sterowanie wskaźnikiem myszy za pomocą klawiatury) nie jest emulatorem klawiatury.

-   Uwagi do KS 2.1.1:
    -   *Uwaga 1*: Ten wyjątek dotyczy danej funkcji, a nie techniki wprowadzania. Na przykład, jeśli do wprowadzania tekstu używa się pisma odręcznego, technika wprowadzania (pismo odręczne) wymaga wprowadzenia informacji w&nbsp;oparciu o ścieżkę, jednak powiązana z tym funkcja (wprowadzenie tekstu) już tego nie wymaga.
    -   *Uwaga 2*: To nie powinno blokować ani ograniczać użycia interfejsu innymi metodami niż klawiatura, np. za pomocą myszki.
-   Uwaga do KS 2.1.2:
    -   *Uwaga 1*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej strony, cała treść danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: [Wymaganie zgodności: 5. Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5).

## Procedura testowa dla KS 2.1.1 Klawiatura

Identyfikator testu bazowego: *1.A-KeyboardAccess*

### Identyfikacja treści
Wszystkie funkcje treści, które są dostępne za pomocą myszy, muszą być dostępne za pomocą klawiatury. Określ funkcjonalność widocznych i ukrytych interaktywnych komponentów interfejsu (np. łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka/lightboxy, ramki i ramki iframe) dostępnych za pomocą myszy (najechanie kursorem i/lub kliknięcie).

### Instrukcje testowania
1.  Sprawdź, czy wszystkie funkcje są dostępne i uruchamiane tylko za pomocą klawiatury.
    1.  Użyj klawiatury, aby wykonywać funkcje dostępne za pomocą myszy (w tym rozwijane menu, pola formularzy, odsłanianie/ukrywanie treści, podpowiedzi **ORAZ** wszystkie interaktywne komponenty interfejsu).
        1.  Jeśli jakiś interaktywny komponent interfejsu nie jest dostępny za pomocą klawiatury, sprawdź, czy na stronie znajduje się inna kontrolka z tą samą funkcjonalnością, która jest dostępna za pomocą klawiatury. (Wszystkie funkcje muszą spełniać to wymaganie).
2.  Sprawdź, czy poszczególne naciśnięcia klawiszy nie wymagają określonego czasu aktywacji.
    1.  Jeśli operacja wymaga określonego czasu poszczególnych naciśnięć klawiszy, sprawdź, czy na stronie znajduje się inna kontrolka z tą samą funkcjonalnością, która nie wymaga określonych czasów działania. (Wszystkie funkcje muszą być dostępne bez konieczności określania czasu działania poszczególnych naciśnięć).


### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test *1.A-KeyboardAccess* kończy się niepowodzeniem.

## Procedura testu dla KS 2.1.2 Bez pułapki na klawiaturę

Identyfikator testu bazowego: *1.B-NoKeyboardTrap*


### Identyfikacja treści
Wszystkie komponenty, na których można ustawić fokus klawiatury.

### Instrukcja testowania
1.  Sprawdź, czy fokus można zawsze przenieść z elementu na inny. Nie może być ŻADNEJ „PUŁAPKI”, która zakłóca nawigację klawiaturą. [KS 2.1.2, Wymaganie zgodności 5]
    1.  Jeśli zostanie znaleziona pułapka klawiaturowa, sprawdź wszelką pomoc (pomoc kontekstową lub pomoc aplikacji) oraz dokumentację, aby znaleźć informacje o dostępnych alternatywnych poleceniach klawiaturowych (np. o niestandardowym sterowaniu klawiaturą, klawiszach dostępu, skrótach klawiaturowych).
    2. Jeśli do nawigacji z komponentu lub zestawu komponentów wymagane są niestandardowe polecenia klawiaturowe, sprawdź, czy te polecenia działają.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test *1.B-NoKeyboardTrap* kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

- Komponenty, na których można ustawić fokus klawiatury, to łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka/lightboxy, ramki i ramki iframe, do których można nawigować za pomocą klawiatury. Komponenty, na których można ustawić fokus, mogą być również „ukryte”, znajdować się poza ekranem, nie mieć widocznych wskaźników fokusu.  
-   Polecenia klawiaturowe obejmują standardowe i wszelkie niestandardowe polecenia klawiaturowe.
-   Dostęp z klawiatury dla atrybutu `title` jest możliwy w programie Internet Explorerze 11 dla systemu Windows 8.1 i 10. Przydatne może być powiadomienie testerów, aby zatrzymywali się na chwilę podczas nawigowania klawiszem Tab, aby sprawdzić, czy podczas nawigacji jest ujawniana treść `title`.
-   Ten test można połączyć z testami widoczności fokusu i kolejności tabulacji.
-   Testerzy mogą potrzebować wskazówek i podpowiedzi technik wyszukiwania ukrytych treści.
-   Przydatne może być udostępnienie testerom przewodnika po klawiaturze Windows.
-   Treść, która zostanie uznana za niezgodną z KS 2.1.1, może zostać oznaczona do dalszej analizy pod kątem wyjątku z Sekcji 508, jeżeli „podstawowa funkcja wymaga wprowadzenia danych, które zależy od ścieżki ruchu użytkownika, a nie tylko punktów końcowych”.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G21.md %}
- {% include techniki/G202.md %}
- {% include techniki/F10.md %}
- {% include techniki/F54.md %}