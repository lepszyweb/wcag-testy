---
title: 12. Tytuły stron i ramek


sidebar: testy_sidebar
permalink: tz-12-tytuly
folder: testy/tz
---
## Cel scenariusza testowego

Celem tego scenariusza testowego jest sprawdzenie, czy każda strona, każda ramka i każda ramka wbudowana ma programowo określony opisowy tytuł lub nazwę. Opisowe tytuły i nazwy umożliwiają użytkownikom szybkie i łatwe określenie, czy treści zawarte na stronie lub w ramce są dla nich istotne, oraz decyzję, czy chcą z nimi wchodzić w&nbsp;interakcje. Tytuły i&nbsp;nazwy umożliwiają użytkownikom rozróżnianie tematu i celu treści. 


Scenariusz testowy „Tytuły stron i ramek” obejmuje cztery testy:

1.	Test 12.A 2-4-2-okreslono-tytul-strony
2.	Test 12.B 2-4-2-tytul-opisuje-tresc-strony
3.	Test 12.C 4-1-2-okreslono-tytul-ramki
4.	Test 12.D 4-1-2-nazwa-ramki-łaczonej

## Tytuły stron

### Test 12.A 2-4-2-okreslono-tytul-strony

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2-4-2-okreslono-tytul-strony | 12.A    | Strona ma tytuł zdefiniowany w kodzie znacznikiem `<title>`. |

### Cel testu 12.A 2-4-2-okreslono-tytul-strony

Każda strona powinna mieć tytuł opisujący jej treść. Celem tego testu jest sprawdzenie, czy tytuł został określony programowo dla każdej strony internetowej. Tytuły stron pomagają szczególnie użytkownikom z ograniczeniami wzroku, mobilności i poznawczymi określać i rozróżniać treść oraz łatwo nawigować między stronami internetowymi. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 2-4-2 Tytuły stron](https://wcag.lepszyweb.pl/#page-titled).


### Metody i narzędzia testowe 
1.	ANDI: struktury > „Alerty dostępności”.

### Identyfikacja treści
Wszystkie strony witryny. Wymagania testów 12.A oraz 12.B obowiązują zawsze.

### Zastosowanie
Nie możesz uznać (ocenić) wyniku tego testu jako **nie ma zastosowania** (**ND**). Wszystkie strony powinny mieć tytuł, aby użytkownicy wiedzieli, jaki jest jej cel strony i co jest jej treścią.

### Jak testować

1.  Uruchom ANDI: struktury. Przejrzyj alerty w sekcji „Alerty dostępności”, aby ustalić, czy ANDI wyświetla którykolwiek z poniższych alertów:

    1.  „Strona nie ma znacznika `<title>`”

    2.  „Znacznik `<title>` nie może być pusty”

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.2:

1.  Tytuł strony internetowej jest określony programowo w znaczniku `<title>`.

### Uwaga

W tym teście oceniamy tylko, czy tytuł strony został określony i czy określenie tytułu strony znajduje się w znaczniku `<title>`. Jeśli w kodzie strony nie ma znacznika `<title>` z tytułem strony lub znacznik `<title>` jest pusty, strona nie spełnia wymagania testowego.

Nie ma znaczenia, czy w kodzie strony znajduje się więcej niż jeden element `<title>`. Jeśli zobaczysz alert ANDI „Strona ma więcej niż jeden znacznik `<title>`”, zignoruj go. Nie stanowiło to naruszenia kryterium sukcesu 2.4.2.

## Opisowe tytuły

### Test 12.B 2-4-2-tytul-opisuje-tresc-strony

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2-4-2-tytul-opisuje-tresc-strony | 12.B    | Tytuł strony opisuje jej treść lub cel. |

### Cel testu 12.B 2-4-2-tytul-opisuje-tresc-strony

Celem tego testu jest sprawdzenie, czy istniejący tytuł strony opisuje jej cel lub temat strony i pomaga odróżnić jedną stronę od drugiej.                                                                                                                  Opisowy tytuł strony pomaga użytkownikom z ograniczeniami wzroku, mobilności i poznawczymi identyfikować, znajdować i nawigować do żądanych treści. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 2-4-2 Tytuły stron](https://wcag.lepszyweb.pl/#page-titled).

### Metody i narzędzia testowe 
1.	Analiza poznawcza.
2.	ANDI: struktury > więcej szczegółów > tytuł strony.


### Identyfikacja treści
Wszystkie strony witryny. Wymagania testów 12.A oraz 12.B obowiązują zawsze.

### Zastosowanie
Nie możesz uznać (ocenić) wyniku tego testu jako **nie ma zastosowania** (**ND**). Wszystkie strony powinny mieć tytuł, aby użytkownicy wiedzieli, jaki jest jej cel strony i co jest jej treścią.


### Jak testować

1.  Uruchom ANDI: struktury, wybierz „więcej szczegółów”, a następnie „tytuł strony”.

    1.  Pojawi się okno dialogowe z tekstem tytułu strony.

2.  Oceń cel i zawartość strony internetowej.

3.  Ustal, czy tytuł strony jest znaczącym przedstawieniem lub wskazaniem zawartości strony. 3.

    1.  Jeżeli strona internetowa jest częścią zestawu stron internetowych, określ, czy tytuł strony jest wystarczający do odróżnienia jej od innych stron.

    2.  W przypadku dokumentów lub aplikacji internetowych, nazwa dokumentu lub aplikacji internetowej wystarcza do opisania celu strony.

### Uwaga

-  Aplikacja internetowa to aplikacja (oprogramowanie) działająca w przeglądarce internetowej (np. webmail) i&nbsp;może nie mieć adresu URL, który zmienia się wraz ze zmianą treści na stronie internetowej.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.4.2:

1.  Tytuł strony dokładnie określa treść lub przeznaczenie strony internetowej **oraz**

2.  Jeśli strona internetowa jest częścią zestawu stron internetowych, tytuł strony dokładnie odróżnia ją od innych stron w witrynie.


## Ramki

### Test 12.C 4-1-2-okreslono-tytul-ramki

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4-1-2-okreslono-tytul-ramki | 12.C    | Każdy element `<frame>`ma atrybut tytułu, który opisuje treść ramki. 

### Cel testu 12.C 4-1-2-okreslono-tytul-ramki


Celem tego testu jest sprawdzenie, czy każda ramka ma atrybut `title` z tytułem opisującym treść ramki. Użytkownicy, którzy polegają na powiązaniach programowych, np. użytkownicy czytników ekranu, potrzebują sposobu na określenie celu lub tematu ramki, oraz i podjęcie decyzji, czy chcą z nimi wchodzić w interakcje.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 4-1-2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value).


