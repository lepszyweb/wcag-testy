## Nawigacja - Widoczny wskaźnik fokus

### Metoda badania: 
Kontrola wizualna. Test nawigacji za pomocą klawiatury

### Oczekiwania:
Kryterium sukcesu: [2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible)
-	Wskaźnik punktu uwagi (fokus) podczas nawigacji klawiaturą po stronie jest zawsze widoczny i wyraźny:
    -	Kontur, tło lub podkreślenie ma współczynnik kontrastu 4,5:1 w stosunku do tła.
    -	Zmiana koloru obiektu ma współczynnik kontrastu pomiędzy dwoma kolorami wynoszący co najmniej 3:1

*Uwaga:* Wyrazistość widocznego fokusa jest subiektywna. Minimalnym wymaganym poziomem wyrazistości są domyślne ustawienie wyświetlacza przeglądarki (lub platformy systemu operacyjnego).

*Uwaga2*: Wskaźnik fokusa może przybierać różne formy: obramowania elementu, migającego kursora w polu tekstowym, wizualnej zmiany wyglądu przycisku.

### Procedura testowania:
Uwaga: W środowisku testowym podczas testowania nie należy używać żadnych narzędzi modyfikujących wygląd fokusa. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus.  Chociaż takie narzędzia mogą być pomocne w śledzeniu fokusa, to w testowaniu zgodności z KS [2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible) nie mogą być stosowane, bo spowodują uzyskanie nieprawdziwych wyników testu.  
1.	Użyj klawiatury, aby poruszać się po wszystkich interaktywnych komponentach strony.
    1.	Użyj Tab i kombinacji klawiszy Shift+Tab, aby poruszać się między widżetami zarówno do przodu, jak i do tyłu.
    2.	Użyj klawiszy strzałek, aby poruszać się między elementami, na których można ustawiać fokus w złożonym widżecie.
2.	Gdy przenosisz fokus do każdego kolejnego komponentu, sprawdź, czy następuje widoczna i wyraźna zmiana wyglądu elementu, wskazująca, że otrzymał fokus. 

### Zasoby

#### Pomocne narzędzia:

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 
