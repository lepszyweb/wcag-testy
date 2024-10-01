---
title: Formularze - Etykiety i instrukcje

sidebar: testy_sidebar
permalink: H5-01-formularze-etykiety-i-instrukcje
folder: testy/jbt
---


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
1.	Sprawdź, czy każde pole formularza zbierające dane ma etykietę lub instrukcję.
2.	Sprawdź, czy etykiety i instrukcje wystarczająco jasno informują użytkowników, jakie informacje i jaki format danych są wymagane 
3.	Sprawdź, czy kombinacje dostępnej nazwy, dostępnego opisu i innych powiazań programowych (np. powiązane kolumny i wiersze tabeli) zrozumiale opisują każdą kontrolkę zbierającą dane i zawierają instrukcje i wskazówki niezbędne i odpowiednie do poprawnego podania danych. Zobacz [Mapowanie API dostępności HTML 1.0](https://www.w3.org/TR/html-aam-1.0/#input-type-text-input-type-password-input-type-search-input-type-tel-input-type-url-and-textarea-element), aby uzyskać szczegółowe informacje na temat technik określania dostępnej nazwy i opisu.
4.	Sprawdź, czy znaczniki legend są poprawnie i odpowiednio stosowane do oznaczania grupy powiązanych pól.
5.	Sprawdź, czy atrybuty ARIA używane do znakowania formularzy są używane prawidłowo, w tym czy:
    - atrybuty `aria-labelledby` wskazują na identyfikator etykiety
    - atrybuty `aria-describedby` wskazuje na identyfikator elementu z dodatkowymi informacjami instruktażowymi, takich jak formatowanie lub wymagania dotyczące hasła.
    - atrybuty `aria-label` są używane tylko wtedy, gdy etykieta tekstowa nie byłaby odpowiednia dla osoby korzystającej z czytnika ekranu (preferowany tytuł)

### Wykorzystanie skryptozkładki ANDI
![Wykorzystanie skryptozkładki ANDI](/images/andi/andi-forms.png)
1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *interaktywne*.
2.	Użyj przełącznika między wykrytymi elementami strony, aby wybierać komponenty formularzy do analizy.
3.	Dane wybranego komponentu (znacznik, typ,...) pojawiają obok etykiety *Element*.
4.	Sprawdź w sekcji podsumowującej informacje statystyczne o liczbie wykrytych elementów i możliwych problemach
5.	Sprawdź w sekcji *Komponenty dostępności*, jakie właściwości decydujące o dostępności komponentu zostały wdrożone oraz jakie defekty lub możliwe defekty zostały wykryte. Zbadaj dokładnie każdy z wykrytych defektów.
6.	Sprawdź w sekcji *Wyjście ANDI*, czy użytkownik technologii wspomagającej zostanie wystarczająco i odpowiednio poinstruowany, jakie podać dane i w jakim formacie.   

### Zasoby
- [Forms Tutorial](https://www.w3.org/WAI/tutorials/forms/)
- [Jim Allan’s Slides on Accessible Forms](https://patterns.tsbvi.edu/forms/1-welcome.html)
- [Form accessibility: a practical guide](https://itnext.io/form-accessibility-a-practical-guide-4062b7e2dd14)
- [The Anatomy of Accessible Forms: The Problem with Placeholders](https://www.deque.com/blog/accessible-forms-the-problem-with-placeholders/)
- [The Anatomy of Accessible Forms: Required Form Fields](https://www.deque.com/blog/anatomy-of-accessible-forms-required-form-fields/)
- [The Anatomy of Accessible Forms: Best Practices](https://www.deque.com/blog/anatomy-of-accessible-forms-best-practices/)
- [The Anatomy of Accessible Forms: Error Messages](https://www.deque.com/blog/anatomy-of-accessible-forms-error-messages/)
- [Forms, Form Validation, and CAPTCHAs](http://web-accessibility.carnegiemuseums.org/code/forms/)
- [How to make an accessible form: it’s easier than you think](https://www.freecodecamp.org/news/how-to-make-an-accessible-form-its-easier-than-you-think-672d3f4ff573/)
- [Creating Accessible Forms](https://webaim.org/techniques/forms/controls)
- [Designing Accessible Forms](https://blog.prototypr.io/designing-accessible-forms-82f2ea11697f)
- [Forms, Form Validation, and CAPTCHAs](http://web-accessibility.carnegiemuseums.org/code/forms/)
- [A Definitive Guide to Sensible Form Validations](http://form.guide/best-practices/form-validations-definitive-guide.html)
- [Form data validation](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Form_validation)


#### Pomocne narzędzia:
-	skryptozakładka [Forms](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakładka [Form Labels](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera
-	skryptozakładka [Forms](https://accessibility-bookmarklets.org/install.html) z kolekcji Pixo i University of Illinois. z kolekcji Pixo i University of Illinois.
-	Opcja interaktywne w skryptozakładce [ANDI](https://lepszyweb.pl/andi/help/install.html)
-	Opcja łącza/przyciski w skryptozakładce [ANDI](https://lepszyweb.pl/andi/help/install.html)

#### Techniki WCAG 2.1

**Techniki wystarczające** dla kryterium sukcesu 3.3.2

- [G131: Zapewnienie opisowych etykiet](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [ARIA1: Użycie właściwości aria-describedby, aby zapewnić opisowe etykiety dla kontrolek interfejsu użytkownika](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA1)
  - [ARIA9: Użycie atrybutu aria-labelledby, aby połączyć etykietę z kilku węzłów tekstowych](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA9)
  - [ARIA17: Użycie ról grupowania do identyfikowania powiązanych kontrolek formularzy](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA17)
  - [G89: Podanie oczekiwanego formatu danych i przykładu](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [G184: Podanie na początku formularza lub zestawu pól instrukcji tekstowych opisujących niezbędne dane wejściowe](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [G162: Umieszczanie etykiet w bezpośredniej bliskości kontrolek, aby zmaksymalizować postrzeganie relacji](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [G83: Zapewnienie opisów tekstowych wskazujących wymagane pola, które nie zostały wypełnione](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [H90: Wskazanie wymaganych kontrolek formularza za pomocą elementów label i legend](https://www.w3.org/WAI/WCAG22/Techniques/html/H90)
  - [PDF5: Wskazanie wymaganych kontrolek formularzy w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF5)
- [H44: Użycie elementu label do kojarzenia etykiet tekstowych z kontrolkami formularzy](https://www.w3.org/WAI/WCAG22/Techniques/html/H44)
- [PDF10: Zapewnianie etykiet dla interaktywnych kontrolek formularzy w dokumentach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF10)
- [H71: Zapewnienie opisu dla grup kontrolek formularzy przy użyciu elementów fieldset i legend](https://www.w3.org/WAI/WCAG22/Techniques/html/H71)
- [G167: Użycie sąsiadującego przycisku, aby oznaczyć przeznaczenie pola](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
> **Uwaga**: Techniki znajdujące się na końcu powyższej listy powinny być uważane za ostateczność i stosowane tylko wtedy, gdy inne techniki nie mogą być zastosowane na stronie. Wcześniejsze techniki są preferowane, ponieważ zwiększają one dostępność dla szerszej grupy użytkowników.

**Techniki pomocnicze** dla kryterium sukcesu 3.3.2
- [G13: Opisywanie, co się stanie, zanim nastąpi zmiana w formancie formularza, który powoduje zmianę kontekstu](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)

**Błędy** kryterium sukcesu 3.3.2
- [F82: Niespełnienie kryterium sukcesu 3.3.2 poprzez wizualne sformatowanie zestawu pól numeru telefonu, ale bez etykiety tekstowej](https://www.w3.org/WAI/WCAG22/Techniques/failures/F82)

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