### Metody i narzędzia testowe 
1.	Powiadomienie ANDI o ramkach.
2.	Ręczna kontrola strony pod kątem zawartości i celu.


### Identyfikacja treści

Użyj ANDI, aby wykryć wszystkie ramki.

1.  Uruchomić ANDI. Jeśli do budowy strony zostały zastosowane ramki, ANDI powiadomi, że wykryte zostały ramki.

    1.  Jeśli na stronie nie ma ramek, ANDI nie wyświetli żadnego powiadomienia o ramkach.


### Zastosowanie

Test 12.C: 4-1-2-okreslono-tytul-ramki  **nie ma zastosowania**, jeśli na stronie nie ma ramek. W takim przypadku oznacz wynik testu jako **ND**. 

### Jak testować

1.	Uruchom ANDI. Jeśli ANDI wykryje na stronie ramki, ANDI wyświetli okno dialogowe z informacją o wykryciu ramek i dwoma opcjami: „OK”, aby pozostać na stronie oraz „Anuluj”, aby przetestować pojedynczą ramkę. Wybierz Anuluj.

2.	ANDI wyświetli listę wszystkich ramek i powiązane z każdą ramką atrybuty `title`, jeśli istnieją.

    1.  Jeśli nie ma atrybutu tytułu, ANDI zgłosi alert.

3.  Wybierz kolejno łącze, aby zobaczyć treść każdej ramki. Przejrzyj ramkę, aby zrozumieć jej cel lub temat. Użyj przycisku Wstecz w przeglądarce, aby powrócić do testowanej strony i ponownie uruchomić ANDI.

