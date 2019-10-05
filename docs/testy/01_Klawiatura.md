# 1. Dostęp z klawiatury

## Wymogi dostępności
-   [KS WCAG: 2.1.1 Klawiatura](https://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-keyboard-operable.html) – Cała treść oraz wszystkie zawarte w niej funkcjonalności dostępne są z interfejsu klawiatury, bez wymogu określonego czasu użycia poszczególnych klawiszy, poza tymi przypadkami, kiedy dana funkcja wymaga wprowadzenia informacji przez użytkownika w oparciu o ścieżkę ruchów, a nie w oparciu o punkty końcowe wejścia.
-   [KS WCAG: 2.1.2 Brak pułąpki na klawiaturę](https://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-trapping.html) – Jeśli fokus klawiatury można przemieścić do danego komponentu \[treści\] za pomocą interfejsu klawiatury, to może on być z niego usunięty również za pomocą interfejsu klawiatury, w przypadku gdy wymagane, a jeśli wówczas jest wymagane użycie czegoś więcej niż samych strzałek, tabulatora lub innych standardowych metod wyjścia, użytkownik musi otrzymać odpowiednią podpowiedź, w jaki sposób usunąć fokus z danego komponentu.

-   [Wymogi zgodności: 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) - Następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Brak pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.


## Uzasadnienie metody badania
Wymóg ten polega na użyciu klawiatury do sprawdzenia poprawności dostępu i kontroli działania wszystkich funkcji zawartości poprzez sprawdzenie użycia standardowych poleceń klawiaturowych (TAB, Spacja, Enter, Escape, itp.). Jeśli interfejs korzysta z niestandardowych poleceń klawiatury, interfejs musi wyraźnie dokumentować polecenia i uświadamiać użytkownikom, że polecenia istnieją.

Dostęp i kontrola za pomocą klawiatury obejmuje możliwość nawigowania do ORAZ z treści interaktywnych przy użyciu tylko klawiatury.

## Ograniczenia, założenia lub wyjątki
-   Ten test został napisany do wykonania na standardowej klawiaturze fizycznej dla komputera z systemem Windows. Chociaż można stosować emulatory klawiatury (takie jak klawiatury ekranowe, klawiatury alternatywne, wprowadzanie mowy itp.), instrukcje testowania mogą się różnić. Klawisze myszy (funkcja systemu Windows i Mac OS, która umożliwia sterowanie wskaźnikiem myszy za pomocą klawiatury) nie jest emulatorem klawiatury.

-   Uwagi do KS 2.1.1:
    -   Uwaga 1: jeśli do wprowadzania tekstu używa się pisma odręcznego, technika wprowadzania (pismo odręczne) wymaga wprowadzania danych zależnych od ścieżki, ale podstawowa funkcja (wprowadzanie tekstu) tego nie robi.
    -   Uwaga 2: Nie zabrania to i nie powinno zniechęcać do wprowadzania danych za pomocą myszy lub innych metod wprowadzania poza obsługą klawiatury.
-   Uwaga do KS 2.1.2:
    -   Uwaga 1: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu, może zakłócać zdolność użytkownika do korzystania z całej strony, cała treść strony internetowej (niezależnie od tego, czy jest używana do spełnienia innych kryteriów sukcesu, czy nie) musi spełniać to kryterium sukcesu. Patrz Wymogi zgodności: 5. Brak zakłóceń.
	

## Procedura testu dla KS 2.1.1 Klawiatura

### Identyfikacja treści
Cała funkcjonalność treści, która jest dostępna za pomocą myszki, musi być dostępna za pomocą klawiatury. Określić funkcjonalność widocznych i ukrytych elementów interaktywnego interfejsu (np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka pop-up/light box, ramki, iframes).


### Instrukcja testowania
1.  Sprawdź, czy wszystkie funkcje są dostępne i uruchamiane tylko za pomocą klawiatury.
    1.  Użyj klawiatury, aby wykonywać funkcje dostępne myszką (w tym rozwijane menu, pola formularzy, ujawnianie/ukrywanie treści, podpowiedzi ORAZ wszystkie elementy interfejsu interaktywnego).
        1.  Jeśli jakiś komponent interfejsu interaktywnego nie jest dostępny za pomocą klawiatury, sprawdź, czy na stronie znajduje się inny element sterujący o tej samej funkcjonalności, co klawiatura. (Wszystkie funkcje muszą spełniać to wymaganie).
2.  Sprawdź, czy poszczególne naciśnięcia klawiszy nie wymagają określonego czasu aktywacji.
    1.  Jeśli operacja wymaga określonego czasu poszczególnych naciśnięć klawiszy, sprawdź, czy na stronie znajduje się inny element sterujący o tej samej funkcjonalności, który nie wymaga określonego czasu działania. (Cała funkcjonalność musi być dostępna bez konieczności określania czasu dla poszczególnych naciśnięć klawiszy).


### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.1.1 oraz wymaganie podstawowe nr 1 kończy się niepowodzeniem.

## Procedura testu dla KS 2.1.2 Brak pułapki na klawiaturę

### Identyfikacja treści
Widoczne i ukryte elementy interaktywnego interfejsu (łącza, pola formularzy, rozwijane menu, pokazywanie/ukrywanie treści, widoki drzewa, wyskakujące okienka/light box, ramki, iframe itp.), do których można nawigować za pomocą klawiatury.

### Instrukcja testowania
1.  Sprawdź, czy fokus można zawsze przenieść z elementu na inny. Nie może być ŻADNEJ “PUŁAPKI”, która zakłóca nawigację klawiaturą.
    1.  W przypadku znalezienia pułapki klawiaturowej należy sprawdzić wszelką pomoc (pomoc kontekstową lub pomoc aplikacji) oraz dokumentację w celu powiadomienia o dostępnych alternatywnych poleceniach klawiaturowych (np. o niestandardowym sterowaniu klawiaturą, klawiszach dostępu, klawiszach skrótów).
    2. Jeśli do nawigacji z komponentu lub zestawu komponentów wymagane są niestandardowe polecenia klawiaturowe, sprawdź, czy te polecenia działają.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.1.2, 5 wymóg zgodności oraz wymaganie podstawowe nr 1 kończy się niepowodzeniem.

## Porada: Wskazówki dotyczące usprawniania procesu testów

-   Polecenia klawiaturowe obejmują standardowe i wszelkie niestandardowe polecenia klawiaturowe.
-   Dostęp z klawiatury dla atrybutu title jest możliwy w Internet Explorerze 11 dla Windows 8.1 i 10. Przydatne może być powiadomienie testerów, aby zatrzymywali się podczas tabulacji interaktywnych treśc nad atrybutem TITLE, aby sprawdzić, czy zawartość TITLE jest ujawniana podczas testowania nawigacji za pomocą klawiatury.
-   Ten test można połączyć z testami widoczności fokusa i kolejności tabulacji.
-   Wskazówki i techniki wyszukiwania ukrytych treści mogą być potrzebne testerom.
-   Przydatne może być udostępnienie testerom przewodnika po klawiaturze Windows.
-   Treść, która zostanie uznana za niezgodną z KS 2.1.1, może zostać oznaczona do dalszej analizy pod kątem wyjątku z Sekcji 508, jeżeli „podstawowa funkcja wymaga danych wejściowych, które zależą od ścieżki ruchu użytkownika, a nie tylko punktów końcowych”..


## Techniki WCAG 2.1
-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

    -   [G202: Zapewnienie sterowania klawiaturą dla wszystkich funkcji](http://www.w3.org/TR/WCAG20-TECHS/G202.html)
    -   [G21: Zapewnienie, że użytkownicy nie zostaną uwięzieni w treści](http://www.w3.org/TR/WCAG20-TECHS/G21.html)

-------------------------------------------------
[Początek/Spis treści](index.md)    |    [[Następny]](02WidocznyFokus.md)
