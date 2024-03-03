---
title: Metodologia oceniania zgodności w zakresie dostępności internetowej (WCAG-EM) 1.0
summary: "Publikacja jest nieoficjalnym roboczym tłumaczeniem dokumentu W3C Website Accessibility Conformance Evaluation Methodology (WCAG-EM) 1.0"
sidebar: metoda_sidebar
permalink: met-wcag-em-pl
folder: metoda
---

## Streszczenie  {#abstract}

Ten dokument zawiera wskazówki dla oceny, w jaki sposób witryny internetowe są zgodne z [Wytycznymi dla dostępności treści internetowych (WCAG) 2.1](https://www.w3.org/Translations/WCAG21-pl/) [*w oryginale odniesienie do WCAG 2.0*]. Opisuje procedurę oceny stron internetowych oraz zawiera wskazówki, które pomogą oceniającym stosować dobre praktyki. Nie zawiera instrukcji oceny poszczególnych aspektów treści internetowych, do których odnoszą się kryteria sukcesu WCAG 2.0. Ten dokument jest jednym z serii materiałów informacyjnych W3C/WAI na temat [oceny stron internetowych pod kątem dostępności](http://www.w3.org/WAI/eval/), które uzupełniają [Dokumenty WCAG 2.0](http://www.w3.org/WAI/intro/wcag20). Nie definiuje dodatkowych wymagań WCAG 2.0, nie zastępuje ich ani nie zmienia w żaden sposób.

Metodologia opisana w tym dokumencie jest przeznaczona dla osób, które mają doświadczenie w ocenie dostępności za pomocą WCAG 2.0 i ich zasobów pomocniczych. Zawiera wskazówki dotyczące dobrych praktyk w zakresie definiowania zakresu oceny, badania ocenianej witryny, wyboru reprezentatywnych próbek próbek stron z witryn, których nie jest możliwe ocenienie całej treści, audytu wybranych próbek i raportowania wyników oceny. Jest przeznaczona przede wszystkim do oceny istniejących stron internetowych, na przykład, aby dowiedzieć się o ich dostępności i monitorować poziom dostępności. Może być również przydatna na wcześniejszych etapach projektowania i tworzenia stron internetowych. Dotyczy to statycznych i dynamicznie generowanych stron internetowych, witryn i aplikacji mobilnych oraz innych typów stron internetowych. Nie wskazuje konkretnych technologii internetowych, narzędzi oceny, przeglądarek internetowych, technologii wspomagających ani innego oprogramowania, które należy wykorzystać do oceny. Nadaje się do stosowania w różnych kontekstach oceny, w tym do samooceny i oceny przez podmioty zewnętrzne.

## Status dokumentu  {#status}

{% include note.html content="W tej części opisano status tego dokumentu w momencie jego publikacji. Inne dokumenty mogą zastąpić ten dokument. Listę bieżących publikacji W3C i najnowszą wersję tego raportu technicznego można znaleźć w&nbsp;[indeksie raportów technicznych W3C](http://www.w3.org/TR/) pod adresem http://www.w3.org/TR/." %}

Ten dokument jest [Notatką Grupy Roboczej](http://www.w3.org/Consortium/Process/tr#WGNote) opracowaną przez [grupę zadaniową ds. Metodologii oceny WCAG 2.0 (Eval TF)](http://www.w3.org/WAI/ER/2011/eval/eval-tf), oraz [Grupę Roboczą ds. wytycznych dla dostępności treści internetowych (WCAG WG)](http://www.w3.org/WAI/GL/) i [Grupy Roboczej ds. narzędzi oceny i naprawy (ERT WG)](http://www.w3.org/WAI/ER/). Zawiera wskazówki informacyjne na temat oceny zgodnie z [Wytycznymi dla dostępności treści internetowych (WCAG) 2.0](http://www.w3.org/WAI/intro/wcag).

Jako Notatka Grupy Roboczej ten materiał jest stabilny. Na obecnym etapie Grupa Robocza nie planuje dalszych zmian. Jeśli jednak zajdzie taka potrzeba, dokument może zostać zaktualizowany. Uwagi otrzymane na temat tego dokumentu pomogą Grupie Roboczej zdecydować, czy aktualizacje są potrzebne lub zostaną  wzięte pod uwagę w przypadku planowania ponownej publikacji.  Wszelkie uwagi, w tym wykryte błędy, prosimy wysyłać na publiczną listę mailingową [public-wcag-em-comments@w3.org](mailto:public-wcag-em-comments@w3.org) (publicznie widoczne [archiwum listy mailingowej](http://lists.w3.org/Archives/Public/public-wcag-em-comments/). W komentarzach prosimy podać następujące informacje: lokalizację w dokumencie, sugerowaną zmianę oraz uzasadnienie komentarza.

Ten dokument został opracowany w ramach [Inicjatywy W3C na rzecz dostępności internetowej (WAI)](http://www.w3.org/WAI/). Cele grup roboczych WCAG WG i ERT WG zostały omówione odpowiednio w [Karcie Grupy Roboczej WCAG](http://www.w3.org/WAI/GL/2010/06/charter) i [Karcie Grupy Roboczej ERT](http://www.w3.org/WAI/ER/charter4). WCAG WG i ERT WG są częścią [WAI Technical Activity](http://www.w3.org/WAI/Technical/Activity).

Publikacja w formie Notatki Grupy Roboczej nie oznacza poparcia przez Członków W3C. Jest to wersja robocza dokumentu i może zostać w każdej chwili zaktualizowana, zamieniona lub uchylona przez inne dokumenty. Cytowanie tego dokumentu jako innego niż „praca w toku” jest niewłaściwe.

Ten dokument został opracowany przez dwie grupy działające w ramach W3C [Polityki patentowej W3C z 5 lutego 2004 roku](http://www.w3.org/Consortium/Patent-Policy-20040205/). Grupy nie oczekują, że dokument ten stanie się Rekomendacją W3C. W3C prowadzi [pełną listę zgłoszonych publicznie patentów WCAG WG](http://www.w3.org/2004/01/pp-impl/35422/status) oraz [pełną listę zgłoszonych publicznie patentów ERT WG](http://www.w3.org/2004/01/pp-impl/32094/status) wykonanych w związku z produktami każdej grupy; strony te zawierają również instrukcje zgłaszania patentu. Osoby, które twierdzą, że posiadają faktyczną wiedzę na temat patentów zawierających [istotne zastrzeżenia](http://www.w3.org/Consortium/Patent-Policy-20040205/#def-essential), muszą ujawnić informacje zgodnie z&nbsp;rozdziałem [6 Polityki patentowej W3C](http://www.w3.org/Consortium/Patent-Policy-20040205/#sec-Disclosure).

## Uwagi tłumacza

{% include callout.html content="**Uwaga 1:** Poniższe tłumaczenie ma charakter roboczy. Celem tłumacza było przygotowanie dokumentu przetłumaczonego na tyle dokładnie, aby pomagał osobom podejmującym się prób oceny dostępności stron internetowych odpowiednio przygotować do oceny i rozumieć konsekwencje podejmowanych wyborów metodologicznych.<br><br>**Uwaga 2:** Wszystkie odniesienia do WCAG 2.0 zostały zastąpione w tłumaczeniu odniesieniami do WCAG 2, wskazujac tym samym także na WCAG 2.1 i WCAG 2.2.<br><br>**Uwaga 3:** W przypadkach gdy istnieją polskie tłumaczenia przywoływanych dokumentów, odnośniki do wersji oryginalnych zostały zastąpione odnośnikami do wersji polskich." type="success" %}



## Wprowadzenie  {#introduction}

Ocena stopnia, w jakim strona internetowa jest zgodna z [Wytycznymi dla dostępności treści internetowych (WCAG) 2], jest procesem składającym się z kilku etapów. Na działania prowadzone w ramach tych etapów wpływ ma wiele czynników, takich jak: rodzaj strony internetowej (np. statyczna, dynamiczna, responsywna, mobilna, itp.); jej rozmiar, złożoność oraz technologie wykorzystywane do stworzenia strony internetowej (np. <acronym title="Hipertekstowy Język Znaczników">HTML</acronym>, <acronym title="Bogate Dostępne Aplikacje Internetowe">WAI-ARIA</acronym>, <acronym title="Przenośny Format Dokumentów">PDF</acronym>, itp.); poziom wiedzy oceniających na temat procesu zastosowanego w projektowaniu i tworzeniu witryny internetowej; oraz główny cel oceny (np. wydanie deklaracji dostępności, zaplanowanie procesu przeprojektowania, przeprowadzenie badań itp.)

Ta metodologia opisuje kroki, które są wspólne dla procesów kompleksowej oceny stopnia zgodności stron internetowych z <acronym>WCAG</acronym> 2. Wskazano w niej kwestie, które oceniający powinni rozważyć, aby zastosować opisane tu kroki w kontekście konkretnej witryny internetowej. Nie zastępuje to potrzeby stosowania środków zapewnienia jakości, które są wdrażane podczas projektowania, tworzenia i utrzymania witryn w celu zapewnienia ich zgodności z wymaganiami dostępności. Stosowanie tej metodologii pomoże oceniającym stosować dobre praktyki, unikać powszechnie popełnianych błędów i osiągać bardziej porównywalne wyniki. Jednak w większości sytuacji stosowanie wyłącznie tej metodologii, bez dodatkowych środków zapewnienia jakości, nie prowadzi bezpośrednio do stwierdzenia zgodności z <acronym>WCAG</acronym> 2.0.

**Ta metodologia w żaden sposób nie uzupełnia, ani nie zmienia wymagań określonych w normatywnym standardzie WCAG 2**, ani też nie dostarcza instrukcji oceny poszczególnych aspektów treści internetowych. Metodologia może być stosowana w połączeniu z technikami spełniania kryteriów sukcesu [WCAG 2.0[(http://www.w3.org/TR/WCAG20-TECHS/), takimi jak [Techniki dla <acronym>WCAG</acronym> 2.0](http://www.w3.org/TR/WCAG20-TECHS/) udokumentowane przez W3C/WAI, ale nie wymaga stosowania tego, ani żadnego innego konkretnego zestawu technik.</p>
	
## Cele metodologii  {#purpose}

W wielu sytuacjach konieczna jest ocena dostępności strony internetowej, na przykład przed wydaniem, nabyciem lub przeprojektowaniem witryny, a także w celu okresowego monitorowania dostępności witryny. Ta metodologia jest przeznaczona dla każdego, kto chce stosować wspólne podejście do oceny zgodności stron internetowych z WCAG 2.0. W kręgu osób, które mogą być zainteresowane metodologią, są:

 - Konsultanci internetowi, którzy chcą analizować i raportować zgodność z&nbsp;wymogami dostępności stron internetowych, aby informować ich właścicieli.
 - Dostawcy usług oceny dostępności cyfrowej, którzy chcą oceniać strony internetowe, aby potwierdzić zgodność z wymogami dostępności.
 - Twórcy witryn, którzy chcą ocenić zgodność swoich stron internetowych z wymogami dostępności, aby je monitorować lub ulepszać.
 - Właściciele witryn, zamawiający i dostawcy, którzy chcą dowiedzieć się o&nbsp;zgodności swoich stron internetowych  z&nbsp;wymogami dostępności.
 - Menedżerowie ds. zgodności z przepisami i zapewnienia jakości, którzy chcą mieć pewność, że spełniają wymagania dotyczące jakości i polityki.
 - Podmioty monitorujące dostępność cyfrową w celu testowania i porównywania postępów zgodności z&nbsp;wymogami dostępności.
 - Naukowcy zajmujący się zagadnieniami związanymi z&nbsp;dostępnością cyfrową oraz rzecznicy osób z niepełnosprawnościami, którzy chcą zbadać praktyki w&nbsp;zakresie zgodności z&nbsp;wymogami dostępności.
 - Trenerzy i edukatorzy ds. dostępności cyfrowej, którzy chcą uczyć podejścia do oceny dostępności stron internetowych.
 - Twórcy stron internetowych, autorzy treści, projektanci i inne osoby, które chcą dowiedzieć się więcej na temat dostępności i oceny witryn internetowych.

## Stosunek do wymogów zgodności WCAG 2  {#context}

WCAG 2.0 definiują [wymagania zgodności](http://www.w3.org/TR/WCAG20/#conformance-reqs) dla  pojedynczych stron internetowych (a&nbsp;w&nbsp;niektórych przypadkach także zestawów stron internetowych), ale nie opisują, jak oceniać całe witryny. Określają również, w jaki sposób można składać opcjonalne [deklaracje zgodności](http://www.w3.org/TR/WCAG20/#conformance-claims) w&nbsp;odniesieniu pojedynczych stron internetowych, serii stron internetowych, takich jak formularz wielostronicowy, oraz wielu powiązanych stron internetowych, takich jak witryna internetowa. Ma to zastosowanie do przypadków, gdy wszystkie strony internetowe objęte deklaracją zgodności zostały ocenione lub utworzone w procesie zapewniającym, że każda spełnia wszystkie wymagania dotyczące zgodności.

**Deklaracje zgodności z WCAG 2.0** **w odniesieniu do całych witryn internetowych nie mogą być formułowane na podstawie oceny wybranego podzbioru stron internetowych i samej funkcjonalności**, ponieważ zawsze możliwe jest, że na tych stronach pojawią się niezidentyfikowane błędy dotyczące zgodności. Jednak w większości zastosowań tej metodologii do oceny wybiera się tylko próbkę stron internetowych i funkcjonalności witryny. Dlatego w większości przypadków **samo zastosowanie tej metodologii nie daje wystarczających podstaw do stwierdzenia zgodności ocenianych witryn z WCAG 2.0**. Wskazówki dotyczące formułowania deklaracji zgoddnoścci w wyniku zastosowania tej metodologii znajdują się w [Kroku 5.c: Przygotuj deklarację zgodności (opcjonalnie)](#step5c).


### Lektury wprowadzające  {#reading}

Poniższe informacje związane z podstawami dostępności cyfrowej, ocenianiem i&nbsp;2.0 są niezbędne do korzystania z&nbsp;tej metodologii. Od osób oceniających, które korzystają z tej metodologii, oczekuje się dogłębnej znajomości wszystkich wymienionych poniżej materiałów:

### Podstawy dostępności cyfrowej

Poniższe dokumenty przedstawiają podstawowe elementy dostępności internetowej i wyjaśniają, jak osoby z&nbsp;niepełnosprawnościami korzystają z&nbsp;Internetu. Mają one kluczowe znaczenie dla zrozumienia szerszego kontekstu oceny dostępności internetowej:

- [Podstawowe komponenty dostępności stron internetowych](https://www.w3.org/WAI/fundamentals/components/),
- [Jak osoby z niepełnosprawnością korzystają z Internetu](https://www.w3.org/WAI/people-use-web/) (w jezyku angielskim).

### Ocena stron internetowych pod kątem dostępności  {#evaluating}

Są to szczególnie ważne materiały, które nakreślają różne podejścia do oceny stron internetowych pod kątem dostępności:

- [**Łatwe testy** – pierwszy przegląd dostępności stron internetowych](00-P-wprowadzenie); oryginał: [Easy Checks – A First Review of Web Accessibility](https://www.w3.org/WAI/test-evaluate/preliminary/)
- [Włączanie użytkowników do oceny dostępności cyfrowej](https://lepszyweb.pl/blog2/wlaczanie-uzytkownikow-do-oceny-dostepnosci-cyfrowej); oryginał: [Involving Users in Evaluating Web Accessibility](https://www.w3.org/WAI/test-evaluate/involving-users/)
- [Wybieranie narzędzi do oceny dostępności internetowej (Web Accessibility Evaluation Tools)](http://www.w3.org/WAI/eval/selectingtools) (w języku angielskim)
- [Wykorzystanie połączonej wiedzy specjalistycznej do oceny dostępności ](http://www.w3.org/WAI/eval/reviewteams) (w języku angielskim)

### Wytyczne dla dostępności treści internetowych(WCAG) 2.0  {#wcag2}

Jest to uznawany na całym świecie standard wyjaśniający, w jaki sposób sprawić, by treści internetowe były bardziej dostępne dla osób z&nbsp;niepełnosprawnościami. Poniższe materiały są szczególnie ważne dla oceny dostępności stron internetowych:

*   [Omówienie WCAG 2.0](https://www.w3.org/WAI/standards-guidelines/wcag/)
*   [Specyfikacja techniczna WCAG 2.0](http://www.w3.org/TR/WCAG20/)
*   [Jak spełnić WCAG 2.0 (Krótki przewodnik)](http://www.w3.org/WAI/WCAG20/quickref/)
*   [Objaśnienia WCAG 2.0](http://www.w3.org/TR/UNDERSTANDING-WCAG20/)
*   [Techniki dla WCAG 2.0](http://www.w3.org/TR/WCAG20-TECHS/)

### Terminy i definicje

Na potrzeby niniejszego dokumentu stosujemy następujące terminy i definicje:

    <dl>
        <dt id="complete">całe procedury</dt>
        <dd>Z <a href="http://www.w3.org/TR/WCAG20/#cc3">wymagań zgodności <acronym>WCAG</acronym> 2.0 dla całych procedur</a>: <br /><q><em>Gdy strona internetowa jest jedną z&nbsp;serii stron przedstawiających procedurę (czyli sekwencję kroków niezbędną, aby wykonać jakieś zadanie), to wszystkie strony przedstawiające etapy procedury są zgodne na deklarowanym poziomie lub wyższym. (Zgodność nie jest możliwa na deklarowanym poziomie, jeżeli którakolwiek strona w procedurze nie jest zgodna na tym poziomie lub wyższym).</em></q></dd>

        <dt id="functionality">niezbędna funkcjonalność</dt>
        <dd>
            Funkcjonalność strony internetowej, która, jeśli zostanie usunięta, zasadniczo zmienia sposób korzystania lub cel strony internetowej dla użytkowników. Obejmuje to informacje, do których odwołują się użytkownicy, jak i&nbsp;czynności, które wykonują, aby użyć tej funkcjonalności.
            <p class="note">
                <strong>Uwaga:</strong> Przykłady niezbędnych funkcjonalności obejmują „wybór i zakup produktu w sklepie internetowym”, „wypełnienie i&nbsp;przesłanie formularza kontaktowego”, „rejestrację konta użytkownika”.
            </p>
            <p class="note"><strong>Uwaga:</strong> Stosowanie pojęcia „niezbędnej funkcjonalności” nie wyłącza z zakresu oceny innych funkcjonalności. Termin „niezbędna funkcjonalność” ma pomóc w&nbsp;rozpoznaniu krytycznych stron internetowych i&nbsp;uwzględnieniu ich w&nbsp;ocenie obok innych. </p>
        </dd>
        <dt id="evaluator">oceniający</dt>
        <dd>Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot odpowiedzialny za przeprowadzenie oceny.</dd>
        <dt id="relied">polegać na (technologii)</dt>
        <dd>Z definicji pojęcia <a href="http://www.w3.org/TR/WCAG20/#reliedupondef">„polegać na”</a> w&nbsp;<acronym>WCAG</acronym> 2.0 <br /><q><em>Treść nie będzie zgodna, jeżeli taka technologia nie zostanie objęta oceną lub nie jest obsługiwana.</em></q></dd>
        <dt id="states">stan strony internetowej</dt>
        <dd>
            Dynamicznie generowane strony internetowe prezentują czasami znacznie różniące się od siebie treści, funkcjonalności i&nbsp;wygląd w&nbsp;zależności od użytkownika, interakcji, urządzenia i&nbsp;innych parametrów. W kontekście tej metodologii takie stany stron internetowych można traktować jako pomocnicze dla stron internetowych (rejestrowane w&nbsp;próbce strony internetowej jako dodatkowy stan strony internetowej) lub jako pojedyncze strony internetowe.
            <p class="note">
                <strong>Uwaga:</strong> Przykładami stanów stron internetowych są poszczególne strony wieloczęściowego formularza internetowego, które są generowane dynamicznie w&nbsp;zależności od danych wprowadzonych przez użytkownika. Poszczególne stany mogą nie mieć unikalnych <acronym title="Uniwersalnych Identyfikatorów Zasobu">URI</acronym> i&nbsp;mogą wymagać identyfikacji poprzez opisanie ustawień, danych wejściowych lub działań wymaganych do ich wygenerowania.
            </p>
        </dd>
        <dt id="webpage">strona internetowa</dt>
        <dd>
            Z definicji <a href="http://www.w3.org/TR/WCAG20/#webpagedef"> „strony internetowej” w <acronym>WCAG</acronym> 2.0:</a> <br /><q><em>Nieosadzony zasób, uzyskany z pojedynczego identyfikatora <acronym>URI</acronym> za pomocą protokołu <acronym>HTTP</acronym> wraz z wszelkimi innymi zasobami użytymi do renderowania strony w programie użytkownika lub takimi, które potencjalnie mogą być użyte do renderowania.</em></q>
            <p class="note">
                <strong>Uwaga:</strong> Strony internetowe mogą zawierać treści multimedialne, komponenty interaktywne oraz bogate i&nbsp;mobilne aplikacje internetowe. Pojęcie strony internetowej nie ogranicza się do formatu HTML, strony internetowe mogą być dokumentami PDF, a&nbsp;także dokumentami w innych formatach.
            </p>
        </dd>
        <dt id="common">strony wspólne</dt>
        <dd>
            Strony internetowe i <em>stany stron</em> internetowych odnoszące się do całej witryny. Obejmuje to stronę główną, stronę logowania i inne strony początkowe oraz, w stosownych przypadkach, mapę witryny, stronę kontaktową, stronę pomocy, stronę informacji prawnych i podobne, które są zazwyczaj połączone ze wszystkimi innymi stronami witryny (zwykle poprzez łącze w nagłówku, stopce lub w menu nawigacyjnym).
            <p class="note">
                <strong>Uwaga:</strong> Definicja <a href="#states" class="termref">stanu strony internetowej</a> znajduje się powyżej.
            </p>
        </dd>
        <dt id="template">szablony</dt>
        <dd>Z definicji pojęcia <a href="http://www.w3.org/TR/ATAG20/#def-Template">„szablony” w <acronym>ATAG</acronym> 2.0</a>:<br /><q><em>Wzorce treści, które są wypełniane przez autorów lub za pomocą narzędzia autorskiego (np. szablony dokumentów, szablony w systemach zarządzania treścią, motywy prezentacji). Szablony zwykle zastępują autorów, przynajmniej częściowo, w decydowaniu o układzie i stylizacji treści.</em></q></dd>
        <dt id="developer">twórca witryny</dt>
        <dd>Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot zaangażowany w proces tworzenia witryny, w tym między innymi autorzy treści, projektanci, programiści, testerzy zapewniania jakości oraz kierownicy projektu.</dd>
        <dt id="website">witryna internetowa</dt>
        <dd>
            Spójny zbiór jednej lub więcej powiązanych stron internetowych, które razem zapewniają wspólne użytkowanie lub funkcjonalność. Pojęcie obejmuje statyczne strony internetowe, dynamicznie generowane strony internetowe oraz strony i aplikacje mobilne.
            <p class="note"><strong>Uwaga:</strong> Ta metodologia koncentruje się na całych, samodzielnych witrynach internetowych. Witryny mogą składać się z mniejszych zbiorów stron, z których każdy można uznać za odrębną witrynę. Na przykład witryna może zawierać wyodrębnione obszary, takie jak sklep internetowy, forum dyskusyjne albo odrębne obszary dla każdego działu czy filii w organizacji, obszar blogów i inne, powiązane wspólnym adresem domenowym. Każdy taki podzbiór może być uznany za odrębną witrynę.</p>
        </dd>
        <dt id="owner">właściciel witryny</dt>
        <dd>Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot odpowiedzialny za publikację witryny internetowej.</dd>
        <dt id="conformance">zgodność</dt>
        <dd>Z definicji <a href="http://www.w3.org/TR/WCAG/#conformancedef">„zgodności” w <acronym>WCAG</acronym> 2.0:</a> <br /><q><em>Spełnienie wszystkich wymagań danej normy, wytycznych lub specyfikacji.</em></q></dd>
        <dt id="commissioner">zleceniodawca oceny</dt>
        <dd>
            Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot, który zlecił ocenę.
            <p class="note" style="margin-top: 0;"><strong>Uwaga:</strong> W wielu przypadkach zleceniodawcą oceny może być właściciel witryny internetowej lub jej twórca, w innych przypadkach może to być inny podmiot, taki jak zamawiający lub właściciel ankiety monitorującej dostępność. </p>
        </dd>

    </dl>
	
## Korzystanie z metodologii  {#usage}

Metodologia ta służy do dokładnej oceny witryn internetowych przy użyciu <acronym>WCAG</acronym> 2.0. Przed oceną całej witryny dobrze jest przeprowadzić wstępną ocenę różnych stron internetowych z ocenianej witryny, aby rozpoznać oczywiste bariery dostępności i zdobyć ogólne rozeznanie w dostępności witryny. <a href="http://www.w3.org/WAI/eval/preliminary">Łatwe testy - wstępny przegląd dostępności internetowej</a> opisuje takie podejście do wstępnej oceny, które jest uzupełnieniem tej metodologii.


### Wymagana wiedza specjalistyczna  {#expertise}

Zakłada się, że użytkownicy tej metodologii mają solidną wiedzę na temat oceniania treści internetowych przy użyciu <acronym>WCAG</acronym> 2.0, dostępnego projektowania internetowego, technologii wspomagających oraz tego, jak osoby z różnymi rodzajami niepełnosprawności korzystają z Internetu. Obejmuje to zrozumienie technologii internetowych, barier dostępności, których doświadczają osoby z niepełnosprawnościami, technologii wspomagających i strategii adaptacyjnych stosowanych przez osoby z niepełnosprawnościami, oraz technik oceny, narzędzi i metod rozpoznawania barier dla osób z niepełnosprawnościami. W szczególności zakłada się, że użytkownicy tej metodologii są dogłębnie zaznajomieni ze wszystkimi materiałami wymienionymi w rozdziale [Lektury wprowadzające](#reading).


### Zbiorowa wiedza specjalistyczna (opcjonalnie)   {#combined}

    <p>Metodologię tę może stosować indywidualny oceniający, który posiada kwalifikacje opisane w poprzedniej sekcji [(Wymagana wiedza specjalistyczna](#expertise)), lub zespół oceniających posiadających zbiorową wiedzę specjalistyczną. Korzystanie z połączonej wiedzy specjalistycznej różnych oceniających może czasami być konieczne lub korzystne, gdy jeden oceniający sam nie posiada całej wymaganej wiedzy specjalistycznej. Więcej wykraczających poza zakres tego dokumentu wskazówek na temat korzystania ze zbiorowej wiedzy specjalistycznej zespołów oceniających znajduje się w opracowaniu [Korzystanie ze zbiorowej wiedzy specjalistycznej do oceny dostępności stron internetowych](https://www.w3.org/WAI/test-evaluate/combined-expertise/).
	

### Włączanie użytkowników (opcjonalnie)  {#users}

   Włączanie osób z niepełnosprawnościami, w tym osób z trudnościami związanymi ze starzeniem się (które nie są doświadczonymi testerami lub członkami zespołu oceniającego), może pomóc w rozpoznaniu dodatkowych barier dostępności, które nie są łatwe do wykrycia w drodze oceny eksperckiej. Chociaż nie jest to wymagane do stosowania tej metodologii, oceniający mogą czasem być zmuszeni do zaangażowania w proces oceny osób doświadczających autentycznych problemów z dostępnością. Więcej wykraczających poza zakres tego dokumentu wskazówek na temat angażowania użytkowników w ocenę dostępności znajduje się w opracowaniu [Włączanie użytkowników do oceny dostępności cyfrowej](https://www.w3.org/WAI/test-evaluate/involving-users/).
	

### Narzędzia oceny (opcjonalnie)  {#tools}

    Metodologia jest niezależna od jakiegokolwiek konkretnego narzędzia oceny dostępności internetowej, przeglądarki internetowej i innych narzędzi programowych. Chociaż większość testów nie jest w pełni zautomatyzowana, to narzędzia oceny mogą znacznie pomóc oceniającym w procesie oceny i przyczynić się do bardziej efektywnej oceny. Na przykład, niektóre narzędzia oceny dostępności cyfrowej mogą skanować całe witryny, aby pomóc w typowaniu odpowiednich stron do oceny ręcznej. Narzędzia mogą być również pomocne podczas ręcznej (ludzkiej) oceny testów dostępności. Więcej wykraczających poza zakres tego dokumentu wskazówek na temat korzystania z narzędzi oceny zawiera opracowanie [Wybieranie narzędzi do oceny dostępności cyfrowej](https://www.w3.org/WAI/test-evaluate/tools/selecting/)

## Zakres stosowania   {#tools}

    Metodologia została zaprojektowana do oceny całych [witryn internetowych](#website). Oznacza to, że dla każdej [strony internetowej](#webpage) jest jednoznaczne, czy jest ona częścią witryny, czy nie. Dotyczy to witryn organizacji, podmiotów, osób, wydarzeń, produktów i usług.

### Przykłady witryn internetowych

Oto kilka konkretnych przykładów witryn internetowych:

*   „Publiczna witryna Przykładowej Organizacji pod adresem http://www.przykladowa-organizacja.org”
*   „Witryna intranetowa Przykładowej Organizacji pod adresem http://intranet.przykladowa-organizacja.org”
*   „Sklep internetowy Przykładowej Organizacji pod adresem http://www.przykladowa-organizacja.org /sklep/”
*   „Wydanie wersji 1.5.3 aplikacji System rezerwacji internetowej (SRI)”
*   „Mobilna wersja witryny Przykładowej Organizacji pod adresem http://m.przykladowa-organizacja.org”
*   „Holenderska wersja witryny Przykładowej Organizacji pod adresem http://nl.przykladowa-organizacja.org”


Witryna może być częścią większej witryny, jak na przykład sklep internetowy w przykładach powyżej. Witryna może być także wyraźnie oddzielną wersją witryny, taką jak wersja mobilna lub wersja w języku holenderskim, jak pokazano w przykładach powyżej. Metodologia może być zastosowana do każdej takiej możliwej do określenia witryny, niezależnie od tego, czy jest ona częścią większej witryny, czy też nie. Precyzyjne określenie witryny jest ustalane w ramach [Kroku 1.a](#step1a).

### Zasady uwzględniania stron w ocenie  {#enclosure}

W przypadku, gdy do oceny została wyznaczona witryna internetowa, istotne jest, aby wszystkie strony internetowe, stany stron internetowych i funkcjonalności objęte zakresem jej definicji były uwzględnione w ocenie. Wyłączenie takich aspektów witryny z zakresu oceny prawdopodobnie byłoby sprzeczne z wymogami zgodności <acronym>WCAG</acronym> 2.0 dla [całych witryn](http://www.w3.org/TR/WCAG20/#cc2) i [całych procedur](http://www.w3.org/TR/WCAG20/#cc3) lub w inny sposób zniekształcałoby wyniki oceny.

#### Przykład włączania witryny do oceny  {#example_enclosure}

![Schemat witryny uniwersytetu ilustrujący zasadę uwzględniania stron w ocenie objaśniony w następnym akapicie.](./WCAG-EM-1-0_files/website.svg)

Powyższy schemat pokazuje witrynę uniwersytetu złożoną z odrębnych obszarów; „Informacje dla studentów”, „Informacje dla wykładowców”, „Kursy” i „Biblioteka”.  Aplikacja „Kursy” obejmuje „Kurs fizyki”, „Kurs medycyny” i „Kurs historii”, które są zgrupowane w tym obszarze. Witryna uniwersytecka ma również pojedyncze strony internetowe, takie jak informacje prawne, mapa witryny i inne strony wspólne dla wszystkich obszarów.

W powyższym przykładzie, jeśli witryna uniwersytetu jest wyznaczona do oceny w całości, to wszystkie przedstawione obszary są objęte oceną. Obejmuje to wszelkie zagregowane i osadzone treści, takie jak mapy kampusu, formularze płatności internetowej i fora dyskusyjne, także jeśli takie części pochodzą ze źródeł zewnętrznych. Jeśli natomiast tylko określony obszar witryny, taki jak „Kursy”, zostanie wyznaczony do oceny, wówczas zakresem oceny objęte są wszystkie części tego obszaru, a więc obszary poświęcone każdemu z kursów, a także strony internetowe wspólne dla wszystkich obszarów witryny uniwersytetu. W tym przypadku zakres oceny obejmowałby wszystkie przedstawione kursy, a także poszczególne strony internetowe, które są [wspólne](#common) dla wszystkich obszarów witryny uniwersytetu. 

### Konkretne typy witryn  {#specialcases}

Metodologia ma zastosowanie do szerokiej gamy typów witryn internetowych. Poniżej przedstawiono uwagi dotyczące konkretnych sytuacji, pamiętając, że witryny internetowe mogą łączyć łączyć kilka różnych kryteriów. Zatem poniższa lista nie jest wyłączna i wyczerpująca:

    <dl>
        <dt id="smallsites">Małe witryny</dt>
        <dd>W przypadku witryn z kilkoma stronami procedura próbkowania zdefiniowana w <a href="#step3" class="termref">kroku 3: Wybierz reprezentatywną próbkę stron</a> prawdopodobnie doprowadzi do wybrania większości lub wszystkich stron internetowych z ocenianej witryny. W przypadkach, w których można ocenić wszystkie strony internetowe, procedurę próbkowania można pominąć, a za wybraną próbkę w pozostałych krokach uznaje się całą witrynę.</dd>
        <dt id="applications">Aplikacje internetowe</dt>
        <dd>
            Aplikacje internetowe składają się zazwyczaj z dynamicznie generowanej treści i funkcjonalności (zobacz <a href="#states" class="termref">stany stron internetowych</a>). Aplikacje internetowe są zazwyczaj bardziej złożone i interaktywne. Przykładami aplikacji internetowych są programy pocztowe, edytory dokumentów i sklepy internetowe. Aplikacja internetowa może być częścią większej witryny internetowej, ale w kontekście tej metodologii może również stanowić odrębną witrynę internetową, to znaczy, indywidualną i oddzielną jednostkę do oceny.
            <p class="note">
                <strong>Uwaga:</strong> Ze względu na wiele możliwości generowania treści i funkcjonalności w aplikacjach internetowych czasami nie jest wykonalne wyczerpujące rozpoznanie wszystkich możliwych stron internetowych, ich stanów i funkcjonalności. Aplikacje internetowe zwykle wymagają więcej czasu i wysiłku, aby je ocenić, i zazwyczaj potrzebują większych próbek stron internetowych, aby odzwierciedlić różne typy treści, funkcjonalności i procedur.
            </p>
        </dd>
        <dt id="separable">Witryny internetowe z odrębnymi obszarami</dt>
        <dd>
            W niektórych przypadkach witryny mogą mieć wyraźnie wydzielone obszary, w których korzystanie z jednego obszaru nie wymaga, ani nie zależy od korzystania z innego obszaru witryny. Na przykład organizacja może zapewnić tylko dla swoich pracowników ekstranet, który jest połączony z publiczną witryną internetową, ale poza tym jest oddzielny, lub może mieć podstrony dla poszczególnych działów organizacji, z których każda jest wyraźnie oddzielona od innych. Takie wyodrębnione obszary mogą być traktowane jako indywidualne witryny internetowe do oceny. W niektórych przypadkach mogą istnieć <a href="#common" class="termref">wspólne strony internetowe</a>, takie jak informacje prawne, które należy uwzględnić jako część każdego obszaru witryny.
            <p class="note">
                <strong>Uwaga:</strong> Niektóre strony internetowe zapewniają dodatkową lub różną treść i funkcjonalność w zależności od użytkownika (zazwyczaj po zalogowaniu się).  Ta dodatkowa treść i funkcjonalność jest zasadniczo częścią podstawowego celu i funkcjonalności witryny i dlatego nie jest uważana za odrębny obszar witryny.
            </p>
        </dd>
        <dt id="versions">Witryny internetowe w wielu wersjach</dt>
        <dd>
            Niektóre witryny internetowe istnieją w wielu wersjach, które są od siebie niezależne, to znaczy korzystanie z jednej wersji nie wymaga, ani nie zależy od korzystania z innej wersji witryny.  Na przykład witryna internetowa może mieć wersję mobilną i mogą istnieć wersje witryny internetowej w różnych językach, które spełniają tę cechę.  Zwykle każda taka wersja witryny ma inny zestaw <acronym title="Uniwersalnych Identyfikatorów Zasobu">URI</acronym>. Takie wersje witryn można traktować jako indywidualne witryny do oceny.
            <p class="note">
                <strong>Uwaga:</strong> Witryny internetowe wykorzystujące techniki responsywnego projektowania (tzn. dostosowujące prezentację do sprzętu, oprogramowania i preferencji użytkownika) w przeciwieństwie do witryn, na które użytkownicy zostali przekierowani z innych miejsc, nie są uznawane za niezależne wersje witryn internetowych.
            </p>
        </dd>
        <dt id="responsive">Witryny internetowe wykorzystujące projektowanie responsywne</dt>
        <dd>
            Techniki projektowania responsywnego dostosowują kolejność, przepływ, a czasami także zachowanie treści tak, aby jak najlepiej pasowały do urządzenia, na którym są używane. Na przykład, aby dopasować treść i funkcjonalność do rozmiaru rzutni, rozdzielczości ekranu, orientacji ekranu i innych aspektów urządzenia mobilnego oraz kontekstu, w którym jest ono używane. W tej metodologii takie zmiany treści, funkcjonalności, wyglądu i zachowania nie są uważane za niezależne wersje witryn internetowych, ale raczej za <a href="#states" class="termref">stany strony internetowej</a>, które należy uwzględnić w zakresie oceny.
            <p class="note">
                <strong>Uwaga:</strong> W przypadku witryn korzystających z elastycznych technik projektowania należy wziąć pod uwagę urządzenia mobilne, systemy operacyjne i technologie wspomagające, w szczególności podczas <a href="#step1c" class="termref">kroku 1.c:  Określ poziom bazowy obsługi dostępności</a>.
            </p>
        </dd>
    </dl>

### Konkretne konteksty oceny  {#considerations}

Ta metodologia ma być elastyczna, aby ułatwić jej zastosowanie w różnych sytuacjach i kontekstach.  Poniższe rozważania odnoszą się do konkretnych sytuacji i kontekstów oceny.

    <dl>
        <dt id="selfassessment">Samoocena zgodności</dt>
        <dd>Wewnętrzni oceniający oraz oceniający, którzy biorą udział w procesie programowania, często mają łatwiejszy dostęp do programistów i opiekunów witryn, środowisk programistycznych i hostingowych, narzędzi autorskich oraz materiałów wykorzystywanych do programowania i konserwacji. W szczególności przypadki użycia, analizy projektu, specyfikacje techniczne i dokumentacja oraz zasoby testowe mogą zwiększyć efektywność oceny i powinny być wykorzystywane tam, gdzie to możliwe.</dd>
        <dt id="certification">Zewnętrzna ocena zgodności</dt>
        <dd>Niezależni zewnętrzni oceniający zazwyczaj mają mniej informacji na temat wewnętrznego oprogramowania, obszarów i funkcjonalności witryny internetowej, ponieważ nie byli zaangażowani w jej zamawianie oraz w sposób, w jaki witryna została zaprojektowana i opracowana.  Często osoby oceniające w takich sytuacjach muszą skontaktować się z właścicielem lub twórcą witryny, aby uzyskać niezbędne informacje, które czynią ocenę efektywniejszą.</dd>
        <dt id="indevelopment">Ocena podczas tworzenia</dt>
        <dd>Chociaż ta metodologia została zaprojektowana przede wszystkim do oceny witryn internetowych, które już zostały zaprojektowane i wdrożone, kluczowe znaczenie ma ocena dostępności na wszystkich etapach projektowania i wdrażania witryny, aby zapewnić jej zgodność.  Wskazówki zawarte w tej metodologii mogą być przydatne na tych wcześniejszych etapach procesu projektowania i tworzenia, choć może być konieczne pewne dostosowanie. Ważne jest jednak, aby pamiętać, że oceny przeprowadzone na tych wcześniejszych etapach mogą szybko stać się nieaktualne poprzez wprowadzenie nawet drobnych zmian.  W związku z tym oceny przeprowadzane na tych etapach nie powinny być wykorzystywane do składania deklaracji ani oświadczeń o zgodności dotyczących sfinalizowanej witryny internetowej.</dd>
        <dt id="composite">Ocena złożonych witryn internetowych</dt>
        <dd>Podczas oceny witryn internetowych z <a href="#separable" class="termref">odrębnymi obszarami</a>, takimi jak sklep internetowy, obszar blogów i inne podstrony, przydatne może być przeprowadzenie najpierw osobnej oceny każdego obszaru strony internetowej zgodnie z tą metodologią, a następnie ogólnej oceny z próbkami z każdego obszaru witryny i wszelkich wspólnych stron internetowych.  Zapewniłoby to pełniejsze objęcie oceną całej witryny, jak również zapewniłoby wgląd w sposób, w jaki każdy obszar witryny jest realizowany, który może się różnić w zależności od obszaru.</dd>
        <dt id="aggregated">Ocena witryn agregujących treści z innych źródeł</dt>
        <dd>Witryny internetowe, które są generowane przy użyciu treści łączonych z różnych źródeł, takich jak portale z portletami, są zwykle znacznie trudniejsze do oceny ze względu na wiele różnych instancji treści, które mogą być generowane.  Ogólnie rzecz biorąc, nie jest możliwe oddzielne ocenianie treści z ich źródeł osobno, a raczej ich wyświetlanie użytkownikom, gdy są połączone.</dd>
        <dt id="thirdparty">Ocena treści innych podmiotów</dt>
        <dd>Treści osób trzecich nie są kontrolowane przez witrynę internetową lub dostawców usług internetowych; na przykład treści generowane przez użytkowników witryny internetowej na forum internetowym.  <acronym>WCAG</acronym> 2.0 zawiera szczegółowe rozważania dotyczące zgodności tego typu treści w rozdziale <a href="http://www.w3.org/TR/WCAG20/#conformance-partial">Oświadczenie o częściowej zgodności</a>. W takich przypadkach osoby oceniające będą musiały ustalić, czy takie treści są regularnie monitorowane i naprawiane (w ciągu dwóch dni roboczych) oraz czy treści niezgodne są wyraźnie oznaczone jako takie na wszystkich stronach internetowych, na których się pojawiają.</dd>
        <dt id="rerun">Ponowna ocena witryny internetowej</dt>
        <dd>
            <p>Ocena witryny internetowej, zgodnie z tą metodologią, może być ponownie przeprowadzona po krótkim czasie; na przykład, gdy problemy zostaną zidentyfikowane i naprawione przez właściciela witryny lub jej twórcę, lub okresowo w celu monitorowania postępów.  W takich przypadkach ocena może być przeprowadzona przy użyciu próbki stron internetowych, która zawiera:</p>
            <ul>
                <li>Podzbiór stron internetowych, które zostały użyte w poprzedniej ocenie, aby ułatwić porównanie wyników;</li>
                <li>Zastąpiony podzbiór stron internetowych z tych, które zostały wykorzystane w poprzedniej ocenie w celu poprawy zasięgu witryny.</li>
            </ul>
            <p>O ile w witrynie internetowej nie wprowadzono istotnych zmian, zwykle nie ma potrzeby zmiany wielkości wybranej próbki stron internetowych ani podejścia zastosowanego do próbkowania.  Liczba zastąpionych stron internetowych w nowej próbce wynosi zazwyczaj około połowy pierwotnej próbki, choć można ją zwiększyć, gdy strony internetowe w większości są zgodne z <acronym>WCAG</acronym> 2.0.</p>
        </dd>
        <dt id="largescale">Ocena na dużą skalę</dt>
        <dd>Przeprowadzanie masowej oceny wielu witryn internetowych, na przykład na potrzeby krajowych lub międzynarodowych badań sondażowych, jest zazwyczaj wykonywane głównie za pomocą automatycznych narzędzi oceny.  Stosunkowo niewiele stron internetowych poddawanych jest pełnej kontroli ręcznej.  Takie oceny zwykle nie uwzględniają niezbędnej jakościowej oceny zgodności dla każdej witryny, dla której opracowano tę metodologię.</dd>
    </dl>

## Procedura oceny  {#procedure}

W tej części opisano etapy i czynności związane z procedurą oceny. Etapy te niekoniecznie muszą następować po sobie. Dokładna kolejność działań wykonywanych w kolejnych etapach oceny również zależy od rodzaju witryny, celu oceny i procedury stosowanej przez oceniającego.  Niektóre działania mogą się pokrywać lub mogą być prowadzone równolegle.  Poniższy schemat ilustruje iteracje pomiędzy etapami zdefiniowanymi w tej części:

![Schemat procedury oceny - iteracje między etapami oceniania. Wyjaśnienie w następnym akapicie.](./WCAG-EM-1-0_files/process.svg)

Powyższy schemat toku pracy przedstawia pięć następujących po sobie kroków:  1. Ustal zakres oceny; 2. Poznaj ocenianą witrynę; 3. Wybierz reprezentatywną próbkę; 4. Wykonaj audyt wybranej próbki i 5. Sporządź raport z oceny. Każdy krok ma strzałkę do następnego kroku i strzałki do wszystkich poprzednich kroków. Ilustruje to, w jaki sposób osoby oceniające przechodzą od jednego kroku do następnego i mogą powrócić do każdego poprzedniego kroku, gdy podczas procesu oceny zostaną ujawnione nowe informacje.

### Krok 1: Ustal zakres oceny  {#step1}

**Wymóg metodologiczny 1 {#req1} :** Ustal zakres oceny zgodnie z [wymogiem metodologicznym 1.a](#req1a), [wymogiem metodologicznym 1.b](#req1b) i [wymogiem metodologicznym 1.c](#req1c) oraz opcjonalnie z [wymogiem metodologicznym 1.d](#req1d).

Na tym etapie określa się ogólny zakres oceny. Jest to podstawowy krok, który wpływa na kolejne etapy procedury oceny.  Najlepiej ustalić zakres oceny w porozumieniu z zlecającym ocenę (który może, ale _nie musi_ być właścicielem witryny), aby zagwarantować spełnienie oczekiwań co do zakresu oceny. Na tym etapie może być konieczne wstępne rozpoznanie witryny, aby lepiej poznać jej specyfikę i wymagania oceny.  Szczegółowa eksploracja witryny jest przeprowadzana w [kroku 2: Poznaj ocenianą witrynę](#step2).
	

#### Krok 1.a: Określ zakres stron witryny  {#step1a}

<p id="#req1a"><strong>Wymóg metodologiczny 1.a</strong>: Zdefiniuj [witrynę internetową](#website) do oceny zgodnie z [zakresem stosowania metodologii](#applicability), tak aby dla każdej [strony internetowej](#webpage) było jasne, czy znajduje się ona w zakresie stron podlegających ocenie.</p>

Na tym etapie określa się witrynę docelową (strony i stany stron internetowych podlegające ocenie). Zakres witryny jest określany zgodnie z warunkami określonymi w sekcji [Zakres zastosowania](#applicability).

Aby uniknąć późniejszych rozbieżności oczekiwań między oceniającym, osobą zlecającą ocenę i odbiorcami wynikowego raportu z oceny, ważne jest, aby określić ocenianą witrynę internetową tak, aby było jednoznaczne, które strony internetowe wchodzą w jej zakres. Tam, gdzie to możliwe, zaleca się stosowanie formalizacji, w tym [wyrażeń regularnych](http://en.wikipedia.org/wiki/Regular_expression) i wykazów adresów internetowych (<acronym title="Uniwersalnych Identyfikatorów Zasobu">URI</acronym>).

Ważne jest również udokumentowanie wszelkich szczególnych aspektów z punktu widzenia ocenyocenianej witryny. Są to między innymi:

*   Wykorzystywanie treści i usług stron trzecich;
*   Mobilne i językowe wersje witryny;
*   Wyodrębnione obszary, np. sklep internetowy, które pomimo innego adresu URI są uznawane za część witryny wyznaczonej do oceny (takie obszary mogą być trudne do zidentyfikowania).

#### Krok 1.b: Określ wymagany poziom zgodności  {#step1b}

**Wymóg metodologiczny 1.b {#req1b} :** Określ wymagany [poziom zgodności](http://www.w3.org/TR/WCAG20/#cc1) z WCAG 2.0 ("A", "AA" lub "AAA") .

Częścią rozpoczęcia procesu oceny jest określenie, który poziom zgodności z WCAG 2.0 ("A", "AA" lub "AAA") będzie punktem odniesienia dla oceny. Ogólnie przyjętym i zalecanym celem jest zgodność z <acronym>WCAG</acronym> 2.0 na poziomie AA.

**Uwaga:** Często przydatna jest ocena wykraczająca poza wymagany poziom zgodności, aby uzyskać pełniejszy obraz dostępności witryny. Na przykład, chociaż witryna może nie spełniać całkowicie określonego poziomu zgodności, ale może spełniać niektóre wymagania z wyższego poziomu zgodności. Posiadanie tych informacji może pomóc w bardziej efektywnym planowaniu przyszłych ulepszeń.

#### Krok 1.c: Określ bazowy zestaw obsługi dostępności  {#step1c}

**Wymóg metodologiczny 1.c {#req1c} :** Określ podstawowy zestaw kombinacji przeglądarek, technologii wspomagających i innych [programów użytkownika](http://www.w3.org/TR/WCAG20/#useragentdef) (np. odtwarzaczy mediów), w których treści i cechy witryny mają być [obsługiwane pod względem dostępności](http://www.w3.org/TR/WCAG20/#accessibility-supporteddef).

Szczególnie w przypadku nowych technologii internetowych nie zawsze jest możliwe zapewnienie, że każda cecha dostępności istniejąca w witrynie, np. taka jak funkcja „pokaż napisy rozszrzone” w odtwarzaczu multimedialnym, będzie obsługiwana przez każdą możliwą kombinację systemu operacyjnego, przeglądarki internetowej, technologii wspomagającej i innych programów użytkowników. <acronym>WCAG</acronym> 2.0 nie określa z góry, które kombinacje cech i technologii muszą być obsługiwane, ponieważ zależy to od konkretnego kontekstu witryny, w tym jej języka, technologii internetowych wykorzystywanych do tworzenia treści oraz aktualnie dostępnych programów użytkownika. Więcej wskazówek na temat koncepcji _obsługi dostępności_ w WCAG 2.0 znajduje się w opracowaniu [Objaśnienie obsługi dostępności](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance#uc-accessibility-support-head).

W trakcie tego etapu oceniający określa minimalny zestaw kombinacji systemów operacyjnych, przeglądarek internetowych, technologii wspomagających i innych programów użytkownika, z którymi witryna ma pracować, i które są zgodne z wytycznymi <acronym>WCAG</acronym> 2.0 dotyczącymi obsługi dostępności (łącze powyżej). Zestaw technologii bazowych najlepiej ustalić w porozumieniu ze zlecającym ocenę, aby zagwarantować, że oczekiwania zlecającego i oceniającego co do poziomu wsparcia technologii będą takie same. Właściciel witryny i jej twórca również mogą dysponować taką listą kombinacji, do obsługi których witryna została zaprojektowana, co może stanowić punkt wyjścia dla tego kroku.  W zależności od celu oceny taka lista może wymagać aktualizacji, na przykład w celu oceny, jak dobrze działa strona internetowa z nowszymi przeglądarkami.

**Uwaga:** Ta wstępna bazowa lista technologii nie ogranicza oceniającego w możliwościach wykorzystania później dodatkowych systemów operacyjnych, przeglądarek internetowych, technologii wspomagających i innych programów użytkowników, na przykład w celu oceny treści, które nie zostały zauważone na tym wczesnym etapie procesu oceny.  W takim przypadku bazowy zestaw technologii jest rozszerzany o dodatkowe narzędzia, które zostały wykorzystane.
	
**Uwaga:** W przypadku niektórych witryn internetowych w sieciach zamkniętych, takich jak witryna intranetowa, w których znani są zarówno użytkownicy, jak i komputery używane do uzyskania dostępu do witryny, bazowa lista technologii może być ograniczona do systemów operacyjnych, przeglądarek internetowych i technologii wspomagających  używanych w ramach tej zamkniętej sieci.  Jednak w większości przypadków bazowa lista technologii jest znacznie szersza i obejmuje większość aktualnie używanych przez osoby z niepełnosprawnościami w danym regionie geograficznym i społeczności językowej programów użytkownika i innych technologii.

#### Krok 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)  {#step1d}

**Wymóg metodologiczny 1.d {#req1d} :** Określ wszelkie dodatkowe wymagania dotyczące oceny uzgodnione przez [oceniającego](#evaluator) i [zlecającego ocenę](#commissioner) (opcjonalnie).

Zlecający ocenę może być zainteresowany dodatkowymi informacjami wykraczającymi poza to, co jest potrzebne do oceny stopnia zgodności ocenianej witryny z WCAG 2.0. Na przykład, zlecający może być zainteresowany:

-   oceną dodatkowych stron internetowych wykraczających poza to, co jest potrzebne do utworzenia reprezentatywnej próbki stron;
-   raportami o wszystkich wystąpieniach problemów zamiast reprezentatywnych przykładów typów problemów;
-   analizą konkretnych przypadków użycia, sytuacji i grup użytkowników w interakcjach z ocenianą witryną;
-   propozycjami i opisami rozwiązań innych napotkanych problemów, nieobjętych zakresem oceny;
-   oceną dokonaną przez użytkowników z niepełnosprawnościami;
-   sporządzeniem określonej dokumentacji lub stosowaniem konkretnych szablonów raportowania.

Takie dodatkowe wymagania dotyczące oceny, które zostały uzgodnione z oceniającym, muszą zostać wyjaśnione na wczesnym etapie i udokumentowane. Należy je również odzwierciedlić w raporcie wynikowym, na przykład w celu wyjaśnienia, w jaki sposób dokonano wyboru próbki do audytu.

### Krok 2: Poznaj ocenianą witrynę   {#step2}

**Wymóg metodologiczny 2 {#req2} :** Zapoznaj się z witryną internetową, która ma być oceniana zgodnie z [wymogiem metodologicznym 2.a](#req2a), [wymogiem metodologicznym 2.b](#req2b), [wymogiem metodologicznym 2.c](#req2c), [wymogiem metodologicznym 2.d](#req2d) oraz [wymogiem metodologicznym 2.e](#req2e).

Na tym etapie oceniający przegląda witrynę, która ma zostać poddana ocenie, aby się z nią zapoznać, zrozumieć jej cel, przeznaczenie, organizację treści, funkcjonalności. Te istotne aspekty witryny niekoniecznie są od razu widoczne dla oceniających, w szczególności dla osób spoza zespołu programistów. Niekiedy podczas tego wstępnego przeglądu nie będzie też możliwe wyczerpujące określenie i zestawienie wszystkich funkcjonalności, typów stron internetowych i technologii wykorzystywanych do realizacji witryny internetowej i jej aplikacji.  Analiza wstępna przeprowadzona na tym etapie jest zwykle dopracowywana w późniejszym krokach - [kroku 3: Wybierz reprezentatywną próbkę](#step3) i [kroku 4: Audyt wybranej próbki](#step4), w miarę jak oceniający dowiaduje się więcej na temat ocenianej witryny. Zaangażowanie właścicieli i twórców witryny internetowej może pomóc oceniającym w zwiększeniu skuteczność ich badań.

**Uwaga:** Przeprowadzenie wstępnych pobieżnych testów podczas tego kroku pomaga zidentyfikować strony internetowe, które później będą  istotne dla bardziej szczegółowej oceny. Na przykład, oceniający może zidentyfikować strony, które wydają się być pozbawione kontrastu kolorów, strony z zaburzoną strukturą dokumentu lub niespójną nawigacją.

**Uwaga:** Aby wykonać ten krok, konieczne jest, aby oceniający miał dostęp do wszystkich istotnych części witryny.   Na przykład, konieczne może być utworzenie kont lub zapewnienie w inny sposób dostępu do zastrzeżonych obszarów witryny internetowej, które są częścią oceny. Zapewnienie oceniającym takiego dostępu może wymagać szczególnych środków ostrożności w zakresie bezpieczeństwa i ochrony prywatności.

#### Krok 2.a: Rozpoznaj wspólne strony witryny  {#step2a}

**Wymóg metodologiczny 2.a {#req2a} :** Określ [strony wspólne](#common) dla całej ocenianej witryny (mogą to być także stany stron internetowych).

Zbadaj ocenianą witrynę internetową, aby zidentyfikować wszystkie strony wspólne dla całej witryny. W aplikacjach internetowych mogą to być również stany stron internetowych. Zazwyczaj są one linkowane bezpośrednio z głównego punktu wejścia (strony głównej) ocenianej witryny i często połączone z nagłówkiem, nawigacją i sekcją innych stron internetowych. Wynikiem tego kroku jest lista wszystkich [wspólnych stron](#common) internetowych ocenianej witryny.

#### Krok 2.b: Rozpoznaj podstawowe funkcjonalności witryny   {#step2b}

**Wymóg metodologiczny 2.b {#req2b} :** Określ wstępną listę [podstawowych funkcjonalności](#functionality) ocenianej witryny internetowej.

Przejrzyj ocenianą witrynę internetową, aby rozpoznać jej podstawowe funkcjonalności. Niektóre funkcjonalności będą łatwe do zidentyfikowania, inne będą wymagały bardziej celowego odkrywania.  Na przykład, łatwiejsze może być znalezienie funkcjonalności zakupu produktów w sklepie internetowym niż funkcjonalności przewidzianej dla sprzedawców do sprzedaży produktów za pomocą sklepu. Wynikiem tego kroku jest lista funkcjonalności, które użytkownicy mogą wykonywać w witrynie. Lista ta zostanie wykorzystana w kolejnych krokach, aby pomóc wybrać do oceny reprezentatywne przypadki stron internetowych.

**Uwaga:** Celem tego kroku nie jest wyczerpująca lista wszystkich funkcjonalności witryny internetowej, ale określenie tych, które są niezbędne do osiągnięcia celu ocenianej witryny.  Będzie to miało wpływ na późniejszy wybór stron internetowych i ich ocenę. Inne funkcjonalności również zostaną uwzględnione w ocenie, ale na skutek innych mechanizmów selekcji.

##### Przykłady funkcjonalności witryny internetowej  {#example_functionality}

Niektóre przykłady funkcjonalności witryny obejmują:

-   wybór i zakup produktów w sklepie internetowym;
-   wypełnianie i przesyłanie formularzy kontaktowych;
-   rejestracja konta użytkownika w witrynie.

#### Krok 2.c: Rozpoznaj różne typy stron   {#step2c}

**Wymóg metodologiczny 2.c {#req2c} :** Rozpoznaj wszystkie _typy_ stron internetowych i stany stron internetowych.

Strony internetowe i ich stany o różnych stylach, układach, strukturach i funkcjonalnościach często mają różną obsługę w zakresie dostępności. Są one często generowane przez różne szablony i skrypty lub zostały stworzone przez różne osoby. Mogą wyglądać inaczej, zachowywać się inaczej i zawierać różne treści w zależności od konkretnego użytkownika witryny i kontekstu.

Na tym etapie oceniający bada ocenianą witrynę internetową, aby odkryć różne **typy** stron internetowych i stany stron internetowych. Wynikiem tego kroku jest lista opisująca rozpoznane typy treści, a nie konkretnych wystąpień stron internetowych i stanów stron internetowych. Lista ta zostanie wykorzystana w kolejnych krokach, aby pomóc wybrać do oceny reprezentatywne przypadki stron internetowych.

##### Przykłady typów stron internetowych  {#example_types}

Oto kilka przykładów różnych typów stron i stanów stron internetowych, których mogą szukać oceniający:

-   … z różnymi stylami, układem, strukturą, nawigacją, interakcją i wyglądem;
-   z różnymi rodzajami treści, takimi jak formularze, tabele, listy, nagłówki, multimedia i skrypty;
-   z różnymi elementami funkcjonalnymi, takimi jak selektor dat, lightbox, suwak i inne;
-   wykorzystujące różne technologie, takie jak <acronym title="Hypertext Markup Language"> (HTML)</acronym>, <acronym title="Cascading Style Sheets"> (CSS)</acronym>, JavaScript, <acronym title="Accessible Rich Internet Applications"> (WAI-ARIA)</acronym>, <acronym title="Portable Document Format"></acronym> (PDF) itp.; 
-   z różnych obszarów witryny (strona główna, sklep internetowy, działy itp.), w tym wszelkie aplikacje;
-   z różnymi stylami kodowania i utworzonymi przy użyciu różnych [szablonów](#template) (jeśli jest to znane oceniającemu);
-   autorstwa różnych osób, działów i innych podmiotów (jeśli jest to znane oceniającemu)
-   które zmieniają wygląd i zachowanie w zależności od użytkownika, urządzenia, przeglądarki, kontekstu i ustawień;
-   z  treścią dynamiczną, komunikatami o błędach, oknami dialogowymi, wyskakującymi oknami i innymi interakcjami.

#### Krok 2.d: Rozpoznaj zaufane technologie internetowe   {#step2d}

**Wymóg metodologiczny 2.d {#req2d} :** Rozpoznaj [zaufane](#relied) technologie internetowe, użyte do tworzenia treści witryny.

Na tym etapie identyfikowane są technologie internetowe, które muszą być obsługiwane, aby treść spełniała wymogi zgodności. Obejmuje to podstawowe technologie internetowe, takie jak <acronym title="Hypertext Markup Language">HTML</acronym> i <acronym title="Cascading Style Sheets">CSS</acronym>, pomocnicze technologie internetowe, takie jak JavaScript i <acronym title="Accessible Rich Internet Applications">WAI-ARIA</acronym>, a także specyficzne technologie internetowe, takie jak <acronym title="Synchronized Multimedia Integration Language"></acronym>SMIL, <acronym title="Scalable Vector Graphics"></acronym>SVG i <acronym title="Portable Document Format"></acronym>PDF. Wynikiem tego kroku jest lista zaufanych technologii internetowych użytych do tworzenia treści witryny [zgodnie](http://www.w3.org/TR/WCAG20/#reliedupondef) z [WCAG 2.0](http://www.w3.org/TR/WCAG20/#reliedupondef). Lista ta posłuży w następnych krokach do wyboru reprezentatywnej próbki stron.

**Uwaga:** Tam, gdzie to możliwe, często przydatne jest również zidentyfikowanie wersji i konfiguracji użytego systemu zarządzania treścią, ponieważ może to być istotne dla wyjaśnienia wyników oceny. Istotne mogą być również wszelkie biblioteki i komponenty użyte do utworzenia witryny internetowej, takie jak Dojo, jQuery i inne.  Zwłaszcza w przypadku aplikacji internetowych znaczna część obsługi dostępności jest wbudowana w biblioteki i komponenty, a ocena może stać się bardziej efektywna i wydajna, gdy zostaną  zidentyfikowane.

#### Krok 2.e: Rozpoznaj inne istotne strony witryny   {#step2e}

**Wymóg metodologiczny 2.e {#req2e} :** Zidentyfikuj inne strony i stany stron internetowych, które są istotne dla osób z niepełnosprawnościami i dla dostępności witryny.

Niektóre witryny zawierają specjalne strony i stany stron internetowych, które są szczególnie istotne dla osób z niepełnosprawnościami i dla dostępności witryny.  Wynikiem tego kroku jest lista takich stron i stanów stron internetowych, jeśli nie zostały one jeszcze zidentyfikowane w ramach [Kroku 2.a: Rozpoznaj wspólne strony witryny](#step2a).

##### Przykłady innych istotnych stron internetowych  {#example_relevant}

Przykłady innych odpowiednich stron internetowych i stanów stron internetowych obejmują te:

-   … z objaśnieniami cech dostępności witryny;
-   … z pomocą w zakresie korzystania z witryny;
-   … z objaśnieniami ustawień, preferencji, opcji, skrótów itp.;
-   … z danymi kontaktowymi, wskazówkami i instrukcjami pomocy technicznej..

### Krok 3: Wybór reprezentatywnej próbki   {#step3}

**Wymóg metodologiczny 3 {#req3} :** Wybierz reprezentatywną próbkę stron internetowych z witryny zgodnie z [wymogiem metodologicznym 3.a](#req3a), [wymogiem metodologicznym 3.b](#req3b) oraz [wymogiem metodologicznym 3.c](#req3c).

Na tym etapie oceniający wybiera próbkę stron internetowych i stanów stron internetowych, która jest reprezentatywna dla ocenianej witryny internetowej. Celem tego wyboru jest zapewnienie, że wyniki oceny z rozsądną pewnością będą odzwierciedlać dostępność witryny. W przypadkach, gdy możliwe jest dokonanie oceny wszystkich stron i stanów stron internetowych witryny internetowej, co jest wysoce zalecane, procedura wyboru próbki stron może zostać pominięta. W tych przypadkach „wybraną próbką” w pozostałych etapach procesu oceny jest cała witryna.  W niektórych przypadkach, np. w przypadku małych witryn, procedura próbkowania może skutkować wyborem wszystkich stron i stanów stron internetowych.

Rzeczywista wielkość próbki stron internetowych i stanów stron internetowych potrzebnych do oceny witryny internetowej zależy od wielu czynników, w tym:

-   **Rozmiar witryny** - witryny z większą liczbą stron internetowych zazwyczaj wymagają większej próbki do oceny.
-   **Wiek witryny** - starsze witryny mają zazwyczaj więcej treści (często niełatwych do znalezienia) o różnym stopniu złożoności, spójności oraz procesach projektowania i tworzenia, dlatego do oceny zwykle wymagana jest większa próbka.
-   **Złożoność witryny** - większa złożoność wymaga większej próby do oceny; należy rozważyć następujące kwestie:
    -   **Jak interaktywna jest treść** - witryny z treścią bogatą w interakcje wymagają większych próbek, aby uwzględnić funkcjonalności zapewniane przez strony internetowe i różne stany stron;
    -   **Jak generowana jest treść** - witryny zawierające treści agregowane z różnych źródeł lub treści przetwarzane w miarę ich wyświetlania zazwyczaj wymagają większych próbek, aby uwzględnić kombinacje treści, które mogą być generowane;
    -   **Jak treść została wdrożona** - witryny dostępne w różnych wersjach, są obsługiwane zgodnie z użytkownikami i ich preferencjami lub przystosowują się do urządzeń dostępowych, wymagają większych próbek, aby uwzględnić te różne sytuacje.
-   **Spójność witryny** - niższa spójność wymaga większej próby do oceny; rozważ następujące kwestie:
    -   **Różnorodność typów stron internetowych** - witryny z szerszą gamą typów stron internetowych (zobacz [Krok 2.c: Rozpoznaj różne typy stron internetowych](#step2c)) wymagają większych próbek do oceny
    -   **Różnorodność funkcjonalności** - witryny oferujące szerszą gamę funkcjonalności (zobacz [Krok 2.b: Rozpoznaj podstawowe funkcjonalności witryny](#step2b)), w szczególności różne typy aplikacji, wymagają do oceny większych próbek
    -   **Różnorodność technologii** - witryny z szerszą gamą używanych technologii internetowych (zobacz [Krok 2.d: Rozpoznaj zaufane technologie internetowe](#step2d)) wymagają większych próbek do oceny
    -   **Różnorodność stylów kodowania** - witryny z szerszą gamą stylów kodowania (zazwyczaj są to różne skrypty, które generują kod, szablony, obszary pochodzące od różnych autorów stron internetowych) wymagają większych próbek do oceny.
-   **Przestrzeganie procedur projektowych** - nieprzestrzeganie wymaga większej próbki do oceny; rozważ następujące kwestie:
    -   **Sformalizowanie procesu** - witryny ze sformalizowanymi procesami rozwoju i zapewniania jakości wykazują większą spójność w kodowaniu i jakości stron internetowych, dlatego zwykle wymagają mniejszych próbek do oceny;
    -   **Dokształcanie programistów** - witryny z projektantami, programistami i autorami treści, którzy przechodzą regularne szkolenia, mają tendencję do bardziej spójnego działania w zakresie dostępności, dlatego zwykle wymagają mniejszych próbek do oceny;
    -   **Wykorzystywane narzędzia programistyczne** - witryny opracowywane i utrzymywane przy użyciu spójnego zestawu narzędzi, takich jak system zarządzania treścią (CMS), są również bardziej spójne i wymagają mniejszych próbek do oceny;
    -   **Liczba autorów stron internetowych** - witryny tworzone i utrzymywane przez bardziej ograniczony zestaw autorów stron internetowych, w tym redaktorów treści, wydają się być bardziej spójne i wymagają mniejszych próbek do oceny.
-   **Wymagany poziom wiarygodności oceny** - większe wymagane zaufanie do wyników oceny często wymaga oceny większej próbki.
-   **Dostępność wcześniejszych wyników oceny** - gdy osoby oceniające mają dostęp do wcześniejszych wyników oceny, w tym wyników testów z ręcznego i automatycznego testowania dostępności, mogą być wymagane mniejsze próbki.

Wybór dokonany podczas tego kroku opiera się początkowo na eksploracji przeprowadzonej w [kroku 2: Poznaj ocenianą witrynę](#step2). Wybór jest również stale udoskonalany podczas kolejnego [Kroku 4: Audyt wybranej próbki](#step4), w miarę jak oceniający dowiadują się więcej o poszczególnych aspektach ocenianej witryny.

#### Krok 3.a: Uwzględnij próbkę strukturalną  {#step1a}

**Wymóg metodologiczny 3.a {#req3a} :** Wybierz strony internetowe i stany stron internetowych, które odzwierciedlają wszystkie zidentyfikowane (1) [wspólne strony internetowe](#common), (2) [podstawowe funkcjonalności](#functionality), (3) typy stron internetowych, (4) zaufane technologie internetowe oraz (5) inne istotne strony internetowe.

Wybierz próbkę stron internetowych i stanów stron internetowych, które zawierają:

1.  Wszystkie wspólne strony i stany stron internetowych, które zostały zidentyfikowane w [Kroku 2.a: Rozpoznaj wspólne strony witryny](#step2a):
2.  Wszystkie inne istotne strony i stany stron internetowych, które zostały zidentyfikowane w [Kroku 2.e: Zidentyfikuj inne istotne strony internetowe](#step2e);
3.  Jeśli nie zostało to odzwierciedlone w poprzednich punktach, wybierz dodatkowe strony i stany stron za pomocą:
    1.  Treść z każdą niezbędną funkcjonalnością określoną w [Kroku 2.b: Rozpoznaj podstawowe funkcjonalności witryny](#step2b);
    2.  Treść z różnymi typami stron internetowych zidentyfikowanych w [Krok 2.c: Rozpoznaj różne typy stron internetowych](#step2c);
    3.  Treści dostarczane przy użyciu technologii internetowych określonych w [Krok 2.d: Rozpoznaj zaufane technologie internetowe](#step2d).

**Uwaga:** Pojedyncza strona lub stan strony internetowej może odzwierciedlać więcej niż jedno z powyższych kryteriów. Na przykład pojedyncza strona internetowa może być reprezentatywna dla określonego układu projektu, funkcjonalności i zastosowanych technologii internetowych.  Celem tego kroku jest zapewnienie reprezentatywnej próbki różnych typów stron i stanów stron, funkcjonalności i technologii internetowych występujących w witrynie.  Staranny dobór tych reprezentatywnych wystąpień może znacznie zmniejszyć wymaganą wielkość próbki przy zachowaniu odpowiedniej reprezentacji całej witryny. Liczba wymaganych wystąpień stron internetowych i ich stanów zależy od konkretnych aspektów strony internetowej wyjaśnionych w poprzedniej sekcji, [czynników wpływających na wielkość próby](#sample).

#### Krok 3.b: Uwzględnij próbkę losową  {#step1a}

**Wymóg metodologiczny 3.b {#req3b} :** Wybierz losową próbkę stron i stanów stron internetowych i włącz je do audytu.

Losowo wybrana próbka stron internetowych i stanów stron internetowych służy jako wskaźnik pozwalający sprawdzić, czy próbka strukturalna wybrana w poprzednich krokach jest wystarczająco reprezentatywna dla treści zamieszczonych na stronie internetowej.  Zaufanie do ogólnego wyniku oceny wzrasta, gdy wyniki oceny obu metod selekcji są ze sobą skorelowane.

Liczba stron internetowych i stanów stron internetowych, które należy losowo wybrać, wynosi **10% próbki strukturalnej** wybranej w poprzednich krokach. Na przykład, jeśli próbka strukturalna wybrana dla strony internetowej dała 80 stron i stanów stron internetowych, wówczas wielkość próbki losowej wynosi 8 stron i stanów stron internetowych. (Uwaga: wielkość próbki strukturalnej jest inna niż wielkość witryny.)

Aby dokonać tego wyboru, losowo wybierz unikalne wystąpienia stron i stanów stron internetowych z ocenianej witryny, które nie są jeszcze częścią próbki strukturalnej uzyskanej w poprzednich krokach. W zależności od rodzaju strony internetowej i dostępu, jaki ma do niej oceniający, do tego wyboru można zastosować różne techniki. Między innymi:

-   skorzystanie z narzędzia, które przejdzie przez witrynę i zaproponuje listę losowo wybranych stron i stanów stron internetowych;
-   skorzystanie ze skryptu, który wygeneruje listę wszystkich stron i stanów stron internetowych w witrynie, do wyboru;
-   skorzystanie z dzienników serwera, wyszukiwarek i innych metod dotarcia do losowo wybranej próbki.

Udokumentuj strony i stany stron internetowych, które zostały losowo wybrane, ponieważ będą musiały zostać porównane z pozostałą próbką strukturalną w [Kroku 4.c: Porównaj próbki strukturalną i losową](#step4c).

**Uwaga:** Chociaż próbka losowa nie musi być wybierana według kryteriów ściśle naukowych, to zakres wyboru musi obejmować cały zakres witryny internetowej (można wybrać dowolną stronę i dowolny stanu strony w witrynie), a wybór poszczególnych stron i stanów stron internetowych nie powinien następować według przewidywalnego wzorca. Rejestracja metody zastosowanej do wygenerowania próbki losowej jest ważna dla powtarzalności i wiarygodności wyników.

#### Krok 3.c: Uwzględnij całe procedury  {#step1a}

**Wymóg metodologiczny 3.c {#req3c} :** Uwzględnij w próbce wszystkie strony i stany stron internetowych, które są częścią [całych procedur](#complete).

Wybrana próbka musi obejmować wszystkie strony i stany stron, które należą do serii stron prezentujących każdą procedurę. Żadna strona internetowa ani stan strony internetowej w wybranej próbce nie może być częścią procedury, chyba że w wybranej próbce uwzględnione są wszystkie inne strony internetowe i stany stron internetowych, które są częścią tej procedury.

Wykonaj poniższe kroki, aby włączyć do próbki niezbędne strony i stany stron:

1.  Wykonaj poniższe kroki, aby włączyć do próbki niezbędne strony i stany stron w [kroku 3.a: Uwzględnij próbkę strukturalną](#step3a) i [kroku 3.b: Uwzględnij próbkę losową](#step3b), która jest częścią procedury, znajdź punkt początkowy (stronę internetową lub stan strony internetowej) dla procedury i uwzględnij go w wybranej próbce;
2.  Dla każdego punktu początkowego procedury określ i zapisz co najmniej domyślną sekwencję stron i stanów stron internetowych niezbędnych, aby zakończyć procedurę. Dodaj te strony i stany stron do wybranej próbki.  
    **Uwaga:** Domyślna sekwencja jest zgodna ze standardowym przypadkiem użycia, opisującym domyślną ścieżkę przez całą procedurę. Zakłada się, że nie ma błędów wprowadzania danych przez użytkownika ani wyboru dodatkowych opcji. Na przykład w przypadku aplikacji sklepu internetowego użytkownik przejdzie do kasy, potwierdzi domyślną opcję płatności, poprawnie poda wszystkie wymagane szczegóły płatności i dokona zakupu bez zmiany zawartości koszyka, korzystając z zapisanego profilu użytkownika, wybierając alternatywne opcje płatności lub adresu wysyłki, podając błędne dane wejściowe itd.
3.  Dla każdej procedury rozpoznaj i zanotuj sekwencje rozgałęzień stron internetowych i stany stron internetowych, do których często uzyskiwany jest dostęp i które mają kluczowe znaczenie dla pomyślnego ukończenia procesdury. Dodaj te strony i stany stron do wybranej próbki.  
    **Uwaga:** Sekwencje rozgałęzień mogą się kończyć tam, gdzie ponownie wchodzą do domyślnej gałęzi procesu. Na przykład dodanie nowego adresu wysyłki zostanie zarejestrowane jako kluczowa gałąź alternatywna, która prowadzi z powrotem do domyślnej gałęzi procedury.

**Uwaga:** W większości przypadków konieczne jest rejestrowanie i określenie działań niezbędnych do przejścia z jednej strony i stanu strony internetowej do następnej w kolejności, aby zakończyć proces, tak aby można je było później powielić. Przykładem takiej akcji może być „Wpisz nazwę i adres oraz wybierz przycisk Wyślij”.  W większości przypadków adres internetowy (<acronym title="Uniwersalnych Identyfikatorów Zasobu">URI</acronym>) nie będzie wystarczający do zidentyfikowania strony internetowej i stanu strony internetowej w całym procesie. Przydatne jest również wyraźne zapisywanie, kiedy strony i stany stron internetowych są częścią procesu, tak aby osoby oceniające mogły skupić swoje wysiłki na istotnych zmianach, takich jak elementy, które zostały dodane, zmodyfikowane lub uwidocznione.

### Krok 4: Wykonaj audyt wybranej próbki   {#step4}

**Wymóg metodologiczny 4 {#req4} :** Wykonaj audyt wybranej próbki stron internetowych zgodnie z [wymogiem metodologicznym 4.a](#req4a), [wymogiem metodologicznym 4.b](#req4b) oraz [wymogiem metodologicznym 4.c](#req4c).

Podczas tego kroku oceniający przeprowadza szczegółową ocenę wszystkich stron i stanów stron internetowych wybranych w [Kroku 3: Wybierz reprezentatywną próbkę](#step3) i porównuje wyniki oceny próbki strukturalnej z wynikami oceny próbki wybranej losowo. Audyt jest przeprowadzany zgodnie z pięcioma [wymogami zgodności](http://www.w3.org/TR/WCAG20/#conformance-reqs) WCAG 2.0 na poziomie zgodności ustalonym w [Kroku 1.b: Określ wymagany poziom zgodności](#step1b).

Pięć wymagań zgodności z WCAG 2.0 to:

1.  [Poziom zgodności](http://www.w3.org/TR/WCAG20/#cc1)
2.  [Całe strony](http://www.w3.org/TR/WCAG20/#cc2)
3.  [Całe procedury](http://www.w3.org/TR/WCAG20/#cc3)
4.  [Tylko technologie obsługujące dostępność](http://www.w3.org/TR/WCAG20/#cc4)
5.  [Bez zakłóceń](http://www.w3.org/TR/WCAG20/#cc5)

Wskazówki dotyczące oceny tych wymagań zgodności podano w sekcjach poniżej. Więcej informacji i wskazówek dotyczących wymagań zgodności WCAG 2.0 znajduje się w opracowaniach [WCAG 2.0 Warstwy i wytyczne](http://www.w3.org/TR/WCAG20/#intro-layers-guidance) oraz [Objaśnienie zgodności](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance). Ich prezentacja wykracza poza zakres tego dokumentu.

**Uwaga:** Wykonanie tego kroku wymaga dogłębnego zrozumienia wymagań zgodności WCAG 2.0 i wiedzy specjalistycznej przedstawionej w części [Wymagana wiedza specjalistyczna](#expertise).

#### Krok 4.a: Sprawdź wszystkie strony początkowe  {#step1a}

**Wymóg metodologiczny 4.a {:#req4a} :** Sprawdź, czy każda strona internetowa lub stan strony w wybranej próbce, które nie są częścią żadnej procedury, jest zgodna z każdym z pięciu wymagań zgodności WCAG 2.0 na wymaganym poziomie zgodności.

Dla każdej strony i stanu strony internetowej w próbce wybranej w [Kroku 3: Wybierz reprezentatywną próbkę](#step3), która nie znajduje się w obrębie lub na końcu całej procedury, sprawdź jej zgodność z każdym z pięciu wymagań zgodności WCAG 2.0, z wymaganym poziomem zgodności ustalonym w [Kroku 1.b: Określ wymagany poziom zgodności](#step1b). Obejmuje to wszystkie elementy strony internetowej lub stanu strony internetowej bez aktywowania jakichkolwiek funkcji, wprowadzania jakichkolwiek danych lub inicjowania procesu w inny sposób. Taka funkcjonalność i interakcja, w tym strony i stany stron internetowych, które znajdują się w obrębie lub na końcu całego procesu, będą oceniane w kolejnym etapie.

**Uwaga:** Wiele stron i stanów stron internetowych w próbce będzie zawierało takie elementy, jak nagłówek, paski nawigacyjne, formularz wyszukiwania i inne, które występują wielokrotnie. Chociaż wymaganiem jest sprawdzenie [całych stron](http://www.w3.org/TR/WCAG20/#cc2), zazwyczaj te elementy nie muszą być poddawane ponownej ocenie przy każdym wystąpieniu, chyba że pojawiają się lub zachowują inaczej, lub gdy w [Kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#step1d) zostały określone dodatkowe wymagania oceny.

##### Kryteria sukcesu WCAG 2.0  {#success-criteria}

Zazwyczaj istnieje kilka sposobów ustalenia, czy kryteria sukcesu WCAG 2.0 zostały spełnione, czy też nie. WAI W3C zapewnia (nienormatywny) zestaw [Technik dla WCAG 2.0](http://www.w3.org/TR/WCAG20-TECHS/), który dokumentuje wystarczające i dodatkowe sposoby spełnienia określonych kryteriów sukcesu WCAG 2.0. W zestawie tym udokumentowano również _typowe błędy_, które opisują znane sposoby prezentacji treści, niespełniające określonych kryteriów sukcesu WCAG 2.0. Więcej wskazówek na temat koncepcji _technik_ WCAG 2.0 znajduje się w opracowaniu [Objaśnienie technik dla kryteriów sukcesu](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques) WCAG.

Oceniający mogą skorzystać z tych udokumentowanych wskazówek, aby sprawdzić, czy dana treść internetowa spełnia lub nie spełnia kryteriów sukcesu WCAG 2.0. Udokumentowane techniki i błędy mogą być również użytecznym elementem raportów z oceny. Nie jest jednak wymagane stosowanie konkretnego zestawu technik i błędów udokumentowanych przez  WAI W3C. W gruncie rzeczy osoby oceniające wcale nie muszą odwoływać się do technik i błędów. Oceniający mogą zastosować inne podejścia, aby ocenić, czy kryteria sukcesu WCAG 2.0 zostały spełnione, czy też nie. Na przykład oceniający mogą wykorzystywać określone instrukcje i protokoły testowe, które spełniają [wymagania dotyczące technik wystarczających](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques.html#ut-understanding-techniques-sufficient-head) i które mogą być publicznie udokumentowane lub dostępne wyłącznie dla osób oceniających. Więcej wskazówek na temat korzystania z technik znajduje się w poprzednio przywołanym opracowaniu [Objaśnienie technik dla kryteriów sukcesu WCAG](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques).

**Uwaga:** Kryteria sukcesu WCAG 2.0 są sformułowane jako „_testowalne stwierdzenia, które są prawdziwe lub fałszywe, gdy zostaną zastosowane do określonej treści WWW_”. Jeśli użytkownikowi nie jest prezentowana żadna treść odnosząca się do konkretnego kryterium sukcesu (na przykład w witrynie nie ma wideo), wówczas zgodnie z WCAG 2.0.kryteria sukcesu są „spełnione”. Opcjonalnie w raporcie z oceny można wskazać konkretne kryteria sukcesu, które pominięto dlatego, że w witrynie nie ma podlegających im treści. W opracowaniu [Objaśnienie zgodności](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html) znajduje się więcej informacji i wskazówek.

##### Zgodne wersje alternatywne  {#alternate-versions}

Treść strony internetowej lub stanu strony internetowej może mieć wersje alternatywne. Na przykład treści wideo mogą być dostarczane w wersji z napisami i bez nich. W niektórych przypadkach cała strona internetowa lub stan strony internetowej (lub ich seria) może być zapewniona jako zgodna wersja alternatywna do strony lub stanu strony internetowej. Zgodność z WCAG 2.0 można osiągnąć za pomocą wersji alternatywnych, które spełniają wymagania [zgodności wersji alternatywnej](http://www.w3.org/TR/WCAG20/#conforming-alternate-versiondef) wymienione w definicji WCAG. Na przykład, strona internetowa z treścią wideo bez podpisów może nadal spełniać wymagania WCAG 2.0, jeśli zapewniono alternatywną wersję wideo, która kwalifikuje się jako _zgodna wersja alternatywna_. Więcej informacji i wskazówek dotyczących zgodności wersji alternatywnej, które wykraczają poza zakres niniejszego dokumentu, znajduje się w opracowaniu [Objaśnienie zgodnych wersji alternatywnych](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conforming-alt-versions-head).

**Uwaga:** Wersje alternatywne nie są uważane za osobne strony internetowe ani stany stron internetowych, ale za część ich treści. Strony i stany stron internetowych są oceniane razem z ich zgodnymi wersjami alternatywnymi jako jedna jednostka [(cała strona](http://www.w3.org/TR/WCAG20/#cc2)).

##### Obsługa dostępności  {#accessibility-support}

Treść strony internetowej lub stanu strony internetowej musi być dostarczona w sposób, który jest _obsługiwany pod względem dostępności_ (bezpośrednio lub poprzez zgodną wersję alternatywną). Na przykład, napisy rozszerzone do filmu muszą być zapewnione w taki sposób, aby mogły być wyświetlane użytkownikom. Definicja [obsługiwanej dostępności](http://www.w3.org/TR/WCAG20/#accessibility-supporteddef) WCAG 2 określa konkretne szczegółowe wymagania dotyczące korzystania z [technologii tworzenia treści internetowych](http://www.w3.org/TR/WCAG20/#technologydef), aby zakwalifikować je jako obsługiwane pod względem dostępności. Więcej wskazówek dotyczących obsługi dostępności, a wykraczających poza zakres niniejszego dokumentu, znajduje się w opracowaniu [Understanding Accessibility-Supported Web Technology Uses](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-documented-lists-head). WCAG 2.0 nie definiuje jednak konkretnego progu ani zestawu oprogramowania, które witryna musi obsługiwać w celu zapewnienia dostępności. Definicja takiego poziomu bazowego zależy od kilku parametrów, w tym celu, odbiorców i języka witryny. Poziom bazowy używany do oceny konkretnej witryny strony jest zdefiniowany w [Kroku 1.c: Określ bazowy poziom obsługi dostępności](#step1c).

##### Bez zakłóceń  {#non-interference}

Treść strony lub stanu strony internetowej może nie być zgodna z WCAG 2, nawet jeśli strona lub stan strony internetowej jako całość będzie zgodna z WCAG 2.0 (a raczej mogłaby być zgodna). Na przykład informacje i funkcjonalności mogą być zapewnione za pomocą [technologii treści internetowych](http://www.w3.org/TR/WCAG20/#technologydef), które nie są jeszcze szeroko wspierane przez technologie wspomagające lub w sposób, który nie jest obsługiwany przez technologie wspomagające, wraz z odpowiadającą im alternatywną wersją dla informacji i funkcjonalności obsługiwanych przez dostępność. W takim przypadku treść niezgodna nie może negatywnie wpływać na treść zgodną, aby strona lub stan strony internetowej odpowiadały wymogom zgodności z WCAG 2.0. Wymóg zgodności WCAG 2.0 dotyczący [braku zakłóceń](http://www.w3.org/TR/WCAG20/#cc5) określa szczegółowe wymagania dla treści, aby zakwalifikować się jako niezakłócającą. Informacje, które wykraczają poza zakres tego dokumentu, dotyczące braku zakłóceń, znajdują się w opracowaniu [Objaśnienia wymagania zgodności 5](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance#uc-conf-req5-head).

#### Krok 4.b: Sprawdź wszystkie całe procesy  {#step1a}

**Wymóg metodologiczny 4.b {:#req4b} :** Sprawdź, czy wszystkie interakcje dla każdej strony i stanu strony internetowej w [całej procedurze](http://www.w3.org/TR/WCAG20/#cc3) są zgodne z każdym z pięciu wymagań zgodności WCAG 2.0 na wymaganym poziomie zgodności.

Dla każdej całej procedury określonej w [Kroku 3.c: Uwzględnij całe procedury](#step3c), postępuj zgodnie ze wskazanymi domyślnymi i rozgałęzionymi sekwencjami stron i stanów stron internetowych i oceń każdy zgodnie z [krokiem 4.a: Sprawdź wszystkie strony początkowe](#step4a). Jednak w tym przypadku nie jest konieczna ocena wszystkich treści, a jedynie treści, które zmieniają się w trakcie procesu.

Poddaj ocenie funkcjonalność, wprowadzanie danych, powiadomienia i inne interakcje. W szczególności sprawdzanie powinno objąć:

-   Interakcję z formularzami, polami danych, przyciskami, oknami dialogowymi i innymi składnikami strony internetowej;
-   Potwierdzenia wprowadzenia danych, komunikaty o błędach i innych informacje zwrotne;
-   Zachowanie po zastosowaniu różnych ustawień, preferencji, urządzeń i parametrów interakcji.

#### Krok 4.c: Porównaj próbki strukturalną i losową  {#step1a}

**Wymóg metodologiczny 4.c {#req4c} :** Sprawdź, czy żadna strona i żaden stan strony internetowej w próbce wybranej losowo nie pokazuje innych typów treści i wyników, niż typy treści i wyniki w próbce strukturalnej.

Chociaż poszczególne wystąpienia kryteriów sukcesu WCAG 2.0 będą się różnić pomiędzy próbkami strukturalnymi i losowo wybranymi, losowo wybrana próbka nie powinna pokazywać nowych _typów_ treści, które nie występują w próbie strukturalnej. Również wyniki oceny próbki wybranej losowo nie powinny pokazywać nowych ustaleń w stosunku do wyników oceny próby strukturalnej. Jeśli losowo wybrana próbka zawiera nowe typy treści lub nowe ustalenia z oceny, oznacza to, że próbka strukturalna nie była wystarczająco reprezentatywna dla treści zamieszczonych w witrynie. W takim przypadku oceniający muszą wrócić do [Kroku 3: Wybierz reprezentatywną próbkę](#step3), aby wybrać dodatkowe strony internetowe i stany stron internetowych, które odzwierciedlają nowo zidentyfikowane typy treści i ustalenia. Również ustalenia z [Kroku 2: Poznaj ocenianą witrynę](#step2) mogą wymagać odpowiedniego dostosowania. Ten krok powtarza się, dopóki próbka strukturalna nie będzie odpowiednio reprezentatywna dla treści dostarczanych w witrynie

### Krok 5: Sporządź raport z oceny  {#step5}

**Wymóg metodologiczny 5 {#req5} :** Przedstaw wyniki oceny zgodnie z [wymogiem metodologicznym 5.a](#req5a) oraz opcjonalnie z [wymogiem metodologicznym 5.b](#req5b), [wymogiem metodologicznym 5.c](#req5c), [wymogiem metodologicznym 5.d](#req5d) oraz [wymogiem metodologicznym 5.e](#req5e).

Chociaż wyniki oceny są raportowane na koniec procesu, ich dokumentowanie ma miejsce w trakcie całego procesu oceny, aby zapewnić możliwość weryfikacji wyników. Dokumentacja ma zwykle różne poziomy poufności. Na przykład dokumentacja konkretnych metod stosowanych do oceny poszczególnych wymagań może pozostać tajemnicą osoby oceniającej, ale raporty o wynikach tych testów są zwykle udostępniane zlecającemu ocenę. Właściciele stron internetowych mogą ponadto zdecydować się na podanie do publicznej wiadomości informacji o wynikach oceny zgodnie z tą metodologią.

#### Krok 5.a: Udokumentuj wyniki każdego kroku  {#step1a}

**Wymóg metodologiczny 5.a {#req5a} :** Udokumentuj każdy wynik ustaleń dokonanych w [Kroku 1: Ustal zakres oceny](#step1), [Krok 2: Poznaj ocenianą witrynę](#step2), [Krok 3: Wybierz reprezentatywną próbkę](#step3) i [Krok 4: Wykonaj audyt wybranej próbki](#step4).

Dokumentowanie wyników każdego z poprzednich kroków (w tym wszystkich podsekcji) jest niezbędne dla zapewnienia przejrzystości procesu oceny, powtarzalności wyników oceny oraz uzasadnienia wszelkich oświadczeń złożonych na podstawie tej oceny. **Dokumentacja ta nie musi być jawna**, poziom poufności zwykle określa zlecający ocenę.

Dokumentowanie wyników każdego kroku obejmuje co najmniej następujące elementy:

-   **Metryka audytu**
    -   Nazwa osoby/podmiotu [oceniającego](#evaluator)
    -   Nazwa [zlecającego ocenę](#commissioner)
    -   Data przeprowadzenia oceny (data zakończenia lub czas trwania)
-   **Zakres oceny**
    -   Zakres stron witryny określony w [Kroku 1.a: Określ zakres stron witryny](#step1a)
    -   Wymagany poziom zgodności określony w [Kroku 1.b. Określ wymagany poziom zgodności](#step1b)
    -   Zestaw technologii bazowych określony w [Kroku 1.c: Określ bazowy poziom obsługi dostępności](#step1c)
    -   Dodatkowe wymagania, jeżeli istnieją, określone w [kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#step1d)
-   **Wstępne rozpoznanie witryny**
    -   Zaufane technologie internetowe określone w [Kroku 2.d: Rozpoznaj zaufane technologie internetowe](#step2d)
    -   Opcjonalnie: Wspólne strony witryny określone w [Kroku 2.a: Rozpoznaj wspólne strony witryny](#step2a)
    -   Opcjonalnie: Niezbędne funkcjonalności witryny określone w [Kroku 2.b: Rozpoznaj podstawowe funkcjonalności witryny](#step2b)
    -   Opcjonalnie: Różne typy stron określone w [Kroku 2.c: Rozpoznaj różne typy stron witryny](#step2c)
    -   Opcjonalnie: Opcjonalnie: Inne istotne strony określone w [Kroku 2.e: Rozpoznaj inne istotne strony witryny](#step2e)
-   **Reprezentatywna próbka stron**
    -   Strony i stany stron internetowe wybrane w ramach próbkowania strukturalnego w [Kroku 3.a: Uwzględnij próbkę strukturalną](#step3a)
    -   Strony wybrane losowo i metoda wyboru zastosowana w [Kroku 3.b: Uwzględnij próbkę losową](#step3b)
    -   Całe procedury wybrane w [Kroku 3.c: Uwzględnij całe procedury](#step3c)
-   **Audyt wybranej próbki**
    -   Wyniki oceny z [Kroku 4.a: Sprawdź wszystkie strony początkowe](#step4a)
    -   Wyniki oceny z [Kroku 4.b: Sprawdź wszystkie całe procedury](#step4b)
    -   Wyniki oceny z [Kroku 4.c: Porównaj próbki strukturalną i losową](#step4c)

**Uwaga:** W zależności od pożądanej szczegółowości raportu, wyniki [Kroku 4: Wykonaj audyt wybranej próbki](#step4) mogą być dostarczone mogą być dostarczone dla każdej ocenianej strony i stanu strony internetowej lub zagregowane dla całej próbki. Raporty powinny zawierać co najmniej jeden przykład dla każdego wymogu zgodności i kryterium sukcesu WCAG 2, które nie zostało spełnione.  Raporty powinny zawierać co najmniej jeden przykład dla każdego wymogu zgodności i kryterium sukcesu <acronym>WCAG</acronym> 2.0, które nie zostało spełnione.  Dobrą praktyką jest również wskazywanie powtarzających się problemów.

Raporty mogą również zawierać dodatkowe informacje w zależności od dodatkowych wymogów oceny określonych w [Kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#step1d). Na przykład, osoba zlecająca ocenę może poprosić o raport wskazujący każde wystąpienie błędu dla każdej strony i stanu strony internetowej w wybranej próbce, o więcej informacji na temat charakteru i przyczyn wykrytych błędów lub sugestie naprawy w celu usunięcia błędów.

#### Krok 5.b: Zapisz szczegóły oceny (opcjonalnie)  {#step1a}

**Wymóg metodologiczny 5.b {#req5b} :** Zarchiwizuj skontrolowane strony i stany stron internetowych oraz zapisz narzędzia oceny, przeglądarki internetowe, technologie wspomagające, inne oprogramowanie i metody użyte do ich audytu (opcjonalnie).

Chociaż jest to opcjonalne, dobrą praktyką jest, aby oceniający prowadzili rejestr szczegółów oceny, na przykład w celu wsparcia rozwiązywania konfliktów w przypadku sporu. Obejmuje to archiwizację stron internetowych i stanów stron internetowych poddanych audytowi oraz rejestrowanie narzędzi oceny, przeglądarek internetowych, technologii wspomagających, innego oprogramowania i metod wykorzystywanych do ich kontroli. Zapis ten jest zazwyczaj przechowywany wewnętrznie i nie jest udostępniany przez oceniającego, chyba że uzgodniono inaczej w [Kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#step1d).

Zapisy dotyczące specyfikacji oceny mogą obejmować dowolne z poniższych kwestii:

-   Kopie plików i zasobów stron internetowych i stanów stron internetowych;  
    **Uwaga:** Niektóre narzędzia mogą zapisać dynamicznie wygenerowaną lub zmodyfikowaną treść (DOM) wyświetlaną podczas oceny, a nie początkową zawartość plików i zasobów, która często jest inna;
-   Zrzuty ekranu stron internetowych i stanów stron internetowych;
-   Opisy ścieżek do lokalizowania stron i stanów stron internetowych, szczególnie gdy są one częścią procesu;
-   Opis ustawień, wprowadzanych danych i działań służących do generowania stron lub nawigowania do stron i stanów stron internetowych. Specyficzne poświadczenia testowe (identyfikatory użytkownika itp.) wymagane do odtworzenia unikalnego zestawu danych lub przepływu pracy;
-   Nazwy i wersje narzędzi oceny, przeglądarek internetowych i dodatków, technologii wspomagających oraz innego używanego oprogramowania;
-   Metody, procedury i techniki stosowane do oceny zgodności z WCAG 2.0.

Zapis ten może obowiązywać globalnie dla całej oceny, dla poszczególnych stron internetowych lub dla poszczególnych testów przeprowadzanych w ramach sprawdzanych stron i stanów stron internetowych. Do rejestrowania informacji można wykorzystać tabelę lub siatkę.

**Uwaga:** Zapisy dotyczące specyfikacji oceny mogą zawierać poufne informacje, takie jak kod wewnętrzny, hasła i kopie danych. Mogą one wymagać szczególnych środków ostrożności w zakresie bezpieczeństwa i ochrony prywatności.

#### Krok 5.c: Przygotuj oświadczenie o zgodności (opcjonalnie)  {#step1a}

**Wymóg metodologiczny 5.c {#req5c} :** Przygotuj oświadczenie o zgodności (opcjonalnie).

**Przypomnienie:** W większości przypadków samo zastosowanie tej metodologii nie skutkuje [oświadczeniami o zgodności z WCAG 2.0](http://www.w3.org/TR/WCAG20/#conformance-claims) badanych witryn; zobacz [Związek z deklaracjami zgodności z WCAG 2.0](#context), aby uzyskać więcej informacji.

Właściciele witryn mogą chcieć złożyć publiczne oświadczenia na temat wyników ocen przeprowadzonych zgodnie z tą metodologią. Można to zrobić, gdy spełnione są co najmniej wszystkie nieopcjonalne wymagania metodologiczne, poziom zgodności określony w [Kroku 1.b. Określ wymagany poziom zgodności](#step1b) jest spełniony przez wszystkie strony i stany stron internetowych poddane audytowi (w [Kroku 4): Wykonaj audyt wybranej próbki](#step4)), a właściciel witryny zobowiązuje się do zapewnienia poprawności i zachowania dokładności złożonego oświadczenia z oceny.

Oświadczenie oceniające zgodne z tą metodologią zawiera co najmniej następujące informacje:

1.  **Data** wydania oświadczenia o ocenie;
2.  **Tytuł, wersja i URI:** wytycznych: „Wytyczne dla dostępności treści internetowych 2.0” pod adresem [http://www](http://www.w3.org/TR/WCAG20/).w3.org/TR/WCAG20/";
3.  **Oceniony poziom zgodności:**: Poziom A, AA lub AAA, zgodnie z definicją w [kroku 1.b. Określ wymagany poziom zgodności](#step1b);
4.  **Definicja witryny internetowej** określona w [Kroku 1.a: Określ zakres stron witryny](#step1a);
5.  **Zaufane technologie internetowe** określone w [Kroku 2.d Rozpoznaj użyte technologie internetowe](#step2d);
6.  **Bazowy poziom obsługi dostępności,** jak określono w [Kroku 1.c: Określ bazowy poziom obsługi dostępności](#step1c).

Oświadczenia oceniające zgodnie z tą metodologią mogą być również sporządzane, gdy osiągnięto jedynie [częściową zgodność](http://www.w3.org/TR/WCAG20/#conformance-partial) z WCAG 2.0. W takich przypadkach stwierdzenia ewaluacyjne zawierają również następujące informacje:

7.  **Obszary strony internetowej**, które nie są zgodne z WCAG 2.0;
8.  **Powód niezgodności** z **WCAG 2.0:** „treści stron trzecich” lub „brak wsparcia dla języków”.

#### Krok 5.d: Podaj zagregowany wynik (opcjonalnie)  {#step1a}

**Wymóg metodologiczny 5.d {#req5d} :** Podaj zagregowany wynik (opcjonalnie).

Chociaż zagregowane wyniki stanowią wskaźnik liczbowy, który pomaga komunikować postępy w czasie, obecnie nie ma jednej miary, która uwzględniałaby wymaganą wiarygodność, dokładność i praktyczność. W rzeczywistości zagregowane wyniki mogą wprowadzać w błąd i nie zapewniają wystarczającego kontekstu i informacji, aby zrozumieć rzeczywistą dostępność strony internetowej. Z tego i innych powodów WCAG 2.0 nie zapewnia systemu klasyfikacji. [Raport z badań nad metrykami dostępności stron internetowych](http://www.w3.org/TR/accessibility-metrics-report/) zawiera więcej informacji na temat bieżących badań, różnych podejść i ograniczeń oceniania wskaźników, które wykraczają poza zakres tego dokumentu. Za każdym razem, gdy podawana jest punktacja, istotne jest, aby sposób punktacji został udokumentowany i udostępniony [zlecającemu ocenę](#commissioner) wraz z raportem, aby ułatwić przejrzystość i powtarzalność.

#### Krok 5.e: Sporządź wersję raportu do odczytu maszynowego (opcjonalnie)  {#step1a}

**Wymóg metodologiczny 5.e {#req5e} :** Sporządź sprawozdanie z wyników oceny nadające się do odczytu maszynowego (opcjonalnie).

Raporty nadające się do odczytu maszynowego ułatwiają przetwarzanie wyników oceny przez autorów, narzędzia oceny dostępności stron internetowych oraz narzędzia zapewniania jakości. [Język oceny i raportowania (EARL)](http://www.w3.org/WAI/intro/earl) jest formatem do odczytu maszynowego, który został specjalnie zaprojektowany do tego celu. Zaleca się korzystanie z EARL w celu zapewnienia raportów do odczytu maszynowego. Aby dowiedzieć się więcej na temat wykorzystania metadanych, w tym raportów odczytywanych maszynowo, takich jak EARL, zobacz [Objaśnienie metadanych](http://www.w3.org/TR/UNDERSTANDING-WCAG20/appendixC#understanding-metadata) z WCAG 2.0.

* * *

## Załączniki  {#appendices}

### Dodatek A: Współtwórcy  {#contributors}

Dawni i obecni aktywni uczestnicy projektu [Grupy Roboczej ds. Metodologii Oceny Zoodności z WCAG 2.0 (Eval TF)](http://www.w3.org/WAI/ER/2011/eval/eval-tf) obejmują: Shadi Abou-Zahra; Frederick Boland; Denis Boudreau; Amy Chen; Vivienne Conway; Bim Egan; Michael Elledge; Gavin Evans; Wilco Fiers; Detlev Fischer; Elizabeth Fong; Vincent François; Alistair Garrison; Emmanuelle Gutiérrez y Restrepo; Katie Haritos-Shea; Martijn Houtepen; Peter Korn; Maureen Kraft; Aurelien Levy; David MacDonald; Mary Jo Mueller; Donald Raikes; Corominas Ramon; Roberto Scano; Samuel Sirois; Sarah J Swierenga; Eric Velleman; Konstantinos Votis; Kathleen Wahlbin; Elle Waters; Richard Warren; Léonie Watson.

### Dodatek B: Bibliografia  {#references}

<dl>
        <dt id="atag20">ATAG20</dt>
        <dd>Richards J, Spellman J, Treviranus J, eds (2013). Wytyczne dla dostępności narzędzi autorskich 2.0. W3C. Dostępne pod adresem: <a href="http://www.w3.org/TR/ATAG20/">http://www.w3.org/TR/ATAG20/</a></dd>
        <dt id="easychecks">Łatwe testy</dt>
        <dd>Lawton Henry S, ed (2014). Łatwe testy - Pierwszy przegląd dostępności internetowej. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/eval/preliminary">http://www.w3.org/WAI/eval/preliminary</a></dd>
        <dt id="essential-components">Podstawowe komponenty dostępności stron internetowych</dt>
        <dd>Lawton Henry S, red. (2005). Podstawowe komponenty dostępności stron internetowych. Wersja 1.3. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/intro/components.php">http://www.w3.org/WAI/intro/components.php</a></dd>
        <dt id="people-use-web">Jak osoby z niepełnosprawnością korzystają z Internetu</dt>
        <dd>Abou-Zahra S, ed (2012). Jak osoby z niepełnosprawnością korzystają z Internetu Wersja robocza. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/intro/people-use-web/">http://www.w3.org/WAI/intro/people-use-web/</a></dd>
        <dt id="involving-users">Włączanie użytkowników w ocenę dostępności stron internetowych</dt>
        <dd>Lawton Henry S, ed (2010). Włączanie użytkowników w ocenę dostępności stron internetowych. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/eval/users">http://www.w3.org/WAI/eval/users</a></dd>
        <dt id="selecting-tools">Wybieranie narzędzi do oceny dostępności internetowej</dt>
        <dd>Abou-Zahra S, ed (2005). Wybieranie narzędzi do oceny dostępności internetowej. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/eval/selectingtools">http://www.w3.org/WAI/eval/selectingtools</a></dd>
        <dt id="combined-expertise">Wykorzystanie połączonej wiedzy specjalistycznej do oceny dostępności internetowej</dt>
        <dd>Brewer J, ed (2002). Wykorzystanie połączonej wiedzy specjalistycznej do oceny dostępności internetowej. W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/eval/reviewteams">http: </a>//www.w3.org/WAI/eval/reviewteams </dd>
        <dt id="uwem">UWEM</dt>
        <dd>Velleman E.M, Velasco C.A, Snaprud M (red.) (2007). D-WAB4 Unified Web Evaluation Methodology (UWEM 1.2 Core). Wabcluster. Dostępne pod adresem: <a href="http://www.wabcluster.org/uwem1_2/">http://www.wabcluster.org/uwem1_2/</a></dd>
        <dt id="wcag20-overview">Omówienie WCAG</dt>
        <dd>Lawton Henry S, ed (2012). Omówienie Wytycznych dla dostępności treści internetowych (WCAG). W3C. Dostępne pod adresem: <a href="http://www.w3.org/WAI/intro/wcag">http://www.w3.org/WAI/intro/wcag</a></dd>
        <dt id="wcag20">WCAG20</dt>
        <dd>Caldwell B, Cooper M, Guarino Reid L, Vanderheiden G, eds (2008). Wytyczne dla dostępności treści internetowych 2.0. W3C. Dostępne pod adresem: <a href="http://www.w3.org/TR/WCAG20/">http://www.w3.org/TR/WCAG20/</a></dd>
        <dt id="wcag20-techs">WCAG20-TECHS</dt>
        <dd>Cooper M, Kirkpatrick A, O Connor J, eds (2014). Techniki i błędy dla Wytycznych dla dostępności treści internetowych 2.0. W3C. Dostępne pod adresem: <a href="http://www.w3.org/TR/WCAG20-TECHS/">http://www.w3.org/TR/WCAG20-TECHS/</a></dd>
        <dt id="understanding-wcag20">Objaśnienia-WCAG20</dt>
        <dd>Cooper M, Kirkpatrick A, O Connor J, eds (2014). Objaśnienia WCAG 2.0 - Przewodnik po zrozumieniu i wdrożeniu Wytycznych dla dostępności treści internetowych 2.0. W3C. Dostępne pod adresem: <a href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/">http://www.w3.org/TR/UNDERSTANDING-WCAG20/</a></dd>
</dl>