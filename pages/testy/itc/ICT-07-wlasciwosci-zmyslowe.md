---
title: 7. Właściwości zmysłowe


sidebar: testy_sidebar
permalink: ICT-07-wlasciwosci-zmyslowe
folder: testy/itc
---

## Wymagania dostępności
- {% include ks/1-4-1.md %}  
- {% include ks/1-3-3.md %}  

## Uzasadnienie metody badania
------------------------------
Użytkownicy, których dotyczy ten wymóg, nie ograniczają się tylko do użytkowników technologii wspomagających, w tym użytkowników ze ślepotą barw. Inni użytkownicy korzystający z technologii wspomagających mogą nie mieć możliwości określenia kształtu, rozmiaru, lokalizacji lub postrzegania dźwięku. Wymagana jest kontrola wzrokowa, aby określić adekwatność instrukcji lub treści, aby uwzględnić wszelkie ograniczenia postrzegania sensorycznego lub kolorów.

## Ograniczenia, założenia lub wyjątki
-   Wymóg ten nie zabrania używania kolorów lub cech sensorycznych do dostarczania informacji, wskazówek lub instrukcji. Jednak należy ich używać w połączeniu z kontekstowymi, tekstowymi i/lub innymi wizualnymi wskazówkami.
-   To nie jest test alternatywnych opisów tekstowych, wymaganych i wykorzystywanych przez technologie wspomagajace. Użytkownicy ze ślepotą barw zazwyczaj nie używają technologii wspomagajacych.


## Procedura testu dla KS 1.4.1 Użycie koloru
---------------------------------------------
### Identyfikacja treści
Treść, która od koloru uzależnia znaczenie informacji, tylko kolorem sygnalizuje bądź wskazuje akcję, podpowiada reakcję, wyróżnia element wizualny lub identyfikuje błędy.


### Instrukcja testowania
1.  Sprawdź, czy jest spełniony co najmniej jeden z poniższych warunków:
    1.  Element wykorzystujący kolor do przekazania znaczenia zapewnia również widoczny na ekranie odpowiednik tekstowy opisujący kolor lub znaczenie przekazywane przez kolor.
    2.  Element wykorzystujący kolor do przekazania znaczenia zapewnia również (np. kształt, położenie, rozmiar, podkreślenie) z wyraźnym wskazaniem jego znaczenia.

### Wynik testów
Jeżeli OBIE powyższe próby zakończą się niepowodzeniem, wówczas test KS 1.4.1 oraz wymaganie podstawowe nr 7 kończy się niepowodzeniem.

## Procedura testu dla KS 1.3.3 Właściwości zmysłowe
----------------------------------------------------
### Identyfikacja treści
Zidentyfikuj instrukcje dotyczące rozumienia i obsługi treści, które wykorzystują informacje sensoryczne do przekazywania informacji. Może to obejmować odwołania do kształtu, rozmiaru, wizualnej lokalizacji, orientacji lub dźwięku.

### Instrukcja testowania
1.  Sprawdź, czy instrukcje zawierają dodatkowe informacje, które pozwalają na lokalizację, identyfikację i zrozumienie elementu bez jakiejkolwiek wiedzy o jego kształcie, rozmiarze lub względnej pozycji. Na przykład,
    -   Aby zobaczyć zmiany, wybierz okrągły przycisk z napisem „Idź” (dodatkowa informacja o napisie na przycisku).
    -   Linki po prawej stronie, z nagłówkiem „Zasoby”, zawierają dalsze informacje (dodatkowa informacja o nagłówku).
    -   Wybierz przycisk \[Anuluj\] w prawym dolnym rogu, aby zamknąć tę sesję (podana nazwa przycisku).
2.  Sprawdź, czy wszelkie wskazówki dźwiękowe dostarczają wskazówek wizualnych i/lub tekstowych określonych programowo. Na przykład,
    -   „Rozpocznij quiz po usłyszeniu sygnału dźwiękowego i pojawieniu się zegara”.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.3.3 oraz Wymaganie podstawowe nr 7 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------
-   Treść, która używa kolorów z innymi różnicami wizualnymi, musi także zapewniać wskazówki tekstowe, aby przekazać te same informacje, aby spełnić zarówno KS 1.3.3, jak i 1.4.1; dlatego zaleca się połączenie obu wymagań w jednym teście.
-   Powiązane testy mogą obejmować treść dynamiczną, obrazy, łącza i strony alternatywne.
-   Wyświetlenie treści w skali szarości może pomóc w identyfikacji treści wykorzystujących wyłącznie kolor do przekazywania informacji.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G14.md %}
- {% include techniki/G205.md %}
- {% include techniki/G182.md %}
- {% include techniki/G111.md %}
- {% include techniki/F73.md %}
- {% include techniki/F81.md %}
- {% include techniki/G96.md %}
- {% include techniki/F14.md %}
- {% include techniki/F26.md %}
