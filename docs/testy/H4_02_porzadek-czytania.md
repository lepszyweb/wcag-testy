# Porządek czytania/treści

### Metoda badania:
Kontrola wizualna, test z czytnikiem ekranu, linearyzacja treści  

### Zastosowanie:
Cała treść strony.

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence)
-	Kolejność odczytu treści strony jest logiczna i zrozumiała. 
-	Kolejność wizualna treści w kluczowych obszarach strony jest zrozumiała i logiczna.   
-	Kolejność odczytu przez technologię wspomagającą odpowiada wizualnemu układowi strony.
-	Wszystkie widoczne teksty są odczytywane przez czytnik ekranu.
-	Wszystkie treści ukryte przed osobami widzącymi, są ukryte również przed czytnikami ekranu.

### Procedura testowania:
1.	Sprawdź, czy zawartość jest uporządkowana w znaczącej kolejności po linearyzacji, na przykład gdy arkusze stylów są wyłączone. *Uwaga*: po wyłączeniu CSS mogą być widoczne niektóre treści przeznaczone do ukrycia.
2.	Sprawdź, czy kolejność, w jakiej treść strony jest odczytywana przez czytnik ekranu, jest logiczna i znacząca.

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi-reading-order.png) 
1.	Uruchom skryptozakładkę ANDI i wybierz z menu ANDI opcję *structures*.
2.	Wybierz z menu poziomego opcję *reading order* (Porządek czytania) 
3.	Możesz użyć łącza *View outline*, aby rozwinąć konspekt strony. 
4.	Posługując się przełącznikiem między wykrytymi elementami struktury strony, badaj porządek czytania w kolejnych sekcjach strony. 
5.	Sprawdź, czy porządek czytania w każdej przeglądanej części strony jest logiczny i znaczący. ANDI oznacza kolejność czytania elementów liczbami porządkowymi.  
    
### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Reading Order Bookmarklet](https://adrianroselli.com/2019/04/reading-order-bookmarklet.html) z kolekcji Adriana Roselli
-	bezpłatny czytnik ekranu [NVDA](https://www.nvda.pl/pobierz) dla Windows
-	skryptozakładka [Screen Curtain](http://whatsock.com/training/matrices/screen_curtain.htm) z kolekcji WhatSock. 
-	opcja structure w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/images/andi/help/install.html) 

*Uwaga*: Aby odsłuchać treść strony czytnikiem NVDA, użyj najpierw kombinacji klawiszy Ctrl+Home, a następnie [NVDA]+Strzałka w dół ([NVDA] to klawisz modyfikujący, domyślnie Insert, często zmieniany na CAPSLock).

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 
