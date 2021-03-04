---
title: Nawigacja sekwencyjna

sidebar: testy_sidebar
permalink: H1-08-nawigacja-sekwencyjna
folder: testy/jbt
---


# Porządek nawigacji tabulatorem

### Metoda badania:
Test nawigacji klawiaturą, narzędzie ujawniające sekwencję nawigacji tabulatorem po stronie.

## Zastosowanie
Wszystkie interaktywne elementy strony, np. łącza, kontrolki formularzy, rozwijane menu, rozwijane panele (karty, harmonijki, drzewa), okienka wyskakujące, lightboksy, ramki, ramki włączone (iframes).

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [2.4.3 Kolejność fokusu](https://wcag.lepszyweb.pl/#focus-order)
-	Podczas nawigacji po stronie  tabulatorem (klawiszem Tab na klawiaturze) wszystkie interaktywne obiekty otrzymują fokus.
-	Żaden nieinteraktywny element strony nie otrzymuje wskaźnika fokusu (pola formularzy oznaczone „tylko do odczytu” uznajemy za elementy interaktywne).
-	Kolejność, w jakiej obiekty otrzymują fokus, jest logiczna i odpowiada oczekiwanej kolejności wizualnej.
-	Jeśli na stronie pojawia się dialogowe okno modalne, fokus przechodzi do okna dialogowego i pozostaje w nim dopóki użytkownik nie zamknie okna.  
-	Zmiany treści w obszarach dynamicznych (*żywe regiony*), o ile nie zawierają treści interaktywnych, nie wymagają zmiany fokusu.

*Uwaga*: Chociaż jest to powszechna i dobra praktyka, nie jest wymagane, aby oznaczanie fokusem następowało w kolejności od lewej do prawej krawędzi strony i od góry do dołu.

### Procedura testowania:
1.	Ustaw kursor w pasku adresu przeglądarki, a następnie użyj klawisza Tab, aby przemieszczać się do kolejnych interaktywnych elementów strony (łącza, przyciski, przełączniki, pola formularzy, itd.).  Nie używaj myszy.
2.	Sprawdź, czy kolejność ustawiania fokusu zachowuje znaczenie i użyteczność strony.

### Wykorzystanie skryptozkładki ANDI

{% include image.html file="andi/andi_kolejnosc_fokusu.png" alt="Wykorzystanie skryptozkładki ANDI" %}

1.	Uruchom skryptozakładkę ANDI.
2.	Wybierz z menu ANDI opcję *interaktywne* i zaznacz w menu poziomym opcję *porządek tabulacji*.
3.	Sprawdź czy porządek otrzymywania fokusu przez elementy interaktywne oznaczony liczbami odpowiada jest logiczny i oczekiwany.  
### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Focus Interactive Controls](http://adrianroselli.com/2015/01/css-bookmarklets-for-testing-and-fixing.html) z kolekcji Adriana Roselliego. Zamiast uderzać wielokrotnie w klawisz tabulatura, aby sprawdzić style fokusu, kolejność odczytu, usłyszeć, jak czytnik ekranu ogłasza kolejne elementy, uruchom tę zakładkę. Nie będzie można jej zatrzymać do ukończenia zadania. Na każdym elemencie wskaźnik fokusu zostanie zatrzymany na 1 sekundę (możesz dostosować ten czas w kodzie zakładki). Możesz również dostosować selektor CSS, aby testować interaktywne elementy np. tylko w obszarze main.
-	skryptozakładka [Force show focus](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Dodaje jednolity pomarańczowy kontur o rozmiarze 4 pikseli wokół wszystkich elementów interaktywnych, gdy staja się punktem uwagi podczas tabulacji.
-	Opcja *interaktywne* w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html)
-	Opcja *Trace tab path* oferowana w dodatku [ChromeLens](https://chrome.google.com/webstore/detail/chromelens/idikgljglpfilbhaboonnpnnincjhjkd). Z testu tabulacji otrzymasz plik graficzny w formacie PNG pokazujący trasę fokusu.  
-	Opcja *Show Tab Stops* w narzędziu [Accessibility Insights for Web](https://accessibilityinsights.io/) firmy Microsoft

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
