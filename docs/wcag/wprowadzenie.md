## Wprowadzenie

Niniejsza sekcja pełni funkcję <a title="definicja: informacyjne" href="#informativedef" class="termref">informacyjną</a></p>

„Wytyczne dla dostępności treści internetowych 2.0 (WCAG 2.0)” to dokument określający, w jaki sposób uczynić treści internetowe bardziej 
dostępnymi dla osób niepełnosprawnych. Mowa tutaj o wielu rodzajach niepełnosprawności: ze względu na wzrok, słuch, kłopoty z mową, 
trudności w uczeniu się, ograniczenia kognitywne, ruchowe, lingwistyczne czy też neurologiczne. Chociaż wytyczne poruszają szereg zagadnień, nie jest możliwe, aby odpowiadały szczegółowo na potrzeby wszystkich możliwych rodzajów, stopni niepełnosprawności, czy też niepełnosprawności złożonych. Wytyczne pozwalają jednak tworzyć bardziej przyjazne treści, zarówno dla starszych użytkowników, których 
sprawność zmienia się wraz z wiekiem, jak i dla każdego innego użytkownika.

Wytyczne WCAG 2.0 zostały opracowane zgodnie z [procedurami Konsorcjum W3C](http://www.w3.org/WAI/intro/w3c-process.php),
 we współpracy z osobami indywidualnymi oraz różnymi organizacjami z całego świata. Celem było stworzenie wspólnego standardu dostępności 
treści internetowych, który spełniałby oczekiwania użytkowników, firm czy administracji państwowej w różnych krajach. Wytyczne WCAG 2.0 są 
oparte na wersji 1.0 <a href="#WCAG10">[WCAG10]</a> i mają mieć szerokie zastosowanie dla różnych technologii internetowych zarówno teraz, jak i w przyszłości. Są one tak skonstruowane, aby ich spełnienie można było sprawdzić za pomocą kombinacji narzędzi automatycznych i ewaluacji dokonywanej przez człowieka. Na stronie „[Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/intro/wcag.php)”, znajduje się więcej informacji ogólnych na temat wytycznych WCAG.

Dostępność sieci nie jest uzależniona jedynie od treści stron internetowych, ale również od dostępnych przeglądarek internetowych czy 
innych programów stosowanych przez użytkownika. Narzędzia do tworzenia treści również spełniają ważną rolę w dostępności. Dalsze informacje na ten temat znajdują się na następujących stronach:

- [Essential Components of Web Accessibility](http://www.w3.org/WAI/intro/components)
- [User Agent Accessibility Guidelines (UAAG) Overview)](http://www.w3.org/WAI/intro/uaag.php)
- [Authoring Tool Accessibility Guidelines (ATAG) Overview](http://www.w3.org/WAI/intro/atag.php)
    
### Poziomy wytycznych WCAG 2.0</h3>

Osoby indywidualne i organizacje, które korzystają z wytycznych WCAG 2.0 to różnorodna grupa, obejmująca między innymi osoby projektujące serwisy internetowe, decydentów, nabywców usług, nauczycieli czy studentów. Aby sprostać różnym potrzebom tych grup docelowych, stworzono kilka poziomów wytycznych, w tym zasady ogólne, wytyczne, mierzalne kryteria sukcesu, bogaty zbiór wystarczających technik, technik dodatkowych, oraz udokumentowane, często występujące błędy, poparte przykładami, odnośnikami do zasobów i fragmentami kodu źródłowego.

- **Zasady** — na szczycie hierarchii znajdują się 4 zasady, które stanowią fundament dostępności: *postrzegalność, funkcjonalność, zrozumiałość i solidność*. Więcej informacji: ”[Understanding the Four Principles of Accessibility](http://www.w3.org/TR/UNDERSTANDING-WCAG20/intro.html#introduction-fourprincs-head)”.
- **Wytyczne** — na kolejnym poziomie, znajdują się wytyczne. 12 wytycznych definiuje podstawowe cele, jakie stoją przed 
osobami projektującymi i zarządzającymi serwisami internetowymi. Realizacja tych celów służy dostępności treści internetowych dla osób 
niepełnosprawnych. Wytyczne nie są mierzalne, ale stanowią ogólne ramy i cele do osiągnięcia. Mają pomóc autorom serwisów i treści, zrozumieć kryteria sukcesu i pozwolić na ich skuteczniejsze wdrażanie.
- **Kryteria sukcesu** — dla każdej wytycznej opracowano mierzalne kryteria sukcesu. Pozwala to na zastosowanie WCAG 
2.0 wszędzie tam, gdzie konieczne jest sprawdzenie zgodności z wytycznymi, np. przy specyfikacji projektu, zamawianiu usług 
internetowych, w przepisach prawnych oraz przy umowach. Aby zaspokoić potrzeby różnych grup oraz sprostać wymogom różnych sytuacji, stworzono trzy poziomy zgodności z wytycznymi: A (najniższy) AA oraz AAA (najwyższy). Dodatkowe informacje na temat poziomów wytycznych WCAG 2.0 znajdują się na stronie „[Understanding Levels of Conformance](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-levels-head)”.
- **Techniki wystarczające i doradcze** — dla każdej *wytycznej* oraz *kryterium sukcesu* WCAG 2.0, grupa robocza zebrała szereg *technik* (dokument ma charakter informacyjny, ale nie formalny). Podzielono je na dwie kategorie: *techniki wystarczające* by spełnić kryteria sukcesu, oraz techniki *dodatkowe*. Techniki dodatkowe wybiegają ponad to, co jest wymagane przez dane kryteria sukcesu i pozwalają wykonawcom i autorom na jeszcze doskonalszą realizację wytycznych. Niektóre techniki dodatkowe określają bariery dostępności, które nie zostały ujęte w mierzalnych kryteriach sukcesu. Często występujące błędy zostały w miarę możliwości udokumentowane. Więcej informacji w: „[Sufficient and Advisory Techniques in Understanding WCAG 2.0](http://www.w3.org/TR/UNDERSTANDING-WCAG20/intro.html#introduction-layers-techs-head)”.


Wszystkie powyższe poziomy (zasady, wytyczne, kryteria sukcesu, techniki wystarczające i dodatkowe) uzupełniają się wzajemnie i wskazują w jaki sposób tworzyć bardziej dostępne treści internetowe. Wykonawcom i autorom treści doradza się stosowanie w miarę możliwości
wszystkich poziomów, w tym także technik doradczych, aby zaspokoić potrzeby jak najszerszej grupy użytkowników.

Należy pamiętać, iż nawet zawartość, która jest na najwyższym (AAA) poziomie zgodności, nie będzie dostępna dla osób ze wszystkimi rodzajami i stopniami niepełnosprawności, czy też z niepełnosprawnością złożoną, szczególnie w zakresie problemów z uczeniem się oraz zrozumieniem języka. Zachęca się wykonawców i autorów treści do zastosowania szerokiego zakresu technik, w tym technik dodatkowych, ale także do poszukiwania najlepszych praktyk stosowanych w danym momencie rozwoju Internetu, aby treści były w możliwie największym stopniu dostępne dla osób z różnymi dysfunkcjami. [Metadane](http://www.w3.org/TR/UNDERSTANDING-WCAG20/appendixC.html#understanding-metadata) mogą pomóc użytkownikom w znalezieniu treści najbardziej dostosowanych do ich potrzeb.


### Dokumenty uzupełniające WCAG 2.0

WCAG 2.0 jest sformułowany w taki sposób, aby odpowiedzieć na oczekiwania tych, którzy potrzebują stabilnej dokumentacji technicznej —
 punktu odniesienia do zasad dostępności. Pozostałe dokumenty, zwane tu dokumentami uzupełniającymi, bazują na WCAG 2.0 i spełniają 
inne ważne funkcje. W odróżnieniu od samego WCAG 2.0, mogą być aktualizowane gdy zaistnieje potrzeba wdrażania WCAG 2.0 w nowych technologiach internetowych. Do dokumentów uzupełniających należą:

1. „**[How to Meet WCAG 2.0](http://www.w3.org/WAI/WCAG20/quickref/)**” — Aktualizowana i dostosowywana na bieżąco lista odniesień (referencji) do WCAG 2.0. Może posłużyć wykonawcom i autorom do projektowania i ewaluacji treści.
2.  „**[Understanding WCAG 2.0](http://www.w3.org/TR/UNDERSTANDING-WCAG20/intro.html)**” — przewodnik ułatwiający zrozumienie i wdrożenie WCAG 2.0. Do każdej wytycznej i kryterium sukcesu WCAG 2.0 powstał krótki poradnik pomagający zrozumieć ich kluczowe aspekty.
3. „**[Techniques for WCAG 2.0](http://www.w3.org/TR/WCAG20-TECHS/)**” — zbiór technik oraz często występujących błędów, każdy z elementów przedstawiony jest w osobnym dokumencie, zawierającym opis, przykłady, kody źródłowe oraz testy.
4.  „**[The WCAG 2.0 Documents](http://www.w3.org/WAI/intro/wcag20)**” — opis dokumentów technicznych WCAG 2.0 w postaci wykresu. Pokazuje, w jaki sposób są one ze sobą połączone.

W dokumencie „[Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/intro/wcag.php)”, umieszczono opis materiałów powiązanych z WCAG 2.0, w tym materiały edukacyjne. Materiały dodatkowe, obejmujące takie tematy, jak analiza kosztów i korzyści (business case) w zakresie dostępności, propozycje planowania wdrażania wytycznych dostępności oraz kwestie prawne dotyczące dostępności znajdują się na stronie [WAI Resources](http://www.w3.org/WAI/Resources/Overview).

### Ważne pojęcia zastosowane w WCAG 2.0
    
WCAG 2.0 zawiera trzy ważne pojęcia, które były inaczej definiowane w WCAG 1.0. Są one w skrócie opisane poniżej, a zdefiniowane szerzej w słowniku terminów.
<dl>   
    <dt class="label">
      Strona internetowa
    </dt>
    <dd>
      Należy zauważyć, iż w niniejszym standardzie termin „<a title="definicja: strona internetowa" href="#webpagedef" class="termref">strona internetowa</a>” to coś więcej, niż statyczna strona HTML. Ten termin obejmuje również coraz bardziej dynamiczne strony internetowe, które pojawiają się w sieci, w tym „strony” prezentujące całe wirtualne, interaktywne społeczności. Przykładowo, pojęcie „strona internetowa” będzie prawidłowym określeniem na stronę zawierającą elementy interaktywne i filmowe, znajdujące się pod jednym adresem internetowym (URI). Więcej informacji: „[Understanding «Web Page»](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-web-page-head)”.
    </dd>
    <dt>
      Możliwość odczytania przez program komputerowy
    </dt>
    <dd>
      W kilku kryteriach sukcesu wymaga się, aby treści (albo pewne ich aspekty) były „<a title="definicja: możliwy do odczytania przez program komputerowy" href="#programmaticallydetermineddef" class="termref">możliwe do odczytania przez program komputerowy</a>”. 
Oznacza to, że treść jest dostarczona w taki sposób, aby <a title="definicja: program użytkownika" href="#useragentdef" class="termref">programy używane przez użytkownika (user agents)</a>, w tym programy z kategorii <a title="definicja: technologie wspomagające (w rozumieniu tego dokumentu)" href="#atdef" class="termref">technologii wspomagających</a>, mogły odczytać i przedstawić użytkownikowi 
dane informacje w odpowiedni sposób. Więcej informacji: „[Understanding Programmatically Determined](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-programmatically-determined-head)”.
    </dd>
    <dt>
      Wsparcie dla dostępności
    </dt>
    <dd>
     Używanie technologii w taki sposób, aby wspierana była dostępność oznacza, iż współpracuje ona z technologiami wspomagającymi użytkownika (AT — ang. assistive technologies) jak również z odpowiednimi właściwościami dostępności systemów operacyjnych,
 przeglądarek oraz programów użytkownika (user agents). Żeby daną technologię zakwalifikować, jako stanowiącą <a title="definicja: (technologie) stanowiące podstawę zgodności" href="#reliedupondef" class="termref">wiarygodną podstawę</a> spełnienia kryteriów sukcesu wytycznych WCAG 2.0, musi ona być użyta w taki sposób, aby „<a title="definicja: wspierający dostępność" href="#accessibility-supporteddef" class="termref">wspierać dostępność</a>”. Technologie mogą być używane w sposób nie wspierający dostępności (np. nie współpracują z technologiami wspomagającymi, itp.), pod warunkiem, że nie podlegają kryteriom 
sukcesu (tzn. ta sama informacja czy funkcja jest dostępna w sposób wspomagany).</p>
        
      <p>Definicja „wsparcia dla dostępności” znajduje się <a href="#_Za%C5%82%C4%85cznik_A:_S%C5%82ownik">w słowniku terminów w załączniku A</a> do niniejszego dokumentu. Więcej informacji: [Understanding Accessibility Support](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-accessibility-support-head).</p>
    </dd>
  </dl>

