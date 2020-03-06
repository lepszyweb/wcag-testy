## Jak zapewnić dostepność?
{% include callout.html content="Całą treść każdej strony rozmieść w&nbsp;kluczowych obszarach zgodnie z ich przeznaczeniem." type="primary" %}

## Dlaczego to jest ważne?
Przejrzysta i zrozumiała **<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.struktura}}">struktura strony</a>** znacząco wpływa na dostępność treści, na jej znajdowanie, przeglądanie, rozumienie i&nbsp;wykorzystanie.

Gdy osoba widząca przegląda stronę na ekranie monitora, ogarnia wzrokiem całość i widzi różne bloki zawartości. Doświadczenie mówi jej, co jest nagłówkiem strony, co jest główną treścią i gdzie się ona znajduje, gdzie znajdują się treści poboczne, gdzie znajduje się menu nawigacyjne, gdzie znajduje się obszar wyszukiwania.

Użytkownicy niewidomi i słabowidzący nie mają takiego wspaniałego doświadczenia. Ale technologia wspomagająca, np. czytnik ekranu, może im pomóc zorientować się w organizacji i strukturze strony pod warunkiem, że cała treść strony znajdzie się w odpowiednio oznaczonych obszarach.

## Kto odnosi korzyści z dobrej organizacji treści na stronach?
Dobrze zorganizowana treść jest przydatna dla wszystkich użytkowników, ale szczególnie potrzebna jest:

- osobom z problemami poznawczymi i trudnościami w nauce, bo mogą łatwiej znajdować treści na stronach i&nbsp;ustalać ich priorytety,
- osobom korzystajacym z czytnikow ekranu, bo mogą bezpośrednio przejść do głównej treści i&nbsp;innych ważnych miejsc na stronie,
- osobom nawigującym tylko za pomocą klawiatury, bo mogą efektywniej przeglądać strony i&nbsp;korzystać z&nbsp;ich funkcjonalności,
- osobom korzystającym z oprogramowania wyświetlającego tylko główną treść strony, gdy jest dobrze oznakowana,
- osobom z wadami wzroku, w tym słabowidzącym, bo pomaga orientować się w&nbsp;rozmieszczeniu treści.

## Standard dostępności
Standard dostępności wyznaczają **WCAG 2.1** w  **kryterium sukcesu**: {% include ks/1-3-1.md %}

## Struktura stron a technologie internetowe
Starsze wersje HTML nie posiadały efektywnego sposobu oznaczania struktury stron. Zapewnił je dopiero HTML5, wprowadzając:

- **nowe znaczniki semantyczne**, takie jak `header`, `nav`, `main`, `aside`, `footer` czy `section`.
- **atrybuty roli obszarów**, takie jak `banner`, `navigation`, `complementary`, `contentinfo`, `region`, `search`,
- atrybuty wzbogacające możliwości etykietowania treści - `aria-label` oraz `aria-labelledby`.

Nowymi znacznikami semantycznymi oraz atrybutami roli można oznaczyć kluczowe <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obszar}}">obszary stron</a>, nazywane **punktami orientacyjnymi** (ang. *landmark*).

Nowy w HTML5 atrybut `role` wywodzi się z technologii WAI-ARIA, a jego początki sięgają jeszcze 2006 roku. Specyfikacja WAI-ARIA określa sposoby  uczynienia treści internetowych i aplikacji internetowych bardziej dostępnymi dla osób z niepełnosprawnościami. Pomaga zwłaszcza w zapewnianiu dostępności treści dynamicznych oraz zaawansowanych kontrolek interfejsu użytkownika opracowanych przy użyciu Ajax, HTML, JavaScript i pokrewnych technologii.

Nowe znaczniki strukturalne, a w razie potrzeby atrybuty `role` oraz  `aria-label` i `aria-labelledby` w&nbsp;zupełności wystarczają, aby oznaczyć kluczowe obszary stron internetowych, takie jak **nagłówek strony**, **treść główna**, **nawigacja**, **wyszukiwanie**, **stopka**, **treści uzupełniające** oraz inne, zdefiniowane przez twórcę strony.

Możliwości definiowania kluczowych obszarów strony przedstawia tabela poniżej:

