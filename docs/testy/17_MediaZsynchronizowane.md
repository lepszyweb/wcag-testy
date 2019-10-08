# 17. Multimedia zsynchronizowane 

## Wymagania dostępności
------------------------------
-   [KS WCAG: 1.2.2 Napisy rozszerzone (nagranie)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-captions.html) -- Napisy rozszerzone dołączone są do wszystkich nagrań audio w multimediach zsynchronizowanych (dźwięk i obraz), za wyjątkiem sytuacji, kiedy są one alternatywami dla tekstu i w taki sposób są oznaczone.
-   [KS WCAG: 1.2.3 Audiodeskrypcja lub alternatywa dla mediów (nagranie)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc.html) -- Zapewnia się alternatywę dla mediów zmiennych w czasie lub audiodeskrypcję dla nagrań wideo w multimediach zsynchronizowanych (dźwięk i obraz), za wyjątkiem sytuacji, kiedy są one alternatywami dla tekstu i w taki sposób są oznaczone.
-   [KS WCAG: 1.2.4 Napisy rozszerzone (na żywo)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-real-time-captions.html) -- Napisy rozszerzone dołączone są do wszystkich treści audio przekazywanych na żywo w multimediach zsynchronizowanych (dźwięk i obraz).
-   [KS WCAG: 1.2.5 Audiodeskrypcja (nagranie)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc-only.html) -- Zapewniona jest audiodeskrypcja dla wszystkich nagrań wideo w multimediach zsynchronizowanych (dźwięk i obraz).


## Uzasadnienie metody badania
------------------------------
Ocena nadpisów i opisów dźwiękowych w celu oceny ich równoważności z zsynchronizowanymi treściami medialnymi zazwyczaj obejmuje ręczne, poznawcze porównanie oryginalnej treści z jej alternatywami.

