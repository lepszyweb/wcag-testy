---
title: Określenie języka

sidebar: testy_sidebar
permalink: H4-01-identyfikacja-jezyka
folder: testy/jbt
---


## Określenie języka

### Uzasadnienie testu
Domyślny język naturalny (ludzki) dla każdej strony internetowej oraz język fragmentów tekstu, które używają języka innego niż domyślny, muszą być określone programowo, aby programy użytkownika, w tym technologie wspomagające poprawnie interpretowały i prezentowały informacje. 

### Metoda badania:
Kontrola wzrokowa. Inspekcja kodu HTML.

## Założenia, zastrzeżenia lub wyjątki
-   W przypadku treści internetowych atrybut języka `lang` może być atrybutem wielu znaczników HTML. Jego struktura to `<[znacznik HTML] lang="[podstawowy podznacznik języka\]">`. Podstawowy podznacznik języka jest pierwszym 2- lub 3- znakowym kodem w wartości atrybutu `lang`. Dialekty określone w podznacznikach języka (dodatkowe 2 lub 3 znaki) nie są częścią tego testu.
-   **Wyjątek**:  Nazwy własne, terminy techniczne, słowa nieokreślonego języka oraz słowa lub frazy, które stały się częścią języka bezpośrednio otaczającego tekstu, nie są objęte językiem części.

**Uwaga**: Język strony można ustawić innymi metodami niż atrybut `lang`, na przykład za pomocą nagłówków HTTP lub elementu `meta`. Te metody nie są obsługiwane przez wszystkie technologie wspomagające. Te inne metody są niewystarczające do spełnienia kryterium sukcesu 3.1.1.

## Obsługa dostępności
W przypadku tej reguły nie są znane żadne poważne problemy z obsługą dostępności.

### Oczekiwania:
Kryterium sukcesu: [3.1.1 Język strony](https://wcag.lepszyweb.pl/#language-of-page), kryterium sukcesu: [3.1.2 Język części](https://wcag.lepszyweb.pl/#language-of-parts).

- Element `<html>` zawiera atrybut języka `lang`, a określony w nim język pasuje do języka głównej treści strony.
- Treść w innych językach ma odpowiednio zdefiniowany atrybut językowy w elemencie HTML obejmującym fragment innojęzyczny.
- Jeśli istnieje atrybut `xml-lang`, jego wartość jest taka sama, jak wartość atrybutu `lang`.

### Procedura testowania:
1.	Przeglądając treść strony, określ domyślny naturalny język strony. Domyślnym jest język, w którym prezentowana jest główna treść strony.
2.	Zobacz źródło strony i sprawdź, czy w znaczniku `<html>` zdefiniowany jest atrybut `lang`.
3.	Sprawdź, czy wartość atrybutu `lang` odpowiada domyślnemu językowi strony.
4.	Przejrzyj ponownie stronę i sprawdź, czy istnieją na stronie pojedyncze słowa lub grupy słów w innych językach, niż domyślny język strony.
5.	Korzystając z funkcji *Zbadaj element* w przeglądarce, sprawdź, czy każdy znaleziony innojęzyczny element strony został objęty odpowiednim znacznikiem z poprawną wartością atrybutu `lang`.


### Zasoby

#### Pomocne narzędzia:
- skryptozakładka [Lang Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access
- opcja *struktura* w skryptozakładce ANDI  https://lepszyweb.pl/andi/help/install.html

#### Wykorzystanie skryptozkładki ANDI
![Testowanie języka strony za pomocą skryptozkładki ANDI](/images/andi/andi_lang.png)

1.	Uruchom skryptozakładkę ANDI i wybierz z menu opcję *struktura*.
2.	Wybierz z menu poziomego opcję  *więcej szczegółów*.
3.	Wybierz z rozwijanej listy opcję *język strony*.
4.	Sprawdź w oknie dialogowym, czy domyślny język strony  został określony poprawnie.

#### Techniki WCAG 2.1
-   [H57: Używanie atrybutu lang dla elementu html](https://www.w3.org/WAI/WCAG21/Techniques/html/H57.html)
-   [H58: Używanie atrybutu lang do wskazywania zmian w języku naturalnym](https://www.w3.org/WAI/WCAG21/Techniques/html/H58.html)


### Przypadki testowe

#### Zaliczone
Element `html` ma atrybut `lang` o niepustej wartości ("").
`&lt;html lang="en"&gt;&lt;/html&gt;

Element `html` ma atrybut `lang` ze poprawnym podznacznikiem języka podstawowego, mimo że podznacznik regionu jest określony niepoprawnie.

`&lt;html lang="en-US-GB"&gt;&lt;/html&gt;`

Element `html` ma identyczne podznaczniki języka podstawowego dla swoich atrybutów `lang` i `xml:lang`.

`&lt;html lang="EN" xml:lang="en"&gt;&lt;/html&gt;`



#### Niezaliczone
Element `html` nie ma atrybutu `lang`
`&lt;html&gt;&lt;/html&gt;`

Element `html` ma atrybut `lang` bez tekstu (tylko spację)
`&lt;html lang=" "&gt;&lt;/html&gt;`

Element `html` ma atrybut `xml:lang` 
`&lt;html xml:lang="en"&gt;&lt;/html&gt;`


Element `html` ma atrybut `lang` z niepoprawnym podznacznikiem języka podstawowego.

`&lt;html lang="em-US"&gt;&lt;/html&gt;


Atrybut `lang` tej strony to trzyliterowy kod ISO 639.2, który nie ma znanego podznacznika języka podstawowego.

```
&lt;html lang="eng"&gt;
	&lt;body&gt;
		&lt;p lang="en"&gt;Lubię reguły testowe ACT!&lt;/p&gt;
	&lt;/body&gt;
&lt;/html&gt;
```



