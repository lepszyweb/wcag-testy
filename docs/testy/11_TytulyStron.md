# 11. Tytuły stron

## Wymagania dostępności
--------------------------
-   [WCAG2: KS 2.4.2 Tytuły stron](http://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-title.html) -- Strony internetowe posiadają tytuły, które opisują ich cel lub przedstawiają ich temat.

## Uzasadnienie metody badania
------------------------------
Element &lt;title&gt; określa tytuł dokumentu i jest wymagany we wszystkich dokumentach HTML/XHTML. Ten test ocenia obecność opisowego tytułu dla strony internetowej.

## Ograniczenia, założenia lub wyjątki
-   Każda strona internetowa musi mieć opisowy tytuł. Ten test jest zawsze obowiązkowy.
-   Element &lt;title&gt; w tym teście różni się od atrybutu *title* używanego do dodawania podpowiedzi/dodatkowych informacji o elemencie.
-   Niektóre aplikacje internetowe i inne niż internetowe mogą zawierać treści, które zmieniają się dynamicznie. W takich przypadkach tytuł strony powinien wystarczająco opisywać cel aplikacji.
-   [Specyfikacja HTML5](https://www.w3.org/TR/html50/document-metadata.html#the-title-element) stanowi, że dokument HTML powinien mieć tylko jeden element &lt;title&gt; ORAZ że element &lt;title&gt; powinien być dzieckiem elementu &lt;head&gt; element.Jednak w praktyce wszystkie nowoczesne przeglądarki korygują błędy składniowe związane z lokalizacją i zagnieżdżaniem elementu &lt;title&gt;.  Dlatego gdy programy klienckie korzystające z Obiektowego MOdelu Dokumentu (DOM)  umieszczą element &lt;title&gt; w prawidłowej lokalizacji i zazwyczaj będą przedstawiać użytkownikowi tylko pierwszy element &lt;title&gt; (jeśli jest więcej niż jeden).

## Procedura testu dla KS 2.4.2 Tytuły stron
---------------------------------------
### Identyfikacja treści
Element &lt;title&gt; dla strony.

### Instrukcja testowania

1.  Sprawdź, czy dla strony jest zdefiniowany element &lt;title&gt;.
2.  Sprawdź, czy tytuł strony określa treść lub przeznaczenie strony internetowej.
    1.  W przypadku stron w witrynie internetowej sprawdź, czy po tytułach stron można je rozróżniać.
    2.  W przypadku dokumentów lub aplikacji internetowych, do opisania celu wystarcza nazwa dokumentu lub aplikacji internetowej.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 2.4.2 oraz Wymaganie podstawowe nr 11 kończy się niepowodzeniem.

### Techniki WCAG 2.1
-   Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
    -   [G88: Zapewnienie opisowych tytułów stron internetowych](https://www.w3.org/TR/WCAG20-TECHS/G88.html)
    -   [H25: Zapewnienie tytułu za pomocą elementu title](https://www.w3.org/TR/WCAG20-TECHS/H25.html)
    -   [F25: Niespełnienie kryterium sukcesu 2.4.2 ze względu na tytuł strony internetowej, która nie identyfikuje treści](https://www.w3.org/TR/WCAG20-TECHS/F25.html)

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](10_Formularze.md) | [[Następny]](12_TabeleDanych.md)
