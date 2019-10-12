## Identyfikacja języka

### Metoda badania: 
Kontrola wzrokowa. Inspekcja kodu HTML. 

### Oczekiwania:
Kryterium sukcesu: [3.1.1 Język strony](https://wcag.lepszyweb.pl/#language-of-page), kryterium sukcesu: [3.1.2 Język części](https://wcag.lepszyweb.pl/#language-of-parts).

- Element `<html>` zawiera atrybut języka `lang`, a określony w nim język pasuje do głównego języka strony. 
- Treść w innych językach ma odpowiednio zdefiniowany atrybut językowy na elemencie obejmującym fragment innojęzyczny. 

### Procedura testowania: 
1.	Przeglądając treść strony, zidentyfikuj domyślny naturalny język strony. Domyślnym jest język, w którym prezentowana jest większość treści.
2.	Zobacz źródło strony i sprawdź, czy w znaczniku `<html>` zdefiniowany jest atrybut `lang`.
3.	Sprawdź, czy wartość atrybutu `lang` odpowiada domyślnemu językowi strony.
4.	Przejrzyj ponownie stronę i sprawdź, czy pojawiają się na stronie pojedyncze słowa lub zestawienia słów w innych językach, niż naturalny język strony.
5.	Korzystając z funkcji Zbadaj element w przeglądarce, sprawdź, czy każdy znaleziony innojęzyczny element strony został objęty odpowiednim znacznikiem z poprawną wartością atrybutu `lang`.


### Zasoby

#### Pomocne narzędzia:
- skryptozakładka [Images](http://pauljadam.com/bookmarklets/index.html)  z kolekcji Paula J. Adama
- skryptozakładka [Lang Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 