# Formularze - Etykiety i instrukcje

### Metoda badania: 
Kontrola wzrokowa, inspekcja kodu 

### Zastosowanie:
-	Wszystkie komponenty zbierające dane (kontrolki formularzy), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru oraz przyciski zarządzania wypełnionymi formularzami (wyślij, zrezygnuj, wyczyść).
-	Wszystkie instrukcje i wskazówki tekstowe i graficzne związane z kontrolkami formularzy, w tym dotyczące zgrupowania pól, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania, itp.   

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryteria sukcesu: [1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content), [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#headings-and-labels), [1.3.5 Określenie pożądanej wartości](https://wcag.lepszyweb.pl/#identify-input-purpose), [2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels), [3.3.2 Etykiety lub instrukcje](https://wcag.lepszyweb.pl/#labels-or-instructions), [2.5.3 Etykieta w nazwie](https://wcag.lepszyweb.pl/#label-in-name)
-	Wszystkie pola i kontrolki w formularzu posiadają powiązaną programowo etykietę tekstową (grupy pól mogą współdzielić etykietę). 
-	Pola formularza z wieloma etykietami są oznaczone za pomocą legendy grupy pól lub etykietą wskazaną atrybutem `aria-labelldedby`.
-	Elementom `label` zawierającym unikalne etykiety tekstowe w atrybucie `for` przypisane są prawidłowe wartości identyfikatorów pól, do których się odnoszą  
-	Każda etykieta tekstowa wyraźnie określa cel lub funkcję pola formularza lub kontrolki.
-	Wszystkie etykiety pól i kontrolek formularzy są z nimi powiązane programowo ALBO istnieje alternatywna etykieta zapewniona za pomocą atrybutu `title` bądź `aria-label`
-	Etykieta tekstowa pozostaje widoczna, gdy pole posiada fokus klawiatury i po wypełnieniu pola 
-	Etykiety i instrukcje zawierają wystarczające szczegóły, w tym wszelkie wymagania dotyczące formatowania (w tym reguły dotyczące hasła) oraz informacje, czy pole jest wymagane.
-	Opisy formatowania lub inne krytyczne instrukcje w celu prawidłowego wypełnienia pola są dodawane za pomocą atrybutu `aria-describedby` lub w etykiecie pola formularza.
-	Stosowane są odpowiednie atrybuty typu danych (Zobacz: [HTML 5 input types](http://www.w3.org/TR/html52/sec-forms.html#sec-states-of-the-type-attribute)).
-	Stosuje się odpowiednie atrybuty autouzupełniania.

### Instrukcje testowania
1.	Sprawdź, czy każdy komponent formularza zbierający dane ma etykietę(-y) lub instrukcje.
2.	Sprawdź, czy etykiety i  instrukcje dla każdej kontrolki zbierającej dane informują użytkowników, jakie informacje i – w stosownych przypadkach - jaki format jest wymagany.
3.	Sprawdź, czy kombinacje dostępnej nazwy, dostępnego opisu i innych powiazań programowych (np. powiązane kolumny i wiersze tabeli) zrozumiale opisują każdą kontrolkę zbierającą dane i zawierają instrukcje i wskazówki niezbędne i odpowiednie do poprawnego podania danych. Zobacz [Mapowanie API dostępności HTML 1.0](https://www.w3.org/TR/html-aam-1.0/#input-type-text-input-type-password-input-type-search-input-type-tel-input-type-url-and-textarea-element), aby uzyskać szczegółowe informacje na temat technik określania dostępnej nazwy i opisu. 
4.	Sprawdź, czy znaczniki legend są poprawnie i odpowiednio stosowane do oznaczania grupy powiązanych pól. 
5.	Sprawdź, czy atrybuty ARIA używane do znakowania formularzy są używane prawidłowo, w tym czy: 
    - atrybuty `aria-labelledby` wskazują na identyfikator etykiety
    - atrybuty `aria-describedby` wskazuje na identyfikator elementu z dodatkowymi informacjami instruktażowymi, takich jak formatowanie lub wymagania dotyczące hasła.
    - atrybuty `aria-label` są używane tylko wtedy, gdy etykieta tekstowa nie byłaby odpowiednia dla osoby korzystającej z czytnika ekranu (preferowany tytuł)

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/img/andi-forms.png) 
1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *focusable elements*.
2.	Użyj przełącznika między wykrytymi elementami strony, aby wybierać komponenty formularzy do analizy.
3.	Dane wybranego komponentu (znacznik, typ,...) pojawiają obok etykiety *Element*.
4.	Sprawdź w sekcji podsumowującej informacje statystyczne o liczbie wykrytych elementów i możliwych problemach 
5.	Sprawdź w sekcji *Accessibility Component*, jakie właściwości decydujące o dostępności komponentu zostały wdrożone oraz jakie defekty lub możliwe defekty zostały wykryte. Zbadaj dokładnie każdy z wykrytych defektów. 
6.	Sprawdź w sekcji *ANDI Output*, czy użytkownik technologii wspomagającej zostanie wystarczająco i odpowiednio poinstruowany, jakie podać dane i w jakim formacie.   

### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Forms](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakładka [Form Labels](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera
-	skryptozakładka [Forms](https://accessibility-bookmarklets.org/install.html) z kolekcji Pixo i University of Illinois. z kolekcji Pixo i University of Illinois.
-	Opcja focusable elements w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 
-	Opcja links/buttons w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html) 

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 