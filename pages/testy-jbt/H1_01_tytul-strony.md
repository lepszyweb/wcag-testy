---
title: Tytuł strony
tags: [WCAG_2.1, testy]
summary: "Strona ma sensowny tytuł, który opisuje jej cel lub temat"
sidebar: testy-jbt_sidebar
permalink: H1_01_tytul-strony
folder: testy-jbt
---

## Tytuł strony

### Metoda badania: 
Inspekcja kodu. Użycie narzędzia ujawniającego tytuł strony. 

## Zastosowanie
Znacznik `<title>` dla strony.
## Założenia, zastrzeżenia lub wyjątki
-   [Specyfikacja HTML5](https://www.w3.org/TR/html50/document-metadata.html#the-title-element) stanowi, że dokument HTML powinien mieć tylko jeden element `<title>` ORAZ że element `<title>` powinien być dzieckiem elementu `<head>`. Ale w praktyce wszystkie nowoczesne przeglądarki korygują błędy składniowe związane z lokalizacją i zagnieżdżaniem elementu `<title>`. Oznacza to, że nawet jeśli w kodzie sttrony zostanie umieszczonych więcej niż jeden element `<title>`, to programy korzystające z Obiektowego Modelu Dokumentu (DOM) umieszczą element `<title>` w prawidłowej lokalizacji i zazwyczaj będą przedstawiać użytkownikowi tylko pierwszy element `<title>`.
-   Niektóre aplikacje internetowe mogą zawierać treści, które zmieniają się dynamicznie. W takich przypadkach tytuł strony powinien wystarczająco opisywać cel aplikacji.

## Obsługa dostępności
W HTML do nadawania stronie tytułu istnieje znacznik `<title>` potomny do znacznika <head>.
Technologie pomocnicze odczytują tytuł strony ze znacznika `<title>`.

### Oczekiwania:
Kryterium sukcesu: [2.4.2 Tytuły stron](https://wcag.lepszyweb.pl/#page-titled)
-	Strona ma tytuł zdefiniowany w kodzie znacznikiem `<title>`.
-	Tytuł strony jest unikalny i opisuje jej treść.
-	Tytuł strony zawiera temat strony i nazwę witryny.
-	Tytuł strony nie zawiera zbędnej interpunkcji. 
-	Strona posiada tylko jeden tytuł.

### Procedura testowania:
1.	Sprawdź, czy strona ma tytuł zdefiniowany w kodzie znacznikiem `<title>`.
2.	Sprawdź, czy tytuł strony jest inny od pozostałych.
3.	Sprawdź, czy tytuł zawiera temat strony i nazwę witryny.
4.	Sprawdź, czy tytuł krótko i odpowiednio opisuje treść strony.
5.	Sprawdź, czy tytuł nie zawiera zbędnej interpunkcji.
5.	Sprawdź, czy w kodzie strony nie znajduje się więcej niż jeden  tytuł w znaczniku `title`.

### Zasoby
- [Easy Checks - A First Review of Web Accessibility. Title](https://www.w3.org/WAI/test-evaluate/preliminary/#title)
- [Descriptive HTML page titles help users quickly understand a web page’s content](https://accessibility.iu.edu/creating-content/web-content/titles.html)
- [Accessible page titles in a Single Page App](https://hiddedevries.nl/en/blog/2018-07-19-accessible-page-titles-in-a-single-page-app)
- [ Accessible Publishing Knowledge Base. Page Title](http://kb.daisy.org/publishing/docs/html/title.html)
#### Pomocne narzędzia:
-	skryptozakładka [Page Title](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Wyświetla tytuł strony w oknie dialogowym. Umożliwia skopiowanie tytułu do schowka.
-	opcja *structure* w skryptozakładce ANDI  https://www.ssa.gov/accessibility/andi/help/install.html 

#### Wykorzystanie skryptozkładki ANDI 

{% include image.html file="andi/andi_page-title.png" alt="Wykorzystanie skryptozkładki ANDI" %}
1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *structure*. 
2.	Wybierz z menu poziomego opcję *more details* (więcej szczegółów).
3.	Wybierz z rozwijanej listy opcję *page title* (tytuł strony). 
4.	Sprawdź w oknie dialogowym, czy tytuł został określony, czy opisuje treść strony, czy zawiera temat strony i nazwę witryny, czy zawiera tylko uzasadnione zasadami pisowni znaki interpunkcyjne.

#### Techniki WCAG 2.1
-   [G88: Zapewnienie opisowych tytułów stron internetowych](https://www.w3.org/TR/WCAG20-TECHS/G88.html)
-   [H25: Zapewnienie tytułu za pomocą elementu title](https://www.w3.org/TR/WCAG20-TECHS/H25.html)
-   [F25: Niespełnienie kryterium sukcesu 2.4.2 ze względu na tytuł strony internetowej, która nie identyfikuje treści](https://www.w3.org/TR/WCAG20-TECHS/F25.html)
-   [[G127: Określenie relacji strony internetowej z większym zbiorem stron internetowych](https://www.w3.org/WAI/WCAG21/Techniques/general/G127.html)

### Przypadki testowe

#### Zaliczone
```<title>Strona główna | Pracownia Dostępności Cyfrowej LepszyWeb.pl</title>```
```<title>O nas | LepszyWeb.pl</title>```
```<title>Usługi | LepszyWeb.pl</title>```

#### Niezaliczone
- brak tytułu w znaczniku `<title>` (pusty znacznik)
  ```<title></title>```
- tytuły nieopisujące treści:
  ```<title>xxxx</title>```
  ```<title>12345</title>```
- tytuły z nagromadzeniem zbędnych znaków interpunkcyjnych:
  ```<title>... == Jakiś tytuł strony == ...</title>```
  ```<title>:: Jakiś tytuł strony :: </title>```