4.	W ANDI przejrzyj odpowiedni atrybut tytułu każdej ramki i oceń, czy opisuje treść ramki.


### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 4.1.2:

1.  Wszystkie ramki mają arybut `title`, który opisuje treść ramki.


### Uwaga

-   W HTML5 element  `<frame>` jest oznaczony jako przestarzały.  Mimo to testerzy mogą spotkać się ze stronami internetowymi lub aplikacjami mobilnymi z przestarzałym kodem, który choć jest przestarzały, może i powinien być nadal dostępny.

-  Treść każdej ramki musi być testowana na zgodność z wszystkimi innymi obowiązującymi testami (testy 12.A i 12.B nie dotyczą treści ramki).

## Ramki łaczone (iframe)

### 4.	Test 12.D 4-1-2-nazwa-ramki-łaczonej

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4-1-2-nazwa-ramki-łaczonej | 12.D    | Kombinacja dostępnej nazwy i opisu każdej `<iframe>` opisuje jej treść. |

### Cel testu 12.D 4-1-2-nazwa-ramki-łaczonej

Celem tego testu jest sprawdzenie, czy każda ramka łączona  ma dostępną nazwę lub dostępny opis, które opisują treść ramki. Użytkownicy, którzy polegają na powiązaniach programowych, np. użytkownicy czytników ekranu, potrzebują sposobu na określenie celu lub tematu ramki łączonej i podjęcie decyzji, czy chcą z nimi wchodzić w interakcje.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 4-1-2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value).

### Metody i narzędzia testowe 

1.	ANDI: iframe.
2.	Ręczna kontrola zawartości strony.


### Identyfikacja treści

Użyj ANDI, aby zidentyfikować wszystkie ramki `iframe` w kolejności tabulatorów

1.	Uruchom ANDI: ramki iframe (iANDI), aby wyróżnić `iframe` na stronie i nawigować między nimi. Jeśli w&nbsp;opcjach modułu nie ma pozycji „ramki iframe”, to znaczy, że na stronie nie ma ramek łączonych.

2.  Użyj przycisku „Następny element”, aby znaleźć wszystkie elementy `iframe`, które w komponentach dostępności:
	
   -   mają nieujemną wartość atrybutu `tabindex`, która (np. 0, 1) oznacza, że ramka `iframe` jest w&nbsp;kolejności tabulacji (ujemny indeks tabulacji, np. -1 oznacza, że ramka `iframe` jest poza porządkiem tabulacji) **lub**
   -   nie ma atrybutu `tabindex`.


**Przetestuj tylko te ramki iframe **. Nie testuj ramek `<iframe>`, które mają ujemną wartość atrybutu `tabindex` lub nie mają attrybutu `tabindex`.


### Zastosowanie

Test 12.D 4-1-2-nazwa-ramki-łaczonej  **nie ma zastosowania**, jeśli na stronie nie ma ramek łączonych **lub** jeśli istniejące ramki `<iframe>` są poza porządkiem tabulacji. W takim przypadku oznacz wynik testu jako **ND**. 


### Jak testować

1.  Uruchom ANDI: ramki iframe

2.  Przejrzyj dane wyjściowe ANDI dla każdego elementu iframe, który ma nieujemną wartość `tabindex`, aby ustalić, czy dostępna nazwa i opis dokładnie opisują zawartość każdego elementu `<iframe>`.

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 4.1.2:

1.  Wszystkie ramki mają arybut `title`, który opisuje treść ramki.

2.  Wyjście ANDI Output dla każdej ramki `<iframe>` znajdującej się w porządku tabulacji wystarczająco dokładnie opisują treść ramki.

### Uwaga

-  Treść każdej ramki łaczonej musi być testowana na zgodność z wszystkimi innymi obowiązującymi testami (testy 12.A i 12.B nie dotyczą treści ramek `<iframe>`).

- Aby otworzyć każdą `<iframe>` do przetestowania należy w module ANDI: ramki iframe wybrać przycisk „testuj na nowej karcie”.

## Obowiązujące normy
- {% include ks/2-4-2.md %}
- {% include ks/4-1-2.md %}
- [11. Tytuły stron](ICT-11-tytuly-stron)
- [19. Ramki](ICT-19-ramki)


