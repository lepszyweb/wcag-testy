---
title: Zmiany rozmiarów i orientacji

summary: "Cała treść strony umieszczona jest w oznaczonych głównych obszarach (punktach orientacyjnych)."
sidebar: testy_sidebar
permalink: H3_04_zmiany-rozmiaru-i-orientacji
folder: testy/jbt
---


## Zmiany rozmiarów i orientacji

### Metoda badania: 
Testy ręczne, kontrola wzrokowa 

### Zastosowanie:
-	Wszystkie treści przeznaczone do prezentacji zarówno na dużych stacjonarnych wyświetlaczach, jak i na wyświetlaczach urządzeń mobilnych.
-	Wszystkie treści, które można powiększyć za pomocą funkcji oprogramowania użytkownika, 

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [1.3.4 Orientacja](https://wcag.lepszyweb.pl/#orientation), [1.4.4 Zmiana rozmiaru tekstu](https://wcag.lepszyweb.pl/#resize-text), [1.4.10 Dopasowanie do ekranu](https://wcag.lepszyweb.pl/#reflow), [1.4.12 Odstępy w tekście](https://wcag.lepszyweb.pl/#text-spacing) 
-	Całą treść strony można powiększyć na ekranie wyświetlacza do 200% bez utraty informacji lub funkcjonalności, w tym czytelności.
-	Powiększenie na stronie tekstu do 200% za pomocą oprogramowania użytkownika lub kontrolek zapewnionych przez stronę nie zaburza czytelności strony i nie powoduje utraty informacji lub funkcjonalności.
-	Jeśli można na stronie lub ekranie powiększyć do 200% tylko tekst Cały tekst na stronie można powiększyć  
-	Całą treść strony można wyświetlać zarówno w pionowym, jak i poziomym ułożeniu ekranu wyświetlacza, z wyjątkiem przypadków, gdy określona orientacja jest niezbędna ze względu na znaczenie lub funkcjonalność.
-	Całą treść strony można przeglądać bez konieczności przewijania w dwóch kierunkach zarówno w pionowym, jak i poziomym ułożeniu ekranu wyświetlacza, z wyjątkiem przypadków, gdy określona orientacja jest niezbędna ze względu na znaczenie lub funkcjonalność.

### Procedura testowania:
1.	Sprawdź, czy możliwe jest skorzystanie z mechanizmu zmiany rozmiaru, skalowania lub powiększenia treści co najmniej do 200% oryginalnego rozmiaru. Mogą to być m.in. poniższe rozwiązania:
    -	funkcja powiększania w przeglądarce,
    -	funkcje powiększania zapewniane przez platformę lub system operacyjny,
    -	przełączniki rozmiaru tekstu zapewnione przez stronę  
2.	Sprawdź, czy po dwukrotnym powiększeniu szerokości i wysokości obszaru roboczego (o 200 %):
    -	cała treść strony jest nadal dostępna,
    -	cała funkcjonalność strony jest nadal dostępna, 
    -	tekst nie jest skracany, obcinany ani zasłaniany,
    -	tekst w polach formularza również zmienia rozmiar,
3.	Sprawdź, czy po dwukrotnym powiększeniu szerokości i wysokości tekstu (o 200 %):
    -	cała treść strony jest nadal dostępna,
    -	cała funkcjonalność strony jest nadal dostępna, 
    -	tekst nie jest skracany, obcinany ani zasłaniany,
    -	tekst w polach formularza również zmienia rozmiar,
4.	Sprawdź czy po zmianie ułożenia (orientacji) wyświetlacza z poziomego na pionowe i odwrotnie cała treść dostosowuje swój rozmiar do zmienionej orientacji wyświetlacza, z wyjątkiem przypadków, gdy do wyświetlenia zawartości konieczna jest określona orientacja ekranu.
    -	Sprawdź czy po zmianie ułożenia (orientacji) wyświetlacza z poziomego na pionowe i odwrotnie całą treść można przeglądać bez konieczności przewijania jej w dwóch kierunkach, z wyjątkiem przypadków, gdy określona orientacja jest niezbędna ze względu na znaczenie lub funkcjonalność.


### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Reset Text Size](http://adrianroselli.com/2015/01/css-bookmarklets-for-testing-and-fixing.html) z kolekcji Adriana Roselliego. Przywraca domyślny rozmiar tekstu dla elementu body, dostosowując rozmiar tekstu do preferencji ustawionych w przeglądarce.
-	skryptozakładka [Text Spacing Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access. Zwiększa odstępy w tekście, aby przetestować kryterium sukcesu 1.4.12
-	skryptozakładka [LargeText](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera
-	skryptozakładka [Set text size](https://github.com/ThePacielloGroup/bookmarklets) z kolekcji Pacciello Group 
-	skryptozakładka [Text spacing](https://github.com/ThePacielloGroup/bookmarklets) z kolekcji Pacciello Group 


#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 