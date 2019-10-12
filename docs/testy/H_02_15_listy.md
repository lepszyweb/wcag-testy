## Listy

### Metoda badania: 
Inspekcja kodu, wykorzystanie narzędzia ujawniającego listy, kontrola wzrokowa

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


### Pomocne narzędzia:
-	skryptozakładka [Lists](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	Opcja Structures w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi-listy.png)
1.	Uruchom skryptozakładkę ANDI. 
2.	Wybierz z menu ANDI opcję *structures*, a następnie z menu poziomego *XX lists* (XX oznacza liczbę list wykrytych na stronie) 
3.	Zobacz szczegółową informację o liczbie i typie wykrytych list.
4.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, zbadaj każdą listę według zaleceń powyżej w sekcji Instrukcje.    
 

