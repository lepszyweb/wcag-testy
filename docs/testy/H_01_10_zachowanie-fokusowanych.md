## Nawigacja - Zachowanie fokusowanych komponentów

### Metoda badania: 
Kontrola wizualna. Test nawigacji za pomocą klawiatury, wykorzystanie narzędzia ujawniającego interaktywne elementy strony

### Oczekiwania:
Kryteria sukcesu: [2.1.2 Brak pułapki na klawiaturę](https://wcag.lepszyweb.pl/#no-keyboard-trap), [3.2.1 Po oznaczeniu fokusem](https://wcag.lepszyweb.pl/#on-focus)
-	Z każdego komponentu strony, na który został przeniesiony fokus klawiatury można go przenieść na inny komponent za pomocą klawiatury (klawisza Tab lub kombinacji Tab+Shitf)
-	Wprowadzenie lub usunięcie danych w polu formularza, w tym w opcjach wyboru nie powoduje zmiany położenia fokusa.
-	Gdy przeniesienie fokusa klawiatury na interaktywny element strony odsłania schowaną treść,  w której znajdują się elementy interaktywne, nawigacja klawiaturą przenosi fokus na pierwszy element interaktywny w odkrytej treści. 

### Procedura testowania:
1.	Użyj klawiatury, aby poruszać się po wszystkich interaktywnych komponentach strony.
    1.	Użyj Tab i kombinacji klawiszy Shift+Tab, aby poruszać się między widżetami zarówno do przodu, jak i do tyłu.
    2.	Użyj klawiszy strzałek, aby poruszać się między elementami, na których można ustawiać fokus w złożonym widżecie.
2.	Sprawdź, że zawsze można przenieść fokus na poprzedni lub następny interaktywny element strony (znajdujący się w porządku tabulacji).
3.	Gdy trafisz na tzw. pułapkę klawiatury (czyli nie będzie możliwe przeniesienie fokusa za pomocą klawiatury na inny element), odnotuj ten defekt w ustaleniach, a następnie myszki, aby wyprowadzić fokus z pułapki.
4.	Sprawdź również, czy przeniesienie fokusa klawiatury nie powoduje niespodziewanych zdarzeń, np. nie wywołuje akcji skojarzonej z pozycją na rozwijanej liście wyboru w formularzu    

### Pomocne narzędzia:






