## Jak zapewnić dostępność
{% include callout.html content="Nadaj każdemu dokumentowi zwięzły unikalny tytuł opisujący jego treść i związek z zestawem dokumentów, jeśli istnieje." type="primary" %}

## Dlaczego tytuł dokumentu jest ważny?
- Tytuły nazywają wszelkie utwory, identyfikują je. Bez tytułu trudno byłoby się odwołać do dokumentu.
- Unikalne tytuły pozwalają ludziom szybko ustalić, gdzie się znajdują oraz czy są zainteresowani treścią dokumentu.
- Znaczące tytuły stron pomagają użytkownikom zrozumieć treść i cel dokumentu.
- Dobre tytuły sprawiają, że różne sposoby wyszukiwania w Internecie potrzebnych treści stają się bardziej wydajne i skuteczne.

Krótko mówiąc, tytuły są ważne nie tylko ze względu na dostępność.

## Tytuły stron internetowych
Tytuły stron internetowych są:
-	wyświetlane na kartach przeglądarek,
-	wyświetlane w wynikach wyszukiwania,
-	wykorzystywane do tworzenia ulubionych zakładek w przeglądarce,
-	odczytywane przez czytniki ekranu.

## Kto odnosi korzyści z tytułów?
Tytuły są użyteczne dla wszystkich użytkowników, ale szczególnie przydatne są dla:
-  osób niewidomych i słabowidzących, ponieważ są zawsze pierwszym elementem dokumentu ogłaszanym przez oprogramowanie do odczytywania ekranu.
-  osób z problemami poznawczymi, ograniczoną pamięcią krótkotrwałą i trudnościami, bo pomagają rozróżniać dokumenty, gdy otwartych jest wiele okien lub kart,
-  osób z ograniczeniami ruchu, które podczas nawigacji między dokumentami kierują się dźwiękiem, bo pomagają je rozróżniać.

{% include note.html content="Gdy brakuje tytułu, technologie pomocnicze ogłaszają zwykle nazwę pliku dokumentu, która często nie ma znaczenia." %}



## Standard dostępności
**WCAG 2.1, kryterium sukcesu**: {% include ks/2-4-2.md %}

## Wpływ niespełnienia KS 2.4.2 Tytuł strony na osoby z niepełnosprawnościami

{% include ks/wplyw.md %}
{% include ks/wplyw-01-bez-wzroku.md %}
{% include ks/wplyw-02-z-ogr-wzroku.md %}
{% include ks/wplyw-07-z-ogr-manipulacji.md %}
{% include ks/wplyw-08-z-ogr-sily.md %}
{% include ks/wplyw-09-z-ogr-poznawczymi.md %}

### Tytuł strony w kodzie HTML
W kodzie strony tytuł strony określony jest za pomocą znacznika `<title>` umieszczanego na początku sekcji `<head>`. Może wyglądać np. tak:

```html
<title>Dostępny tytuł strony internetowej | Lepszy Web</title>
```

{% include note.html content="Znacznik elementu TITLE, znajdujący się w sekcji HEAD kodu HTML strony internetowej, nie powinien być mylony z atrybutem TITLE, który można zastosować do większości elementów HTML." %}

### Tytuły ramek i ramek wbudowanych
Dokumenty osadzane na stronach internetowych za pomocą ramek i ramek wbudowanych (*iframe*) również powinny mieć znaczący tytuł. Tytuły dokumentów osadzonych nadaje się za pomocą atrybutu `title=""`.

### Przykłady

| Tytuł | Ocena | Wyjaśnienie |
|------------------------------------|----------|------------------------|
| Skontaktuj się z&nbsp;nami | dobry | Nie identyfikuje witryny, ani nie wyjaśnia, kto to są „my” |
| LepszyWeb.pl - Skontaktuj się z&nbsp;nami | lepszy | Prawdopodobnie unikalny, ale nie zaczyna się od najbardziej szczegółowych informacji |
| Skontaktuj się z&nbsp;nami - LepszyWeb.pl | najlepszy | Tytuł jest zwięzły, opisowy, prawdopodobnie unikalny i identyfikuje witrynę. I wyświetla najpierw najbardziej szczegółowe informacje. |

## Tytuły innych dokumentów

### Dokumenty biurowe
Cyfrowe dokumenty biurowe utworzone w programach MS Word, Libre Office Writter i&nbsp;innych powinny zawierać tytuł dokumentu umieszczony na początku dokumentu i&nbsp;oznakowany stylem **Nagłówek 1**.

Ponadto, tytuły tych dokumentów powinny być umieszczone w metadanych, które wypełnia się w&nbsp;specjalnym oknie informacji o&nbsp;dokumencie.  

{% include warning.html content="Style takie jak: „Tytuł”, „Podtytuł” lub „Tytuł dokumentu” nie są rozpoznawane przez technologie pomocnicze jako znaczniki tytułów. Służą raczej do stylizacji napisów na okładkach publikacji. " %}

### Dokumenty PDF
Mimo poprawnego określenia tytułu dokumentu biurowego w aplikacji źródłowej, takiej jak MS Word, tytuł dokumentu zapisanego do dostępnego formatu PDF nie jest rozpoznawany przez przeglądarki i&nbsp;technlogie pomocnicze. Jeśli nie mamy możliwości skorygowania właściwości dokumentu PDF w programie Adobe Acrobat Pro, można zapewnić dostępność tytułu, wpisując go w nazwie pliku - bez spacji, wyrazy oddzielamy myślnikami lub znakami podkreślenia.

### Prezentacje PowerPoint, Impress...
Każdy ze slajdów utworzonych w takich programach, jak PowerPoint czy Impress, powinnien mieć tytuł, aby czytniki ekranu mogły nawigować do poszczególnych slajdów.
