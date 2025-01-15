---
title: 7. Właściwości zmysłowe
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 07-wlasciwosci-zmyslowe-doc
folder: testy/doc
---

## Wymagania dostępności
- {% include ks/1-1-1.md %}  
- {% include ks/1-3-3.md %}  
- {% include ks/1-4-1.md %} 

## Uzasadnienie metody testowej

Użytkownicy, których dotyczy ten wymóg, mogą być osobami widzącymi i nie są to wyłącznie użytkownicy technologii wspomagających, w tym osoby z zaburzeniami widzenia kolorów. Niektórzy użytkownicy korzystający z technologii wspomagających mogą nie mieć możliwości określenia kształtu, rozmiaru, lokalizacji lub postrzegania dźwięku. Aby określić adekwatność instrukcji lub treści i uwzględnić wszelkie ograniczenia postrzegania sensorycznego lub kolorów, wymagana jest kontrola wzrokowa. 

## Ograniczenia, założenia lub wyjątki
- KS 1.4.1 nie zabrania używania koloru i może być spełnione za pomocą dodatkowej wskazówki wizualnej (np. koloru i kształtu). Opisy alternatywne, które nie są dostępne wizualnie, nie przejdą tych testów.
- Zgodnie z [Objaśnieniem KS 1.4.1 Użycie koloru](https://wcag.irdpl.pl/understanding/uzycie-koloru.html), gdy sam kolor jest zastosowany do rozróżnienia łączy odwiedzonych i nieodwiedzonych, nie powoduje to niespełnienia tego kryterium sukcesu.
- Zgodnie z [Objaśnieniem KS 1.4.1 Użycie koloru](https://wcag.irdpl.pl/understanding/uzycie-koloru.html), użycie kolorów różniących się odcieniem i jasnością o współczynniku kontrastu 3:1 lub większym spełnia ten wymóg. Jeśli jednak poznanie treści zależy od zdolności użytkownika do dokładnego postrzegania lub rozróżniania określonego koloru, wymagany będzie dodatkowy wskaźnik wizualny, niezależnie od odpowiedniego współczynnika kontrastu między tymi kolorami.
-   KS 1.3.3 ma zastosowanie do instrukcji i nie może być spełnione poprzez podanie wielu cech sensorycznych (np. koloru i kształtu).
-   Test sygnałów dźwiękowych obejmuje krótkie dźwięki używane do powiadamiania użytkownika, takie jak sygnały potwierdzenia i powiadomienia o błędach. Dźwięk w mediach opartych na czasie jest omówiony w teście podstawowym [16. Tylko audio i tylko wideo](16-tylko-audio-tylko-wideo-doc.md).


## 7.A Procedura testowa użycia koloru
Identyfikator testu podstawowego: _7.A-Color_

### Identyfikacja treści
<p id="d7aIC">Znajdź treści, w których użyto koloru, aby przekazać znaczenie, wskazać działanie, zachęcić do odpowiedzi, wyróżnić element wizualnie lub oznaczyć błędy. Wyklucz kolory wskazujące łącza odwiedzone lub nieodwiedzone.</p>

### Instrukcja testowania
1.	Sprawdź, czy spełniony jest co najmniej jeden z poniższych warunków:
    1.  Treść wykorzystująca kolor do przekazania znaczenia zapewnia również widoczny na ekranie odpowiednik tekstowy opisujący kolor lub znaczenie przekazywane przez kolor, gdy użytkownik musi być w stanie dokładnie dostrzec lub rozróżnić określony kolor. [KS 1.4.1]
    2.  Treść wykorzystująca kolor do przekazania znaczenia zapewnia również inne wizualne odróżnienie (np. kształt, położenie, rozmiar, podkreślenie) z wyraźnym wskazaniem jego znaczenia, gdy użytkownik musi być w stanie dokładnie dostrzec lub rozróżnić określony kolor. [KS 1.4.1]
    3.  Treść wykorzystująca tylko różnicę w kolorach do przekazania znaczenia używa kolorów (odcieni) o współczynniku kontrastu 3:1 lub większym. Treść ta nie wymaga od użytkownika umiejętności dokładnego postrzegania lub rozróżniania konkretnego koloru. [KS 1.4.1]

### Wynik testów
<p id="d7aTR">Jeśli WSZYSTKIE powyższe testy zakończą się niepowodzeniem, test podstawowy <em>7.A-Color</em> kończy się niepowodzeniem.</p>

## 7.B  Procedura testowa użycia cech sensorycznych
Identyfikator testu podstawowego: _7.B-SensoryCharacteristics_

### Identyfikacja treści
<p id="d7bIC">Znajdź instrukcje (wskazówki) dotyczące rozumienia i obsługi treści, które opierają się na informacjach sensorycznych w celu przekazywania informacji. Mogą to być odwołania do kształtu, rozmiaru, wizualnej lokalizacji, orientacji lub dźwięku.</p>

### Instrukcja testowania
1.  Sprawdź, czy instrukcje zawierają dodatkowe informacje, które pozwalają na zlokalizowanie, rozpoznanie i zrozumienie elementu bez jakiejkolwiek wiedzy o jego kształcie, rozmiarze lub względnej pozycji. [KS 1.3.3] Na przykład:
    -   Aby zobaczyć zmiany, wybierz okrągły przycisk z napisem „Idź” (dodatkowa informacja o napisie na przycisku).
    -   Łącza po prawej stronie, z nagłówkiem „Zasoby”, zawierają dalsze informacje (dodatkowa informacja o nagłówku).
    -   Wybierz przycisk „Anuluj” w prawym dolnym rogu, aby zamknąć tę sesję (podana także nazwa przycisku).
2.  Sprawdź, czy wszelkie wskazówki dźwiękowe dostarczają również wskazówek wizualnych i/lub tekstowych określonych programowo. Na przykład,
    -   „Rozpocznij quiz po usłyszeniu sygnału dźwiękowego i pojawieniu się zegara”.

### Wynik testów

<p id="d7bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>7.B-SensoryCharacteristics</em> kończy się niepowodzeniem.</p>

## 7.C Procedura testowa użycia sygnałów dźwiękowych
Identyfikator testu bazowego: _7.C-AudibleCues_

### Identyfikacja treści
<p id="d7cIC">Znajdź wszelkie krótkie sygnały dźwiękowe/dźwiękowe, które służą jako powiadomienie dla użytkownika, takie jak sygnał dźwiękowy oznaczający wystąpienie błędu lub sygnał dźwiękowy wskazujący wiadomość przychodzącą.</p>

### Instrukcja testowania
1.  Sprawdź, czy tekst alternatywny, który opisuje przeznaczenie dźwięku, jest wyposażony we wskazówkę dźwiękową. [KS 1.1.1]<br />Na przykład:
    -   W wymaganym polu rozlega się krótki sygnał dźwiękowy i gwiazdka, aby powiadomić użytkownika, że pole musi zostać wypełnione.
    -   Gdy minutnik odlicza czas, rozlega się dzwonek, a na ekranie pojawia się komunikat „Zostały dwie minuty!”.

### Wynik testów
<p id="d7cTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>7.C-AudibleCues</em> kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   Treści, w których użyto koloru, muszą mieć dodatkową wskazówkę wizualną.
-   Instrukcje, które opierają się na charakterystyce sensorycznej, muszą zawierać wskazówkę niesensoryczną.
-   Wyświetlenie treści w skali szarości może pomóc w identyfikacji treści wykorzystujących wyłącznie kolor do przekazywania informacji.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G14.md %}
- {% include techniki/G96.md %}
- {% include techniki/G111.md %}
- {% include techniki/G182.md %}
- {% include techniki/G205.md %}
- {% include techniki/F14.md %}
- {% include techniki/F26.md %}
- {% include techniki/F73.md %}
- {% include techniki/F81.md %}