<table>
<caption>Role obszarów i odpowiadające im znaczniki HTML</caption>
<thead>
<tr>
<th>rola obszaru</th>
<th>znacznik HTML5</th>
<th>opis</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">`banner`</td>
<td markdown="span">`header`,<br />gdy jest obszarem najwyższego poziomu (bezpośrednim potomkiem elementu body)</td>
<td>obszar nagłówka strony z takimi elementami identyfikującymi, jak logo, nazwa, nazwa wydawcy, streszczenie (wiersz witryny); w nagłówku strony mogą się znajdować inne kluczowe obszary, takie jak nawigacja czy&nbsp;wyszukiwanie</td>
</tr>
<tr>
<td markdown="span">`navigation`</td>
<td markdown="span">`nav`</td>
<td>obszar z&nbsp;elementami służącymi do nawigacji po witrynie lub zawartości strony</td>
</tr>
<tr>
<td markdown="span">`main`</td>
<td markdown="span">`main`</td>
<td>obszar strony z główną treścią</td>
</tr>
<tr>
<td markdown="span">`complementary`</td>
<td markdown="span">`aside`</td>
<td>obszar strony z treścią poboczną uzupełniającą treść główną</td>
</tr>
<tr>
<td markdown="span">`contentinfo`</td>
<td markdown="span">`footer`,<br />gdy jest obszarem najwyższego poziomu (bezpośrednim potomkiem elementu body)</td>
<td>obszar stopki strony zawierający takie informacje, jak noty o prawach autorskich, łącza do&nbsp;warunków użytkowania i&nbsp;oświadczeń wydawcy o polityce prywatności, dostępności, itp.</td>
</tr>
<tr>
<td markdown="span">`form`</td>
<td markdown="span">`form`</td>
<td>obszar strony z kolekcją pozycji i obiektów tworzących razem formularz</td>
</tr>
<tr>
<td markdown="span">`region`</td>
<td markdown="span">`section`</td>
<td>obszar zawierający kluczowe treści strony, których nie opisują role innych obszarów</td>
</tr>
<tr>
<td markdown="span">`search`</td>
<td>----</td>
<td>obszar ze zbiórem pozycji i obiektów tworzących razem centrum wyszukiwania</td>
</tr>
</tbody>
</table>

Najlepiej używać znaczników. A w przypadku, gdy odpowiedni znacznik nie istnieje albo z jakiegoś powodu nie może być zastosowany, używamy atrybutów roli. Atrybutów roli można również użyć na stronach zbudowanych w starszych wersjach (x)HTML. Używamy ich wówczas jako atrybutów opisujących znaczniki `div`, np. `<div role="main">`.  

Niekiedy można się jeszcze spotkać z praktyką równoczesnego stosowania znacznika semantycznego oraz atrybutu `role`, np. `<main role="main"`. Z&nbsp;technicznego punktu widzenia jawne przypisywanie znacznikom domyślnej roli jest nadmiarowe, zbędne. Ale takiej praktyki nie uznaje się za błąd. Zalecano ją w&nbsp;pierwszych latach funkcjonowania HTML5,, aby zmaksymalizować kompatybilność z&nbsp;przeglądarkami internetowymi i technologiami pomocniczymi, które obsługiwały WAI-ARIA, ale nie jeszcze obsługiwały HTML5. Aktualnie nowoczesne przegladarki nie powinny mieć żadnych problemów z ich interpretacją, co można sprawdzić na stronie [Czy mogę użyć](https://caniuse.com/).

Jak widać w tabeli, tylko obszar pełniący rolę „search” nie ma swego odpowiednika w znacznikach HTML. Rozwiązaniem problemu jest w takim przypadku użycie znacznika ogólnego zastosowania, np. `div` i przypisanie mu atrybutu `role="search"`. Może to być nie tylko formularz wyszukiwarki, ale też łącza do mapy witryny, rozwijana lista łączy do najważniejszych stron na witrynie, czy inne elementy, które znacznie ułatwią użytkownikowi odnalezienie potrzebnych informacji.

## Oznacz kluczowe obszary strony
Twórcy mogą oznaczać kluczowe obszary stron w ich szablonach.  

### Zasady oznaczania obszarów struktury strony
{% include warning.html content="WCAG nie wymagają stosowania omawianych tutaj znaczników strukturalnych i atrybutów roli. Jeśli jednak twórcy korzystają z nich na swoich stronach, powinni przestrzegać **15 reguł** przedstawionych poniżej." %}

- na kluczowe <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obszar}}">obszary</a> należy podzielić całą stronę, żadna treść nie może się znajdować poza tymi obszarami,
- każdy obszar musi mieć określoną rolę w strukturze strony nadaną znacznikiem strukturalnym lub atrybutem `role`,
- tylko jeden obszar może mieć rolę `main`, czyli strona może mieć tylko jedną treść główną,
- obszar `main` musi być obszarem najwyższego poziomu,
- tylko jeden obszar może mieć rolę `banner`, czyli strona może mieć tylko jeden nagłówek strony,
- obszar `banner` musi być obszarem najwyższego poziomu,
- tylko jeden obszar może mieć rolę `contentinfo`, czyli strona może mieć tylko jedną stopkę strony,
- obszar `contentinfo` musi być obszarem najwyższego poziomu,
- więcej niż jeden obszar może mieć rolę `nav`,
- obszar `nav` może być częścią innego obszaru,
- więcej niż jeden obszar może mieć rolę `complementary`,
- obszary `complementary` muszą być obszarami najwyższego poziomu
- więcej niż jeden obszar może mieć rolę `search`,
- więcej niż jeden obszar może mieć rolę `region`,
- więcej niż jeden kluczowy obszar tego samego typu (pełniący tę samą rolę) musi mieć unikalną nazwę.

