---
title: Nawigacja - Widoczny fokus

sidebar: testy_sidebar
permalink: H1-09-widoczny-fokus
folder: testy/jbt
---

## Nawigacja - Widoczny fokus

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.7-widoczny-fokus |   ??  | Gdy fokus znajduje się na komponencie interfejsu użytkownika,  widoczny jest graficzny wskaźnik fokusu. |

### Cel testu

Celem tego testu jest ustalenie, czy podczas nawigacji sekwencyjnej klawiszem <kbd>Tab</kbd> po stronie każdy komponent interfejsu użytkownika, który otrzymał fokus i jest gotowy na odbieranie zdarzeń związanych z naciskaniem klawiatury, ma widoczne oznaki fokusu.

### Dlaczego to jest ważne?
Osoby, które obsługują stronę internetową tylko za pomocą klawiatury muszą wiedzieć, który z&nbsp;elementów interaktywnych na stronie jest aktualnie w&nbsp;stanie gotowości na odbieranie zdarzeń związanych z naciskaniem klawiatury. Taki stan nazywa się *skupieniem*, *punktem uwagi* albo z angielskiego *fokusem*. W&nbsp;otwartym oknie strony lub aplikacji tylko jeden element w&nbsp;danym momencie może się znajdować w stanie skupienia.

Wizualny sygnał stanu skupienia jest również bardzo pomocny osobom z&nbsp;ograniczeniami uwagi, pamięci krótkotrwałej, zręczności, procesów wykonawczych.

Fokus można przenosić z jednego elementu na następny za pomocą klawiszy <kbd>Tab</kbd> oraz <kbd>Shift+Tab</kbd>, a wewnątrz złożonych elementów za pomocą klawiszy strzałek.

Elementy mogą się znaleźć w stanie skupienia także w wyniku kliknięcia myszą, ale w&nbsp;reakcji na kliknięcie wykonują zwykle jeszcze dodatkowe funkcje.

Wskaźnik fokusu może przybierać różne formy: obramowania elementu, migającego kursora (karetka) w polu tekstowym, wizualnej zmiany wyglądu przycisku.

Twórcy stron i aplikacji mogą umożliwiać i&nbsp;wyłączać możliwość otrzymywania fokusu przez elementy strony, a&nbsp;także zmieniać kolejność przenoszenia fokusu, korzystając z&nbsp;atrybutu `tabindex` oraz ze skryptów.

## Mapowanie do wymagań dostępności
{% include ks/2-4-7.md %}

### Metoda badania:
Kontrola wizualna. Test nawigacji za pomocą klawiatury

## Zastosowanie
Komponenty interfejsu dostępne dla klawiatury, np. łącza, pola formularzy, rozwijane menu, treść rozwijana/zwijana treści, widoki drzewa, okienka wyskakujące, lightbox, ramki, ramki włączone (iframes).

## Założenia, ograniczenia, wyjątki
-   W porządku tabulacji mogą być niektóre elementy interfejsu, które nie są zwykle uważane za interaktywne (np. tekst instrukcji wypełniania formularzy). Takie komponenty interfejsu powinny otrzymywać widoczny fokus, gdy użytkownik nawiguje do nich za pomocą klawiatury.
-   Częścią tego testu jest widoczność fokusu na łączach pomijających.
-   Przełączanie fokusu na odkrywane treści nie jest tutaj testowane.
-   Podczas ręcznego przesuwania fokusu przez stronę (za pomocą <kbd>Tab</kbd> lub klawiszy strzałek) nie powinno wystąpić zniknięcie fokusu. Jednak po uruchomieniu funkcji, która przemieszcza fokus (np. odsłonięcie wewnętrznego łącza strony lub ukrytej zawartości), może być konieczne ręczne przesunięcie fokusu za pomocą klawiatury, zanim fokus stanie się ponownie widoczny. To nie jest uważane za defekt.

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryterium sukcesu: [2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible)
-	Wskaźnik punktu uwagi (fokus) podczas nawigacji klawiaturą po stronie jest zawsze widoczny i wyraźny:
    -	Kontur, tło lub podkreślenie ma współczynnik kontrastu 4,5:1 w stosunku do tła.
    -	Zmiana koloru obiektu ma współczynnik kontrastu pomiędzy dwoma kolorami wynoszący co najmniej 3:1

*Uwaga:* Wyrazistość widocznego fokusu jest subiektywna. Minimalnym wymaganym poziomem wyrazistości są domyślne ustawienie wyświetlacza przeglądarki (lub platformy systemu operacyjnego).

*Uwaga2*: Wskaźnik fokusu może przybierać różne formy: obramowania elementu, migającego kursora w polu tekstowym, wizualnej zmiany wyglądu przycisku.


## Metoda badania
Nawigacja klawiaturą, kontrola wzrokowa

Ręczna nawigacja lub sterowanie interfejsem tylko za pomocą klawiatury umożliwi testerowi rozpoznanie, kiedy nie ma wizualnego rozróżnienia między elementem posiadajacym fokus a resztą interfejsu lub zawartości.

#### Pomocne narzędzia:


### Procedura testowania:
**Uwaga**: W środowisku testowym podczas testowania nie należy używać żadnych narzędzi modyfikujących wygląd fokusu. Niektóre narzędzia testowe dodają widoczny kontur wokół elementów, które otrzymują fokus.  Chociaż takie narzędzia mogą być pomocne w śledzeniu fokusu, to w testowaniu zgodności z KS [2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible) nie mogą być stosowane, bo spowodują uzyskanie nieprawdziwych wyników testu.

1.	Użyj klawiatury, aby poruszać się po wszystkich interaktywnych komponentach strony.
    1.	Użyj <kbd>Tab</kbd> i kombinacji klawiszy <kbd>Shift+Tab</kbd>, aby poruszać się między widżetami, zarówno do przodu, jak i do tyłu.
    2.	Użyj klawiszy <kbd>strzałek</kbd>, aby poruszać się między elementami, na których można ustawiać fokus w złożonym widżecie.
2.	Gdy przenosisz fokus do każdego kolejnego komponentu, sprawdź, czy następuje widoczna i wyraźna zmiana wyglądu elementu, wskazująca, że otrzymał fokus.

### Zasoby

#### Techniki WCAG
- {% include techniki/G149.md %}
- {% include techniki/G165.md %}
- {% include techniki/G195.md %}

#### Opracowania
-	[Funkcjonalność jest dostępna z klawiatury](http://www.w3.org/WAI/intro/people-use-web/principles#keyboard) - sekcja w <span lang="en">Accessibility Principles</span>; w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Przeglądanie stron internetowych za pomocą klawiatury](http://www.w3.org/WAI/users/browsing#keyboard) - sekcja na stronie <span lang="en">Better Web Browsing: Tips for Customizing Your Computer</span>; w&nbsp;języku angielskim, skorzystaj z&nbsp;tłumaczenia Google.
-	[Zrozumieć Kryterium sukcesu 2.4.7 Widoczny fokus](https://www.w3.org/WAI/WCAG21/Understanding/focus-visible.html)(poziom AA); w&nbsp;języku angielskim, skorzystaj z&nbsp;tłumaczenia Google.



### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
