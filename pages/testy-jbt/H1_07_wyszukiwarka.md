---
title: Nagłówek - Wyszukiwarka

summary: "Cała treść strony umieszczona jest w oznaczonych głównych obszarach (punktach orientacyjnych)."
sidebar: testy-jbt_sidebar
permalink: H1_07_wyszukiwarka
folder: testy-jbt
---


## Nagłówek - Wyszukiwarka

### Metoda badania:
Kontrola wizualna, test ręczny, inspekcja kodu, test obsługi z czytnikiem ekranu 

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships), [2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels), [2.4.5 Wiele dróg](https://wcag.lepszyweb.pl/#multiple-ways).
-	Wyszukiwarka znajduje się na początku strony w miejscu, w którym spodziewają się ją znaleźć użytkownicy
-	Wyszukiwarka jest łatwo rozpoznawalna na podstawie stylizacji graficznej lub etykiety „Szukaj” lub równorzędnej ogłoszonej użytkownikom czytników ekranu.    
-	Wyszukiwanie rozpoczyna się tylko na żądanie użytkownika – po naciśnięciu klawisza Enter bądź odpowiedniego przycisku.
-	Użytkownik klawiatury może opuścić pole wyszukiwania (brak pułapki na klawiaturę).

### Procedura testowania:
1.	Sprawdź, czy na każdej stronie wyszukiwarka znajduje się w tym samym miejscu.
2.	Sprawdź, czy na każdej stronie wyszukiwarka ma taką samą funkcjonalność.
3.	Sprawdź, czy do pola wyszukiwania można wejść i opuścić je tylko za pomocą klawiatury (klawisza Tab).
4.	Sprawdź, czy wyszukiwanie szukanego tekstu rozpoczyna się dopiero po naciśnięciu klawisza Enter lub uaktywnieniu przycisku Szukaj lub równorzędnego  
5.	Sprawdź, czy w kodzie źródłowym łącze do wyszukiwarki pojawia się zawsze w tym samym porządku.
6.	Odsłuchaj stronę czytnikiem ekranu i sprawdź, czy czytnik ogłasza etykiety pola wyszukiwania i przycisku wyzwalającego wyszukiwanie.  

### Test z wykorzystaniem ANDI

{% include image.html file="andi/andi-wyszukiwarka2.png" alt="Wykorzystanie skryptozkładki ANDI" %}

1.	Uruchom skryptozakładkę ANDI. 
2.	Wybierz z menu ANDI opcję *focusable elements*, a następnie z menu poziomego *label tags*. 
3.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, znajdź komponent wyszukiwarki. 
4.	Sprawdź, czy w informacjach o komponencie znajduje się tekst zdefiniowanej etykiety (tekst po słowie label poniżej wylistowanych składników.
5.	Sprawdź, czy w sekcji *ANDI Output* znajduje się ikona symbolizująca dźwięk i napis z tekstem etykiety Szukaj lub równoważnym (jest to tekst ogłaszany przez czytnik ekranu).
6.	Jeśli obok pola wyszukiwania umieszczony jest przycisk „Znajdź”, „Idź” lub podobny, wybierz go za pomocą przełącznika między wykrytymi elementami struktury i sprawdź, czy posiada dostępną nazwę ogłaszaną przez czytnik ekranu.       
 
### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Sr-only Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access. Wyświetla zawartość objętą znacznikiem z klasą „sr-only”, czyli „widoczną” tylko dla czytników ekranu.
-	skryptozakładka [[Forms](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakładka [Form Labels](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera. Oznacza etykiety formularzy, zlicza i wyróżnia błędy etykietowania.

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_