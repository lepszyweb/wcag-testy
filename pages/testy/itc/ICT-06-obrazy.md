---
title: 6. Obrazy


sidebar: testy_sidebar
permalink: ICT-06-obrazy
folder: testy/itc
---


## Wymagania dostępności
-   [KS WCAG: 1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content) -- Wszelkie treści nietekstowe przedstawione użytkownikowi posiadają swoją tekstową alternatywę, która pełni tę samą funkcję, za wyjątkiem sytuacji \[specyficznych wyszczególnionych sytuacji\].
-   [KS WCAG: 1.4.5 Obrazy tekstu](https://wcag.lepszyweb.pl/#images-of-text) -- Jeśli wykorzystywane technologie mogą przedstawiać treść wizualnie, do przekazywania informacji wykorzystuje się tekst, a nie tekst w postaci grafiki, za wyjątkiem \[specyficznych wyszczególnionych sytuacji\].
-   [KS WCAG: 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value) -- Dla wszystkich komponentów interfejsu użytkownika (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów wygenerowanych przez skrypty) nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; zawiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

## Uzasadnienie metody badania
Wszystkie obrazy  znaczące i dekoracyjne muszą zostać ocenione. Określono testy dla niektórych typów obrazów.

## Ograniczenia, założenia lub wyjątki
-   Powszechnie używane formaty obrazów to  .jpg, .png, .svg, .gif, .tiff, .bmp. W użyciu są również inne formaty graficzne i należy wziąć je pod uwagę w tym teście.
-   **Cele dekoracyjne, formatowanie, treść niewidoczna**: Jeśli treść nietekstowa pełni jedynie funkcję dekoracyjną, używana jest do formatowania wizualnego lub też nie jest przedstawiana użytkownikowi, powinna być wdrożona w sposób umożliwiający technologiom wspomagającym jej zignorowanie.
-   **CAPTCHA**: Jeśli celem treści nietekstowej jest potwierdzenie, że do treści ma dostęp człowiek, a nie komputer, wtedy dostarcza się alternatywę w postaci tekstu, która identyfikuje oraz opisuje cel treści nietekstowej. Dostarcza się również alternatywnych zabezpieczeń typu CAPTCHA, dostosowanych do różnych możliwości percepcji użytkowników, uwzględniając różne rodzaje niepełnosprawności.
-   Obrazy tekstu, które są niezbędne do przekazywania informacji, są wyłączone z KS 1.4.5. Tekst, który jest częścią logo lub nazwy własnej produktu, jest w tym przypadku uznawany za istotny.
-   [Definicja obrazu tekstu](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-text-presentation.html#images-of-textdef) zawiera uwagę: „Uwaga: Nie dotyczy to tekstu znajdującego się na obrazie, w którym ważna jest inna treść wizualna.” Przykłady takich zdjęć obejmują wykresy, zrzuty ekranu i diagramy, które wizualnie przekazują ważne informacje za pomocą czegoś więcej niż tylko tekstu.
-   Równoważne opisy obrazu w tekście strony pozwolają uznać obraz za dekoracyjny. Nie wymaga to jednak usunięcia z obrazu żadnych dostępnych atrybutów tekstowych.
-   Chociaż historycznie atrybut longdesc był używany w celu zapewnienia rozszerzonego opisu obrazów i jest wymieniony jako wystarczająca technika w WCAG ([H45](http://www.w3.org/TR/WCAG20-TECHS/H45.html)), technika  ta [nie jest obecnie dobrze obsługiwana pod względem dostępności ](https://webaim.org/techniques/alttext/longdesctestcases.htm) i nie jest częścią [dostępnej nazwy ani sposobem zapewnienia dostępnego opisu dla obrazu](https://www.w3.org/TR/html-aam-1.0/#img-element); dlatego ten test podstawowy nie akceptuje wspomnianej techniki.

## Procedura testu dla KS 1.1.1 Treść nietekstowa oraz 4.1.2 Nazwa, rola, wartość
### Identyfikacja treści
1.  Zidentyfikuj wszystkie obrazy
2.  Przejrzyj kontekst każdego obrazu, aby określić jego przeznaczenie::
    -   **Znaczący:** przekazuje informacje (obejmuje obrazy tekstu; obrazy funkcjonalne używane do inicjowania akcji, przekazywania znaczenia lub zachęcania do odpowiedzi; mapy obrazów itp.)
    -   **Dekoracyjny:** nie przekazuje żadnych istotnych informacji lub jest opisany w treści tekstu
    -   **CAPTCHA:** zaprojektowany w celu ustalenia, czy dostęp do treści ma osoba, czy komputer
    -   **Tekst:** obraz tekstu, z wyjątkiem sytuacji, gdy tekst jest częścią logo

### Obrazy znaczące

#### Instrukcja testowania
Jeśli jest to obraz znaczący (przekazuje informacje):
1.  Sprawdź, czy kombinacja dostępnej nazwy i dostępnego opisu zapewnia równoważny opis. Wiele atrybutów służy do ustalenia dostępnej nazwy i dostępnego opisu. Zobacz [Mapowanie API dostępności HTML 1.0 dla img](https://www.w3.org/TR/html-aam-1.0/#img-element).
    1.  Opisy obrazu dostarczane w treści strony muszą być powiązane programowo.
2.  Sprawdź, czy NIE określono dla obrazu atrybutu ARIA role="presentation".
3.  Sprawdź, czy atrybut aria-hidden NIE jest ustawiona na "true".


#### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.1.1, KS 4.1.2  oraz wymaganie podstawowe nr 6 kończy się niepowodzeniem.

### Obrazy dekoracyjne
#### Instrukcja testowania

Jeśli obraz jest dekoracyjny, sprawdź, czy spełniony jest przynajmniej jeden z poniższych warunków:
1.  Ustawiono  dla obrazu atrybut ARIA role="presentation".
2.  Ustawiono  dla obrazu atrybut aria-hidden="true".
3.  Kombinacja dostępnej nazwy i dostępnego opisu jest pusta (np. ""). Wiele atrybutów służy do ustalenia dostępnej nazwy i dostępnego opisu. Zobacz [Mapowanie API dostępności HTML 1.0 dla img](https://www.w3.org/TR/html-aam-1.0/#img-element).
4.  Obraz jest wstawiany za pomocą CSS (np. za pomoca właściwości *background-image*).

#### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.1.1, KS 4.1.2  oraz wymaganie podstawowe nr 6 kończy się niepowodzeniem.

### Obrazy CAPTCHA
#### Instrukcja testowania

Jeśli obraz jest obrazem Captcha:
1.  Sprawdź, czy kombinacja [dostępnej nazwy i dostępnego opisu](https://www.w3.org/TR/html-aam-1.0/#accessible-name-and-description-computation) wskazuje i wyjaśnia sens CAPTCHA.
2.  Sprawdź, czy zapewnione są alternatywne formy CAPTCHA przynajmniej dla użytkowników niewidomych i niedosłyszących.

#### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.1.1, KS 4.1.2  oraz wymaganie podstawowe nr 6 kończy się niepowodzeniem.

## Procedura testu dla KS 1.4.5 Obrazy tekstu
### Identyfikacja treści

Zidentyfikuj wszelkie obrazy tekstu, z wyjątkiem przypadków, w których konkretna prezentacja tekstu jest niezbędna dla przekazywanych informacji (np. logotypy lub tekst, który jest częścią logo lub nazwy marki).

### Instrukcja testowania
1.  Sprawdź, czy za pomocą tekstu nie można uzyskać takiej samej wizualnej prezentacji i efektu, jak za pomocą obrazu tekstu.
2.  Sprawdź, czy obraz tekstu można dostosować wizualnie do wymagań użytkownika.
    -   Na przykład strona internetowa pozwala użytkownikom określić ustawienia czcionki, rozmiaru, koloru i tła, a następnie wszystkie obrazy tekstu są dostarczane na podstawie tych ustawień.


### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.4.5  oraz wymaganie podstawowe nr 6 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego

## Techniki WCAG 2.1

-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
    -   [ARIA6: Używanie atrybutu aria-label, aby zapewnić etykiety dla obiektów](https://www.w3.org/TR/WCAG20-TECHS/ARIA6.html)
    -   [ARIA15: Używanie atrybutu aria-describedby, aby zapewnić odpowiedniki tekstowe dla obrazów](https://www.w3.org/TR/WCAG20-TECHS/ARIA15.html)
    -   [H36: Używanie atrybutów alt na obrazach używanych jako przyciski przesyłania](https://www.w3.org/TR/WCAG20-TECHS/H36.html)
    -   [H37: Używanie atrybutów alt na elementach img](https://www.w3.org/TR/WCAG20-TECHS/H37.html)
    -   [H67: Używanie pustego tekstu alternatywnego i nieużywanie atrybutu title w elementach img dla obrazów, które powinny być zignorowane przez technologię asystującą](https://www.w3.org/TR/WCAG20-TECHS/H67.html)
    -   [G143: Zapewnienie tekstu alternatywnego opisującego zadanie CAPTCHA](https://www.w3.org/TR/WCAG20-TECHS/G143.html)
    -   [G144: Zapewnienie, że strona internetowa zawiera inny CAPTCHA służący temu samemu celowi przy użyciu innej modalności](https://www.w3.org/TR/WCAG20-TECHS/G144.html)
    -   [H86: Zapewnienie tekstowych alternatyw dla sztuki ASCII, emotikonów i tekstu szyfrowanego](https://www.w3.org/TR/WCAG20-TECHS/H86.html)
    -   [F30: Niespełnienie kryterium sukcesu 1.1.1 i 1.2.1 z powodu użycia alternatyw tekstowych, które nie są alternatywne (np. nazw plików lub tekstu zastępczego)](https://www.w3.org/TR/WCAG20-TECHS/F30.html)
    -   [F38: Niespełnienie kryterium sukcesu 1.1.1 z powodu pominięcia w HTML atrybutu alt dla treści nietekstowych wykorzystywanych wyłącznie w celach dekoracyjnych](https://www.w3.org/TR/WCAG20-TECHS/F38.html)
    -   [F39: Niespełnienie kryterium sukcesu 1.1.1 ze względu na dostarczenie tekstu alternatywnego, który nie jest pusty (np. alt="spacja" lub alt="obraz") dla obrazów, które powinny zostać zignorowane przez technologię asystującą](https://www.w3.org/TR/WCAG20-TECHS/F39.html)
    -   [F65: Niespełnienie kryterium sukcesu 1.1.1 z powodu pominięcia atrybutu alt lub tekstu  alternatywnego w elementach img, elementach area i polach typu "image"](https://www.w3.org/TR/WCAG20-TECHS/F65.html)
    -   [C9: Używanie CSS do dodawania obrazów dekoracyjnych](http://www.w3.org/TR/WCAG20-TECHS/C9.html)
