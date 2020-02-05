## Współczynnik kontrastu tekstu do tła

### Metoda badania: 
Użyj narzędzia do testowania kontrastu, aby określić współczynniki kontrastu.

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryteria sukcesu: [1.4.3 Kontrast (minimalny)](https://wcag.lepszyweb.pl/#contrast-minimum), [1.4.11 Kontrast elementów nietekstowych](https://wcag.lepszyweb.pl/#non-text-contrast)
-	Współczynnik kontrastu dla wszystkich standardowych tekstów na stronie jest równy lub większy niż 4,5:1.
-	Współczynnik kontrastu dla dużych tekstów (Nagłówki i inne duże pozycje) przekracza 3,0:1.
-	Współczynnik kontrastu dla obrazów tekstu, innych niż logotypy i wizerunki marki, które są wykorzystywane do przekazywania informacji przekracza 3,0:1.
-	Współczynnik kontrastu dla wszystkich tekstów w aktywnych kontrolkach przekracza 4,5:1.
    -	Wyłączone elementy sterujące nie wymagają kontrastu.
-	Aktywne elementy interfejsu strony, takie jak linki, przyciski, kontrolki formularzy, styl domyślnego fokusa,  mają współczynnik kontrastu  w stosunku do tła 3:1 zarówno w stanie domyślnym, po wczytaniu strony, jak i w stanie aktywności (wskazywania, po otrzymaniu fokusa) 
-	Obiekty graficzne na grafikach wymaganych do zrozumienia treści mają współczynnik kontrastu w stosunku do tła co najmniej 3:1

### Procedura testowania:
1.	Użyj wybranego narzędzia, aby sprawdzić czy współczynnik kontrastu między tekstem a tłem wynosi co najmniej 4.5:1.
2.	 Jeśli współczynnik kontrastu jest mniejszy niż 4.5:1, sprawdź, czy współczynnik wynosi co najmniej 3:1  ORAZ czy czcionka spełnia jedno z poniższych wymagań: 
   -	ma rozmiar co najmniej 18 punktów (23,94 pikseli)
   -	ma rozmiar co najmniej 14 punktów  (18.62 pikseli) ORAZ pogrubienie (wagę co najmniej 700)
3.	Sprawdź, czy na obiektach graficznych między elementami pierwszego planu wymaganymi do zrozumienia treści a tłem współczynnik kontrastu wynosi co najmniej 3:1
4.	Sprawdź, czy współczynnik kontrastu między wizualnymi wskaźnikami aktywnych elementów interfejsu w stosunku do tła wynosi co najmniej 3:1. Przetestuj te wskaźniki kontrastu w każdym stanie.

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi-kontrast.png) 
1.	Uruchom skryptozakładkę ANDI i wybierz z menu ANDI opcję *color contrast*. 
2.	Zobacz informację o liczbie wykrytych na stronie elementów oraz zapoznaj się z alertami dotyczącymi wykrytych problemów z kontrastem.  
3.	ANDI przedstawia wynik testu kontrastu dla każdego wykrytego na stronie elementu.
4.	Informacja obejmuje faktyczny współczynnik kontrastu, stwierdzenie zgodności z wymaganiami (*FAIL* – niezgodny, *PASS* – zgodny), właściwości stylu (kolor tekstu, kolor tła, rozmiar fontu) oraz sugerowaną wartość koloru tła, aby zapewnić zgodność).
5.	Jeżeli kontrast jest niezgodny z wymaganiami, ANDI wyświetla stosowny komunikat.   
6.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, sprawdź poprawność kontrastu wszystkich wykrytych na stronie elementów 

### Zasoby

- [The Myths of Color Contrast Accessibility](https://uxmovement.com/buttons/the-myths-of-color-contrast-accessibility/)


#### Pomocne narzędzia:
-	[Colour Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/)
-	skryptozakładka [Tota11y](https://khan.github.io/tota11y/) 
-	skryptozakładka [Grayscale](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakładka [Grayscale](https://thomaspark.co/2013/11/3-simple-design-bookmarklets-to-improve-your-aesthetics/) z kolekcji Thomasa Parka. Wyświetla stronę w skali szarości. Pomaga wykryć obszary, które mogą mieć wystarczający kontrast w kolorze, ale nie mają wystarczającego kontrastu w skali szarości, co ma znaczenie dla dostępności dla osób dotkniętych zaburzeniami widzenia kolorów.
-	opcja contrast w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/images/andi/help/install.html)

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 