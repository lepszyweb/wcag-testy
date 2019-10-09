## Nagłówki

### Metoda badania: 
Inspekcja kodu, wykorzystanie narzędzia ujawniającego nagłówki i kontrola wzrokowa

### Oczekiwania:
Kryteria sukcesu: [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships), [2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels)
-	Nagłówki służą do określania części strony.  
-	Znacznikami `h1` – `h6` oznaczone są tylko i wyłącznie elementy strony będące tytułami bądź śródtytułami (znaczniki `h1`-`h6` nie są używane tylko do graficznego wyróżniania tekstu). 
-	Tekst nagłówków odpowiednio opisuje treść sekcji lub strony  
-	Hierarchia i zagnieżdżenie nagłówków odzwierciedla hierarchię treści strony. 
-	Tytuł głównej treści strony jest oznaczony nagłówkiem `<h1>` (rozwiązanie preferowane) 
-	Poziomy nagłówków nie są pomijane (rozwiązanie preferowane).

Uwaga: Nagłówki mogą być również zdefiniowane za pomocą atrybutu ARIA `role="heading"`, a poziom nagłówków za pomocą atrybutu `aria-level="x"`, gdzie x to liczba definiująca poziom nagłówka.  

### Instrukcja testowania: 
1.	Sprawdź, czy każdy nagłówek opisuje temat lub cel następującej po nim treści.
2.	Sprawdź, czy ważniejsze nagłówki mają wyższy poziom. Na przykład, `<h1>` jest poziomem wyższym niż `<h2>`, który jest wyższy niż `<h3>`.
3.	Sprawdź, czy nagłówki z wyższym poziomem rozpoczynają nowe sekcje, a nagłówki z niższym poziomem nowe podsekcje, które są częścią sekcji o wyższym poziomie.
4.	Sprawdź, czy każdy element zdefiniowany w kodzie jako nagłówek służy rzeczywiście jako nagłówek (tytuł, śródtytuł).

### Pomocne narzędzia:
-	skryptozakładka [Headings](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakladka [H123](https://hinderlingvolkart.github.io/h123/). Wyświetla konspekt nagłówków przeglądanej strony. Autorzy z Hinderling Volkart AG  promują ją hasłem „Zobacz nagłówki jak czytnik ekranu!”.
-	Opcja *struktures* w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi_headings.png)
1.	Uruchom skryptozakładkę ANDI. 
2.	Wybierz z menu ANDI opcję *struktures*, a następnie z menu poziomego *XX headings* (XX oznacza liczbę nagłówków wykrytych na stronie) 
3.	Użyj łącza *View outline*, aby rozwinąć konspekt i sprawdź, czy hierarchia nagłówków nie jest bez istotnego powodu zaburzona. 
4.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, przejrzyj wszystkie nagłówki na stronie. 
5.	Zbadaj każdy nagłówek według zaleceń powyżej w sekcji Instrukcje.    
 

