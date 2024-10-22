---
title: 6. Obrazy
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-06-obrazy
folder: testy/itc
---


## Wymagania dostępności
- {% include ks/1-1-1.md %}  
- {% include ks/1-4-5.md %}  
- {% include ks/4-1-2.md %}  

## Uzasadnienie metody testowej
-   Testowanie obrazów ocenia obrazy jako elementy zakodowane, aby ustalić, czy autor treści określił je jako znaczące lub dekoracyjne. Istnieją jednak pewne scenariusze, opisane w testach, w których programowe określenie autora może być nieprawidłowe.
-   Testy wykorzystują wskazówki z samouczka WAI W3C [Images Tutorial](https://www.w3.org/WAI/tutorials/images/)
-   Wszystkie obrazy znaczące i dekoracyjne muszą zostać ocenione. Do obrazu może mieć zastosowanie wiele testów.

## Ograniczenia, założenia lub wyjątki
-   Obraz, który ma alternatywę w postaci niepustego tekstu `alt`, został uznany przez autora treści za znaczący. Autor zdecydował, że ten obraz nie powinien być ignorowany przez technologię wspomagającą.
-   Obraz, który ma alternatywę w postaci pustego tekstu `alt`, został uznany przez autora treści za dekoracyjny. Autor zdecydował, że ten obraz powinien być ignorowany przez technologię wspomagającą.
-   Użycie `role="presentation"` lub `role="none"` w znaczniku obrazu z innymi atrybutami lub rolami może powodować konflikty. Ten warunek podstawowy testuje te konflikty, ponieważ [rozwiązywanie konfliktów ról prezentacyjnych](https://www.w3.org/TR/wai-aria-1.1/#conflict_resolution_presentation_none) ma niespójną obsługę dostępności i może skutkować niedostępną treścią.
   -   „Jeśli element z rolą `"presentation"` ma fokus lub jest w inny sposób interaktywny, programy użytkownika MUSZĄ zignorować normalny efekt roli i wyeksponować element z niejawną rdzenną semantyką, aby zapewnić, że element jest zarówno [zrozumiały](https://www.w3.org/TR/wai-aria-1.1/#dfn-understandable), jak  i [funkcjonalny](https://www.w3.org/TR/wai-aria-1.1/#dfn-operable)”.
         -   Ponieważ obsługa dostępności jest niespójna, ten warunek podstawowy sprawdza, czy obraz z pustą alternatywą tekstową nie znajduje się w kolejności tabulacji, ani nie jest obrazem funkcjonalnym.
   -   „Programy użytkownika MUSZĄ zawsze ujawniać [globalne stany i właściwości WAI-ARIA interfejsom API dostępności](https://www.w3.org/TR/wai-aria-1.1/#global_states), nawet jeśli element ma jawną lub odziedziczoną rolę `"presentation"`. W takim przypadku program użytkownika ignoruje rolę `"presentation"` i eksponuje element zgodnie z jego domyślną (niejawną) rdzenną semantyką”.
   -   „Autorzy NIE POWINNI dodawać sensownego tekstu alternatywnego (na przykład używać `alt=""` w HTML), gdy rola `"presentation"` jest stosowana do obrazu.” [(WAI-ARIA 1.1, presentation (role)](https://www.w3.org/TR/wai-aria-1.1/#presentation).
   -   Ponieważ obsługa dostępności jest niespójna jest niespójna, ten warunek podstawowy sprawdza, czy obraz z atrybutem `role="presentation"` lub `role="none"` nie ma niepustego atrybutu `alt`, a obraz, który ma niepustą alternatywę tekstową, nie ma `role="presentation"` lub `role="none"`.
-   Powszechnie używane formaty obrazów to .jpg, .png, .svg, .gif, .tiff, .bmp. W użyciu są również inne formaty graficzne, które powinny być brane pod uwagę w tym teście.
-   **Cele dekoracyjne, formatowanie, treść niewidoczna**: Jeśli treść nietekstowa pełni funkcję czysto dekoracyjną, używana jest do formatowania wizualnego lub też nie jest przedstawiana użytkownikowi, powinna być wdrożona w sposób umożliwiający technologiom wspomagającym jej zignorowanie.
-   **CAPTCHA**: Jeśli celem treści nietekstowej jest potwierdzenie, że do treści ma dostęp człowiek, a nie komputer, wtedy zapewnia się alternatywę w postaci tekstu, która identyfikuje oraz opisuje cel treści nietekstowej. Zapewnia się również alternatywne zabezpieczenia typu CAPTCHA, dostosowane do różnych możliwości percepcji użytkowników, uwzględniając różne rodzaje niepełnosprawności.
-   Obrazy tekstu, które są niezbędne do przekazywania informacji, są wyłączone z KS 1.4.5. Tekst, który jest częścią logo lub nazwy własnej produktu, jest w tym przypadku uznawany za istotny.
-   [Definicja obrazu tekstu](https://wcag.irdpl.pl/understanding/obrazy-tekstu.html#dfn-obraz-tekstu) zawiera uwagę: „Uwaga: Nie dotyczy to tekstu znajdującego się na obrazie, w którym ważna jest inna treść wizualna.” Przykładami takich obrazów są wykresy, zrzuty ekranu i diagramy, które wizualnie przekazują ważne informacje nie tylko za pomocą tekstu.
-   Zawarte w ilustrowanym tekście strony równoważne opisy obrazu pozwalają uznać obraz za dekoracyjny. Nie wymaga to jednak usunięcia ze znacznika obrazu żadnych istniejących atrybutów tekstowych.
-   Chociaż historycznie w celu zapewnienia długiego opisu obrazu używany był atrybut `longdesc`, nadal wymieniony jako wystarczająca technika w WCAG ([H45](https://www.w3.org/WAI/WCAG22/Techniques/html/H45.html)), technika  ta [nie jest obecnie dobrze obsługiwana pod względem dostępności](https://webaim.org/techniques/alttext/longdesctestcases.htm) i nie jest częścią [dostępnej nazwy, ani sposobem zapewnienia dostępnego opisu dla obrazu](https://www.w3.org/TR/html-aam-1.0/#img-element); dlatego ten test podstawowy nie akceptuje wspomnianej techniki.
-   Połączenie dostępnej nazwy elementu i dostępnego opisu jest jego alternatywą tekstową.


## 6.A Procedura testowa dla obrazów z niepustą alternatywą tekstową
Identyfikator testu podstawowego: _6.A-MeaningfulImage_

### Identyfikacja treści
Znajdź wszystkie obrazy (np. elementy `img` lub element z `role="img"`), które mają niepustą alternatywę tekstową (kombinację dostępnej nazwy i dostępnego opisu) zgodnie z [mapowaniami API dostępności HTML 1.0 dla img](https://www.w3.org/TR/html-aam-1.0/#img-element)


### Instrukcja testowania
1.	Sprawdź, czy żaden z poniższych warunków nie jest prawdziwy:
    -	Obraz jest projektem strony/formatowaniem i może zostać zignorowany przez technologię wspomagającą bez utraty znaczenia strony.
    -	Obraz nie jest widoczny na stronie.
2.	Sprawdź, czy NIE określono dla obrazu atrybutu `role="presentation"`.[ SC 4.1.2]
3. 	Sprawdź, czy NIE określono dla obrazu atrybutu `role="none"`.[ SC 4.1.2]
4.	Sprawdź, czy niepusta tekstowa alternatywa (połączenie dostępnej nazwy i dostępnego opisu) zapewnia równoważny opis celu obrazu.[SC 1.1.1].


### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.A-MeaningfulImage_ kończy się niepowodzeniem.


## 6.B Procedura testowa dla obrazów z pustą alternatywą tekstową
Identyfikator testu podstawowego: _6.B-DecorativeImage_

### Identyfikacja treści
Znajdź wszystkie obrazy (np. elementy img lub element z role="img" lub element, który zawiera obraz tła CSS), które mają pustą alternatywę tekstową.

### Instrukcja testowania
1.	Sprawdź, czy alternatywa pustego tekstu została przypisana programowo przy użyciu jednej z następujących technik [SC 1.1.1]:
   -	obraz ma atrybut `role="prezentation"`.
   -	obraz ma atrybut `role="none"`.
   -	atrybut `aria-hidden' jest ustawiony na wartość "true".
   -	obraz ma arybut `alt=""`.
   -	Obraz jest wstawiany za pomocą CSS (tzn. jest obrazem tła).
> Uwaga: Jeśli żadna z tych technik nie została użyta, test kończy się niepowodzeniem.
2.	Sprawdź, czy żaden z poniższych warunków nie jest prawdziwy [SC 1.1.1]:
   -	Obraz jest jedynym sposobem na przekazanie istotnych informacji.
   -	Obraz jest w kolejności tabulacji.
   -	Obraz jest obrazem funkcjonalnym, który inicjuje działanie.
3.	W przypadku obrazów z `role="presentation"` lub `role="none"` sprawdź, czy nie ma niepustych atrybutów tekstu alternatywnego. Obecność takich atrybutów może spowodować, że technologia wspomagająca nie będzie ignorować obrazu, tj. zapewni użytkownikowi alternatywę tekstową obrazu. [SC 1.1.1]
   -	Przykład niepowodzenia 1: `<img role="none" alt="Użyj swoich notatek">`
   -	Przykład niepowodzenia 2: `<img aria-label="żółw" role="prezentation">`
### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.B-DecorativeImage_ kończy się niepowodzeniem.

## 6.C Procedura testowa dla captcha
Identyfikator testu podstawowego: _6.C-Captcha_

### Identyfikacja treści
Znajdź wszelkie CAPTCHA przeznaczone do potwierdzenia, że dostęp do treści uzyskuje osoba, a nie komputer.

### Instrukcja testowania
1.	Sprawdź, czy alternatywa tekstowa (kombinacja dostępnej nazwy i dostępnego opisu) nie jest pusta. [SC 1.1.1]
2.	Sprawdź, czy alternatywa w postaci niepustego tekstu (połączenie dostępnej nazwy i dostępnego opisu) określa i opisuje cel CAPTCHA. [SC 1.1.1]
3.	Sprawdź, czy zapewnione są alternatywne formy CAPTCHA dla użytkowników niewidomych i niedosłyszących. [SC 1.1.1]

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.C-Captcha_ kończy się niepowodzeniem.

## 6.D Procedura testowa dla obrazów tekstu
Identyfikator testu podstawowego: _6.D-ImageText_

### Identyfikacja treści
Zidentyfikuj wszelkie obrazy tekstu, z wyjątkiem przypadków, w których konkretna prezentacja tekstu jest niezbędna dla przekazywanych informacji (np. logotypy lub tekst, który jest częścią logo lub nazwy marki).

### Instrukcja testowania
1.	Sprawdź, czy za pomocą tekstu nie można uzyskać takiej samej wizualnej prezentacji i efektu, jak za pomocą obrazu tekstu. [SC 1.4.5]
2.  Sprawdź, czy obraz tekstu można dostosować wizualnie do wymagań użytkownika.
    -   Na przykład strona internetowa pozwala użytkownikom określić ustawienia czcionki, rozmiaru, koloru i tła, a następnie wszystkie obrazy tekstu są dostarczane na podstawie tych ustawień.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _6.D-ImageText_ kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/ARIA6.md %}
- {% include techniki/ARIA15.md %}
- {% include techniki/C9.md %}
- {% include techniki/G143.md %}
- {% include techniki/G144.md %}
- {% include techniki/H36.md %}
- {% include techniki/H37.md %}
- {% include techniki/H67.md %}
- {% include techniki/H86.md %}
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






