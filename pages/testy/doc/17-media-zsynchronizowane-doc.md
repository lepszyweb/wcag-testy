---
title: 17. Media zsynchronizowane (dokument)
last_updated: 16 stycznia 2025

sidebar: testy_sidebar
permalink: 17-media-zsynchronizowane-doc
folder: testy/doc
---

## 17. Media zsynchronizowane

## Wymagania dostępności
- {% include ks/1-2-2.md %}
- {% include ks/1-2-3.md %}
- {% include ks/1-2-4.md %}
- {% include ks/1-2-5.md %}
- [Sekcja 508 503.4 Elementy sterujące napisami i audiodeskrypcją](https://www.federalregister.gov/d/2017-00395/p-630): W przypadku gdy technologia internetowa wyświetla obraz z zsynchronizowanym dźwiękiem, technologia zapewnia kontrolę użytkownika dla napisów kodowanych i&nbsp;audiodeskrypcji zgodnych z 503.4.
- [Sekcja 508 503.4.1 Elementy sterujące napisami](https://www.federalregister.gov/d/2017-00395/p-631): W przypadku gdy elementy sterujące użytkownika służą do regulacji głośności, ICT zapewnia elementy sterujące użytkownika do wyboru napisów na tym samym poziomie menu, co elementy sterujące użytkownika do wyboru głośności lub programu.
- [Sekcja 508 503.4.2 Elementy sterujące audiodeskrypcją](https://www.federalregister.gov/d/2017-00395/p-632): W przypadku gdy do wyboru programu przewidziane są elementy sterujące użytkownika, ICT zapewnia użytkownikowi elementy sterujące do wyboru audiodeskrypcji na tym samym poziomie menu, co elementy sterujące użytkownika do wyboru głośności lub programu.

## Uzasadnienie metody testowej
Badanie napisów i audiodeskrypcji w celu oceny ich równoważności zsynchronizowaną treścią multimedialną zazwyczaj obejmuje ręczne poznawcze porównanie oryginalnej treści z jej alternatywami. Media, które są wyraźnie oznaczone jako alternatywa medialna dla tekstu, są testowane w celu oceny równoważności z tekstem, a jeśli nie są równoważne, należy przeprowadzić testy dla napisów i audiodeskrypcji.
## Ograniczenia, założenia lub wyjątki
-   [Zsynchronizowane multimedia](https://www.w3.org/TR/WCAG22/#dfn-synchronized-media) to dźwięk lub wideo zsynchronizowane z innym formatem prezentacji informacji lub z interaktywnymi komponentami, chyba że medium to nie jest wyraźnie oznaczone jako alternatywa dla tekstu. Zsynchronizowane multimedia to między innymi transmisje internetowe, konferencje prasowe i internetowe prezentacje szkoleniowe.
-   [Alternatywa medialna dla tekstu](https://www.w3.org/TR/WCAG22/#dfn-media-alternative-for-text) to media, które nie przedstawiają więcej informacji niż jest już przedstawione w tekście (bezpośrednio lub za pośrednictwem alternatyw tekstowych). **Uwaga**: Media alternatywne dla tekstu są przeznaczone dla osób, które korzystają z alternatywnych reprezentacji tekstu. Media alternatywne dla tekstu mogą być _tylko audio_, _tylko wideo_ (w tym wideo w języku migowym) lub _audio-wideo_.
-   [Napisy rozszerzone](https://wcag.irdpl.pl/guidelines/22/#dfn-napisy-rozszerzone) - zsynchronizowana z obrazem alternatywa tekstowa dla treści dźwiękowych, zarówno mowy, jak i innych odgłosów, niezbędnych do zrozumienia przekazu multimedialnego:
    -   Uwaga 1: Napisy rozszerzone mają formę podobną do napisów dialogowych, z tą różnicą, że oprócz treści wypowiedzi osób przekazują opis sytuacji pozadialogowej - dodatkowe informacje, potrzebne do zrozumienia treści programu, takie jak identyfikacja mówiących, informacje o istotnych sygnałach dźwiękowych, np. śmiechu, trzaskaniu drzwi, muzyce, oddaleniu, miejscu akcji. Stąd określenie „rozszerzone”.
    -   Uwaga 5: Napisy rozszerzone nie powinny zasłaniać istotnych informacji w filmie.
-   [Audiodeskrypcja](https://wcag.irdpl.pl/guidelines/22/#dfn-audiodeskrypcja) - narracja dodana do ścieżki dźwiękowej w celu opisania istotnych szczegółów obrazu, które nie mogą być zrozumiane z samej głównej ścieżki dźwiękowej. Nazywana jest także „wideodeskrypcją”, „narracją opisową” i „opisem dźwiękowym”.
-   Napisy rozszerzone i audiodeskrypcja muszą być zapewnione, ale nie muszą być domyślnie włączone.
-   Napisy rozszerzone i audiodeskrypcja mogą znajdować się w osobnych plikach multimedialnych, tzn. audiodeskrypcja i wersja z napisami rozszerzonymi mogą być odrębnymi plikami.
-   Same transkrypcje i niezsynchronizowane alternatywy nie spełniają tego wymogu.
-   Napisy rozszerzone nie są potrzebne, gdy zsynchronizowane multimedia same w sobie stanowią alternatywną prezentację informacji, która jest również prezentowana w postaci tekstu na stronie internetowej.
-   **Napisy na żywo - wyjątek**: Dwukierunkowe połączenia multimedialne między dwiema lub więcej osobami za pośrednictwem aplikacji internetowych nie są objęte tym testem; jest przeznaczony tylko do nadawania zsynchronizowanych multimediów.
-   Z [Objaśnienia KS 1.2.5](https://www.w3.org/WAI/WCAG22/Understanding/audio-description-prerecorded) wynika, że: 
    -   Uwaga 1: W przypadku kryteriów sukcesu 1.2.3, 1.2.5 i 1.2.7, jeśli wszystkie informacje zawarte w ścieżce wideo są już zawarte w ścieżce audio, audiodeskrypcja nie jest konieczna.
    -   Uwaga 2: Kryteria sukcesu 1.2.3, 1.2.5 i 1.2.8 w pewnym stopniu pokrywają się ze sobą. Ma to dać autorowi wybór na minimalnym poziomie zgodności i zapewnić dodatkowe wymagania na wyższych poziomach. Na poziomie A w kryterium sukcesu 1.2.3 autorzy mają możliwość zapewnienia audiodeskrypcji lub pełnej alternatywy tekstowej. Jeśli autorzy chcą spełnić wymagania na poziomie AA, zgodnie z kryterium sukcesu 1.2.5 muszą zapewnić audiodeskrypcję – wymóg już spełniony, jeśli wybrali tę alternatywę dla 1.2.3, w przeciwnym razie jest to wymóg dodatkowy.

## 17.A Procedura testowa dla elementów sterujących odtwarzacza multimedialnego
Identyfikator testu podstawowego: _17.A-MediaPlayerCCADControls_

### Identyfikacja treści
<p id="d17aIC">Odtwarzacz multimedialny, który wyświetla wideo ze zsynchronizowanym dźwiękiem.</p>


### Instrukcja testowania
1.	Sprawdź, czy istnieje kontrolka użytkownika umożliwiająca wybór napisów rozszerzonych. [Sekcja 508 503.4]
2.	Sprawdź, czy istnieje kontrolka użytkownika umożliwiająca wybór audiodeskrypcji. [Sekcja 508 503.4]

### Wynik testów
<p id="d17aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.A-MediaPlayerCCADControls</em> również kończy się niepowodzeniem.</p>

## 17.B Procedura testowa dla poziomu kontroli napisów odtwarzacza multimedialnego
Identyfikator testu podstawowego: _17.B-MediaPlayerCCLevel_

### Identyfikacja treści
<p id="d17bIC">Odtwarzacz multimedialny, który wyświetla wideo ze zsynchronizowanym dźwiękiem i ma elementy sterujące regulacją głośności.</p>

### Instrukcja testowania
1.	Sprawdź, czy kontrolka użytkownika umożliwiająca wybór napisów rozszerzonych znajduje się na tym samym poziomie menu, co kontrolki użytkownika służące do regulacji głośności lub wyboru programu. [Sekcja 508 503.4.1]

### Wynik testów
<p id="d17bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.B-MediaPlayerCCLevel</em> również kończy się niepowodzeniem.</p>


## 17.C Procedura testowa dla poziomu kontroli audiodeskrypcji odtwarzacza multimedialnego
Identyfikator testu podstawowego: _17.C-MediaPlayerADLevel_

### Identyfikacja treści
<p id="d17cIC">Odtwarzacz multimedialny, który wyświetla wideo ze zsynchronizowanym dźwiękiem i ma elementy sterujące wyborem programu.</p>

### Instrukcja testowania
1.	Sprawdź, czy kontrolka użytkownika umożliwiająca wybór znajduje się na tym samym poziomie menu, co kontrolki użytkownika służące do regulacji głośności lub wyboru programu. [Sekcja 508 503.4.2]

### Wynik testów
<p id="d17cTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.C-MediaPlayerADLevel</em> również kończy się niepowodzeniem.</p>

## 17.D Procedura testowa dla napisów rozszerzonych (nagranie)
Identyfikator testu podstawowego: _17.D-CaptionsPrerecorded_

### Identyfikacja treści
<p id="d17dIC">Nagrane multimedia zsynchronizowane. Nie uwzględniaj multimediów, które są wyraźnie oznaczone jako alternatywa dla tekstu.</p>

### Instrukcja testowania
1.  Włącz napisy rozszerzone za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia. Jeśli dostarczono osobny plik multimedialny z napisami, przetestuj ten plik.
2.  Sprawdź, czy istnieją napisy rozszerzone
3.  Sprawdź, czy napisy są dokładne i zawierają wszystkie dialogi i odpowiedniki dla nie-dialogowych informacji dźwiękowych, które są niezbędne do zrozumienia treści programu, w tym efektów dźwiękowych, muzyki, śmiechu, identyfikacji i lokalizacji osób mówiących. [KS 1.2.2]
    -  Przesłuchaj dźwięk z całego zsynchronizowanego medium.
    -  Porównaj dźwięk z napisami, aby ocenić dokładności, synchronizację czasową i równoważność.
4.  Sprawdź, czy napisy nie zasłaniają ani nie utrudniają odczytania istotnych informacji w wideo. [KS 1.2.2]


### Wynik testów
<p id="d17dTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.D-CaptionsPrerecorded</em> również kończy się niepowodzeniem.</p>

## 17.E Procedura testu dla audiodeskrypcji (nagranie)
Identyfikator testu podstawowego: _17.E-ADPrerecorded_

### Identyfikacja treści
<p id="d17eIC">Nagrane multimedia zsynchronizowane. Nie uwzględniaj multimediów, które są wyraźnie oznaczone jako alternatywa dla tekstu.</p>

### Instrukcja testowania
1.  Włącz audiodeskrypcję za pomocą funkcji odtwarzacza multimedialnego i odtwarzaj multimedia. Jeśli dostarczono osobny plik multimedialny z audiodeskrypcją, przetestuj ten plik.
2.  Sprawdź, czy dźwięk (z włączoną audiodeskrypcją) odpowiednio opisuje ważną treść wizualną w medium, w tym informuje o działaniach, postaciach, zmianach scen, tekście na ekranie i innych treściach wizualnych. [KS 1.2.5]

### Wynik testów
<p id="d17eTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.E-ADPrerecorded</em> również kończy się niepowodzeniem.</p>

## 17.F Procedura testu dla napisów rozszerzonych (na żywo)
Identyfikator testu podstawowego: _17.F-CaptionsLive_

### Identyfikacja treści
<p id="d17fIC">Zsynchronizowane multimedia na żywo.</p>

### Instrukcja testowania
1.  Włącz napisy rozszerzone za pomocą funkcji odtwarzacza multimedialnego i rozpocznij sesję na żywo.
2.  Sprawdź, czy istnieją napisy rozszerzone
3.  Sprawdź, czy napisy rozszerzone zawierają dialogi i informacje o ważnych dźwiękach.
    -  Przesłuchaj dźwięk z całego zsynchronizowanego medium.
    -  Porównaj dźwięk z napisami rozszerzonymi, aby ocenić dokładność, synchronizację czasową i równoważność. Mniejsza dokładność napisów do transmisji na żywo może być akceptowalna ze względu na ograniczone możliwości tworzenia napisów w czasie rzeczywistym.

### Wynik testów
<p id="d17fTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy <em>17.F-CaptionsLive</em> również kończy się niepowodzeniem.</p>

## 17.G Procedura testowa dla zsynchronizowanego multimedium jako alternatywy dla tekstu (nagranie)
Identyfikator testu podstawowego: 17.G-SyncMediaAlternative

### Identyfikacja treści
<p id="d17gIC">Nagrane zsynchronizowane multimedia, które są wyraźnie oznaczone jako alternatywa dla tekstu.</p>


### Instrukcja testowania
1.  Znajdź tekst, dla którego multimedia są alternatywą.
2.	Odtwórz nagranie oznaczone jako równoważna alternatywa dla tekstu.
3.	Sprawdź, czy w tekście znajdują się znaczące informacje dźwiękowe prezentowane w nagraniu multimedialnym.
4.	Sprawdź, czy w tekście znajdują się znaczące informacje wizualne prezentowane w nagraniu multimedialnym.

### Wynik testów
<p id="d17gTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, oznacza to, że multimedia nie jest alternatywą medialną dla tekstu. Wykonaj procedurę testową testu podstawowego <em>17.D-CaptionsPrerecorded</em> i procedurę testową <em>17.E-ADPrerecorded</em>.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego

-   Testowanie zsynchronizowanych multimediów różni się od testów podstawowych [16. Tylko audio i tylko wideo](16-tylko-audio-tylko-wideo-doc.md).
-   Zsynchronizowane odtwarzacze multimedialne mogą być programami (aplikacjami) lub komponentami HTML.
-   Na poziomie AA kryterium sukcesu 1.2.5 ma zastosowanie do multimediów zsynchronizowanych. Powiązane wymaganie poziomu A, KS 1.2.3, należy oznaczyć w raporcie z testu jako „Nie dotyczy”. Dopuszczalne jest, aby procesy testowe dodawały test dla KS 1.2.3 (ocenianie pełnego tekstu alternatywnego pod kątem równoważności). Dodanie takiego testu przekroczyłoby podstawowe wymagania testowe i nie wpłynęłoby na wynik testu podstawowego nr 17.
-   Wszystkie zsynchronizowane multimedia powinny zostać przetestowane. Jeśli nagrane wcześniej multimedia są oznaczone jako alternatywa dla tekstu, upewnij się, że zawierają one informacje równoważne z tekstem. Jeśli tak nie jest, to nie jest to medialna alternatywa dla tekstu. Przetestuj multimedia pod kątem napisów i audiodeskrypcji. Sensowne może być wykonanie testu 17.G przed testowaniem napisów i audiodeskrypcji.

### Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:
- {% include techniki/G9.md %}
- {% include techniki/G78.md %}
- {% include techniki/G87.md %}
- {% include techniki/G93.md %}
- {% include techniki/F8.md %}
