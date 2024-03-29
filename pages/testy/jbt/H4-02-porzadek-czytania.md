---
title: Porządek czytania

sidebar: testy_sidebar
permalink: H4-02-porzadek-czytania
folder: testy/jbt
---


# Porządek czytania

## Metoda badania:
Kontrola wizualna, test z czytnikiem ekranu, linearyzacja treści  

## Zastosowanie:
Cała treść strony.

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

## Oczekiwania:
Kryterium sukcesu: [1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence)
-	Kolejność odczytu treści strony jest logiczna i zrozumiała.
-	Kolejność wizualna treści w kluczowych obszarach strony jest zrozumiała i logiczna.   
-	Kolejność odczytu przez technologię wspomagającą odpowiada wizualnemu układowi strony.
-	Wszystkie widoczne teksty są odczytywane przez czytnik ekranu.
-	Wszystkie treści ukryte przed osobami widzącymi, są ukryte również przed czytnikami ekranu.

## Procedura testowania:
1.	Sprawdź, czy zawartość jest uporządkowana w znaczącej kolejności po linearyzacji, na przykład gdy arkusze stylów są wyłączone. *Uwaga*: po wyłączeniu CSS mogą być widoczne niektóre treści przeznaczone do ukrycia.
2.	Sprawdź, czy kolejność, w jakiej treść strony jest odczytywana przez czytnik ekranu, jest logiczna i znacząca.

## Wykorzystanie skryptozkładki ANDI
{% include image.html file="andi/andi-reading-order.png" alt="Wykorzystanie skryptozkładki ANDI" %}

1.	Uruchom skryptozakładkę ANDI i wybierz z menu ANDI opcję *struktura*.
2.	Wybierz z menu poziomego opcję *porządek czytania*
3.	Możesz użyć łącza *pokaż konspekt*, aby rozwinąć konspekt strony.
4.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, badaj porządek czytania w kolejnych sekcjach strony.
5.	Sprawdź, czy porządek czytania w każdej przeglądanej części strony jest logiczny i znaczący. ANDI oznacza kolejność czytania elementów liczbami porządkowymi.  

## Zasoby

### Pomocne narzędzia:
-	skryptozakładka [Reading Order Bookmarklet](https://adrianroselli.com/2019/04/reading-order-bookmarklet.html) z kolekcji Adriana Roselli
-	bezpłatny czytnik ekranu [NVDA](https://www.nvda.pl/pobierz) dla Windows
-	skryptozakładka [Screen Curtain](http://whatsock.com/training/matrices/screen_curtain.htm) z kolekcji WhatSock.
-	opcja structure w skryptozakładce [ANDI](https://lepszyweb.pl/andi/help/install.html)

*Uwaga*: Aby odsłuchać treść strony czytnikiem NVDA, użyj najpierw kombinacji klawiszy Ctrl+Home, a następnie [NVDA]+Strzałka w dół ([NVDA] to klawisz modyfikujący, domyślnie Insert, często zmieniany na CAPSLock).

### Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/G57.md %}
- {% include techniki/H34.md %}
- {% include techniki/H56.md %}
- {% include techniki/C6.md %}
- {% include techniki/C8.md %}
- {% include techniki/C27.md %}


## Przypadki testowe

### Zaliczone
_do opracowania_

### Niezaliczone
_do opracowania_




