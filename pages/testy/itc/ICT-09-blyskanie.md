---
title: 9. Błyskanie


sidebar: testy_sidebar
permalink: ICT-09-blyskanie
folder: testy/itc
---
## Wymagania dostępności
- {% include ks/2-3-1.md %}
-   [Wymogi zgodności: 5. Brak zakłóceń](https://www.w3.org/TR/WCAG20/#cc5) - Następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony: 1.4.2 - Kontrola odtwarzania dźwięku, 2.1.2 - Brak pułapki na klawiaturę, 2.3.1 Trzy błyski lub wartości poniżej progu, 2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie.

## Uzasadnienie metody badania
Błyskanie może być spowodowane czynnikami niezależnymi od autorów (np. działaniem wyświetlacza użytkownika, renderowaniem obrazu przez komputer lub problemami z łącznością). Nie ma niezawodnego, ogólnodostępnego lub powszechnie dostępnego rozwiązania do określania wynikowej częstotliwości błyskania dla tego rodzaju czynników.

Ten test rozwiązuje problem błyskania spowodowanego przez samą treść, w tym:
- Określanie szybkości błyskania na podstawie informacji dostępnych programowo
- Określenie, czy łączny obszar błysków pojawiających się jednocześnie nie przekracza .006 sterydianów w obrębie 10 stopni pola widzenia monitora (25% na każde 10 stopni pola widzenia monitora) dla osoby patrzącej na monitor z przeciętnej odległości.
- Określenie, czy [względna luminancja](https://www.w3.org/TR/2008/REC-WCAG20-20081211/#relativeluminancedef)  zmienia się o więcej niż 10% dla „pary przeciwstawnych przejść zawierających ostrą/nasyconą czerwień”.
- Określanie, czy migające elementy zawierają [nasyconą czerwień](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#general-thresholddef)

## Ograniczenia, założenia lub wyjątki
- Możliwe jest, że użytkownicy będą mogli oglądać zawartość w rozdzielczości lub z odległości znacznie różniącej się od rozdzielczości i odległości przewidywanej (założonej).
- Do celów tego testu podstawowego terminy miganie i mruganie mogą być używane synonimicznie z terminem błysk, blyskanie.
- Migające elementy, które spełniają ten wymóg, nadal muszą spełniać wymagania KS 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie, jeśli miganie trwa dłużej niż 5 sekund ([Wymaganie podstawowe 21. Limity czasu](testy/ICT_21_limity-czasu.md)).
- Uwaga z KS 2.3.1:
    - Uwaga 1: Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi skorzystanie z całej strony, cała zawartość danej strony (bez względu na to, czy spełnia inne kryteria, czy nie) musi spełnić powyższe kryterium. Zobacz: Wymagania zgodności: Brak zakłóceń.

## Procedura testu dla KS 2.3.1 Trzy błyski lub wartości poniżej progu

### Identyfikacja treści
Wizualnie określ zawartość, która [błyska](https://www.w3.org/TR/UNDERSTANDING-WCAG20/seizure-does-not-violate.html#flash-def) (poza wyjątkami odnotowanymi w zekcji Ograniczenia, założenia lub wyjątki powyżej).


### Instrukcja testowania
1.  Określ częstotliwość błyskania. Jeśli częstotliwość błyskania wynosi 3 Hz lub mniej (trzy błyski w ciągu jednej sekundy), dalsze badanie nie jest konieczne.
2.  Jeśli zawartość miga powyżej 3 Hz lub nie można ustalić częstotliwości, sprawdź, czy spełnia ona jedną z następujących warunków:
    1.  Łączny obszar błysków pojawiających się jednocześnie w dowolnym kącie widzenia 10 stopni, jest mniejszy niż odpowiednik „małego bezpiecznego obszaru” (tj. mniejszy niż 25% na każde 10 stopni pola widzenia monitora) dla osoby patrzącej na monitor z przeciętnej odległości.
    2.  Pary przeciwstawnych przejść nie zawierają ostrej/nasyconej czerwieni ORAZ
        1.  Względna luminancja najciemniejszego obrazu wynosi powyżej 0,80 lub
        2.  Względna luminancja najciemniejszego obrazu wynosi poniżej 0,80, a maksymalna zmiana względnej luminancji między najciemniejszym i najjaśniejszym obrazem wynosi mniej niż 10%.

### Wynik testów
Jeżeli WSZYSTKIE powyższe próby zakończą się niepowodzeniem, wówczas test KS 2.3.1, 5 wymóg zgodności oraz wymaganie podstawowe nr 9 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
- Jeśli treść będzie wyświetlana lub wyświetlana w znacznie różnych rozmiarach lub odległościach (np. treści responsywne przeznaczone do wyświetlania na pulpicie, w telefonie komórkowym i/lub innych wyświetlaczach), treść należy ocenić dla każdego scenariusza.

## Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G19.md %}
- {% include techniki/G176.md %}

Nagrania dźwiękowe zarejestrowane wcześniej (transmisje na żywo) nie są objęte tym testem.

Wszystkie wideo bez dźwięku (tylko wideo) nagrane wcześniej.

Uwaga: Treść „tylko wideo” nie obejmuje treści wideo z dźwiękiem, nawet jeśli jest to tylko muzyka w tle, która nie niesie żaddnej znaczącej informacji.

Uwaga: Krótkie efekty animacji, takie jak zmiana stanu przycisku na „wciśnięty” lub „niewciśnięty”, zmniejszanie ikony pliku po zamknięciu pliku, nie są treściami wideo.



