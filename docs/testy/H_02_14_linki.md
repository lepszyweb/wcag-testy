# Linki

### Metoda badania: 
Inspekcja kodu

### Oczekiwania:
Kryterium sukcesu: [2.4.4. Cel linku w kontekście](https://wcag.lepszyweb.pl/#link-purpose-in-context) 
-	Każde łącze na stronie prowadzi do miejsca na stronie lub innej strony albo do dokumentu  
-	Tekst łącza opisuje miejsce przeznaczenia (sytuacja preferowana).
-	Jeżeli tekst łącza nie jest jednoznaczny, to miejsce przeznaczenia jest opisane przez kontekst (wymagane), w tym: 
    - tekst w tym samym zdaniu, akapicie, elemencie listy lub komórce tabeli co łącze ALBO
    - tekst w nadrzędnym elemencie listy, ALBO
    - tekst w komórce nagłówka tabeli, który jest powiązany z komórką zawierającą łącze.
-	Naciśnięcie łącza klawiszem Enter wywołuje połączenie z docelową stroną, miejscem lub dokumentem.
-	Łącza z takim samym celem mają taki sam tekst łącza, łącza do różnych celów mają różniące je teksty łączy. 

### Instrukcje testowania:
1.	Sprawdź na stronie każdy element, który został wyróżniony jako łącze (podkreślony, umieszczony w grupie łączy), czy działa on jako łącze, tzn. przenosi do treści na tej samej lub innej stronie.
2.	Sprawdź, czy cel każdego łącza wynika z jego tekstu (jeśli łącze prowadzi do innej strony lub dokumentu, to nazwa lub tytuł strony albo dokumentu jest wystarczająca).
3.	Sprawdź, czy łącza prowadzące do tego samego celu mają takie same teksty łączy ORAZ czy łącza prowadzące do różnych celów mają odróżniające je teksty łączy.
4.	Jeśli cel łącza wynikający z jego tekstu nie jest jednoznaczny, sprawdź, czy można go wywnioskować z kontekstu, w tym:
-	tekstu w tym samym zdaniu, akapicie, elemencie listy lub komórce tabeli co łącze,
-	tekstu w nadrzędnym elemencie listy, ALBO
-	tekstu w komórce nagłówka tabeli, z którym jest powiązana komórka z łączem.  

### Pomocne narzędzia:
-	opcja *Link Text* w skryptozakładce [Tota11y](https://khan.github.io/tota11y/)  
-	skryptozakładka [Restore Link Underlines](http://adrianroselli.com/2015/01/css-bookmarklets-for-testing-and-fixing.html) Adriana Roselliego. Podkreśla łącza na całej stronie.
-	skryptozakładka [Link underlines] https://github.com/ThePacielloGroup/bookmarklets  z kolekcji Pacciello Group 
-	opcja tables w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi-linki.png)
1.	Uruchom skryptozakładkę ANDI. 
2.	Wybierz z menu ANDI opcję *links/buttons* i zaznacz w menu poziomym opcję *XX links*. (XX oznacza liczbę wykrytych łączy).
3.	Uaktywnij łącze View links list i przejrzyj tabelę z listą wykrytych łączy. Można użyć jednego z filtrów (*all links* – wszystkie łącza, *skip links* -  łącza pomijające, *external links* – łącza do lokalizacji zewnętrznych), aby ograniczyć liczbę wyświetlanych pozycji.  
4.	Sprawdź, czy wybrane łącze zostało utworzone znacznikiem `<a>` (*anachor* - kotwica). 
5.	Sprawdź, czy wybrane łącze ma dostępną nazwę oraz atrybut href wskazujący cel łącza
6.	Sprawdź, czy tekst, jaki ogłosi czytnik ekranu, będzie zrozumiały bez kontekstu. Jeśli nie, sprawdź kontekst łącza i oceń, czy cel łącza będzie zrozumiały z kontekstu.   
7.	Użyj przełącznika między wykrytymi elementami strony, aby sprawdzić kolejne łącze.