## Ograniczenia, założenia lub wyjątki
---------------------------------------
-   [Zsynchronizowane multimedia](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-captions.html#synchronizedmediadef) - dźwięk lub wideo zsynchronizowane z innym formatem, w celu prezentacji informacji lub/i z interaktywnymi komponentami, o ile nie jest to wyraźnie oznaczona alternatywa dla tekstu. Zsynchronizowane multimedia obejmują między innymi transmisje internetowe, konferencje prasowe i internetowe prezentacje szkoleniowe.
-   [Napisy rozszerzone](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-captions.html#captionsdef) - informacja w postaci alternatywy tekstowej zsynchronizowana z obrazem, przedstawiająca zarówno mowę, jak i inne dźwięki niezbędne do zrozumienia zawartości danego medium:
    -   Uwaga 1: Napisy rozszerzone mają formę podobną do zwykłych napisów, z tą różnicą, że zawierają nie tylko dialogi, ale również opis sytuacji pozadialogowej
    -   Uwaga 4: Napisy rozszerzone nie powinny być formułowane niejasno lub pomijać informacji ważnych dla zrozumienia obrazu.
-   [Audiodeskrypcja](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc-only.html#audiodescdef) - narracja dodana do ścieżki dźwiękowej w celu opisu istotnych szczegółów obrazu, które nie wynikają z samej ścieżki dźwiękowej. Nazywana jest także „wideodeskrypcją” i „narracją opisową” „opisem dźwiękowym”.
-   Napisy i opisy dźwiękowe muszą być dostępne, ale nie muszą być domyślnie włączone.
-   Napisy i opisy dźwiękowe mogą znajdować się w osobnych plikach multimedialnych, tzn. audiodeskrypcja i wersja z napisami to różne pliki.
-   Same transkrypcje i niezsynchronizowane alternatywy nie spełniają tego wymogu.
-   Napisy nie są potrzebne, gdy zsynchronizowane multimedia same w sobie stanowią alternatywną prezentację informacji, która jest również prezentowana w postaci tekstu na stronie internetowej.
-   **Napisy na żywo - wyjątek**: Dwukierunkowe połączenia multimedialne między dwiema lub więcej osobami za pośrednictwem aplikacji internetowych nie są objęte tym testem; jest przeznaczony tylko do emisji zsynchronizowanych multimediów.
-   Uwagi z [Objaśnienie KS 1.2.5](https://www.w3.org/TR/UNDERSTANDING-WCAG20/media-equiv-audio-desc-only.html):
    -   Uwaga 1: W przypadku KS 1.2.3, 1.2.5 i 1.2.7, jeżeli pełna informacja o wideo jest już zapewniona przez podstawową ścieżkę dźwiękową, dodatkowa audiodeskrypcja jest zbędna.
    -   Uwaga 2: Kryteria sukcesu 1.2.3, 1.2.5 i 1.2.8 nieco się pokrywają. Ma to na celu zapewnienie autorowi pewnego wyboru na minimalnym poziomie zgodności, a także zapewnienie dodatkowych wymagań na wyższych poziomach. Na poziomie A w kryterium sukcesu 1.2.3  mają możliwość wyboru między opisem dźwiękowym a pełną alternatywą tekstową. Jeśli chcą zachować zgodność na poziomie AA, w ramach kryterium sukcesu 1.2.5 muszą przedstawić opis dźwiękowy - wymóg już spełniony, jeśli wybrali tę alternatywę dla 1.2.3, w przeciwnym razie będzie to dodatkowy wymóg.

## Procedura testu dla KS 1.2.2 Napisy rozszerzone (nagranie)
------------------------------
### Identyfikacja treści
Nagrane multimedia zsynchronizowane.

### Instrukcja testowania
1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia. Jeśli dostarczono osobny plik multimedialny z napisami, przetestuj ten plik.
2.  Sprawdź, czy napisy są dokładne i zawierają wszystkie dialogi i odpowiedniki dla nie-dialogowych informacji audio niezbędnych do zrozumienia treści programu, w tym efektów dźwiękowych, muzyki, śmiechu, identyfikacji i lokalizacji osób mowiących.
    1.  Przesłuchaj dźwięk z całego zsynchronizowanego medium.
    2.  Porównaj dźwięk z napisami, aby ocenić dokładności, synchronizację czasową i równoważność.
3.  Sprawdź, czy napisy nie zasłaniają ani nie utrudniają odczytania istotnych informacji w wideo.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test 1.2.2 oraz Wymaganie podstawowe nr 17 kończy się niepowodzeniem.

## Procedura testu dla KS 1.2.4 Napisy rozszerzone (na żywo)
------------------------------
### Identyfikacja treści
Zsynchronizowane multimedia na żywo.

### Instrukcja testowania
1.  Włącz napisy za pomocą funkcji odtwarzacza multimedialnego i rozpocznij sesję na żywo.
2.  Sprawdź, czy dostarczone napisy zawierają dialog i informacje o ważnych dźwiękach.
    1.  Przesłuchaj dźwięk z całego zsynchronizowanego medium.
    2.  Porównaj dźwięk z napisami, aby ocenić dokładności, synchronizację czasową i równoważność. Mniejsza dokładność napisów do transmisji na żywo może być akceptowalna ze względu na ograniczenia możliwości napisów w czasie rzeczywistym.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test 1.2.4 oraz Wymaganie podstawowe nr 17 kończy się niepowodzeniem.

## Procedura testu dla KS 1.2.5 1.2.5 Audiodeskrypcja (nagranie)
------------------------------
### Instrukcja testowania
1.  Włącz opisy dźwiękowe za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia. Jeśli dostarczono osobny plik multimedialny z audiodeskrypcją, przetestuj ten plik.
2.  Sprawdź, czy dźwięk (z włączonymi opisami dźwiękowymi) odpowiednio opisuje ważną treść wizualną w medium, w tym informuje o działaniach, postaciach, zmianach scen, tekście na ekranie i innych treściach wizualnych.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test 1.2.5 oraz Wymaganie podstawowe nr 17 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
------------------------------
-   Testowanie zsynchronizowanych multimediów różni się od testów podstawowych [16. Tylko audio i tylko wideo](16TylkoAudioTylkoWideo.md).
-   Zsynchronizowane odtwarzacze multimedialne mogą być programami (aplikacjami) lub komponentami HTML.
-   Na poziomie AA kryterium sukcesu 1.2.5 ma zastosowanie do multimediów zsynchronizowanych. Powiązane wymaganie poziomu A, KS 1.2.3, należy oznaczyć w raporcie z testu jako „Nie testowano”. Dopuszczalne jest, aby procesy testowe dodawały test dla KS 1.2.3 (ocenianie pełnego tekstu alternatywnego pod kątem równoważności). Dodanie takiego testu przekroczyłoby podstawowe wymagania testowe i nie wpłynęłoby na wynik testu podstawowego nr 18.

## Techniki WCAG 2.1
------------------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G93: Zapewnienie otwartych (zawsze widocznych) napisów](http://www.w3.org/TR/WCAG20-TECHS/G93.html)
-   [G87: Zapewnienie napisów zamkniętych](http://www.w3.org/TR/WCAG20-TECHS/G87.html)
-   [G9: Tworzenie na żywo napisów dla niesłyszących w mediach zsynchronizowanych](http://www.w3.org/TR/WCAG20-TECHS/G9.html)
-   [G78: Zapewnienie drugiej, wybranej przez użytkownika ścieżki dźwiękowej, która zawiera opis dźwiękowy (audiodeskrypcję)](http://www.w3.org/TR/WCAG20-TECHS/G78.html)

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](16TylkoAudioTylkoWideo.md) | [[Następny]](18_ZaleznoscOdCSS.md)
