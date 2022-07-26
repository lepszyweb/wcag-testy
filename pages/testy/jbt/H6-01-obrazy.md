---
title: Obrazy

sidebar: testy_sidebar
permalink: H6-01-obrazy
folder: testy/jbt
---


## Obrazy

### Metoda badania:
Inspekcja kodu, wyłączenie wyświetlania obrazów, użycie narzędzia ujawniającego teksty alternatywne

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content), [1.4.11 Kontrast elementów nietekstowych](https://wcag.lepszyweb.pl/#non-text-contrast)
-	Strona z wyłączonym wyświetlaniem obrazów przekazuje te same informacje i posiada tę samą funkcjonalność, co strona z włączonym wyświetlaniem obrazów.  
-	Każdy obraz, który przekazuje informację, znaczenie lub kontekst ma:
    - tekst alternatywny, który zapewnia te same informacje, znaczenie, kontekst **ALBO**
    - dostępny odpowiednik tekstowy w sąsiedztwie obrazu, który zapewnia te same informacje, znaczenie, kontekst **ALBO**
    - zwięzły tekst alternatywny i łącze do odpowiednika tekstowego, który zapewnia te same informacje, znaczenie, kontekst
-	Każdy obraz, dla którego w bezpośrednim sąsiedztwie zapewniono równoważny odpowiednik tekstowy, może mieć, ale nie musi, zwięzły tekst alternatywny.
-	Każdy obraz, który jest łączem lub kontrolką formularza, np. przyciskiem, posiada tekst alternatywny, który przekazuje cel łącza lub funkcję kontrolki.
-	Każdy obraz dekoracyjny, który nie przekazuje informacji, znaczenia ani kontekstu, spełnia co najmniej jeden z poniższych warunków:
    - posiada pusty tekst alternatywny **ALBO**
    - posiada atrybut roli ARIA: `role="presentation"`, **ALBO**
    - posiada atrybut `aria-hidden="true"`, **ALBO**
    - jest osadzony w tle za pomocą CSS.
-	Obrazy nie są wykorzystywane do przekazywania informacji tekstowych, chyba że prezentacja tekstu w formacie obrazu jest konieczna.
-	Każdy obraz, który przekazuje informacje tekstowe, posiada tekst alternatywny, który przekazuje dokładnie te same informacje.
-	Każdy obraz, który służy jako łącze lub kontrolka formularza, zachowuje wymagany współczynnik kontrastu pierwszego planu do tła wynoszący co najmniej 3:1  
-	Każdy obraz, który przekazuje informacje tekstowe, spełnia wymagania dotyczące kontrastu, z wyjątkiem, gdy jest to obraz logo.

### Procedura testowania:
1.	Znajdź wszystkie obrazy na stronie i oceń każdy obraz, czy jest znaczący, czy dekoracyjny.
2.	Sprawdź, czy kombinacja dostępnej nazwy i dostępnego opisu każdego obrazu niosącego informacje, znaczenie lub kontekst zapewnia równoważne informacje, znaczenie lub kontekst.
3.	Sprawdź, czy znajdujący się w treści strony odpowiednik tekstowy każdego obrazu niosącego informacje, znaczenie lub kontekst jest programowo powiązany z obrazem, którego dotyczy.

### Wykorzystanie skryptozkładki ANDI
{% include image.html file="andi/andi-images.png" alt="Wykorzystanie skryptozkładki ANDI" %}

1.	Uruchom skryptozakładkę ANDI i wybierz z menu ANDI opcję *grafika/obrazy*.  
2.	ANDI wykryje wszystkie elementy graficzne na stronie i poda zwięzłą statystykę: *Znaleziono obrazów* – XX, XX *obrazów osadzonych*, X *łączy graficznych*, XX *ikon z fontów* oraz XX *obrazów tła*.
3.	Sprawdź w sekcji *Element*, czy obraz posiada dostępną nazwę lub opis powiązane programowo (atrybut `alt` lub inny: `title`, `aria-label`, `aria-labelldedby`).
4.	Sprawdź w sekcji *Wyjście ANDI*, treść tekstowego odpowiednika obrazu, jaką ogłoszą czytniki ekranu.  
5.	Rozważ ostrzeżenia wyszczególnione w sekcji *Alertów dostępności*.
6.	Za pomocą przełącznika wykrytych elementów przejdź do testowania następnego obrazu.  

*Uwaga*: ANDI oznacza na stronie analizowane obrazy wyraźnym konturem.  
### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [Images](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama
-	skryptozakładka [Active Images](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera
-	skryptozakładka [Img-Alt Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access
-	opcja graphics/images w skryptozakładce [ANDI](https://lepszyweb.pl/andi/help/install.html)

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
