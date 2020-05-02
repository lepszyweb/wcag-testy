---
title: Tytuł strony
tags: [WCAG-2.1, nawigacja]
summary: "Strona ma sensowny tytuł, który opisuje jej cel lub temat"
sidebar: testy_sidebar
permalink: H1-01-tytul-strony
folder: testy/jbt
---

## Opis testu
Służy ocenie tytułu strony internetowej.

## Mapowanie do standardów dostępności
- **WCAG 2.1 - kryterium sukcesu** {% include ks/2-4-2.md %}

## Zastosowanie
Badanie znacznika `<title>`.

## Obsługa dostępności
- W HTML do nadawania stronie tytułu istnieje znacznik `<title>` potomny do znacznika `<head>`.
- Technologie pomocnicze odczytują tytuł strony ze znacznika `<title>`.

## Oczekiwania
-	Strona ma tytuł zdefiniowany w kodzie znacznikiem `<title>`.
-	Strona posiada tylko jeden tytuł.
-   Tytuł strony jest unikalny w zestawie stron 
-	Tytuł strony opisuje jej treść lub przeznaczenie.
-	Tytuł strony zawiera temat strony i nazwę witryny.
-	Tytuł strony zawiera tylko niezbędną interpunkcję.

## Założenia, zastrzeżenia lub wyjątki
- Ten test jest obowiązkowy. Każda strona internetowa musi mieć tytuł.
- Niektóre aplikacje internetowe i inne niż internetowe mogą zawierać treści, które zmieniają się dynamicznie. W takich przypadkach tytuł strony powinien wystarczająco opisywać cel aplikacji.
- [Specyfikacja HTML5](https://www.w3.org/TR/html50/document-metadata.html#the-title-element) stanowi, że dokument HTML powinien mieć tylko jeden element `<title>` ORAZ że element `<title>` powinien być dzieckiem elementu `<head>`. Ale w praktyce wszystkie nowoczesne przeglądarki korygują błędy składniowe związane z lokalizacją i zagnieżdżaniem elementu `<title>`. Oznacza to, że nawet jeśli w kodzie strony zostanie umieszczonych więcej niż jeden element `<title>`, to programy korzystające z Obiektowego Modelu Dokumentu (DOM) umieszczą element `<title>` w prawidłowej lokalizacji i zazwyczaj będą przedstawiać użytkownikowi tylko pierwszy element `<title>` (jeśli jest więcej niż jeden).
- Nie należy mylić znacznika `<title>`z atrybutem *title*, który służy do dodawania podpowiedzi/dodatkowych informacji o elemencie.

## Testowanie

### Metoda badania
Inspekcja kodu. Użycie narzędzia ujawniającego tytuł strony.
### Pomocne narzędzia:
-	[skryptozakładka Page Title](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Wyświetla tytuł strony w oknie dialogowym. Umożliwia skopiowanie tytułu do schowka.
-	opcja *struktury* w [skryptozakładce ANDI](https://lepszyweb.pl/andi/)

### Procedura testowania:
1.	Sprawdź, czy strona ma tytuł zdefiniowany w kodzie znacznikiem `<title>`.
2.	Sprawdź, czy w kodzie strony nie ma więcej znaczników `title` niż jeden.
3.	Sprawdź, czy tytuł strony w zestawie stron jest inny od pozostałych.
4.	Sprawdź, czy tytuł krótko i odpowiednio opisuje treść strony.
5.	Sprawdź, czy tytuł zawiera temat strony i nazwę witryny.
6.	Sprawdź, czy tytuł nie zawiera zbędnej interpunkcji.


### Wykorzystanie ANDI

{% include image.html file="andi/andi_page-title.png" alt="Wykorzystanie skryptozkładki ANDI" %}
1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *struktura*.
2.	Wybierz z menu poziomego opcję *więcej szczegółów*.
3.	Wybierz z rozwijanej listy opcję *tytuł strony*.
4.	Sprawdź w oknie dialogowym, czy tytuł został określony, czy opisuje treść strony, czy zawiera temat strony i nazwę witryny, czy zawiera tylko uzasadnione zasadami pisowni znaki interpunkcyjne.

## Zasoby
### Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G88.md %}
- {% include techniki/H25.md %}
- {% include techniki/F25.md %}
- {% include techniki/G127.md %}

### Opracowania
{% include doglos/242-tytul-zasoby.md %}

## Przypadki testowe

### Zaliczone

```html
<title>Strona główna | Pracownia Dostępności Cyfrowej LepszyWeb.pl</title>
<title>O nas | LepszyWeb.pl</title>
<title>Usługi | LepszyWeb.pl<title>
```

### Niezaliczone
- brak tytułu w znaczniku `<title>` (pusty znacznik)
  ```html
  <title></title>
  ```  
- tytuły nieopisujące treści:
  ```html
  <title>xxxx</title>
  <title>12345</title>
  ```
- tytuły z nagromadzeniem zbędnych znaków interpunkcyjnych:
  ```html
  <title>... == Jakiś tytuł strony == ...</title>
  <title>:: Jakiś tytuł strony :: </title>
  ```
