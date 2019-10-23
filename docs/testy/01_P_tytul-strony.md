## Tytuł strony
Wymaganie WCAG 2.1: Kryterium sukcesu 2.4.2 Tytuł strony (poziom A)

Wszystkie strony internetowe i dokumenty powinny mieć tytuły opisujące ich temat, funkcję lub cel. W witrynach internetowych tytuł każdej strony powinien zawierać nazwę witryny i temat strony. Ogromnym plusem jest także unikatowość tytułu.
Tytuły stron są:
-	wyświetlane na kartach przeglądarek,
-	wyświetlane w wynikach wyszukiwania,
-	wykorzystywane do tworzenia ulubionych zakładek w przeglądarce,
-	odczytywane przez czytniki ekranu.

### Dlaczego tytuł strony jest ważny? 
Dzięki tytułom identyfikujemy wszelkie utwory, a więc strony internetowe również. Tytuł jest nazwą strony. Bez tytułu trudno byłoby się do strony odwołać. 
Zwięzłe, unikalne tytuły stron pomagają użytkownikom zrozumieć treść i cel strony internetowej. Dzięki tytułom użytkownicy mogą łatwo ustalić, czy są zainteresowani treścią strony.
Dobre tytuły stron sprawiają, że różne sposoby wyszukiwania w Internecie potrzebnych treści stają się bardziej wydajne i skuteczne. 
Tytuły są użyteczne dla wszystkich, ale szczególnie przydatne są dla osób niewidomych, ponieważ są zawsze pierwszym elementem strony ogłaszanym przez oprogramowanie do odczytywania ekranu. 
Krótko mówiąc, tytuły są ważne nie tylko ze względu na dostępność.

### Tytuł strony w kodzie HTML
W kodzie strony tytuł strony określony jest za pomocą znacznika `<title>` umieszczanego na początku sekcji `<head>`. Może wyglądać np. tak:
```<title>Dostępny tytuł strony internetowej | Lepszy Web</title>```

**Uwaga**: Znacznik elementu TITLE, znajdujący się w sekcji HEAD kodu HTML strony internetowej, nie powinien być mylony z atrybutem TITLE, który można zastosować do większości elementów HTML.

### Nadawanie tytułów stronom w systemach zarządzania treścią
W systemach do zarządzania treścią stron internetowych, a także w wielu generatorach witryn statycznych tworzenie tytułów stron jest zwykle zautomatyzowane. 
Sposób generowania tytułów stron zależy od przyjętego przez twórców programu rozwiązania projektowego. Zazwyczaj źródłem tytułu konkretnej strony jest tytuł umieszczonej na tej stronie głównej zawartości, np. tytuł artykułu. W niektórych systemach można zdefiniować tytuły stron w opcjach pozycji menu, np. dla stron z przeglądami artykułów czy produktów w kategorii.
Ogólną zasadę generowania tytułu można często określić w sekcji globalnej konfiguracji witryny.  Na przykład w Joomla można zdecydować, czy do tytułów stron dodawać nazwę witryny oraz czy umieszczać ją przed, czy za tytułem.    

### Dobre praktyki
Tytuł strony powinien być:
-	zwięzły, aby go łatwo zapamiętać – nie więcej niż 60-70 znaków (tyle wyświetla Google),
-	wyjątkowy, aby odróżniał stronę od innych,
-	odpowiedni, aby precyzyjnie opisywał treść strony, jej główny temat,
-	sensowny: aby przekazywał przemyślaną, racjonalną informację, a nie dekoracje.
Dobrą praktyką jest, aby tytuł strony internetowej na witrynie składał się z dwóch części: 
-	unikatowego tematu strony i 
-	nazwy witryny.
Anglojęzyczni specjaliści dostępności podkreślają, że tytuły stron powinny być „front-loaded”, czyli żeby ważne i unikatowe informacje identyfikujące stronę znajdowały się z przodu, a nazwa witryny czy nazwa wydawcy za unikatowym tytułem.
#### Zasady pisowni
Według zasad pisowni polskiej po tytułach, śródtytułach i wyrażeniach hasłowych nie stawiamy kropki. Reguła ta odnosi się również do tytułów stron internetowych. Na końcu tytułu kropki nie stawiamy. Ale inne znaki interpunkcyjne – wykrzykniki i pytajniki – stawiamy. Gdy jednak pytanie w tytule jest pozbawione tonu pytającego, to można znak zapytania pominąć. 
W tytułach kilkuczęściowych, np. złożonych z tematu strony i nazwy witryny, potrzebny jest jakiś znak interpunkcyjny jako separator części składowych. Nie ma jasno zdefiniowanej reguły dotyczących stosowania znaków interpunkcyjnych jako separatorów tytułów. Mogą to być myślniki. Często jest to znak pionowej kreski „|”  (nazywany „pipe”). Można też użyć kropki.  
Nie należy natomiast używać w tytułach znaków interpunkcyjnych do celów dekoracyjnych, na przykład ":: Tytuł ::" lub "... == Tytuł == ...".  Każdy taki znak jest odczytywany przez czytniki ekranu, co sprawia, że odsłuchanie tytułów staje się uciążliwe.   
#### Przykłady złych praktyk w tytułowaniu stron
-	Witamy na stronie głównej Pracowni Dostępności Cyfrowej LepszyWeb.pl
-	Pracownia Dostępności Cyfrowej LepszyWeb.pl | O nas
-	Pracownia Dostępności Cyfrowej LepszyWeb.pl – Usługi
-	Pracownia Dostępności Cyfrowej LepszyWeb.pl :: Skontaktuj się z nami
#### Przykłady dobrych praktyk
-	Strona główna | Pracownia Dostępności Cyfrowej LepszyWeb.pl
-	O nas | LepszyWeb.pl
-	Usługi | LepszyWeb.pl
-	Skontaktuj się z nami | LepszyWeb.pl
Zwróć uwagę, że pełna nazwa witryny w przykładach powyżej została zastosowana tylko na stronie głównej. 

Poniższy obraz przedstawia tytuły trzech stron na zakładkach kart na pasku tytułowym w przeglądarce Firefox. Zauważ, że w kartach wyświetlana jest tylko pierwsza część tytułu strony. Ale gdy otworzymy więcej kart, zakładki z tytułami mogą ulec tak dużemu zwężeniu, że będzie na nich widać jedynie ikonę witryny (favicon).
 
Podobnie jest w przeglądarce Chrome.
 
Jeśli jednak ustawisz kursor myszki nad zakładką, zobaczysz w dymku pełny tytuł witryny.

## Jak testować (co robić):
-	Spójrz na tytuł głównej strony witryny (lub odsłuchaj go, jeśli korzystasz z czytnika ekranu).
-	Spójrz na tytuły co najmniej kilku innych stron w witrynie.
## Co sprawdzać:
-	Czy każda strona ma tytuł? 
-	Czy tytuł każdej strony krótko i odpowiednio opisuje jej treść?
-	Czy tytuł każdej strony jest inny od pozostałych?
-	Czy tytuły nie zawierają zbędnej interpunkcji?
-	Czy tytuły zawierają nazwę witryny?

-------------------------------------
[Baza testów wstępnych. Wprowadzenie &lt; Poprzednia strona](00_P_Wprowadzenie.md) | [Następna strona &gt; Odpowiendiki tekstowe obrazów](testy/02_P_odpowiedniki-tekstowe-obrazow.md)