## Zapewnij kluczowym obszarom dostępne nazwy
Standardowo nazwę kluczowemu obszarowi strony nadaje otaczający go **znacznik strukturalny** bądź **wartość atrybutu role**.

W trzech przypadkach ten standardowy sposób zapewnienia nazwy musi być uzupełniony **etykietą**, aby kluczowy obszar był poprawnie rozpoznawany przez technologię pomocniczą:

- gdy którąś rolę obszaru stosuje się więcej niż jeden raz na stronie,
- gdy rola obszaru nadana jest znacznikiem `section` lub atrybutem `role="region"`,
- gdy domyślna rola obszaru wymaga zmiany lub sprecyzowania.

We wszystkich trzech przypadkach etykietę można zapewnić w dwojaki sposób:

- za pomocą atrybutu `aria-labelledby`,  
- za pomocą atrybutu `aria-label`.

Jeśli treść obszaru rozpoczyna się od nagłówka h1-h6, można go użyć jako nazwy, korzystając z atrybutu `aria-labelledby`. Wartością atrybutu jest w takim przypadku wartość atrybutu `id` elementu nagłówka.

Jeśli obszar nie posiada elementu nagłówka, etykietę zapewniamy za pomocą atrybutu `aria-label`. Wartością atrybutu jest wtedy tytuł treści, czyli jej nazwa.

#### Przykład 1. Etykieta z aria-labelledy
````html
<aside aria-labelledby="reklBok">
   <h3 id="reklBok">Reklama</h3>
....
</aside>
````

#### Przykład 2. Etykieta z aria-label
````html
<nav aria-label="Główna">
....
</nav>
````
W etykietach unikamy używania nazw punktów orientacyjnych, ponieważ czytniki ekranu komunikują użytkownikom typ punktu orientacyjnego (rolę obszaru). Na przykład, jeśli niepotrzebnie oznaczysz obszar nawigacji tytułem „Nawigacja witryny”, to czytnik ekranu zakomunikuje użytkownikowi obszar „nawigacja witryny nawigacja”. Etykietą powinno być po prostu słowo „Witryna” albo „Główna”, „Globalna”.

Obszary nawigacyjne są dobrym przykładem przypadków, w których konieczna jest dodatkowa etykieta, precyzująca rolę - czy jest to nawigacja globalna, czy np. nawigacja lokalna po artykule, czy zestaw łączy promujących najnowsze artykuły.

{% include note.html content="Jeśli dwa obszary `navigation` zawierają identyczne zestawy linków, należy użyć dla każdego z nich takiej samej etykiety." %}

Dobrym przykładem sytuacji, w której domyślna rola obszaru wymaga zmiany jest wykorzystanie elementu `<aside>` do prezentacji reklamy kontekstowej powiązanej z&nbsp;treścią główną. Umieszczenie reklamy kontekstowej w&nbsp;obszarze objętym znacznikiem `<aside>` jest w pełni uzasadnione, bo treść reklamy można uznać za *uzupełnienie treści głównej*, które samo w sobie niesie również *odrębną wartość dla użytkownika* i może być samodzielną jednostką treści. A tak właśnie w specyfikacji scharakteryzowana jest rola `complementary` przypisana domyślnie znacznikowi `aside`. Ale dobrą praktyką jest powiadamianie użytkowników, że mają w tym przypadku do czynienia z reklamą. Oznaczenie tego obszaru etykietą opisującą reklamowy charakter treści będzie z pewnością docenione przez użytkowników korzystajacych z technologii pomocniczych.
