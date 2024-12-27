---
title: 6. Obrazy (dokumenty)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 06-obrazy-doc
folder: testy/doc
---

## 6. Obrazy

## Wymagania dostępności
- {% include ks/1-1-1.md %}  
- {% include ks/1-4-5.md %}  
- {% include ks/4-1-2.md %}  

## Uzasadnienie metody testowej
-   Testowanie obrazów ocenia obrazy jako elementy zakodowane, aby ustalić, czy autor treści określił je jako znaczące lub dekoracyjne. Istnieją jednak pewne scenariusze, opisane w testach, w których programowe określenie autora może być nieprawidłowe.
-   Testy wykorzystują wskazówki z samouczka WAI W3C [Images Tutorial](https://www.w3.org/WAI/tutorials/images/)
-   Wszystkie obrazy znaczące i dekoracyjne muszą zostać ocenione. Do obrazu może mieć zastosowanie wiele testów.

## Ograniczenia, założenia lub wyjątki
-   Obraz, który ma alternatywę w postaci niepustego tekstu alternatywnego, został uznany przez autora treści za znaczący. Autor zdecydował, że ten obraz nie powinien być ignorowany przez technologię wspomagającą.
-   Obraz, który ma pusty tekst alternatywny, został uznany przez autora treści za dekoracyjny. Autor zdecydował, że ten obraz powinien być ignorowany przez technologię wspomagającą.
-   Powszechnie używane formaty obrazów to .jpg, .png, .svg, .gif, .tiff, .bmp. W użyciu są również inne formaty graficzne, które powinny być brane pod uwagę w tym teście.
-   **Cele dekoracyjne, formatowanie, treść niewidoczna**: Jeśli treść nietekstowa pełni funkcję czysto dekoracyjną, używana jest do formatowania wizualnego lub też nie jest przedstawiana użytkownikowi, powinna być wdrożona w sposób umożliwiający technologiom wspomagającym jej zignorowanie.
-   Obrazy tekstu, które są niezbędne do przekazywania informacji, są wyłączone z KS 1.4.5. Tekst, który jest częścią logo lub nazwy własnej produktu, jest w tym przypadku uznawany za istotny.
-   [Definicja obrazu tekstu](https://wcag.irdpl.pl/understanding/obrazy-tekstu.html#dfn-obraz-tekstu) zawiera uwagę: „Uwaga: Nie dotyczy to tekstu znajdującego się na obrazie, w którym ważna jest inna treść wizualna.” Przykładami takich obrazów są wykresy, zrzuty ekranu i diagramy, które wizualnie przekazują ważne informacje nie tylko za pomocą tekstu.

## 6.A Procedura testowa dla obrazów z niepustą alternatywą tekstową
Identyfikator testu podstawowego: _6.A-MeaningfulImage_

### Identyfikacja treści

#### Identify Content

<p id="d6aIC">Znajdź wszystkie obrazy, które mają niepustą alternatywę tekstową (kombinację dostępnej nazwy i dostępnego opisu) zgodnie z [mapowaniami API dostępności HTML 1.0 dla img](https://www.w3.org/TR/html-aam-1.0/#img-element)</a>.</p>

### Instrukcja testowania
1.	Potwierdź, że żaden z poniższych warunków nie jest prawdziwy:
    -	Obraz jest związany z projektowaniem/formatowaniem dokumentu i może zostać zignorowany przez technologię wspomagającą bez utraty znaczenia dokumentu.
    -	Obraz nie jest widoczny w dokumencie.
2.	Sprawdź, czy niepusta tekstowa alternatywa (połączenie dostępnej nazwy i dostępnego opisu) zapewnia równoważny opis celu obrazu.[SC 1.1.1].

### Wynik testów
<p id="d6aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.A-MeaningfulImage_ kończy się niepowodzeniem.</p>

## 6.B Procedura testowa dla obrazów z pustą alternatywą tekstową
Identyfikator testu podstawowego: _6.B-DecorativeImage_

### Identyfikacja treści
<p id="d6bIC">Znajdź wszystkie obrazy (w tym obrazy tła), które mają pustą alternatywę tekstową.</p>

#### Test Instructions

<ol id="d6bTI">
    <li id="d6bTI-1">Check that the empty text alternative has been programmatically assigned using one of the following techniques [SC 1.1.1]:
        <ol>
            <li id="d6bTI-1a">The image is marked as decorative.</li>
            <li id="d6bTI-1b">The image is marked as an artifact.</li>
            <li id="d6bTI-1c">The image is only part of the background, header, footer, or on a hidden layer.</li>
        </ol>
    </li>
    <li id="d6bTI-2">Check that none of the following is true [SC 1.1.1]:
        <ol>
            <li id="d6bTI-2a">The image is the only way to convey meaningful information.</li>
            <li id="d6bTI-2b">The image is in the tab order.</li>
            <li id="d6bTI-2c">The image is a functional image that initiates action.</li>
        </ol>
    </li>
</ol>
### Instrukcja testowania
1.	Sprawdź, czy alternatywa pustego tekstu została przypisana programowo przy użyciu jednej z następujących technik [KS 1.1.1]:
   -	Obraz jest oznaczony jako dekoracyjny.
   -	Obraz jest oznaczony jako artefakt.
   -	Obraz jest tylko częścią tła, nagłówka, stopki lub znajduje się na ukrytej warstwie.
2.	Potwierdź, że żaden z poniższych warunków nie jest prawdziwy [KS 1.1.1]:
   -	Obraz jest jedynym sposobem na przekazanie istotnych informacji.
   -	Obraz jest w kolejności tabulacji.
   -	Obraz jest obrazem funkcjonalnym, który inicjuje działanie.

### Wynik testów


<p id="d6bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.B-DecorativeImage_ kończy się niepowodzeniem.</p>

## 6.C Procedura testowa dla captcha - nie dotyczy dokumentów
Identyfikator testu podstawowego: _6.C-Captcha_

<p>Captcha nie są zaimplementowane w dokumentach innych niż internetowe, więc ten test nie ma zastosowania. Nie został on usunięty w celu zachowania harmonizacji z ICT Testing Baseline for Web.</p>

### Wynik testów

<p>Test podstawowy 6.C-Captcha nie ma zastosowania do dokumentów.</p>

## 6.D Procedura testowa dla obrazów tekstu
Identyfikator testu podstawowego: _6.D-ImageText_

### Identyfikacja treści

<p id="d6dIC">Zidentyfikuj wszelkie obrazy tekstu, z wyjątkiem przypadków, w których konkretna prezentacja tekstu jest niezbędna dla przekazywanych informacji (np. logotypy lub tekst, który jest częścią logo lub nazwy marki).</p>

### Instrukcja testowania
1.	Sprawdź, czy za pomocą tekstu nie można uzyskać takiej samej wizualnej prezentacji i efektu, jak za pomocą obrazu tekstu. [KS 1.4.5]
2.  Sprawdź, czy obraz tekstu można dostosować wizualnie do wymagań użytkownika. [KS 1.4.5] 
    -   Na przykład zawartość dokumentu umożliwia ustawienie czcionki, rozmiaru, koloru i tła, a wszystkie obrazy tekstu są następnie dostarczane na podstawie tych ustawień (np. SmartArt, grafika tekstowa).

### Wynik testów

<p id="d6dTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.D-ImageText_ kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/C9.md %}
- {% include techniki/G143.md %}
- {% include techniki/G144.md %}
- {% include techniki/H36.md %}
- {% include techniki/H37.md %}
- {% include techniki/H67.md %}
- {% include techniki/H86.md %}
- {% include techniki/PDF1.md %}
- {% include techniki/PDF4.md %}
- {% include techniki/PDF7.md %}
- {% include techniki/F3.md %}
- {% include techniki/F20.md %}
- {% include techniki/F30.md %}
- {% include techniki/F38.md %}
- {% include techniki/F39.md %}
- {% include techniki/F65.md %}

### Opracowania
- [Samouczek W3C: Obrazy dekoracyjne](https://www.w3.org/WAI/tutorials/images/decorative/)
- [Samouczek W3C: Obrazy funkcjonalne](https://www.w3.org/WAI/tutorials/images/functional/)
- [Samouczek W3C: Obrazy informacyjne](https://www.w3.org/WAI/tutorials/images/informative/)
