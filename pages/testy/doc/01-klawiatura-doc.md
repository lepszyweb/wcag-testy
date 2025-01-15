---
title: "1. Dostęp z klawiatury (Dokumenty)"
last_updated: 15 stycznia 2025

sidebar: testy_sidebar
permalink: 01-klawiatura-doc
folder: testy/doc
---

## Wymagania dostępności
- {% include ks/2-1-1.md %}  
- {% include ks/2-1-2.md %}  
-   [Wymaganie zgodności: 5. Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Bez pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Pauza, zatrzymanie, ukrycie.

## Uzasadnienie metody testowej

To wymaganie opiera się na użyciu klawiatury w celu sprawdzenia dostępu i możliwości sterowania wykonaniem wszystkich funkcji treści w pierwszej kolejności poprzez sprawdzenie użycia standardowych poleceń klawiaturowych (<kbd>TAB</kbd>, <kbd>Spacja</kbd>, <kbd>Enter</kbd>, <kbd>Escape</kbd>, itp.). Jeśli w dokumencie użyto niestandardowych poleceń klawiaturowych, musi on wyraźnie udokumentować te polecenia i uświadomić użytkownikom, że polecenia te istnieją.

Dostęp i sterowanie za pomocą klawiatury obejmuje możliwość przechodzenia DO **oraz** Z treści interaktywnych przy użyciu  samej klawiatury.

## Ograniczenia, założenia lub wyjątki
-   Ten test został napisany do wykonania na standardowej klawiaturze fizycznej dla komputera z systemem Windows. Chociaż można wykorzystywać emulatory klawiatury (takie jak klawiatury ekranowe, klawiatury alternatywne, wprowadzanie mowy itp.), instrukcje testowania mogą się różnić. Klawisze myszy (funkcja systemu Windows i Mac OS, która umożliwia sterowanie wskaźnikiem myszy za pomocą klawiatury) nie są emulatorem klawiatury.
-   Uwagi do KS 2.1.1:
    -   *Uwaga 1*: Ten wyjątek dotyczy danej funkcji, a nie techniki wprowadzania danych. Na przykład, jeśli do wprowadzania tekstu używa się pisma odręcznego, technika wprowadzania (pismo odręczne) wymaga wprowadzenia informacji w oparciu o ścieżkę, jednak powiązana z tym funkcja (wprowadzenie tekstu) już tego nie wymaga.
    -   *Uwaga 2*: To nie blokuje i nie powinno zniechęcać do wprowadzania danych za pomocą myszy lub innych metod wprowadzania danych oprócz obsługi za pomocą klawiatury
-   Uwaga do KS 2.1.2:
    -   *Uwaga 1*: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu, może utrudnić użytkownikowi korzystanie z całego dokumentu,  cała zawartość dokumentu (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Więcej informacji: [Wymaganie zgodności: 5. Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5).


## 1.A Procedura testowa dostępu z klawiatury
Identyfikator testu bazowego: *1.A-KeyboardAccess*

### Identyfikacja treści
<p id="d1aIC">Wszystkie funkcje treści, które są dostępne za pomocą myszy, muszą być dostępne za pomocą klawiatury. Określ funkcjonalności widocznych i ukrytych interaktywnych elementów dokumentu (łącza, pola formularzy, rozwijane menu, pokazywanie/ukrywanie treści, widoki drzewa, wyskakujące okienka itp.) dostępnych za pomocą myszy (najechanie kursorem i/lub kliknięcie).</p>

### Instrukcje testowania
1.  Sprawdź, czy wszystkie funkcje są dostępne i uruchamiane tylko za pomocą klawiatury. [KS 2.1.1]
    1.  Użyj klawiatury, aby wykonywać funkcje dostępne za pomocą myszy (w tym rozwijane menu, pola formularzy, odsłanianie/ukrywanie treści, podpowiedzi **ORAZ** wszystkie interaktywne komponenty interfejsu).
        1.  Jeśli jakiś interaktywny komponent interfejsu nie jest dostępny za pomocą klawiatury, sprawdź, czy istnieje inna kontrolka pełniąca tę samą funkcję. (Wszystkie funkcje muszą spełniać to wymaganie).
2.  Sprawdź, czy poszczególne naciśnięcia nie wymagają określonego czasu aktywacji. [KS 2.1.1]
    1.  Jeśli operacja wymaga określonego czasu poszczególnych naciśnięć klawiszy, sprawdź, czy w dokumencie znajduje się inna kontrolka pełniąca tę samą funkcję, która nie wymaga określonego czasu działania. (Wszystkie funkcje muszą być dostępne bez konieczności określania czasu działania poszczególnych naciśnięć).


### Wynik testów
<p id="d1aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy <em>1.A-KeyboardAccess</em> kończy się niepowodzeniem.</p>

## 1B. Procedura testowa pułapki na klawiaturę

Identyfikator testu bazowego: *1.B-NoKeyboardTrap*

### Identyfikacja treści
<p id="d1bIC">Wszystkie komponenty, na których można ustawić fokus klawiatury.</p>

### Instrukcja testowania
1.  Sprawdź, czy fokus można zawsze przenieść z elementu na inny. Nie może być ŻADNEJ „PUŁAPKI”, która zakłóca nawigację klawiaturą. [KS 2.1.2, Wymaganie zgodności 5]
    1.  Jeśli zostanie znaleziona pułapka klawiaturowa, sprawdź wszelką pomoc (pomoc kontekstową lub pomoc aplikacji) oraz dokumentację, aby znaleźć informacje o dostępnych alternatywnych poleceniach klawiaturowych (np. o niestandardowym sterowaniu klawiaturą, klawiszach dostępu, skrótach klawiaturowych).
    2. Jeśli do nawigacji z komponentu lub zestawu komponentów wymagane są niestandardowe polecenia klawiaturowe, sprawdź, czy te polecenia działają.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test podstawowy *1.B-NoKeyboardTrap* kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

- Komponenty, na których można ustawić fokus klawiatury, to łącza, pola formularzy, menu rozwijane, odsłanianie/ukrywanie treści, widoki drzewa, wyskakujące okienka. Komponenty, na których można ustawić fokus, mogą być również „ukryte”, znajdować się poza ekranem, nie mieć widocznych wskaźników fokusu.  
-   Polecenia klawiaturowe obejmują standardowe i wszelkie niestandardowe polecenia klawiaturowe.
-   Ten test można połączyć z testami widoczności fokusu klawiatury.
-   Testerzy mogą potrzebować wskazówek i podpowiedzi technik wyszukiwania ukrytych treści.
-   Przydatne może być udostępnienie testerom przewodnika po klawiaturze Windows.
-   Treść, która zostanie uznana za niezgodną z KS 2.1.1, może zostać oznaczona do dalszej analizy pod kątem wyjątku z Sekcji 508, jeżeli „podstawowa funkcja wymaga wprowadzenia danych, które zależy od ścieżki ruchu użytkownika, a nie tylko punktów końcowych”.


## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G21.md %}
- {% include techniki/G202.md %}
- {% include techniki/F10.md %}
- {% include techniki/F54.md %}