---
title: 9. Błyskanie (dokument)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 09-blyskanie-doc
folder: testy/doc
---

## Wymagania dostępności
- {% include ks/2-3-1.md %}
-   [5.2 Wymagania zgodności: Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści w dokumencie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Bez pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Pauza, zatrzymanie, ukrycie.

## Uzasadnienie metody testowej
Miganie może być spowodowane czynnikami niezależnymi od autorów (np. działaniem wyświetlacza użytkownika, renderowaniem obrazu przez komputer lub problemami z łącznością). Nie ma niezawodnego, bezpłatnego i powszechnie dostępnego rozwiązania do określania wynikowej częstotliwości migania dla tego rodzaju czynników.

Ten test dotyczy migania powodowanego przez samą treść, w tym:
- określanie szybkości migania na podstawie informacji dostępnych programowo
- określanie wymiarów w pikselach migającego elementu
- określenie, czy [względna luminancja](https://www.w3.org/TR/2008/REC-WCAG20-20081211/#relativeluminancedef)  zmienia się o więcej niż 10% dla „pary przeciwstawnych przejść zawierających ostrą/nasyconą czerwień”.
- określanie, czy migające elementy zawierają [nasyconą czerwień](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#general-thresholddef)

## Ograniczenia, założenia lub wyjątki
- Użytkownicy mogą wyświetlać treści w rozdzielczości lub z odległości znacznie różniącej się od przewidywanej (założonej) rozdzielczości i odległości oglądania.
- Do celów tego testu podstawowego terminy miganie i mruganie mogą być używane jako synonimy terminu błysk.
- Migające elementy, które spełniają to wymaganie, nadal muszą spełniać wymagania KS 2.2.2 Pauza, zatrzymanie, ukrycie, jeśli miganie trwa dłużej niż 5 sekund ([Wymaganie podstawowe 21. Zdarzenia czasowe](21-zdarzenia-czasowe-doc.md)).
- Uwaga z KS 2.3.1:
    - Uwaga 1: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi korzystanie z całego dokumentu, cała treść dokumentu (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić to kryterium sukcesu. Zobacz: [Wymogi zgodności: Bez zakłóceń](https://wcag.irdpl.pl/guidelines/22/#cc5).

## 9.A Procedura testowa dla trzech błysków lub poniżej progu
Identyfikator testu bazowego: _9.A-Flashes_

### Identyfikacja treści

Wizualnie określ zawartość, która [błyska](https://wcag.irdpl.pl/understanding/trzy-blyski-lub-wartosci-ponizej-progu.html#dfn-blysk).

### Instrukcja testowania
1. Ustaw program użytkownika na standardowym poziomie powiększania, np. 100% w przeglądarce.
2.	Jeśli istnieje opcja wyświetlenia większej wersji treści, takiej jak tryb pełnoekranowy, przetestuj większą wersję. Jeśli istnieje opcja zapętlenia lub powtórzenia zawartości, przetestuj wersję zapętloną.
3.	Sprawdź, czy jedna z poniższych sytuacji jest prawdziwa w odniesieniu do treści: [KS 2.3.1]
   - Częstotliwość jest mniejsza lub równa 3 błyskom w ciągu jednej sekundy (3 Hz).
   - Częstotliwość przekracza 3 Hz lub nie można jej określić, a spełniony jest co najmniej jeden z poniższych warunków:
    1.  Łączny obszar błysków występujących jednocześnie zajmuje nie więcej niż prostokąt o wymiarach 341 x 256 pikseli w dowolnym miejscu wyświetlanego obszaru ekranu, gdy treść jest wyświetlana w rozdzielczości 1024 x 768 pikseli.
    2.  Błysk nie obejmuje „błysków ogólnych” (para przeciwstawnych zmian względnej luminancji wynoszących 10% lub więcej maksymalnej względnej luminancji (1,0), w przypadku gdy względna jasność ciemniejszego obrazu jest mniejsza niż 0,80; i gdzie „para przeciwstawnych zmian” oznacza wzrost, po którym następuje spadek, lub spadek, po którym następuje wzrost)
    3.  błysk nie zawiera żadnej „pary przeciwstawnych przejść obejmujących nasyconą czerwień” (para przeciwstawnych przejść, gdzie jedno przejście jest do lub ze stanu o wartości R/(R + G + B) większej lub równej 0,8, a różnica między stanami jest większa niż 0,2 (bez jednostek) na diagramie chromatyczności CIE 1976 UCS. ([ISO_9241-391](https://www.iso.org/standard/56350.html))

### Wynik testów
<p id="d9aTR">Jeśli wszystkie powyższe testy zakończą się niepowodzeniem, test podstawowy <em>9.A-Flashes</em> kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
- Jeśli treść będzie będą wyświetlane lub oglądane w znacznie różniących się rozmiarach lub odległościach (np. treść responsywna przeznaczona do wyświetlania na komputerach stacjonarnych, urządzeniach mobilnych lub innych wyświetlaczach), treść powinna być oceniona dla każdego scenariusza.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G19.md %}
- {% include techniki/G176.md %}

