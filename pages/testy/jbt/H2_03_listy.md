---
title: Listy

summary: "Cała treść strony umieszczona jest w oznaczonych głównych obszarach (punktach orientacyjnych)."
sidebar: testy_sidebar
permalink: H2_03_listy
folder: testy/jbt
---

## Listy

### Metoda badania: 
Inspekcja kodu, wykorzystanie narzędzia ujawniającego listy, kontrola wzrokowa

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
-	Autor zastosował odpowiednie typy list (nieuporządkowane, uporządkowane, opisów) 
-	Listy jednopoziomowe znajdują się w obrębie jednego elementu listy (`<ol>`, `<ul>` lub `<dl>`).
-	Elementy na listach uporządkowanych i nieuporządkowanych objęte są znacznikami `<li>`, a na listach opisów znacznika `<dd>`. 
-	Zagnieżdżenia list podrzędnych na listach wielopoziomowych są poprawne (listy podrzędne umieszczone są wewnątrz znaczników `<li>`).

### Procedura testowania:
1.	Przejrzyj stronę. Znajdź na stronie zestawienia elementów wyglądające jak listy.
2.	Sprawdź, czy wykazy, w których kolejność elementów nie ma istotnego znaczenia, zostały oznaczone jako listy nieuporządkowane (za pomocą znacznika `<ul>`.
3.	Sprawdź, czy wykazy, w których kolejność elementów jest istotna, bo np. przedstawiają kolejność kroków w procedurze, zostały oznaczone jako listy uporządkowane (za pomocą znacznika `<ol>`.
4.	Sprawdź, czy treści, które prezentują grupy elementów powiązanych na zasadzie nazwa-wartość są oznakowane jako listy opisów (za pomocą znacznika `<dl`>.  
5.	Sprawdź, czy wykazy z hierarchią zagnieżdżonych elementów są zagnieżdżone poprawnie, to znaczy listy podrzędne umieszczone są wewnątrz znaczników `<li>` .  


### Wykorzystanie skryptozkładki ANDI

{% include image.html file="andi/andi-listy.png" alt="Wykorzystanie skryptozkładki ANDI" %} 
1.	Uruchom skryptozakładkę ANDI. 
2.	Wybierz z menu ANDI opcję *structures*, a następnie z menu poziomego *XX lists* (XX oznacza liczbę list wykrytych na stronie) 
3.	Zobacz szczegółową informację o liczbie i typie wykrytych list.
4.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, zbadaj każdą listę według zaleceń powyżej w sekcji Instrukcje.    
 
### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Lists](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	Opcja *structures* w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 
