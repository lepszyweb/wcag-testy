---
title: 9. Błyskanie


sidebar: testy_sidebar
permalink: ICT-09-blyskanie
folder: testy/itc
---
## Wymagania dostępności
- {% include ks/2-3-1.md %}
-   [Wymaganie zgodności: 5. Bez zakłóceń](https://www.w3.org/Translations/WCAG21-pl/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Bez pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Pauza, zatrzymanie, ukrycie.

## Opis metody testowej
Miganie może być spowodowane czynnikami niezależnymi od autorów (np. działaniem wyświetlacza użytkownika, renderowaniem obrazu przez komputer lub problemami z łącznością). Nie ma niezawodnego, bezpłatnego i powszechnie dostępnego rozwiązania do określania wynikowej częstotliwości migania dla tego rodzaju czynników.

Ten test dotyczy migania powodowanego przez samą treść, w tym:
- Określanie szybkości migania na podstawie informacji dostępnych programowo
- Określanie wymiarów w pikselach migającego elementu
- Określenie, czy [względna luminancja](https://www.w3.org/TR/2008/REC-WCAG20-20081211/#relativeluminancedef)  zmienia się o więcej niż 10% dla „pary przeciwstawnych przejść zawierających ostrą/nasyconą czerwień”.
- Określanie, czy migające elementy zawierają [nasyconą czerwień](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#general-thresholddef)


## Ograniczenia, założenia lub wyjątki
- użytkownicy mogą wyświetlać treści w rozdzielczości lub z odległości znacznie różniącej się od przewidywanej (założonej) rozdzielczości i odległości oglądania.
- Do celów tego testu podstawowego terminy miganie i mruganie mogą być używane jako synonimy terminu błysk.
- Migające elementy, które spełniają to wymaganie, nadal muszą spełniać wymagania KS 2.2.2 Pauza, zatrzymanie, ukrycie, jeśli miganie trwa dłużej niż 5 sekund ([Wymaganie podstawowe 21. Limity czasu](ICT_21_limity-czasu.md)).
- Uwaga z KS 2.3.1:
    - Uwaga 1: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi korzystanie z całej strony, cała treść danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić to kryterium sukcesu. Zobacz: [Wymogi zgodności: Bez zakłóceń](https://wcag.irdpl.pl/guidelines/22/#cc5).

	

## 9.A Procedura testowa dla trzech błysków lub poniżej progu
Identyfikator testu bazowego: _9.A-Flashes_

### Identyfikacja treści
Wizualnie określ zawartość, która [błyska](https://wcag.irdpl.pl/understanding/trzy-blyski-lub-wartosci-ponizej-progu.html#dfn-blysk) (poza wyjątkami odnotowanymi w sekcji Ograniczenia, założenia lub wyjątki powyżej).

### Instrukcja testowania
1. Ustaw program użytkownika na standardowym poziomie powiększania, np. 100% w przeglądarce.
2.	Jeśli istnieje opcja wyświetlenia większej wersji treści, takiej jak tryb pełnoekranowy, przetestuj większą wersję. Jeśli istnieje opcja zapętlenia lub powtórzenia zawartości, przetestuj wersję zapętloną.
3.	Sprawdź, czy jedna z poniższych sytuacji jest prawdziwa w odniesieniu do treści: [SC 2.3.1]
   - Częstotliwość jest mniejsza lub równa 3 błyskom w ciągu jednej sekundy (3 Hz).
   - Częstotliwość przekracza 3 herce lub nie można jej określić, a spełniony jest co najmniej jeden z poniższych warunków:
    1.  Łączny obszar błysków występujących jednocześnie zajmuje nie więcej niż prostokąt o wymiarach 341 x 256 pikseli w dowolnym miejscu wyświetlanego obszaru ekranu, gdy treść jest wyświetlana w rozdzielczości 1024 x 768 pikseli.
    2.  Błysk nie obejmuje „błysków ogólnych” (para przeciwstawnych zmian względnej luminancji wynoszących 10% lub więcej maksymalnej względnej luminancji (1,0), w przypadku gdy względna jasność ciemniejszego obrazu jest mniejsza niż 0,80; i gdzie „para przeciwstawnych zmian” oznacza wzrost, po którym następuje spadek, lub spadek, po którym następuje wzrost)
    3.  błysk nie zawiera żadnej „pary przeciwstawnych przejść obejmujących nasyconą czerwień” (para przeciwstawnych przejść, gdzie jedno przejście jest do lub ze stanu o wartości R/(R + G + B) większej lub równej 0,8, a różnica między stanami jest większa niż 0,2 (bez jednostek) na diagramie chromatyczności CIE 1976 UCS. [[ISO_9241-391]])

### Wynik testów
Wyniki testów
Jeśli wszystkie powyższe testy zakończą się niepowodzeniem, test podstawowy _9.A-Flashes_ kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
- Jeśli treść będzie wyświetlana lub wyświetlana w znacznie różnych rozmiarach lub odległościach (np. treść responsywna przeznaczona do wyświetlania na pulpicie, w telefonie komórkowym i/lub innych wyświetlaczach), treść należy ocenić dla każdego scenariusza.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G15.md %}
- {% include techniki/G19.md %}
- {% include techniki/G176.md %}


