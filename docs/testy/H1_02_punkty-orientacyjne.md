## Punkty orientacyjne lub oznaczenia kluczowych sekcji strony

### Metoda badania:
Wykorzystanie narzędzia ujawniającego punkty orientacyjne, inspekcja kodu.

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
*Uwaga*: Kryteria sukcesu WCAG nie wymagają, aby stosować na stronie znaczniki definiujące obszary strony i punkty orientacyjne. Czy strona spełnia wymienione poniżej oczekiwania sprawdzamy tylko wtedy, gdy stosowane są punkty orientacyjne  i oznaczenia sekcji strony. 
   
Kryteria sukcesu: [3.2.3 Konsekwentna nawigacja](https://wcag.lepszyweb.pl/#consistent-navigation), [3.2.4 Konsekwentna identyfikacja](https://wcag.lepszyweb.pl/#consistent-identification)
-	Cała zawartość strony znajduje się w kluczowych obszarach strony objętych znacznikami lub atrybutami ARIA definiującymi punkty orientacyjne, odpowiednie do celów tych obszarów:  
    -	znacznikiem `header` lub atrybutem `role="banner"` (nagłówek strony, tylko jeden)
    -	atrybutem `role="search"` (wyszukiwanie)
    -	znacznikiem `footer` lub atrybutem `role="contentinfo"` (stopka strony, tylko jedna)
    -	znacznikiem `nav` lub atrybutem `role="navigation"` (nawigacja, jeżeli więcej niż jedna, każda jest jednoznacznie określona etykietą)
    -	znacznikiem `main` lub atrybutem `role="main"` (obszar treści głównej, tylko jeden)
    -	znacznikiem `aside` lub atrybutem `role="complementary"`  (jeśli więcej niż jeden, każdy jest jednoznacznie określony etykietą)
-	Gdy używana jest więcej niż jedna instancja typu obszaru, to każdy z nich jest jednoznacznie określony za pomocą
    -	atrybutu `aria-labelledby` wskazującego na widoczny nagłówek.
    -	atrybutu `aria-label`, jeżeli sekcja nie rozpoczyna się od nagłówka.
-	Obszar oznaczony głównym punktem orientacyjnym nie zawiera żadnych bloków treści, które powtarzają się na pozostałych stronach witryny, np. powtarzalnego obszaru nawigacyjnego (nie dotyczy ścieżki powrotu – jej treść jest inna na każdej stronie). 
-	Liczba obszarów została zminimalizowana.

### Procedura testowania:
1.	Uruchom podgląd rozmieszczenia punktów orientacyjnych na stronie za pomocą jednego z narzędzi ujawniających punkty orientacyjne (zobacz niżej: *Pomocne narzędzia*).
2.	Sprawdź, czy typy punktów orientacyjnych określone użytymi znacznikami bądź atrybutami role zostały odpowiednio zastosowane do kluczowych obszarów strony (tzn. czy znacznik header bądź rola banner została zastosowana do nagłówka strony, znacznik bądź rola main została zastosowana do obszaru zawierającego główną treść strony, itd.
3.	Jeżeli na stronie występuje więcej niż jeden obszar tego samego typu, sprawdź, czy każdy z nich został oznaczony odróżniającą go etykietą lub nagłówkiem. (*Uwaga*: jeżeli jakiś obszar nawigacyjny jest powtórzony na stronie dwukrotnie, np. w nagłówku i stopce, wówczas może być oznaczony taką samą etykietą)     
4.	Sprawdź czy w obszarze głównego punktu orientacyjnego (`main`), znajdują się tylko niepowtarzalne treści (obszar `main` nie może zawierać żadnych bloków treści, które powtarzają się na stronach).


### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Active Images](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera. Oznacza punkty orientacyjne. Sprawdza i wyświetla etykiety zdefiniowane przez aria-labelledby, a nawet poprawność ortograficzną nazwy tego atrybutu (częsty błąd =jedno 'l' zamiast dwóch).
-	skryptozakładka [Ladmarks](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Oznacza punkty orientacyjne. Jeśli zdefiniowane są znacznikiem html – umieszcza etykietę ze znacznikiem na żółtym tle. Jeśli zdefiniowane są atrybutem role, umieszcza etykietę z wartością atrybutu
-	skryptozakładka [Duplicate-landmark-roles](https://github.com/ThePacielloGroup/bookmarklets) z kolekcji Pacciello Group. Oznacza obszary, którym zdefiniowano nadmiarowy niepotrzebny atrybut role.
-	skryptozakładka [Ladmarks](https://accessibility-bookmarklets.org/install.html) z kolekcji Pixo i University of Illinois. Oznacza nakładkami punkty orientacyjne. W etykiecie nakładki komunikuje zastosowany element HTML oraz dostępną nazwę punktu orientacyjnego.
-	opcja Landmarks w skryptozakładce [Tota11y](https://khan.github.io/tota11y/) 
-	skryptozakładka [Web Evaluation Tools](https://accessibility.oit.ncsu.edu/tools/web-evaluation-tools/) udostępniona przez IT Accessibility z NC State University 

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 
