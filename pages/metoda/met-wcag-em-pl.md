---
title: Metodologia oceniania zgodności w zakresie dostępności internetowej (WCAG-EM) 1.0
summary: "Publikacja jest nieoficjalnnym roboczym tłumaczeniem dokumentu W3C Website Accessibility Conformance Evaluation Methodology (WCAG-EM) 1.0"
sidebar: metoda_sidebar
permalink: met-wcag-em-pl
folder: metoda
---

## Streszczenie

Ten dokument zawiera wskazówki dotyczące oceny, w jaki sposób strony internetowe są zgodne z [Wytycznymi dla dostępności treści internetowych (WCAG) 2.1](https://testy.lepszyweb.pl/wcag21) [*w oryginale odniesienie do WCAG 2.0*]. Opisuje procedurę oceny stron internetowych oraz zawiera wskazówki, które pomogą oceniającym stosować dobre praktyki. Nie zawiera instrukcji oceny treści stron internetowych według funkcji, do których odnoszą się kryteria sukcesu WCAG 2.1. Ten dokument jest jednym z serii materiałów informacyjnych W3C / WAI [na temat oceny stron internetowych pod kątem dostępności](http://www.w3.org/WAI/eval/), które uzupełniają [Dokumenty WCAG 2](https://www.w3.org/WAI/standards-guidelines/wcag/docs/). Nie definiuje dodatkowych wymagań WCAG 2.1, nie zastępuje ich ani nie zmienia w żaden sposób.

Metodologia opisana w tym dokumencie jest przeznaczona dla osób, które mają doświadczenie w ocenie dostępności za pomocą WCAG 2.1 i ich zasobów pomocniczych. Zawiera wskazówki dotyczące dobrych praktyk w zakresie definiowania zakresu oceny, eksploracji ocenianej witryny, wyboru reprezentatywnych próbek stron z witryn, na których nie jest możliwe ocenienie całej treści, audytu wybranych próbek i raportowania wyników oceny. Jest przeznaczona przede wszystkim do oceny istniejących stron internetowych, na przykład, aby dowiedzieć się o ich dostępności i monitorować poziom dostępności. Może być również przydatna na wcześniejszych etapach projektowania i rozwoju stron internetowych. Dotyczy to statycznych i dynamicznie generowanych stron internetowych, witryn i aplikacji mobilnych oraz innych rodzajów stron internetowych. Nie wskazuje konkretnych technologii internetowych, narzędzi oceny, przeglądarek internetowych, technologii wspomagających ani innego oprogramowania do oceny. Nadaje się do stosowania w różnych kontekstach oceny, w tym samooceny i oceny przez podmioty zewnętrzne.

## Status dokumentu

{% include note.html content="W tej części opisano sttus tego dokumentu w momencie jego publikacji. Inne dokumenty mogą zastąpić ten dokument. Listę bieżących publikacji W3C i najnowszą wersję tego raportu technicznego można znaleźć w&nbsp;indeksie raportów technicznych W3C pod adresem http://www.w3.org/TR/." %}

Niniejszy dokument jest [notatką Grupy Roboczej](http://www.w3.org/Consortium/Process/tr#WGNote) opracowaną przez [grupę zadaniową ds. Metodologii oceny WCAG 2.0 (Eval TF)](http://www.w3.org/WAI/ER/2011/eval/eval-tf), [wspólną grupę zadaniową Grupy Roboczej Wytyczne dla dostępności internetowej (WCAG WG)](http://www.w3.org/WAI/GL/) oraz [Grupy Roboczej ds. Narzędzi oceny i naprawy (ERT WG)](http://www.w3.org/WAI/ER/). Zawiera wskazówki informacyjne na temat oceny zgodnie z [wytycznymi dla dostępności treści internetowych (WCAG).](http://www.w3.org/WAI/intro/wcag)

Jako Notatka Grupy Roboczej ten materiał jest stabilny. Na obecnym etapie Grupa Robocza nie planuje dalszych zmian. Jeśli jednak zajdzie taka potrzeba, dokument może zostać zaktualizowany. Uwagi otrzymane na temat tego dokumentu pomogą Grupie Roboczej zdecydować, czy aktualizacje są potrzebne lub zostaną uwzględnione w przypadku planowania ponownej publikacji.  Wszelkie uwagi, w tym wykryte błędy, prosimy wysyłać na publiczną listę mailingową [public-wcag-em-comments@w3.org](public-wcag-em-comments@w3.org) (publicznie widoczne [archiwum listy mailingowej](http://lists.w3.org/Archives/Public/public-wcag-em-comments/). W komentarzach podaj następujące informacje: lokalizację w dokumencie, sugerowaną zmianę oraz uzasadnienie komentarza.

Niniejszy dokument został opracowany w ramach inicjatywy W3C [Web Accessibility Initiative (WAI)](http://www.w3.org/WAI/eval/preliminary). Cele grup roboczych WCAG WG i ERT WG są omawiane odpowiednio w [Karcie Grupy Roboczej WCAG](http://www.w3.org/WAI/GL/2010/06/charter) i [Karcie Grupy Roboczej ERT](http://www.w3.org/WAI/ER/charter4). WCAG WG i ERT WG są częścią [działalności technicznej WAI](http://www.w3.org/WAI/Technical/Activity).

Publikacja w formie noty grupy roboczej nie oznacza poparcia ze strony członków W3C. Jest to projekt dokumentu i&nbsp;może być w każdej chwili aktualizowany, zastępowany lub zdezaktualizowany przez inne dokumenty. Cytowanie tego dokumentu jako innego niż „praca w toku” jest niewłaściwe.

Dokument ten został opracowany przez dwie grupy działające w ramach [Polityki patentowej W3C z 5 lutego 2004 roku](http://www.w3.org/Consortium/Patent-Policy-20040205/). Grupy nie oczekują, że dokument ten stanie się Rekomendacją W3C. W3C prowadzi [pełną listę zgłoszonych publicznie patentów WCAG WG](http://www.w3.org/2004/01/pp-impl/35422/status)) oraz [pełną listę zgłoszonych publicznie patentów](http://www.w3.org/2004/01/pp-impl/32094/status) ERT WG odnośnie produktami każdej z grup; strony te zawierają również instrukcje zgłaszania patentu. Osoba, które twierdzą, iż posiadają faktyczną wiedzę na temat patentów zawierających [istotne zastrzeżenia](http://www.w3.org/Consortium/Patent-Policy-20040205/#def-essential), musi ujawnić informacje zgodnie z&nbsp;rozdziałem [6 Polityki patentowej W3C.](http://www.w3.org/Consortium/Patent-Policy-20040205/#sec-Disclosure)

## Uwagi tłumacza

{% include callout.html content="**Uwaga 1:** Poniższe tłumaczenie ma charakter roboczy. Celem tłumacza było przygotowanie dokumentu przetłumaczonego na tyle dokładnie, aby pomagał osobom podejmującym się prób oceny dostępności stron internetowych odpowiednio przygotować do oceny i rozumieć konsekwencje podejmowanych wyborów metodologicznych.<br><br>**Uwaga 2:** Wszystkie odniesienia do WCAG 2.0 zostały zastąpione w tłumaczeniu odniesieniami do WCAG 2, wskzaujac tym samym lub WCAG 2.1<br><br>**Uwaga 2:** W przypadkach gdy istnieją polskie tłumaczenia przywoływanych dokumentów, odnośniki do wersji oryginalnych zostały zastąpione odnośnikami do wersji polskich." type="success" %}

## Wprowadzenie

Ocena stopnia, w jakim strona internetowa jest zgodna z [Wytycznymi dotyczącymi dostępności treści internetowych (WCAG) 2](wcag21), jest procesem składającym się z kilku etapów. Na działania prowadzone w ramach tych etapów ma wpływ wiele aspektów, takich jak: rodzaj strony internetowej (np. statyczna, dynamiczna, responsywna, mobilna, itp.); jej rozmiar, złożoność oraz technologie wykorzystywane do stworzenia strony internetowej (np. HTML, WAI-ARIA, PDF, itp.); wiedzy ewaluatorów na temat procesu wykorzystywanego do zaprojektowania i rozwoju strony internetowej; oraz główny cel ewaluacji (np. wydanie oświadczenia o dostępności, zaplanowanie procesu przeprojektowania, przeprowadzenie badań itp.)

Metodologia ta opisuje kroki, które są wspólne dla procesów kompleksowej oceny stopnia zgodności stron internetowych z WCAG 2. Podkreślono, że ewaluatorzy powinni zastosować te kroki w kontekście konkretnej strony internetowej. Nie zastępuje to potrzeby stosowania środków zapewnienia jakości, które są wdrażane podczas projektowania, tworzenia i utrzymania witryn w celu zapewnienia ich zgodności z wymaganiami dostępności. Stosowanie tej metodyki pomoże ewaluatorom w stosowaniu dobrych praktyk, unikaniu powszechnie popełnianych błędów i osiąganiu bardziej porównywalnych wyników. Jednak w większości sytuacji, w których stosuje się tę metodologię samodzielnie, bez dodatkowych środków zapewnienia jakości, nie skutkuje bezpośrednio roszczeniami dotyczącymi zgodności z WCAG 2.

**Metodologia ta w żaden sposób nie dodaje ani nie zmienia wymagań określonych w normatywnym standardzie WCAG 2**, ani też nie dostarcza instrukcji dotyczących oceny treści stron internetowych pod względem cech charakterystycznych. Metodologia może być stosowana w połączeniu z technikami spełniającymi kryteria sukcesu WCAG 2, takimi jak [Techniki dla WCAG 2](https://www.w3.org/WAI/WCAG21/Techniques/#techniques) udokumentowane przez W3C/WAI, ale nie wymaga tego lub innego specyficznego zestawu technik.

## Cele niniejszej metodologii

W wielu sytuacjach konieczna jest ocena dostępności strony internetowej, na przykład przed wydaniem, pozyskaniem lub przeprojektowaniem strony internetowej oraz w celu okresowego monitorowania dostępności strony internetowej. Metodologia ta jest przeznaczona dla każdego, kto chce stosować wspólne podejście do oceny zgodności stron internetowych z WCAG 2. W kręgu osób, które mogą być zainteresowane metodologią, są:

 - Konsultanci sieciowi, którzy chcą analizować i raportować zgodność z&nbsp;wymogami dostępności cyfrowej, aby informować właścicieli stron internetowych.
 - Dostawcy usług oceny dostępności cyfrowej, którzy chcą oceniać strony internetowe w celu potwierdzenia zgodności z wymogami dostępności.
 - Twórcy witryn, którzy chcą ocenić zgodność z wymogami dostępności swoich stron internetowych w celu ich monitorowania lub poprawy.
 - Właściciele witryn, zamawiający i dostawcy, którzy chcą dowiedzieć się o&nbsp;zgodności z&nbsp;wymogami dostępności swoich stron internetowych.
 - Menedżerowie ds. zgodności z przepisami i zapewnienia jakości, którzy chcą mieć pewność, że spełniają wymagania dotyczące jakości i polityki.
 - Podmioty monitorujące dostępność cyfrową w celu testowania i porównywania postępów zgodności z&nbsp;wymogami dostępności.
 - Naukowcy zajmujący się zagadnieniami związanymi z&nbsp;dostępnością cyfrową oraz rzecznicy osób z niepełnosprawnościami, którzy chcą zbadać praktyki w&nbsp;zakresie zgodności z&nbsp;wymogami dostępności.
 - Trenerzy i edukatorzy ds. dostępności cyfrowej, którzy chcą uczyć podejścia do oceny dostępności stron internetowych.
 - Webmasterzy, autorzy treści, projektanci i inni, którzy chcą dowiedzieć się więcej na temat dostępności cyfrowej i&nbsp;oceny stron internetowych.

## Stosunek do Wymagań zgodności WCAG 2

WCAG 2 definiują [wymagania dotyczące zgodności](wcag21#52-wymogi-dotyczące-zgodności) dla pojedynczych stron internetowych (a&nbsp;w&nbsp;niektórych przypadkach także zestawów stron internetowych), ale nie opisują, jak oceniać całe witryny. Określają również, w jaki sposób można składać opcjonalne [oświadczenia o zgodności](wcag21#53-oświadczenie-o-zgodności-opcjonalne) w&nbsp;odniesieniu do poszczególnych stron internetowych, serii stron internetowych, takich jak formularz wielostronicowy, oraz wielu powiązanych stron internetowych, takich jak witryna internetowa. Ma to zastosowanie do przypadków, gdy wszystkie strony internetowe objęte oświadczeniem o&nbsp;zgodności zostały ocenione lub utworzone w procesie zapewniającym, że każda spełnia wszystkie wymagania dotyczące zgodności.

Oświadczenia o zgodności z WCAG 2 dla całych witryn nie można składać na podstawie oceny wybranego podzbioru stron internetowych i samej funkcjonalności, ponieważ zawsze możliwe jest, że na tych stronach pojawią się niezidentyfikowane błędy dotyczące zgodności. Jednak w większości zastosowań tej metodologii do oceny wybiera się tylko próbkę stron internetowych i&nbsp;funkcjonalności witryny. Dlatego w większości sytuacji samo zastosowanie tej metodologii nie daje wystarczających podstaw do stwierdzenia zgodności badanych witryn z  WCAG 2. Wskazówki dotyczące formułowania oświadczeń  na temat wyników zastosowania tej metodologii znajdują się w&nbsp;[kroku 5. c: Przygotuj oświadczenie o zgodności (opcjonalnie)](#krok-5c-przygotuj-oświadczenie-o-zgodności-opcjonalnie).

## Lektury wprowadzające

Poniższe informacje, związane z podstawami dostępności cyfrowej, ocenianiem i&nbsp;WCAG 2, są istotne dla korzystania z&nbsp;tej metodologii. Oczekuje się, że osoby oceniające stosujące tę metodologię będą dobrze zaznajomione ze wszystkimi wymienionymi poniżej pozycjami:

### Podstawy dostępności cyfrowej

Poniższe dokumenty wprowadzają podstawowe elementy dostępności stron internetowych i&nbsp;wyjaśniają, w&nbsp;jaki sposób osoby z&nbsp;niepełnosprawnościami korzystają z&nbsp;sieci. Mają one kluczowe znaczenie dla zrozumienia szerszego kontekstu oceny dostępności stron internetowych:

- [Podstawowe komponenty dostępności stron internetowych](http://dostepny.joomla.pl/dostepnosc/internet-dla-wszystkich/51-podstawowe-komponenty-dostepnosci-sieci),
- [Jak osoby z niepełnosprawnością korzystają z Internetu](http://www.w3.org/WAI/intro/people-use-web/) (w jezyku angielskim).

### Ocena stron internetowych pod kątem dostępności

Są to szczególnie ważne zasoby, które nakreślają różne podejścia do oceny stron internetowych pod kątem dostępności:

- [**Łatwe testy** – pierwszy przegląd dostępności stron internetowych](00-P-wprowadzenie); oryginał: [Easy Checks – A First Review of Web Accessibility](https://www.w3.org/WAI/test-evaluate/preliminary/)
- [Zaangażowanie użytkowników w ocenę dostępności stron internetowych](http://www.w3.org/WAI/eval/users) (w języku angielskim)
- [Wybór narzędzi do oceny dostępności sieci (Web Accessibility Evaluation Tools)](http://www.w3.org/WAI/eval/selectingtools) (w języku angielskim)
- [Wykorzystanie wiedzy specjalistycznej w celu oceny dostępności stron internetowych](http://www.w3.org/WAI/eval/reviewteams) (w języku angielskim)

### Wytyczne dla dostępności treści internetowych (WCAG) 2.1

Jest to uznawany na całym świecie standard wyjaśniający, w jaki sposób sprawić, by treści internetowe były bardziej dostępne dla osób z&nbsp;niepełnosprawnościami. Poniższe materiały są szczególnie ważne dla oceny dostępności stron internetowych:

- [WCAG 2.1 Przegląd](https://www.w3.org/WAI/standards-guidelines/wcag/) (w języku angielskim)
- [WCAG 2.1 Specyfikacja techniczna](https://www.w3.org/TR/WCAG21/)  (w języku angielskim)
- [Jak spełnić WCAG 2 (Krótki przewodnik)](https://wcag.lepszyweb.pl)
- [Zrozumieć WCAG](https://www.w3.org/WAI/WCAG21/Understanding/)  (w języku angielskim)
- [Techniki dla WCAG](https://www.w3.org/WAI/WCAG21/Techniques/)  (w języku angielskim)

## Terminy i definicje

Do celów tego dokumentu obowiązują następujące terminy i definicje:

Całe procesy

: [Zobacz wymaganie zgodności WCAG 2.1 dla całych procesów.](wcag#523-całe-procesy)

  Zgodność oraz poziomy zgodności określa się dla całych procesów.

  W przypadku gdy treść strony jest częścią procedury, to znaczy jest jedną z serii stron prezentujących jakąś procedurę (czyli sekwencję kroków niezbędną, aby wykonać jakieś zadanie), deklarowany poziom zgodności musi być spełniony przez wszystkie strony, na których prezentowana jest ta procedura. Na przykład zgodność na poziomie AA jest osiągnięta tylko wtedy, gdy wszystkie strony prezentujące procedurę, obejmujące wszystkie kroki, są zgodne co najmniej na tym poziomie.

  Gdy tylko niektóre etapy procesu spełniają wymogi zgodności na wyższym poziomie, to cały proces (i strony, na których jest obsługiwany) spełniają wyniki na niższym poziomie. Inaczej - zgodność na danym poziomie nie jest osiągnięta, jeżeli którakolwiek ze stron prezentujących którykolwiek z etapów procesu nie spełnia wszystkich wymogów zgodności na tym poziomie.

Całe witryny

: Zgodność i poziom zgodności określa się dla całych witryn.

  Gdy oświadczenie dotyczy zbioru stron, jakimi są witryny, deklarowany poziom zgodności musi być spełniony przez wszystkie strony (na wszystkich stronach). Nie można osiągnąć zgodności na danym poziomie, jeśli jakaś część witryny zostanie wyłączona z oceny.

Komisarz ds. oceny

: Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot, który zlecił ocenę.

  **Uwaga**: W wielu przypadkach komisarz ds. oceny może być właścicielem lub twórcą witryny, w innych przypadkach może to być inny podmiot, taki jak zamawiający lub właściciel ankiety monitorującej dostępność.

Niezbędna funkcjonalność

: Funkcja (funkcjonalność), której usunięcie zasadniczo zmienia sposób użytkowania lub przeznaczenie witryny. Obejmuje zarówno informacje, do których odnoszą się użytkownicy, jak i czynności, które wykonują, aby użyć tej funkcji.

  **Uwaga**: Przykłady niezbędnych funkcji obejmują „wybór i zakup produktu w sklepie internetowym”, „wypełnienie i przesłanie formularza kontaktowego”, „rejestrację konta użytkownika”.

  **Uwaga**: Stosowanie pojęcia niezbędnej funkcjonalności nie wyłącza z zakresu oceny innych funkcji. Termin „niezbędna funkcjonalność” ma na celu pomóc w identyfikacji kluczowych stron internetowych i uwzględnienie ich między innymi w ocenie.

Oceniający, ewaluator, audytor

: Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot odpowiedzialny za przeprowadzenie oceny.

Stan strony internetowej

: Dynamicznie generowane witryny prezentują czasami znacznie różniące się od siebie treści, funkcjonalności i&nbsp;wygląd w&nbsp;zależności od użytkownika, interakcji, urządzenia i&nbsp;innych parametrów. W&nbsp;kontekście tej metodologii takie stany można traktować jako dodatkowe (zapisywane w&nbsp;próbce do audytu jako dodatkowe stany strony internetowej) lub jako pojedyncze strony internetowe.

  **Uwaga**: Przykładami stanów stron internetowych są poszczególne strony wieloczęściowego formularza internetowego, które są generowane dynamicznie w zależności od danych wprowadzonych przez użytkownika. Poszczególne stany mogą nie posiadać unikalnych URI i&nbsp;mogą wymagać identyfikacji poprzez opisanie ustawień, danych wejściowych lub działań wymaganych do ich wygenerowania.

Strona internetowa

: [Zobacz definicję strony internetowej w WCAG 2.1 ](slownik#s)

  Nieosadzony zasób, uzyskany z pojedynczego identyfikatora URI za pomocą protokołu HTTP wraz z wszelkimi innymi zasobami użytymi do renderowania strony w oprogramowaniu użytkownika lub takimi, które potencjalnie mogą być użyte do renderowania.

  **Uwaga**: Strony internetowe mogą zawierać treści multimedialne, komponenty interaktywne oraz bogate i&nbsp;mobilne aplikacje internetowe. Strony internetowe nie są ograniczone do formatu HTML i&nbsp;mogą być dokumentami PDF, a także dokumentami w&nbsp;innych formatach.

  **Uwaga 2**: Terminu „strona internetowa” używa się potocznie zarówno na oznaczenie pojedynczych stron internetowych, jak serwisów złożonych z wielu stron internetowych, czyli witryn. Powyższa definicja ogranicza stosowanie terminu „strona internetowa” tylko do zasobu uzyskanego z „pojedynczego identyfikatora URI”, a więc do jednej, pojedynczej samodzielnej strony internetowej albo jednej, pojedynczej strony w&nbsp;witrynie złożonej z&nbsp;wielu stron.

Strony wspólne

: Strony i stany stron internetowych wspólne dla całej witryny odnoszące się do całej witryny, istotne dla funkcjonowania całej witryny, takie jak strona główna, strona logowania, mapa witryny, strona kontaktowa, strona pomocy, strona informacji prawnych i&nbsp;podobne, które są zazwyczaj połączone ze wszystkimi innymi stronami witryny (zwykle poprzez łącze w nagłówku, stopce lub w&nbsp;menu nawigacyjnym).

   **Uwaga**: definicja stanów stron internetowych znajduje się powyżej.

Szablony

: [Zobacz definicję \"templates\" w ATAG 2.0:](http://www.w3.org/TR/ATAG20/#def-Template)

  Wzorce, które są wypełniane treścią przez autorów lub za pomocą narzędzia autorskiego (np. szablony dokumentów, szablony zarządzania treścią, motywy prezentacji). Szablony zwykle zastępują autorów, przynajmniej częściowo, w decydowaniu o&nbsp;układzie i&nbsp;stylizacji treści.

Twórca witryny

:  Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot zaangażowany w proces tworzenia witryny, w&nbsp;tym między innymi autorzy treści, projektanci, programiści, programiści, testerzy zapewniania jakości oraz menadżerowie projektu.

Spolegliwa (technologia bazowa)

: [Zobacz definicję \"relied upon\" w glosariuszu WCAG 2.1 ](https://www.w3.org/TR/WCAG21/#dfn-relied-upon)

  Technologia internetowa, które musi być obsługiwana, aby treść spełniała wymogi zgodności. Treść nie będzie zgodna, jeżeli taka technologia zostanie wyłączona z&nbsp;oceny lub nie jest obsługiwana.

Witryna

: Spójny zbiór jednej lub większej liczby połączonych ze sobą stron internetowych, które razem zapewniają wspólne użytkowanie lub funkcjonalności. Obejmuje statyczne strony internetowe, dynamicznie generowane strony internetowe oraz witryny i&nbsp;aplikacje mobilne.

  **Uwaga**: Ta metodologia koncentruje się na całych, samodzielnych witrynach internetowych. Witryny mogą składać się z&nbsp;mniejszych zbiorów stron, z&nbsp;których każdy można uznać za odrębną witrynę. Na przykład witryna może zawierać wyodrębnione obszary, takie jak sklep internetowy, forum dyskusyjne albo odrębne obszary dla każdego działu czy filii w organizacji, obszar blogów i&nbsp;inne obszary, powiązane wspólnym adresem domenowym. Każdy taki podzbiór może być uznany za odrębną witrynę.

Właściciel witryny

: Osoba, zespół ludzi, organizacja, dział wewnętrzny organizacji lub inny podmiot odpowiedzialny za publikację witryny internetowej.

Zgodność

: [Porównaj definicję „zgodności” w WCAG 2.1](slownik#z)

Spełnienie wszystkich wymagań danej normy, wytycznych lub specyfikacji.

## Korzystanie z metodologii

Metodologia ta służy do dokładnej oceny stron internetowych przy użyciu WCAG&nbsp;2. Przed oceną całej witryny dobrze jest przeprowadzić wstępną ocenę różnych stron internetowych z&nbsp;badanej witryny, aby zidentyfikować oczywiste bariery dostępności i&nbsp;wypracować ogólne zrozumienie dostępności witryny. [Łatwe testy – Wstępny przegląd dostępności cyfrowej](00-P-wprowadzenie2) opisuje takie podejście do wstępnej oceny, które jest uzupełnieniem tej metodologii.

## Wymagana wiedza specjalistyczna

Zakłada się, że użytkownicy tej metodologii mają solidną wiedzę na temat oceniania treści internetowych przy użyciu WCAG&nbsp;2, projektowania dostępnych stron internetowych, technologii wspomagających oraz tego, jak osoby z&nbsp;różnymi rodzajami niepełnosprawności korzystają z&nbsp;Internetu. Obejmuje to zrozumienie technologii internetowych, barier dostępności, których doświadczają osoby z niepełnosprawnościami, technologii wspomagających i&nbsp;strategii adaptacyjnych stosowanych przez osoby z&nbsp;niepełnosprawnościami, oraz technik oceny, narzędzi i&nbsp;metod identyfikacji barier dla osób z&nbsp;niepełnosprawnościami. Wvszczególności zakłada się, że użytkownicy tej metodologii są dogłębnie zaznajomieni ze wszystkimi zasobami wymienionymi w&nbsp;sekcji [Lektury wprowadzające.](#lektury-wprowadzające)

## Połączona wiedza specjalistyczna (opcjonalnie)

Metodologię tę może stosować indywidualny ewaluator posiadający umiejętności opisane w poprzedniej sekcji [Wymagana wiedza specjalistyczna](#wymagana-wiedza-specjalistyczna) lub zespół testerów posiadających zbiorową wiedzę specjalistyczną. Korzystanie z&nbsp;połączonej wiedzy specjalistycznej różnych ewaluatorów może czasami być konieczne lub korzystne, gdy jeden ewaluator nie posiada całej wymaganej wiedzy specjalistycznej. Więcej wykraczających poza zakres tego dokumentu wskazówek na temat korzystania z połączonej wiedzy specjalistycznej zespołów recenzujących znajduje się w&nbsp;opracowaniu [Using Combined Expertise to Evaluate Web Accessibility.](http://www.w3.org/WAI/eval/reviewteams)

## Zaangażowanie użytkowników (opcjonalnie)

Zaangażowanie osób niepełnosprawnych, w tym osób z&nbsp;trudnościami związanymi ze starzeniem się (które nie są doświadczonymi ewaluatorami lub członkami zespołu oceniającego), może pomóc w&nbsp;zidentyfikowaniu dodatkowych barier dostępności które nie są łatwe do wykrycia w&nbsp;drodze oceny eksperckiej. Chociaż nie jest to wymagane do stosowania tej metodologii, ewaluatorzy mogą czasem być zmuszeni do zaangażowania w&nbsp;proces oceny osób doświadczających autentycznych problemów z&nbsp;dostępnością. Więcej wykraczających poza zakres tego dokumentu wskazówek na temat angażowania użytkowników w&nbsp;ocenę dostępności cyfrowej znajduje się w&nbsp;opracowaniu [Involving Users in Evaluating Web Accessibility.](http://www.w3.org/WAI/eval/users)

## Narzędzia oceny (opcjonalnie)

Metodologia ta jest niezależna od konkretnego narzędzia oceny dostępności cyfrowej, przeglądarki internetowej i&nbsp;innych narzędzi programowych. Chociaż większości testów nie można przeprowadzić automatycznie, to narzędzia oceny mogą znacznie pomóc ewaluatorom w&nbsp;procesie oceny i&nbsp;przyczynić się do bardziej efektywnej oceny. Na przykład, niektóre narzędzia oceny dostępności cyfrowej mogą skanować całe witryny, aby pomóc w&nbsp;identyfikacji odpowiednich stron do ręcznej oceny. Narzędzia mogą być również pomocne podczas ręcznej (ludzkiej) oceny testów dostępności. Więcej wykraczających poza zakres tego dokumentu wskazówek dotyczących korzystania z&nbsp;narzędzi oceny zawiera opracowanie [Selecting Web Accessibility Evaluation Tools.](http://www.w3.org/WAI/eval/selectingtools). Porównaj również: [Narzędzia audytora dostępności cyfrowej](nod-wprowadzenie).

## Zakres stosowania

Ta metodologia jest przeznaczona do oceny całych <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.witryna_internetowa | strip_html | replace: '*', ''}}">witryn internetowych</a>. Oznacza to, że dla każdej <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa | strip_html | replace: '*', ''}}">strony internetowej</a> jest jednoznaczne, czy jest ona częścią witryny, czy nie. Dotyczy to witryn organizacji, podmiotów, osób, wydarzeń, produktów i&nbsp;usług.

## Przykłady witryn

Oto kilka konkretnych przykładów witryn:

- „Publiczna witryna organizacji Przykładowa pod adresem http://www.przykladowa.org”
- „Witryna intranetowa organizacji Przykładowa pod adresem http://intranet.przykladowa.org”
- „Sklep internetowy organizacji Przykładowa pod adresem http://www.przykladowa.org /sklep/”
- „Wydanie wersji 1.5.3 aplikacji System rezerwacji online (SRO)”
- „Mobilna wersja witryny organizacji Przykładowa pod adresem http://m.przyklad.org”
- „Holenderska wersja witryny organizacji Przykładowa pod adresem http://nl.przykladowa.org”

Witryna może być częścią większej witryny, jak na przykład sklep internetowy w przykładach powyżej. Witryna może być także wyraźnie oddzielną wersją witryny, taką jak wersja mobilna lub wersja w języku holenderskim, jak pokazano w przykładach powyżej. Ta metodologia może być stosowana w odniesieniu do dowolnej strony internetowej, niezależnie od tego, czy jest ona częścią większej witryny, czy też nie. Precyzyjne określenie witryny jest ustalane w ramach [kroku 1.a](#krok-1a-określ-zakres-stron-witryny)

## Zasada włączania stron do oceny

W przypadku, gdy do oceny została wyznaczona witryna internetowa, istotne jest, aby wszystkie strony internetowe, stany stron internetowych i&nbsp;funkcjonalności objęte zakresem jej definicji były uwzględnione w&nbsp;ocenie. Wyłączenie takich aspektów witryny z&nbsp;zakresu oceny prawdopodobnie byłoby sprzeczne z&nbsp;wymogami zgodności WCAG&nbsp;2 dla <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.cala_strona | strip_html | replace: '*', ''}}">całych witryn</a> i <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.cale_procesy | strip_html | replace: '*', ''}}">całych procesów</a> lub w&nbsp;inny sposób zniekształcałoby wyniki oceny.

## Przykład włączania stron do oceny

![Schemat witryny uniwersytetu ilustrujący zasadę włączania stron do wittryny](/images/ogolne/metodologia_3.svg)

Powyższy schemat pokazuje witrynę uniwersytetu złożoną z odrębnych obszarów; „Informacje dla studentów”, „Informacje dla wykładowców”, „Kursy” i&nbsp;„Biblioteka”. Aplikacja „Kursy” obejmuje „Kurs fizyki”, „Kurs medycyny” i&nbsp;„Kurs historii”, które są zgrupowane w&nbsp;tym obszarze. Witryna uniwersytecka ma również pojedyncze strony internetowe, takie jak informacje prawne, mapa witryny i&nbsp;inne strony wspólne dla wszystkich obszarów.

W powyższym przykładzie, jeśli witryna uniwersytetu jest wyznaczona do oceny w całości, to wszystkie przedstawione obszary są objęte oceną. Obejmuje to wszelkie zagregowane i osadzone treści, takie jak mapy kampusu, formularze płatności internetowej i fora dyskusyjne, także jeśli takie części pochodzą ze źródeł zewnętrznych. Jeśli natomiast tylko określony obszar witryny, taki jak „Kursy”, zostanie wyznaczony do oceny, wówczas zakresem oceny objęte są wszystkie części tego obszaru, a&nbsp;więc obszary poświęcone każdemu z&nbsp;kursów, a&nbsp;także strony internetowe wspólne dla wszystkich obszarów uniwersytetu. Zobacz także definicję <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wspolne_strony_internetowe | strip_html | replace: '*', ''}}">wspólne strony</a>.

## Typowe rodzaje witryn

Metodologia ta ma zastosowanie do szerokiej gamy typów stron internetowych. Poniżej przedstawiono uwagi dotyczące konkretnych sytuacji, zwracając uwagę, że strony internetowe mogą łączyć kilka aspektów. Zatem poniższa lista nie jest wyłączna i&nbsp;niewyczerpująca:

### Małe witryny

W przypadku witryn z kilkoma stronami procedura próbkowania zdefiniowana w [kroku 3: Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron) prawdopodobnie doprowadzi do wybrania większości lub wszystkich stron internetowych z&nbsp;docelowej witryny. W&nbsp;przypadkach, w&nbsp;których można ocenić wszystkie strony internetowe, procedurę próbkowania można pominąć, a&nbsp;za wybraną próbkę w&nbsp;pozostałych krokach uznaje się całą witrynę.

### Aplikacje internetowe

Aplikacje internetowe składają się zazwyczaj z dynamicznie generowanych treści i funkcjonalności (zobacz <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.stany_strony_internetowej | strip_html | replace: '*', ''}}">stany stron internetowych</a>.). Aplikacje internetowe są zazwyczaj bardziej złożone i&nbsp;interaktywne. Niektóre przykłady aplikacji internetowych to programy pocztowe, edytory dokumentów i&nbsp;sklepy internetowe. Aplikacje internetowe mogą być częścią większej strony internetowej, ale w&nbsp;kontekście tej metodologii mogą również stanowić odrębną stronę internetową. Oznacza to, że jest to indywidualna i&nbsp;odrębna jednostka do oceny.

**Uwaga**: Ze względu na wiele możliwości generowania treści i&nbsp;funkcjonalności w aplikacjach internetowych czasami nie jest możliwe wyczerpujące zidentyfikowanie każdej możliwej strony internetowej, jej stanu i&nbsp;funkcjonalności. Aplikacje internetowe zwykle wymagają więcej czasu i&nbsp;wysiłku, aby je ocenić, i&nbsp;zazwyczaj potrzebują większych próbek stron internetowych, aby odzwierciedlić różne typy treści, funkcjonalności i&nbsp;procesów.

### Witryny złożone

W niektórych przypadkach witryny mogą mieć wyraźnie wydzielone obszary, w&nbsp;których korzystanie z jednego obszaru nie wymaga, ani nie zależy od korzystania z&nbsp;innego obszaru witryny. Na przykład organizacja może zapewnić tylko dla swoich pracowników ekstranet, który jest połączony z&nbsp;publiczną witryną internetową, ale jest w&nbsp;inny sposób oddzielony, lub może mieć podstrony dla poszczególnych działów organizacji, z&nbsp;których każda wyraźnie się różni od innych. Takie wyodrębnione obszary można traktować jako oddzielne strony internetowe, z&nbsp;których każda może zostać poddana ocenie. W&nbsp;niektórych przypadkach mogą istnieć <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wspolne_strony_internetowe | strip_html | replace: '*', ''}}">wspólne strony internetowey</a>, takie jak informacje prawne, które należy rozpatrywać jako część każdego obszaru witryny.

**Uwaga**: Niektóre strony internetowe zapewniają dodatkową lub różną treść i&nbsp;funkcjonalność w&nbsp;zależności od użytkownika (zazwyczaj po zalogowaniu się). Ta dodatkowa treść i&nbsp;funkcjonalność jest zasadniczo częścią podstawowego celu i&nbsp;funkcjonalności witryny i&nbsp;dlatego nie jest uważana za oddzielny obszar witryny.

### Witryny w wielu wersjach

Niektóre witryny są dostępne w&nbsp;wielu wersjach, które są od siebie niezależne, to znaczy korzystanie z jednej wersji nie wymaga ani nie zależy od korzystania z&nbsp;innej wersji witryny. Na przykład witryna może mieć wersję mobilną i&nbsp;mogą istnieć wersje witryny w różnych językach, które spełniają tę cechę. Niektóre witryny są dostępne w&nbsp;wielu wersjach, które są od siebie niezależne, to znaczy korzystanie z&nbsp;jednej wersji nie wymaga, ani nie zależy od korzystania z&nbsp;innej wersji witryny.

**Uwaga**: Strony internetowe wykorzystujące techniki responsywnego projektowania (tzn. dostosowujące prezentację do sprzętu, oprogramowania i&nbsp;preferencji użytkownika) w&nbsp;przeciwieństwie do stron, na które użytkownicy zostali przekierowani z&nbsp;innych miejsc, nie są uznawane za niezależne wersje stron internetowych.

### Witryny responsywne

Responsywne techniki projektowania dostosowują kolejność, przepływ, a czasami także zachowanie treści, tak aby jak najlepiej pasowały do urządzenia, na którym są używane. Na przykład, aby dopasować zawartość i&nbsp;funkcjonalność do rozmiaru rzutni, rozdzielczości ekranu, orientacji ekranu i&nbsp;innych aspektów urządzenia mobilnego oraz kontekstu, w którym jest ono używane. W&nbsp;tej metodologii takie zmiany treści, funkcjonalności, wyglądu i&nbsp;zachowania nie są uważane za niezależne wersje stron internetowych, ale raczej za stany strony internetowej, które należy uwzględnić w zakresie oceny.

**Uwaga**: Należy wziąć pod uwagę urządzenia mobilne, systemy operacyjne i&nbsp;technologie wspomagające w&nbsp;przypadku witryn korzystających z&nbsp;elastycznych technik projektowania, w&nbsp;szczególności w&nbsp;[kroku 1.c: Określ zestaw technologii bazowych](#krok-1c-określ-zestaw-technologii-bazowych-obsługujących-dostępność).

## Konkretne konteksty oceny

Metodologia ta ma być elastyczna, aby ułatwić jej zastosowanie w&nbsp;różnych sytuacjach i&nbsp;kontekstach. Poniższe uwagi odnoszą się do konkretnych sytuacji i&nbsp;kontekstów oceny:

### Samoocena zgodności

Wewnętrzni ewaluatorzy i testerzy, którzy biorą udział w&nbsp;procesie programowania, często mają łatwiejszy dostęp do programistów i&nbsp;opiekunów witryn, środowisk programistycznych i&nbsp;hostingowych, narzędzi autorskich oraz materiałów wykorzystywanych do programowania i&nbsp;konserwacji. W&nbsp;szczególności przypadki użycia, analizy projektu, specyfikacje techniczne i&nbsp;dokumentacja oraz zasoby testowe mogą zwiększyć efektywność oceny i&nbsp;powinny być wykorzystywane tam, gdzie to możliwe.

### Zewnętrzna ocena zgodności

Niezależni zewnętrzni oceniający zazwyczaj mają mniej informacji o&nbsp;wewnętrznym oprogramowaniu witryn, obszarach i&nbsp;funkcjonalności witryny, ponieważ nie byli zaangażowani w&nbsp;jej pozyskiwanie oraz w&nbsp;sposób projektowania i&nbsp;rozwijania strony. Często osoby oceniające w&nbsp;takich sytuacjach muszą skontaktować się z&nbsp;właścicielem witryny lub progamistą, aby uzyskać niezbędne informacje, które czynią ocenę bardziej skuteczną.

### Ocena podczas rozwoju

Chociaż ta metodologia została zaprojektowana przede wszystkim do przeglądu stron internetowych, które już zostały zaprojektowane i&nbsp;wdrożone, bardzo ważna jest ocena dostępności na wszystkich etapach projektowania i&nbsp;wdrażania witryny, aby zapewnić jej zgodność. Wskazówki zawarte w&nbsp;tej metodologii mogą być przydatne na tych wcześniejszych etapach procesu projektowania i&nbsp;rozwoju, choć mogą być potrzebne pewne dostosowania. Ważne jest jednak, aby pamiętać, że oceny przeprowadzone na tych wcześniejszych etapach mogą szybko stać się nieaktualne poprzez wprowadzenie nawet drobnych zmian. W&nbsp;związku z&nbsp;tym oceny przeprowadzane na tych etapach nie powinny być wykorzystywane do składania deklaracji ani oświadczeń o&nbsp;zgodności dotyczących sfinalizowanej strony internetowej.

### Ocena złożonych witryn internetowych

Podczas oceny [witryn z wydzielonymi obszarami](#witryny-złożone), takimi jak sklep internetowy, obszar blogów i&nbsp;inne podstrony, przydatne może być przeprowadzenie najpierw osobnej oceny każdego obszaru strony internetowej zgodnie z&nbsp;tą metodologią, a&nbsp;następnie ogólnej oceny z próbkami z&nbsp;każdego obszaru strony internetowej i&nbsp;wszelkich wspólnych stron internetowych. Zapewniłoby to pełniejsze objęcie strony internetowej w&nbsp;całości, jak również zapewniłoby wgląd w&nbsp;sposób, w&nbsp;jaki każdy obszar witryny jest realizowany, który może się różnić w&nbsp;zależności od obszaru.

### Ocena witryn agregujących treści z innych źródeł

Witryny, które są generowane przy użyciu treści łączonych z&nbsp;różnych źródeł, takich jak portale z portletami, są zwykle znacznie trudniejsze do oceny ze względu na wiele różnych instancji treści, które mogą być generowane. Ogólnie rzecz biorąc, nie jest możliwe oddzielne ocenianie treści z&nbsp;ich źródeł, a&nbsp;raczej ich wyświetlanie użytkownikom po ich połączeniu.

### Ocena treści innych podmiotów

Treści osób trzecich nie są kontrolowane przez stronę internetową lub dostawców usług internetowych; na przykład treści generowane przez użytkowników strony internetowej na forum internetowym. W WCAG&nbsp;2 w&nbsp;części [Oświadczenie o zgodności częściowej](wcag21#54-oświadczenie-o-częściowej-zgodności--treść-umieszczana-przez-dostawców-zewnętrznych) w&nbsp;szczególny sposób uwzględnia się zgodność tego typu treści. W&nbsp;takich przypadkach osoby oceniające będą musiały ustalić, czy takie treści są regularnie monitorowane i&nbsp;naprawiane (w&nbsp;ciągu dwóch dni roboczych) oraz czy treści niezgodne są wyraźnie zidentyfikowane jako takie na wszystkich stronach internetowych, na których się pojawiają.

### Ponowna ocena witryny

Ocena witryny internetowej, zgodnie z tą metodologią, może być ponownie przeprowadzona po krótkim czasie; na przykład, gdy problemy są identyfikowane i&nbsp;naprawiane przez właściciela witryny lub jej twórcę, lub okresowo w&nbsp;celu monitorowania postępów. W takich przypadkach ocena może być przeprowadzona przy użyciu próbki stron internetowych, które zawierają:

 - Podzbiór stron internetowych, które zostały użyte w poprzedniej ocenie w&nbsp;celu ułatwienia porównywalności wyników;
 - Podzbiór stron internetowych, w których poprawiono dostępność na podstawie wyników poprzednio dokonywanej oceny;

O ile na stronie internetowej nie wprowadzono istotnych zmian, zwykle nie ma potrzeby zmiany wielkości wybranej próbki strony internetowej ani podejścia zastosowanego do próbkowania. Liczba zastąpionych stron internetowych w&nbsp;nowej próbce wynosi zazwyczaj około połowy pierwotnej próbki, choć można ją zwiększyć, gdy strony internetowe w&nbsp;większości są zgodne z WCAG 2.

### Ocena na dużą skalę

Przeprowadzanie masowej oceny wielu stron internetowych, na przykład na potrzeby krajowych lub międzynarodowych badań ankietowych, jest zazwyczaj przeprowadzane przede wszystkim przy użyciu automatycznych narzędzi oceny. Stosunkowo niewiele stron internetowych poddawanych jest pełnej kontroli ręcznej. Takie oceny zwykle nie uwzględniają niezbędnej jakościowej oceny zgodności dla każdej witryny, dla której opracowano tę metodologię.

## Procedura oceny

W tej części opisano etapy i czynności związane z&nbsp;procedurą oceny. Etapy niekoniecznie muszą być sekwencyjne. Dokładna kolejność działań przeprowadzanych w kolejnych etapach oceny zależy również od rodzaju witrynyy, celu oceny i&nbsp;stosowanego przez ewaluatora. Niektóre działania mogą się pokrywać lub mogą być prowadzone równolegle. Poniższy schemat ilustruje iteracje pomiędzy etapami zdefiniowanymi w tej części:

![Procedura oceny - iteracje między etapami procedury oceniania](/images/ogolne/metodologia_2.svg)

Powyższy schemat przepływu pracy przedstawia pięć następujących po sobie kroków: 1.&nbsp;Ustal zakres oceny; 2.&nbsp;Przeprowadź rekonesans witryny; 3.&nbsp;Wybierz reprezentatywną próbkę stron; 4.&nbsp;Wykonaj audyt wybranej próbki i 5.&nbsp;Sporządź raport wyników. Każdy krok ma strzałkę do następnego kroku i&nbsp;strzałki do wszystkich poprzednich kroków. Schemat obrazuje, w&nbsp;jaki sposób osoby oceniające przechodzą z&nbsp;jednego kroku do następnego i&nbsp;mogą powrócić do każdego poprzedniego kroku w&nbsp;procesie, gdy podczas procesu oceny zostaną ujawnione nowe informacje.

## Krok 1: Ustal zakres oceny

**Wymaganie metodologiczne 1**: Ustal zakres oceny zgodnie z [wymaganiem metodologicznym 1.a](#krok-1a-określ-zakres-stron-witryny), [wymaganiem metodologicznym 1.b](#krok-1b-określ-wymagany-poziom-zgodności) i [wymaganiem metodologicznym 1.c](#krok-1c-określ-zestaw-technologii-bazowych-obsługujących-dostępność) oraz opcjonalnie z [wymaganiem metodologicznym 1.d.](#krok-1d-określ-dodatkowe-wymagania-oceny)

Na tym etapie określa się ogólny zakres oceny. Jest to podstawowy krok, który wpływa na kolejne etapy procedury oceny. Najlepiej ustalić zakres oceny w&nbsp;porozumieniu z komisarzem ds. oceny (który może, ale nie musi być właścicielem strony internetowej), aby zagwarantować spełnienie oczekiwań co do zakresu oceny. Na tym etapie może być konieczne wstępne rozpoznanie witryny, aby lepiej poznać jej specyfikę i&nbsp;wymagania oceny. Szczegółowa eksploracja witryny jest przeprowadzana w&nbsp;[kroku 2: Przeprowadź rekonesans witryny](#krok-2-przeprowadź-rekonesans-witryny).

### Krok 1.a: Określ zakres stron witryny

**Wymaganie metodologiczne 1.a**: Zdefiniuj [witrynę] do oceny zgodnie z&nbsp;[zakresem stosowania](#zakres-stosowania) metodologii, tak aby dla każdej strony internetowej na witrynie było jasne, czy znajduje się ona w&nbsp;zakresie stron podlegających ocenie.

Na tym etapie definiuje się witrynę docelową (strony i&nbsp;stany stron internetowych podlegające ocenie). Zakres witryny jest określany zgodnie z warunkami określonymi w sekcji [Zakres stosowania.](#zakres-stosowania)

Aby uniknąć późniejszych nieporozumień, wynikających z&nbsp;niedopasowania oczekiwań zlecającego ocenę, zamierzeń oceniającego oraz oczekiwań odbiorców raportu ustaleń, ważne jest takie zdefiniowanie docelowej witryny, aby było jasne, które strony internetowe mieszczą się w&nbsp;zakresie witryny. W&nbsp;miarę możliwości zaleca się stosowanie formalizacji, w&nbsp;tym [wyrażeń regularnych](https://pl.wikipedia.org/wiki/Wyra%C5%BCenie_regularne) i&nbsp;wykazów adresów internetowych (URI). Ważne jest również udokumentowanie różnych istotnych z&nbsp;punktu widzenia oceny aspektów ocenianej witryny, takich jak:

 - Wykorzystywanie treści i usług stron trzecich;
 - Mobilne i językowe wersje witryny;
 - Wyodrębnione obszary, np. sklep internetowy, które pomimo innego adresu URI są uznawane za część witryny wyznaczonej do oceny (takie obszary mogą być trudne do zidentyfikowania).

### Krok 1.b: Określ wymagany poziom zgodności

**Wymaganie metodologiczne 1.b**: Określ referencyjny [poziom zgodności](wcag21#521-poziom-zgodności) z WCAG&nbsp;2 („A”, „AA” lub „AAA”).

Częścią inicjowania procesu ewaluacji jest określenie, który poziom zgodności z&nbsp;WCAG 2 („A”, „AA” lub „AAA”) będzie punktem odniesienia dla oceny. Ogólnie przyjętym i zalecanym celem jest zgodność z&nbsp;WCAG 2 na poziomie AA.

**Uwaga**: Często przydatna jest ocena wykraczająca poza wymagany poziom zgodności, aby uzyskać pełniejszy obraz dostępności witryny. Na przykład, chociaż witryna może nie spełniać określonego poziomu zgodności w&nbsp;pełni, ale może spełniać niektóre wymagania z&nbsp;wyższego poziomu zgodności. Posiadanie tych informacji może pomóc w&nbsp;bardziej efektywnym planowaniu przyszłych ulepszeń.

### Krok 1.c. Określ zestaw technologii bazowych obsługujących dostępność

**Wymaganie metodologiczne 1.c**: Określ podstawowy zestaw kombinacji przeglądarek, technologii wspomagających i&nbsp;innych <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.program_uzytkownika | strip_html | replace: '*', ''}}">programów użytkownika</a> (np. odtwarzaczy mediów), w&nbsp;których treści i&nbsp;funkcje witryny mają być <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc | strip_html | replace: '*', ''}}">obsługiwane pod względem dostępności.</a> Na przykład, „FireFox z NVDA”, „Internet Explorer (IE) z JAWS” i&nbsp;„Apple z&nbsp;VoiceOver” mogą być takim podstawowym zestawem.

W szczególności w przypadku nowych technologii internetowych nie zawsze jest możliwe zapewnienie, że każda funkcja dostępności obecna na stronie internetowej, np. taka jak funkcja „pokaż napisy” w&nbsp;odtwarzaczu multimedialnym, będzie obsługiwana przez każdą możliwą kombinację systemu operacyjnego, przeglądarki internetowej, technologii wspomagającej i&nbsp;innych programów użytkowników.

WCAG 2 nie określa z góry, które kombinacje funkcji i&nbsp;technologii muszą być obsługiwane, ponieważ zależy to od konkretnego kontekstu witryny, w&nbsp;tym jej języka, technologii internetowych wykorzystywanych do tworzenia treści oraz aktualnie dostępnych programów użytkownika. Więcej wskazówek na temat obsługi dostępności znajduje się w&nbsp;opracowaniu [Understanding Accessibility Support.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance#uc-accessibility-support-head)

W trakcie tego etapu oceniający określa minimalny zestaw kombinacji systemów operacyjnych, przeglądarek internetowych, technologii wspomagających i&nbsp;innych programów użytkowników, z&nbsp;którymi strona ma pracować, i&nbsp;jest to zgodne z&nbsp;wytycznymi WCAG&nbsp;2 dotyczącymi obsługi dostępności (link powyżej). Zestaw technologii bazowych najlepiej ustalić w&nbsp;porozumieniu z&nbsp;komisarzem ds. oceny, aby zagwarantować, że oczekiwania zlecającego i&nbsp;oceniającego co do poziomu wsparcia technologii będą takie same.

Na tym etapie może być konieczna wstępna eksploracja witryny, aby lepiej poznać jej specyfikę i&nbsp;wymagania oceny. Szczegółowa eksploracja witryny jest przeprowadzana w&nbsp;[kroku 2: Przeprowadź rekonesans witryny.](#krok-2-przeprowadź-rekonesans-witryny)

Właściciel witryny i jej twórca również mogą posiadać taką listę kombinacji, dla których witryna została zaprojektowana, co może być punktem wyjścia dla tego kroku. W&nbsp;zależności od celu oceny taka lista może wymagać aktualizacji, na przykład w&nbsp;celu oceny, jak dobrze działa strona internetowa z&nbsp;bardziej aktualnymi przeglądarkami.

**Uwaga**: Ta wstępna bazowa lista technologii nie ogranicza oceniającego w&nbsp;możliwościach wykorzystania później dodatkowych systemów operacyjnych, przeglądarek internetowych, technologii wspomagających i&nbsp;innych programów użytkowników, na przykład w&nbsp;celu oceny treści, które nie zostały zauważone na tym wczesnym etapie procesu oceny. W&nbsp;takim przypadku bazowy zestaw technologii jest rozszerzany o&nbsp;dodatkowe narzędzia, które zostały wykorzystane.

**Uwaga**: W przypadku niektórych witryn internetowych w&nbsp;sieciach zamkniętych, takich jak witryna intranetowa, w&nbsp;których znani są zarówno użytkownicy, jak i&nbsp;komputery używane do uzyskania dostępu do witryny, bazowa lista technologii może być ograniczona do systemów operacyjnych, przeglądarek internetowych i&nbsp;technologii pomocniczych używanych w&nbsp;ramach tej zamkniętej sieci. Jednak w&nbsp;większości przypadków bazowa lista technologii jest znacznie szersza i&nbsp;obejmuje większość aktualnie używanych przez osoby niepełnosprawne w&nbsp;danym regionie geograficznym i&nbsp;społeczności językowej programów użytkownika i&nbsp;innych technologii.

### Krok 1.d: Określ dodatkowe wymagania oceny

**Wymaganie metodologiczne 1.d**: Określ wszelkie dodatkowe wymagania dotyczące oceny uzgodnione przez <a href="#" data-toggle="tooltip" data-original-title="{{site.data.definicje.oceniajacy | strip_html | replace: '*', ''}}">oceniającego</a> i <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.komisarz_ds_oceny | strip_html | replace: '*', ''}}">komisarza ds. oceny (opcjonalnie).</a> Komisarz ds. oceny może być zainteresowany dodatkowymi informacjami wykraczającymi poza to, co jest potrzebne do oceny stopnia zgodności badanej witryny z&nbsp;WCAG&nbsp;2. Na przykład, komisarz ds. oceny może być zainteresowany:

 - oceną dodatkowych stron internetowych wykraczających poza to, co jest potrzebne do utworzenia reprezentatywnej próbki stron;
 - raportami o wszystkich wystąpieniach problemów zamiast reprezentatywnych przykładów typów problemów;
 - analizą konkretnych przypadków użycia, sytuacji i&nbsp;grup użytkowników w&nbsp;interakcjach z badaną witryną;
 - propozycjami i opisami rozwiązań innych napotkanych problemów, nieobjętych zakresem oceny;
 - oceną dokonaną przez użytkowników z&nbsp;niepełnosprawnościami;
 - sporządzeniem określonej dokumentacji lub stosowaniem konkretnych szablonów raportowania.

Takie dodatkowe wymagania dotyczące, które są uzgodnione z&nbsp;osobą oceniającą, muszą zostać wcześniej wyjaśnione i&nbsp;udokumentowane. Należy je również odzwierciedlić w&nbsp;raporcie wynikowym, na przykład w&nbsp;celu wyjaśnienia, w&nbsp;jaki sposób dokonano wyboru próbki do audytu.

## Krok 2: Przeprowadź rekonesans witryny

**Wymaganie metodologiczne 2**: Przejrzyj witrynę, która ma być oceniana zgodnie z [wymaganiem metodologicznym 2.a](#krok-2a-zidentyfikuj-wspólne-strony-internetowe-witryny), [wymaganiem metodologicznym 2.b](#krok-2b-zidentyfikuj-niezbędne-funkcjonalności), [wymaganiem metodologicznym 2.c](#krok-2c-zidentyfikuj-różne-typy-stron-internetowych), [wymaganiem metodologicznym 2.d](#krok-2d-zidentyfikuj-użyte-technologie-internetowe) i [wymaganiem metodologicznym 2.e.](#krok-2e-zidentyfikuj-inne-istotne-strony-internetowe)

Na tym etapie oceniający przegląda witrynę, która ma zostać poddana ocenie, aby się z&nbsp;nią zapoznać, zrozumieć jej cel, przeznaczenie, organizację treści, funkcje. Te istotne aspekty witryny niekoniecznie są od razu widoczne, zwłaszcza dla ewaluatorów zewnętrznych, którzy wcześniej nie znali witryny.

Niekiedy podczas tego wstępnego przeglądu nie będzie też możliwe wyczerpujące określenie i&nbsp;zestawienie wszystkich funkcjonalności, rodzajów stron internetowych i technologii wykorzystywanych do realizacji strony internetowej i&nbsp;jej aplikacji. Analiza wstępna przeprowadzona na tym etapie jest zwykle dopracowywana w późniejszych krokach – [kroku 3 (Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron)) i [kroku 4 (Wykonaj audyt wybranej próbki)](#krok-4-wykonaj-audyt-wybranej-próbki)), gdy audytor dowiaduje się więcej na temat badanej witryny.

Zazwyczaj informację dotyczące tego kroku najlepiej jest uzyskać od właścicieli i projektantów witryny.

**Uwaga**: Przeprowadzenie wstępnych pobieżnych testów podczas tego kroku pomaga zidentyfikować strony internetowe, które później będą przydatne do bardziej szczegółowej oceny. Na przykład, osoba oceniająca może zidentyfikować strony, które wydają się być pozbawione kontrastu kolorów, strony z zaburzoną strukturą dokumentu lub niespójną nawigacją.

**Uwaga**: Aby wykonać ten krok, konieczne jest, aby osoba oceniająca miała dostęp do wszystkich istotnych części witryny. Na przykład, konieczne może być utworzenie kont lub zapewnienie w&nbsp;inny sposób dostępu do zastrzeżonych obszarów witryny internetowej, które są częścią oceny. Zapewnienie ewaluatorom takiego dostępu może wymagać szczególnych środków ostrożności w&nbsp;zakresie bezpieczeństwa i&nbsp;ochrony prywatności.

### Krok 2.a: Zidentyfikuj wspólne strony internetowe witryny

**Wymaganie metodologiczne 2.a**: Określ strony wspólne dla całej ocenianej witryny (mogą to być także stany stron).

Przejrzyj ocenianą witrynę internetową, aby zidentyfikować wszystkie strony wspólne dla całej witryny. W&nbsp;aplikacjach internetowych mogą to być również stany stron internetowych.

Zazwyczaj są one połączone bezpośrednio z&nbsp;głównego punktu wejścia (strony głównej) docelowej witryny i&nbsp;często połączone z&nbsp;nagłówkiem, nawigacją i&nbsp;sekcją innych stron internetowych. Wynikiem tego kroku jest lista wszystkich wspólnych stron internetowych strony docelowej.

### Krok 2.b: Zidentyfikuj niezbędne funkcjonalności

**Wymaganie metodologiczne 2.b**: Zidentyfikuj niezbędne funkcjonalności badanej witryny.

Zbadaj docelową stronę internetową, aby określić jej podstawową funkcjonalność. Podczas gdy niektóre funkcjonalności będą łatwe do zidentyfikowania, inne będą wymagały bardziej celowego odkrycia. Na przykład, łatwiejsze może być zidentyfikowanie funkcji zakupu produktów w&nbsp;sklepie internetowym niż funkcji przewidzianej dla sprzedawców do sprzedaży produktów za pomocą sklepu. Wynikiem tego kroku jest lista funkcji, które użytkownicy mogą wykonywać w&nbsp;witrynie. Lista ta zostanie wykorzystana w następnych krokach, aby pomóc w&nbsp;wyborze reprezentatywnych stron internetowych do oceny.

**Uwaga**: Celem tego kroku nie jest wyczerpująca identyfikacja wszystkich funkcji strony internetowej, ale określenie tych, które są niezbędne do osiągnięcia celu badanej witryny. To wpłynie na późniejszy wybór stron internetowych i&nbsp;ich ocenę. Inne funkcjonalności również zostaną uwzględnione w&nbsp;ocenie, ale na skutek innych mechanizmów selekcji.

#### Przykłady funkcjonalności strony internetowej

Niektóre przykłady funkcjonalności strony internetowej obejmują:

 - wybór i zakup produktów ze sklepu internetowego;
 - wypełnianie i przesyłanie formularzy kontaktowych;
 - rejestracja konta użytkownika.

### Krok 2.c: Zidentyfikuj różne typy stron internetowych

**Wymaganie metodologiczne 2.c**: Zidentyfikuj wszystkie typy stron internetowych na witrynie i&nbsp;ich stany.

Strony internetowe i ich stany o różnych stylach, układach, strukturach i&nbsp;funkcjach często mają różną obsługę w zakresie dostępności. Są one często generowane przez różne szablony i&nbsp;skrypty lub zostały stworzone przez różne osoby. Mogą wyglądać inaczej, zachowywać się inaczej i&nbsp;zawierać różne treści w&nbsp;zależności od konkretnego użytkownika witryny i&nbsp;kontekstu.

Na tym etapie ewaluator bada docelową witrynę internetową, aby zidentyfikować różne **typy stron** i&nbsp;stany stron internetowych. Wynikiem tego kroku jest lista opisów zidentyfikowanych typów treści, a&nbsp;nie konkretnych wystąpień stron i&nbsp;stanów stron internetowych. Ta lista posłuży w&nbsp;następnych krokach do wyboru reprezentatywnej próbki stron, w&nbsp;której powinny się znaleźć instancje różnych typów stron internetowych.

#### Przykłady typów stron internetowych

Niektóre przykłady różnych typów stron i&nbsp;stanów stron internetowych, których osoby oceniające mogą szukać:

 - strony z różnymi stylami, układem, strukturą, nawigacją, interakcją i&nbsp;wyglądem;
 - strony z różnymi rodzajami treści, takimi jak formularze, tabele, listy, nagłówki, multimedia i skrypty;
 - strony z różnymi elementami funkcjonalnymi, takimi jak selektor dat, lightbox, suwak i&nbsp;inne;
 - strony wykorzystujące różne technologie, takich jak HTML, CSS, JavaScript, WAI-ARIA, PDF itp.;
 - strony z różnych obszarów witryny (strona główna, sklep internetowy, działy itp.), w&nbsp;tym wszelkie aplikacje;
 - strony z różnymi stylami kodowania i&nbsp;utworzonymi przy użyciu różnych szablonów (jeśli jest to znane oceniającemu);
 - strony autorstwa różnych osób, działów i&nbsp;innych podmiotów (jeśli jest to znane oceniającemu);
 - strony, które zmieniają wygląd i&nbsp;zachowanie w&nbsp;zależności od użytkownika, urządzenia, przeglądarki, kontekstu i&nbsp;ustawień;
 - strony z dynamiczną treścią, komunikatami o błędach, oknami dialogowymi, wyskakującymi oknami i&nbsp;innymi interakcjami.

### Krok 2.d: Zidentyfikuj użyte technologie internetowe

**Wymaganie metodologiczne 2.d**: Zidentyfikuj użyte do tworzenia treści witryny technologie internetowe, na których opiera się zgodność.

Na tym etapie identyfikuje się technologie internetowe które muszą być obsługiwane, aby treść spełniała wymogi zgodności. Obejmuje to podstawowe technologie internetowe, takie jak HTML i&nbsp;CSS, pomocnicze technologie internetowe, takie jak JavaScript i&nbsp;WAI-ARIA, jak również specyficzne technologie internetowe, takie jak SMIL, SVG i&nbsp;PDF. Wynikiem tego kroku jest lista wiarygodnych technologii internetowych użytych do tworzenia treści witryny. Lista ta posłuży w&nbsp;następnych krokach do wyboru reprezentatywnej próbki stron.

**Uwaga**: Tam, gdzie to możliwe, często przydatne jest również zidentyfikowanie wersji i&nbsp;konfiguracji użytego systemu zarządzania treścią, ponieważ może to być istotne dla wyjaśnienia wyników oceny. Istotne mogą być również wszelkie biblioteki i&nbsp;komponenty użyte do utworzenia strony internetowej, takie jak Dojo, jQuery i&nbsp;inne. Zwłaszcza w&nbsp;przypadku aplikacji internetowych znaczna część obsługi dostępności jest wbudowana w biblioteki i&nbsp;komponenty, a&nbsp;ocena może stać się bardziej efektywna i&nbsp;wydajna po ich zidentyfikowaniu.

### Krok 2.e: Zidentyfikuj inne istotne strony internetowe

**Wymóg metodologiczny 2.e**: Zidentyfikuj inne strony i stany stron internetowych, które są istotne dla osób z&nbsp;niepełnosprawnościami i&nbsp;dla dostępności witryny.

Niektóre witryny zawierają specjalne strony i&nbsp;stany stron internetowych, które są szczególnie istotne dla osób z&nbsp;niepełnosprawnościami i&nbsp;dla dostępności witryny. Wynikiem tego kroku jest lista takich stron i&nbsp;stanów stron internetowych, jeśli nie zostały one jeszcze zidentyfikowane w&nbsp;ramach [kroku 2.a: Zidentyfikuj wspólne strony internetowe witryny](#krok-2a-zidentyfikuj-wspólne-strony-internetowe-witryny).

#### Przykłady innych istotnych stron internetowych

Przykłady innych istotnych stron i stanów stron internetowych obejmują:

 - strony z wyjaśnieniem funkcji dostępności witryny;
 - strony z pomocą w zakresie korzystania z witryny;
 - strony z objaśniające ustawienia, preferencje, opcje, skróty itp.;
 - strony z danymi kontaktowymi, wskazówkami i&nbsp;instrukcjami pomocy technicznej.

## Krok 3: Wybierz reprezentatywną próbkę stron

**Wymaganie metodologiczne 3**: Wybierz reprezentatywną próbkę stron internetowych z witryny zgodnie z [wymaganiem metodologicznym 3.a](#krok-3a-uwzględnij-próbkę-strukturalną), [wymaganiem metodologicznym 3.b](#krok-3b-uwzględnij-losowo-wybraną-próbkę) i [wymaganiem metodologicznym 3.c.](#krok-3c-uwzględnij-całe-procesy)

Podczas tego kroku oceniający wybiera do oceny próbkę stron internetowych i&nbsp;ich stany, które są reprezentatywne dla badanej witryny. Celem tego wyboru jest zapewnienie, że wyniki oceny z&nbsp;rozsądną pewnością będą odzwierciedlać dostępność witryny.

W przypadkach, gdy możliwe jest dokonanie oceny wszystkich stron i&nbsp;stanów stron internetowych witryny internetowej, co jest wysoce zalecane, procedura wyboru próbki stron może zostać pominięta. W&nbsp;tych przypadkach „wybraną próbką” w pozostałych etapach procesu oceny jest cała witryna. W&nbsp;niektórych przypadkach, np. w&nbsp;przypadku małych witryn, procedura próbkowania może skutkować wyborem wszystkich stron i stanów stron internetowych.

Rzeczywista wielkość próbki stron internetowych i&nbsp;stanów stron internetowych potrzebnych do oceny strony internetowej zależy od wielu czynników, w&nbsp;tym:

- **Rozmiar witryny** - witryny z większą liczbą stron internetowych zazwyczaj wymagają większej próbki do oceny.
- **Wiek witryny** - starsze witryny mają zazwyczaj więcej treści (często niełatwych do znalezienia) o&nbsp;różnym stopniu złożoności, spójności oraz procesach projektowania i&nbsp;rozwoju, dlatego do oceny zwykle wymagana jest większa próbka.
- **Złożoność witryny** - większa złożoność wymaga większej próby do oceny; należy rozważyć następujące kwestie:
   - **Jak interaktywna jest treść** - witryny z treściami bogatymi w&nbsp;interakcje wymagają większych próbek, aby uwzględnić funkcje dostarczane przez stronę internetową i&nbsp;różne stany, które mogą mieć poszczególne strony internetowe;
   - **W jaki sposób treść jest generowana** - witryny zawierające treści agregowane z różnych źródeł lub przetwarzane w&nbsp;miarę ich udostępniania zazwyczaj wymagają większych próbek, aby uwzględnić kombinacje treści, które mogą być generowane;
   - **W jaki sposób treść jest wdrażana** - witryny dostępne w różnych wersjach, są obsługiwane zgodnie z użytkownikami i&nbsp;ich preferencjami lub przystosowują się do urządzeń dostępowych, wymagają większych próbek, aby uwzględnić te różne sytuacje.
- **Spójność witryny** - mniejsza spójność wymaga większej próbki do oceny; należy rozważyć następujące kwestie:
   - **Różnorodność typów stron internetowych** - witryny z szerszą gamą typów stron internetowych  wymagają większych próbek do oceny (zobacz [krok 2.c: Zidentyfikuj różne typy stron internetowych](#krok-2c-zidentyfikuj-różne-typy-stron-internetowych));
   - **Różnorodność funkcjonalności** - witryny oferujące szerszą gamę funkcjonalności, w szczególności różne typy aplikacji, wymagają do oceny większych próbek (zobacz [krok 2.b: Zidentyfikuj niezbędne funkcjonalności](#krok-2b-zidentyfikuj-niezbędne-funkcjonalności));
   - **Różnorodność technologii** - witryny z szerszą gamą używanych technologii internetowych  wymagają większych próbek do oceny (zobacz krok 2.d: Zidentyfikuj użyte technologie internetowe);
   - **Różnorodność stylów kodowania** - witryny z szerszą gamą stylów kodowania (zazwyczaj są to różne skrypty, które generują kod, szablony, obszary pochodzące od różnych autorów stron internetowych) wymagają większych próbek do oceny.
- **Przestrzeganie procedur projektowych** - nieprzestrzeganie wymaga większej próbki do oceny; rozważ następujące kwestie:
   - **Sformalizowanie procesu** - witryny ze sformalizowanymi procesami rozwoju i zapewniania jakości wykazują większą spójność w&nbsp;kodowaniu i&nbsp;jakości stron internetowych, dlatego zwykle wymagają mniejszych próbek do oceny;
   - **Dokształcanie programistów** - witryny z projektantami, programistami i&nbsp;autorami treści, którzy przechodzą regularne szkolenia, mają tendencję do bardziej spójnego działania w&nbsp;zakresie dostępności, dlatego zwykle wymagają mniejszych próbek do oceny;
   - **Wykorzystywane narzędzia programistyczne** - witryny opracowywane i&nbsp;utrzymywane przy użyciu spójnego zestawu narzędzi, takich jak system zarządzania treścią (CMS), są również bardziej spójne i&nbsp;wymagają mniejszych próbek do oceny;
   - **Liczba autorów stron internetowych** - witryny tworzone i&nbsp;utrzymywane przez bardziej ograniczony zestaw autorów stron internetowych, w&nbsp;tym redaktorów treści, wydają się być bardziej spójne i&nbsp;wymagają mniejszych próbek do oceny.
- **Wymagany poziom zaufania -** większe wymagane zaufanie do wyników oceny często wymaga oceny większej próbki.
- **Dostępność wyników wcześniejszej oceny** - gdy osoby oceniające mają dostęp do wcześniejszych wyników oceny, w&nbsp;tym wyników testów z&nbsp;ręcznego i&nbsp;automatycznego testowania dostępności, mogą być wymagane mniejsze próbki.

Wybór dokonany podczas tego kroku opiera się początkowo na eksploracji przeprowadzonej w [kroku 2: Przeprowadź rekonesans witryny.](#krok-2-przeprowadź-rekonesans-witryny). Wybór jest również stale udoskonalany podczas następującego [kroku 4: Wykonaj audyt wybranej próbki)](#krok-4-wykonaj-audyt-wybranej-próbki), ponieważ oceniający dowiadują się więcej o&nbsp;poszczególnych aspektach ocenianej witryny.

### Krok 3.a: Uwzględnij próbkę strukturalną

**Wymaganie metodologiczne 3.a**: Wybierz strony i stany stron internetowych, które odzwierciedlają wszystkie zidentyfikowane (1)&nbsp;wspólne strony internetowe, (2)&nbsp;niezbędne funkcje, (3)&nbsp;typy stron internetowych, (4)&nbsp;spolegliwe technologie internetowe oraz (5)&nbsp;inne istotne strony internetowe

1. Wybierz próbkę stron internetowych i stanów stron internetowych, które zawierają:

1. Wszystkie typowe strony i stany stron internetowych, które zostały zidentyfikowane w [kroku 2.a: Zidentyfikuj wspólne strony witryny](#krok-2a-zidentyfikuj-wspólne-strony-internetowe-witryny)
2. Wszystkie inne istotne strony i stany stron internetowych, które zostały zidentyfikowane w&nbsp;[kroku 2.e: Zidentyfikuj inne istotne strony internetowe;](#krok-2e-zidentyfikuj-inne-istotne-strony-internetowe)
3. Jeśli nie zostało to odzwierciedlone w poprzednich punktach, wybierz dodatkowe strony i stany stron za pomocą:
   a. Treści z każdą niezbędną funkcjonalnością określoną w [kroku 2.b: Zidentyfikuj niezbędne funkcjonalności witryny](#krok-2b-zidentyfikuj-niezbędne-funkcjonalności);
   b. Treść z różnymi typami stron internetowych zidentyfikowanych w [kroku 2.c: Zidentyfikuj różne typy stron internetowych](#krok-2c-zidentyfikuj-różne-typy-stron-internetowych);
   c. Treści dostarczane przy użyciu technologii internetowych określonych w [kroku 2.d: Zidentyfikuj użyte technologie internetowe](#krok-2d-zidentyfikuj-użyte-technologie-internetowe).

**Uwaga**: Pojedyncza strona lub stan strony internetowej może odzwierciedlać więcej niż jedno z powyższych kryteriów. Na przykład pojedyncza strona internetowa może być reprezentatywna dla określonego układu projektu, funkcjonalności i&nbsp;zastosowanych technologii internetowych. Celem tego kroku jest zapewnienie reprezentatywnej próbki różnych typów stron i&nbsp;stanów stron, funkcjonalności i&nbsp;technologii internetowych występujących w&nbsp;witrynie. Staranny wybór tych reprezentatywnych instancji może znacznie zmniejszyć wymaganą wielkość próbki przy zachowaniu odpowiedniej reprezentacji całej witryny. Liczba wymaganych wystąpień stron internetowych i&nbsp;ich stanów zależy od konkretnych aspektów strony internetowej wyjaśnionych w poprzedniej sekcji, czynników wpływających na wielkość próby.

### Krok 3.b: Uwzględnij losowo wybraną próbkę

**Wymaganie metodologiczne 3.b**: Wybierz losową próbkę stron i&nbsp;stanów stron internetowych i&nbsp;włącz je do audytu.

Losowo wybrana próbka stron internetowych i&nbsp;stanów stron internetowych służy jako wskaźnik pozwalający sprawdzić, czy próbka strukturalna wybrana w poprzednich krokach jest wystarczająco reprezentatywna dla treści zamieszczonych na stronie internetowej. Zaufanie do ogólnego wyniku oceny wzrasta, gdy wyniki oceny obu metod selekcji są ze sobą skorelowane.

Liczba stron internetowych i stanów stron internetowych, które należy losowo wybrać, wynosi **10% próby strukturalnej** wybranej w&nbsp;poprzednich krokach. Na przykład, jeśli próbka strukturalna wybrana dla strony internetowej dała 80 stron i&nbsp;stanów stron internetowych, wówczas wielkość próbki losowej wynosi 8&nbsp;stron i&nbsp;stanów stron internetowych. (**Uwaga**: wielkość próbki strukturalnej jest inna niż wielkość witryny.)

Aby dokonać tego wyboru, losowo wybierz unikalne wystąpienia stron i&nbsp;stanów stron internetowych z&nbsp;ocenianej witryny, które nie są jeszcze częścią próbki strukturalnej uzyskanej w poprzednich krokach. W&nbsp;zależności od rodzaju witryny i&nbsp;dostępu, jaki ma do niej ewaluator, do tego wyboru można zastosować różne techniki. Między innymi:

 - skorzystanie z narzędzia, które przejdzie przez witrynę i&nbsp;zaproponuje listę losowo wybranych stron i&nbsp;stanów stron internetowych;
 - skorzystanie ze skryptu, który wygeneruje listę wszystkich stron i&nbsp;stanów stron internetowych dostępnych na witrynie, do wyboru;
 - skorzystanie z dzienników serwera, wyszukiwarek i&nbsp;innych metod dotarcia do losowo wybranej próbki.

Udokumentuj strony i stany stron internetowych, które zostały losowo wybrane, ponieważ będą musiały zostać porównane z&nbsp;pozostałą próbką strukturalną w [kroku 4.c: Porównaj próbki strukturalne i&nbsp;losowe.](#krok-4c-porównaj-próbki-strukturalne-i-losowe)

**Uwaga**: Chociaż próbka losowa nie musi być wybierana według kryteriów ściśle naukowych, to zakres wyboru musi obejmować cały zakres strony internetowej (można wybrać dowolną stronę i&nbsp;dowolny stanu strony na witrynie), a&nbsp;wybór poszczególnych stron i&nbsp;stanów stron internetowych nie powinien następować według przewidywalnego wzorca. Rejestracja metody zastosowanej do wygenerowania próbki losowej jest ważna dla powtarzalności i&nbsp;wiarygodności wyników.

### Krok 3.c: Uwzględnij całe procesy

**Wymaganie metodologiczne 3.c**: Uwzględnij w próbce wszystkie strony i&nbsp;stany stron internetowych, które są częścią całych procesów.

Wybrana próbka musi obejmować wszystkie strony i&nbsp;stany stron, które należą do serii stron prezentujących każdy proces. Żadna strona internetowa ani stan strony internetowej w&nbsp;wybranej próbce nie może być częścią procesu, chyba że w&nbsp;wybranej próbce uwzględnione są wszystkie inne strony internetowe i&nbsp;stany stron internetowych, które są częścią tego procesu.

Wykonaj poniższe kroki, aby włączyć do próbki niezbędne strony i&nbsp;stany stron:

1. Dla każdej strony i stanu strony internetowej wybranych w [kroku 3.a: Uwzględnij próbkę strukturalną](#krok-3a-uwzględnij-próbkę-strukturalną) i&nbsp;[krok 3.b: Uwzględnij losowo wybraną próbkę](#krok-3b-uwzględnij-losowo-wybraną-próbkę), która jest częścią procesu, znajdź punkt początkowy (stronę internetową lub stan strony internetowej) dla procesu i&nbsp;uwzględnij go w&nbsp;wybranej próbce;
2. Dla każdego punktu początkowego procesu określ i&nbsp;zapisz co najmniej domyślną sekwencję stron i&nbsp;stanów stron internetowych niezbędnych, aby zakończyć proces. Dodaj te strony i&nbsp;stany stron do wybranej próbki.

   **Uwaga**: Domyślna sekwencja jest zgodna ze standardowym przypadkiem użycia, opisującym domyślną ścieżkę przez cały proces. Zakłada się, że nie ma błędów wprowadzania danych przez użytkownika ani wyboru dodatkowych opcji. Na przykład w przypadku aplikacji sklepu internetowego użytkownik przejdzie do kasy, potwierdzi domyślną opcję płatności, poprawnie poda wszystkie wymagane szczegóły płatności i&nbsp;dokona zakupu bez zmiany zawartości koszyka, korzystając z zapisanego profilu użytkownika, wybierając alternatywne opcje płatności lub adresu wysyłki, podając błędne dane wejściowe itd.
3. Dla każdego procesu zidentyfikuj i zanotuj sekwencje rozgałęzień stron internetowych i&nbsp;stany stron internetowych, do których często uzyskiwany jest dostęp i&nbsp;które mają kluczowe znaczenie dla pomyślnego ukończenia procesu. Dodaj te strony i&nbsp;stany stron do wybranej próbki.

   **Uwaga**: Sekwencje rozgałęzień mogą się kończyć tam, gdzie ponownie wchodzą do domyślnej gałęzi procesu. Na przykład dodanie nowego adresu wysyłki zostanie zarejestrowane jako kluczowa gałąź alternatywna, która prowadzi z&nbsp;powrotem do domyślnej gałęzi procesu.

   **Uwaga**: W większości przypadków konieczne jest zapisanie i&nbsp;określenie działań niezbędnych do przejścia z&nbsp;jednej strony i&nbsp;stanu strony internetowej do następnej w&nbsp;kolejności, aby zakończyć proces, tak aby można je było później powielić. Przykładem takiej akcji może być „Wpisz nazwę i&nbsp;adres oraz wybierz przycisk Wyślij”. W&nbsp;większości przypadków adres internetowy (URI nie będzie wystarczający do zidentyfikowania strony i&nbsp;stanu strony internetowej w&nbsp;całym procesie. Przydatne jest również wyraźne zapisywanie, kiedy strony i&nbsp;stany stron internetowych są częścią procesu, tak aby osoby oceniające mogły skupić swoje wysiłki na istotnych zmianach, takich jak elementy, które zostały dodane, zmodyfikowane lub uwidocznione.

## Krok 4: Wykonaj audyt wybranej próbki

**Wymaganie metodologiczne 4**: Wykonaj audyt wybranej próbki stron internetowych zgodnie z [wymaganiem metodologicznym 4.a](#krok-4a-sprawdź-wszystkie-podstawowe-strony-internetowe), [wymaganiem metodologicznym 4.b](#krok-4b-sprawdź-wszystkie-całe-procesy) i [wymaganiem metodologicznym 4.c.](#krok-4c-porównaj-próbki-strukturalne-i-losowe)

Podczas tego kroku ewaluator przeprowadza szczegółową ocenę wszystkich stron i&nbsp;stanów stron internetowych wybranych w&nbsp;[kroku 3: Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron) i&nbsp;porównuje wyniki oceny próbki strukturalnej z&nbsp;wynikami oceny próbki wybranej losowo. Audyt jest przeprowadzany zgodnie z&nbsp;pięcioma wymogami zgodności WCAG&nbsp;2 na poziomie zgodności ustalonym w&nbsp;[kroku 1.b: Określ wymagany poziom zgodności](#krok-1b-określ-wymagany-poziom-zgodności).

Pięć wymagań zgodności WCAG 2.1 to:

1. [Poziom zgodności](wcag21#521-poziom-zgodności)
2. [Całe strony](wcag21#522-całe-strony)
3. [Całe procesy](wcag21#523-całe-procesy)
4. [Tylko obsługiwane sposoby korzystania z technologii](wcag21#524-tylko-obsługiwane-sposoby-korzystania-z-technologii)
5. [Brak zakłóceń](wcag21#525-brak-zakłóceń)

Wskazówki dotyczące oceny tych wymagań zgodności podano w sekcjach poniżej. Więcej informacji i&nbsp;wskazówek dotyczących wymagań zgodności WCAG&nbsp;2 znajduje się w&nbsp;opracowaniach [WCAG 2.1 Layers of Guidance](http://www.w3.org/TR/WCAG20/#intro-layers-guidance) oraz [Understanding Conformance.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance)

**Uwaga**: Wykonanie tego kroku wymaga głębokiego zrozumienia wymagań zgodności WCAG&nbsp;2 i&nbsp;wiedzy specjalistycznej przedstawionej w sekcji [Wymagana wiedza specjalistyczna.](#wymagana-wiedza-specjalistyczna)

### Krok 4.a: Sprawdź wszystkie podstawowe strony internetowe

**Wymaganie metodologiczne 4.a**: Sprawdź, czy każda strona internetowa lub stan strony w wybranej próbce, które nie są częścią żadnego procesu, jest zgodna z&nbsp;każdym z&nbsp;pięciu wymagań zgodności WCAG&nbsp;2 na wymaganym poziomie zgodności.

Dla każdej strony i stanu strony internetowej w&nbsp;próbce wybranej w [kroku 3: Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron), która nie znajduje się w obrębie lub na końcu całego procesu, sprawdź jej zgodność z&nbsp;każdym z&nbsp;pięciu wymagań zgodności WCAG&nbsp;2, z&nbsp;wymaganym poziomem zgodności ustalonym w&nbsp;[kroku 1.b: Określ wymagany poziom zgodności](#krok-1b-określ-wymagany-poziom-zgodności). Obejmuje to wszystkie składniki strony internetowej lub stanu strony internetowej bez aktywowania jakichkolwiek funkcji, wprowadzania jakichkolwiek danych lub inicjowania procesu w&nbsp;inny sposób. Taka funkcjonalność i&nbsp;interakcja, w&nbsp;tym strony i&nbsp;stany stron internetowych, które znajdują się w&nbsp;obrębie lub na końcu całego procesu, będą oceniane w&nbsp;kolejnym etapie.

**Uwaga**: Wiele stron i stanów stron internetowych w&nbsp;próbce będzie zawierało takie składniki, jak nagłówek, paski nawigacyjne, formularz wyszukiwania i&nbsp;inne, które występują wielokrotnie. Chociaż wymaganiem jest sprawdzenie całych stron, zazwyczaj te składniki nie muszą być poddawane ponownej ocenie przy każdym wystąpieniu, chyba że pojawiają się lub zachowują inaczej, lub gdy  w [kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#krok-1d-określ-dodatkowe-wymagania-oceny) zdefiniowane zostały dodatkowe wymagania oceny.

#### Kryteria sukcesu WCAG 2.1

Zazwyczaj istnieje kilka sposobów ustalenia, czy kryteria sukcesu WCAG&nbsp;2 zostały spełnione, czy nie. W3C/WAI zapewnia (nienormatywny) zestaw technik dla WCAG&nbsp;2, który dokumentuje wystarczające i&nbsp;dodatkowe sposoby spełnienia określonych kryteriów sukcesu WCAG&nbsp;2. W&nbsp;zestawie tym udokumentowano również typowe błędy, które opisują znane sposoby prezentacji treści, nie spełniające określonych kryteriów sukcesu WCAG&nbsp;2. Więcej wskazówek na temat koncepcji technik WCAG&nbsp;2 znajduje się w&nbsp;opracowaniu [Understanding Techniques for WCAG Success Criteria.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques)

Oceniający mogą skorzystać z tych udokumentowanych wskazówek, aby sprawdzić, czy dana treść internetowa spełnia lub nie spełnia kryteriów sukcesu WCAG&nbsp;2. Udokumentowane techniki i&nbsp;błędy mogą być również użytecznym elementem raportów z&nbsp;oceny. Nie jest jednak wymagane stosowanie konkretnego zestawu technik i&nbsp;błędów udokumentowanych przez W3C/WAI. W&nbsp;gruncie rzeczy osoby oceniające wcale nie muszą odwoływać się do technik i&nbsp;błędów. Mogą zastosować inne podejścia, aby ocenić, czy kryteria sukcesu WCAG 2 zostały spełnione, czy nie. Na przykład osoby oceniające mogą stosować określone instrukcje testowania i&nbsp;protokoły, które spełniają [wymagania dotyczące wystarczających technik](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques.html#ut-understanding-techniques-sufficient-head), i&nbsp;które mogą być publicznie udokumentowane lub dostępne wyłącznie dla osób oceniających. Więcej wskazówek na temat stosowania technik znajduje się we wcześniej powiązanych linkach [Zrozumienie technik dla kryteriów sukcesu WCAG.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/understanding-techniques)

**Uwaga**: Kryteria sukcesu WCAG 2 są sformułowane jako „testowalne stwierdzenia, które są prawdziwe lub fałszywe, gdy zostaną zastosowane do określonej treści WWW”. Jeśli użytkownikowi nie przedstawiono treści odnoszącej się do konkretnych kryteriów sukcesu (na przykład na witrynie nie ma wideo), wówczas zgodnie z&nbsp;WCAG&nbsp;2 kryteria sukcesu są „spełnione”. Opcjonalnie w&nbsp;raporcie ustaleń można wskazać konkretne kryteria sukcesu, które pominięto dlatego, że na witrynie nie ma podlegających im treści. W&nbsp;opracowaniu [Understanding Conformance](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html) znajduje się więcej informacji i&nbsp;wskazówek.

#### Zgodność za pomocą wersji alternatywnych

Treść strony internetowej lub stanu strony internetowej może mieć wersje alternatywne. Treści wideo mogą być dostarczane w&nbsp;wersji z&nbsp;napisami i&nbsp;bez. W&nbsp;niektórych przypadkach cała strona internetowa lub stan strony internetowej (lub ich seria) może być dostarczona jako wersja alternatywna do strony lub stanu strony internetowej. Zgodność z&nbsp;WCAG&nbsp;2 można osiągnąć za pomocą wersji alternatywnych, które spełniają wymagania zgodności wersji alternatywnej wymienione w definicji WCAG&nbsp;2. Na przykład, strona internetowa z&nbsp;zawartością wideo bez podpisów może nadal spełniać wymagania WCAG&nbsp;2, zapewniając alternatywną wersję wideo, która kwalifikuje się jako zgodna wersja alternatywna. Więcej informacji i&nbsp;wskazówek dotyczących zgodności wersji alternatywnej, które wykraczają poza zakres niniejszego dokumentu, znajduje się w&nbsp;opracowaniu [Zrozumieć zgodność wersji alternatywnych.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conforming-alt-versions-head)

**Uwaga**: Wersje alternatywne nie są uważane za osobne strony internetowe ani stany stron internetowych, ale za część ich treści. Strony i&nbsp;stany stron internetowych są oceniane razem z&nbsp;ich alternatywnymi wersjami jako jedna jednostka (cała strona).

#### Obsługa dostępności

Treść strony internetowej lub stanu strony internetowej musi być dostarczona w sposób, który jest obsługiwany pod względem dostępności (bezpośrednio lub poprzez alternatywną wersję). Na przykład, napisy do filmu muszą być dostarczone w&nbsp;taki sposób, aby mogły być wyświetlane użytkownikom. Definicja obsługiwanej dostępności WCAG&nbsp;2 określa konkretne szczegółowe wymagania dotyczące korzystania z&nbsp;[technologii tworzenia treści internetowych](http://www.w3.org/TR/WCAG20/#technologydef), aby zakwalifikować je jako obsługiwane pod względem dostępności. Więcej wskazówek dotyczących obsługi dostępności, a&nbsp;wykraczających poza zakres niniejszego dokumentu, znajduje się w&nbsp;opracowaniu [Understanding Accessibility-Supported Web Technology Uses.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-documented-lists-head) WCAG&nbsp;2 nie definiuje jednak konkretnego progu ani zestawu oprogramowania, które witryna musi obsługiwać w&nbsp;celu zapewnienia dostępności. Definicja takiego poziomu bazowego zależy od kilku parametrów, w&nbsp;tym celu, odbiorców i&nbsp;języka witryny. Poziom bazowy używany do oceny konkretnej witryny strony jest zdefiniowany w [kroku 1.c: Określ zestaw technologii bazowych.](#krok-1c-określ-zestaw-technologii-bazowych-obsługujących-dostępność)

#### Brak zakłóceń

Treść strony lub stanu strony internetowej może nie być zgodna z&nbsp;WCAG&nbsp;2, nawet jeśli strona lub stan strony internetowej jako całość będzie zgodna z&nbsp;WCAG 2 (a&nbsp;raczej mogłaby być zgodna). Na przykład informacje i&nbsp;funkcje mogą być dostarczane przy użyciu technologii treści WWW, które nie są jeszcze szeroko wspierane przez technologie wspomagające lub w sposób, który nie jest obsługiwany przez technologie wspomagające, wraz z odpowiadającą im alternatywną wersją dla informacji i&nbsp;funkcji obsługiwanych przez dostępność. W takim przypadku treść niezgodna nie może negatywnie wpływać na treść zgodną, aby strona lub stan strony internetowej odpowiadał wymogom zgodności z&nbsp;WCAG&nbsp;2. Wymóg zgodności z&nbsp;WCAG&nbsp;2 dotyczący braku zakłóceń określa szczegółowe wymagania dla treści, aby zakwalifikować się jako niezakłócającą. Informacje, które wykraczają poza zakres tego dokumentu, dotyczące braku zakłóceń, znajdują się w opracowaniu [Understanding Requirement 5](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance#uc-conf-req5-head)(Zrozumieć wymaganie zgodności).

### Krok 4.b: Sprawdź wszystkie całe procesy

**Wymaganie metodologiczne 4.b**: Sprawdź, czy wszystkie interakcje dla każdej strony i&nbsp;stanu strony internetowej w&nbsp;całym procesie są zgodne z&nbsp;każdym z&nbsp;pięciu wymagań zgodności WCAG&nbsp;2 na wymaganym poziomie zgodności.

Dla każdego całego procesu określonego w [kroku 3.c: Uwzględnij całe procesy](#krok-3c-uwzględnij-całe-procesy), postępuj zgodnie ze wskazanymi domyślnymi i&nbsp;rozgałęzionymi sekwencjami stron i&nbsp;stanów stron internetowych i&nbsp;oceń każdy zgodnie z [krokiem 4.a: Sprawdź wszystkie podstawowe strony internetowe](#krok-4a-sprawdź-wszystkie-podstawowe-strony-internetowe). Jednak w tym przypadku nie jest konieczna ocena wszystkich treści, a&nbsp;jedynie treści, które zmieniają się w trakcie procesu.

Poddaj ocenie funkcjonalność, wprowadzanie danych, powiadomienia i&nbsp;inne interakcje. W&nbsp;szczególności sprawdzanie powinno objąć:

- Interakcję z formularzami, polami danych, przyciskami, oknami dialogowymi i&nbsp;innymi składnikami strony internetowej;
- Potwierdzenia wprowadzenia danych, komunikaty o&nbsp;błędach i&nbsp;innych informacje zwrotne;
- Zachowanie po zastosowaniu różnych ustawień, preferencji, urządzeń i&nbsp;parametrów interakcji.

### Krok 4.c: Porównaj próbki strukturalne i losowe

**Wymaganie metodologiczne 4.c:** Sprawdź, czy żadna strona i&nbsp;żaden stan strony internetowej w próbce wybranej losowo nie pokazuje innych typów treści i&nbsp;wyników, niż typy treści i&nbsp;wyniki w próbce strukturalnej.

Chociaż poszczególne wystąpienia kryteriów sukcesu WCAG&nbsp;2 będą się różnić pomiędzy próbkami strukturalnymi i&nbsp;losowo wybranymi, losowo wybrana próbka nie powinna pokazywać nowych typów treści, które nie występują w&nbsp;próbie strukturalnej.

Również wyniki oceny próbki wybranej losowo nie powinny pokazywać nowych ustaleń w stosunku do wyników oceny próby strukturalnej. Jeśli losowo wybrana próbka zawiera nowe typy treści lub nowe ustalenia z&nbsp;oceny, oznacza to, że próbka strukturalna nie była wystarczająco reprezentatywna dla treści zamieszczonych na witrynie. W&nbsp;takim przypadku osoby oceniające muszą wrócić do [kroku 3: Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron), aby wybrać dodatkowe strony internetowe i&nbsp;stany stron internetowych, które odzwierciedlają nowo zidentyfikowane typy treści i&nbsp;ustalenia. Również ustalenia z&nbsp;[kroku 2: Przeprowadź rekonesans witryny.](#krok-2-przeprowadź-rekonesans-witryny) mogą wymagać odpowiedniego dostosowania.

Ten krok powtarza się, dopóki próbka strukturalna nie będzie odpowiednio reprezentatywna dla treści dostarczanych na witrynie.

## Krok 5. Sporządź raport ustaleń audytu

**Wymaganie metodologiczne 5**: Przedstaw wyniki oceny zgodnie z [wymogiem metodologicznym 5.a](#krok-5a-udokumentuj-wyniki-każdego-kroku) oraz opcjonalnie [wymogiem metodologicznym 5.b](#krok-5b-zapisz-specyfikację-oceny-opcjonalne), [wymogiem metodologicznym 5.c](#krok-5c-przygotuj-oświadczenie-o-zgodności-opcjonalnie), [wymogiem metodologicznym 5.d](#krok-5d-podaj-zagregowany-wynik-opcjonalnie) i&nbsp;[wymogiem metodologicznym 5.e](#krok-5e-sporządź-wersję-raportu-do-odczytu-maszynowego-opcjonalnie)

Chociaż wyniki oceny są raportowane na koniec procesu, ich dokumentowanie ma miejsce w trakcie całego procesu oceny, aby zapewnić możliwość weryfikacji wyników. Dokumentacja charakteryzuje się zwykle różnym stopniem poufności. Na przykład dokumentacja konkretnych metod stosowanych do oceny poszczególnych wymagań może pozostać tajemnicą osoby oceniającej, ale raporty o&nbsp;wynikach tych kontroli są zwykle udostępniane zlecającemu ocenę.

Właściciele stron internetowych mogą ponadto zdecydować się na podanie do publicznej wiadomości informacji o&nbsp;wynikach oceny zgodnie z&nbsp;tą metodologią.

### Krok 5.a: Udokumentuj wyniki każdego kroku

**Wymaganie metodologiczne 5.a**: Udokumentuj każdy wynik ustaleń dokonanych w [kroku 1: Określ zakres oceny](#krok-1-ustal-zakres-oceny), [kroku 2: Przeprowadź rekonesans witryny.](#krok-2-przeprowadź-rekonesans-witryny), [kroku 3: Wybierz reprezentatywną próbkę stron)](#krok-3-wybierz-reprezentatywną-próbkę-stron) i [kroku 4: Wykonaj audyt wybranej próbki)](#krok-4-wykonaj-audyt-wybranej-próbki).

Dokumentowanie wyników każdego z poprzednich kroków (w&nbsp;tym wszystkich podsekcji) jest niezbędne dla zapewnienia przejrzystości procesu oceny, powtarzalności wyników oceny oraz uzasadnienia wszelkich oświadczeń złożonych na podstawie tej oceny. **Dokumentacja ta nie musi być jawna**, poziom poufności zwykle określa komisarz ds. oceny.

Dokumentowanie wyników każdego kroku obejmuje co najmniej następujące elementy:

- Metryka audytu
  - Nazwa podmiotu oceniającego/osoby oceniającej
  - Nazwa zlecającego ocenę - komisarza ds. oceny
  - Data przeprowadzenia oceny (data zakończenia lub czas trwania)
- Zakres oceny
  - Zakres stron witryny określony w [kroku 1.a: Określ zakres stron witryny](#krok-1a-określ-zakres-stron-witryny)
  - Wymagany poziom zgodności określony w [kroku 1.b. Określ wymagany poziom zgodności](#krok-1b-określ-wymagany-poziom-zgodności)
  - Zestaw technologii bazowych określony w [kroku 1.c: Określ zestaw technologii bazowych](#krok-1c-określ-zestaw-technologii-bazowych-obsługujących-dostępność)
  - Dodatkowe wymagania, jeżeli istnieją, określone w [kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#krok-1d-określ-dodatkowe-wymagania-oceny)
- Wstępne rozpoznanie witryny
  - Wiarygodne technologie internetowe określone w [kroku 2.d: Zidentyfikuj użyte technologie](#krok-2d-zidentyfikuj-użyte-technologie-internetowe)
  - Opcjonalnie: Wspólne strony witryny określone w [kroku 2.a: Zidentyfikuj wspólne strony](#krok-2a-zidentyfikuj-wspólne-strony-internetowe-witryny)
  - Opcjonalnie: Niezbędne funkcjonalności witryny określone w [kroku 2.b: Zidentyfikuj niezbędne funkcjonalności](#krok-2b-zidentyfikuj-niezbędne-funkcjonalności)
  - Opcjonalnie: Różne typy stron określone w [kroku 2.c: Zidentyfikuj różne typy stron](#krok-2c-zidentyfikuj-różne-typy-stron-internetowych)
  - Opcjonalnie: Inne istotne strony określone w [kroku 2.e: Zidentyfikuj inne istotne strony](#krok-2e-zidentyfikuj-inne-istotne-strony-internetowe)
- Wybór reprezentatywnej próbki stron
  - Strony i stany stron internetowe wybrane w ramach próbkowania strukturalnego w [kroku 3.a: Uwzględnij próbkę strukturalną](#krok-3a-uwzględnij-próbkę-strukturalną)
  - Strony wybrane losowo i metoda wyboru zastosowana w [kroku 3.b: Uwzględnij próbkę wybraną losowo](#krok-3b-uwzględnij-losowo-wybraną-próbkę)
  - Całe procesy wybrane w [kroku 3.c: Uwzględnij całe procesy](#krok-3c-uwzględnij-całe-procesy)
- Audyt wybranej próbki
  - Wyniki oceny z [kroku 4.a: Sprawdź wszystkie podstawowe strony internetowe](#krok-4a-sprawdź-wszystkie-podstawowe-strony-internetowe)
  - Wyniki oceny z [kroku 4.b: Sprawdź wszystkie całe procesy](#krok-4b-sprawdź-wszystkie-całe-procesy)
  - Wyniki oceny z [kroku 4.c: Porównaj próbki strukturalną i losową](#krok-4c-porównaj-próbki-strukturalne-i-losowe)

**Uwaga**: W zależności od pożądanej szczegółowości raportu, wyniki [kroku 4: Wykonaj audyt wybranej próbki)](#krok-4-wykonaj-audyt-wybranej-próbki) mogą być dostarczone dla każdej ocenianej strony i&nbsp;stanu strony internetowej lub zagregowane dla całej próbki. Raporty powinny zawierać co najmniej jeden przykład dla każdego wymogu zgodności i&nbsp;kryterium sukcesu WCAG&nbsp;2, które nie zostało spełnione. Dobrą praktyką jest również wskazywanie powtarzających się problemów.

Raporty mogą również zawierać dodatkowe informacje w zależności od dodatkowych wymogów oceny określonych w&nbsp;[kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie)](#krok-1d-określ-dodatkowe-wymagania-oceny). Na przykład, komisarz ds. oceny może poprosić o&nbsp;raport wskazujący każde wystąpienie defektu dla każdej strony i&nbsp;stanu strony internetowej w&nbsp;wybranej próbce, o&nbsp;więcej informacji na temat charakteru i&nbsp;przyczyn zidentyfikowanych defektów lub sugestie naprawy w&nbsp;celu usunięcia defektów.

### Krok 5.b: Zapisz specyfikację oceny (opcjonalne)

**Wymaganie metodologiczne 5.b**: Zarchiwizuj skontrolowane strony i&nbsp;stany stron internetowych oraz zapisz narzędzia oceny, przeglądarki internetowe, technologie wspomagające, inne oprogramowanie i&nbsp;metody użyte do ich audytu (opcjonalnie).

Chociaż jest to opcjonalne, dobrą praktyką jest zapisywanie przez oceniających szczegółów oceny, na przykład na wypadek konieczności rozwiązania konfliktu w&nbsp;przypadku sporu. Obejmuje to archiwizację skontrolowanych stron i&nbsp;stanów stron oraz rejestrację narzędzi oceny, przeglądarek internetowych, technologii wspomagających, innego oprogramowania i&nbsp;metod wykorzystywanych do ich kontroli. Zapis ten jest zazwyczaj przechowywany wewnętrznie i&nbsp;nie jest udostępniany przez oceniającego, chyba że uzgodniono inaczej w&nbsp;[kroku 1.d: Określ dodatkowe wymagania oceny (opcjonalnie).](#krok-1d-określ-dodatkowe-wymagania-oceny)

Zapisy dotyczące specyfikacji oceny mogą obejmować dowolne z poniższych kwestii:

- Kopie plików i zasobów stron internetowych i stanów stron internetowych;
   **Uwaga**: Niektóre narzędzia mogą zapisać dynamicznie wygenerowaną lub zmodyfikowaną zawartość (DOM) wyświetlaną podczas oceny, a&nbsp;nie początkową zawartość plików i&nbsp;zasobów, która często jest inna;
- Zrzuty ekranu stron internetowych i&nbsp;stanów stron internetowych;
- Opisy ścieżek do lokalizowania stron i&nbsp;stanów stron internetowych, szczególnie gdy są one częścią procesu;
- Opis ustawień, wprowadzanych danych i&nbsp;działań służących do generowania stron lub nawigowania do stron i&nbsp;stanów stron internetowych. Specyficzne poświadczenia testowe (identyfikatory użytkownika itp.) wymagane do odtworzenia unikalnego zestawu danych lub przepływu pracy;
- Nazwy i wersje narzędzi oceny, przeglądarek internetowych i&nbsp;dodatków, technologii wspomagających oraz innego używanego oprogramowania;
- Metody, procedury i techniki stosowane do oceny zgodności z&nbsp;WCAG&nbsp;2.

Zapis ten może obowiązywać globalnie dla całej oceny, dla poszczególnych stron internetowych lub dla poszczególnych testów przeprowadzanych w ramach sprawdzanych stron i&nbsp;stanów stron internetowych. Do rejestrowania informacji można wykorzystać tabelę lub siatkę.

**Uwaga**: Zapisy dotyczące specyfikacji oceny mogą zawierać poufne informacje, takie jak kod wewnętrzny, hasła i&nbsp;kopie danych. Mogą one wymagać szczególnych środków ostrożności w&nbsp;zakresie bezpieczeństwa i&nbsp;ochrony prywatności.

### Krok 5.c: Przygotuj oświadczenie o zgodności (opcjonalnie)

**Wymaganie metodologiczne 5.c**: Przygotuj oświadczenie o zgodności (opcjonalnie).

Przypomnienie: W większości przypadków samo zastosowanie tej metodologii nie powoduje stwierdzenia zgodności badanych witryn z&nbsp;WCAG&nbsp;2; więcej informacji na temat stosunku do wmagań zgodności z&nbsp;WCAG&nbsp;2.

Właściciele witryn mogą chcieć złożyć publiczne oświadczenia na temat wyników ocen przeprowadzonych zgodnie z&nbsp;tą metodologią. Można to zrobić, gdy

- spełnione są co najmniej wszystkie nieopcjonalne wymagania metodologiczne,
- poziom zgodności określony w [kroku 1.b. Określ wymagany poziom zgodności](#krok-1b-określ-wymagany-poziom-zgodności) jest spełniony przez wszystkie strony i stany stron internetowych poddane audytowi (w&nbsp;[kroku 4: Wykonaj audyt wybranej próbki)](#krok-4-wykonaj-audyt-wybranej-próbki),
- właściciel witryny zobowiązuje się do zapewnienia poprawności i&nbsp;zachowania dokładności złożonego oświadczenia z&nbsp;oceny.

Oświadczenie oceniające zgodne z tą metodologią zawiera co najmniej następujące informacje:

1. Data wydania oświadczenia z oceny;
2. Tytuł, wersja i identyfikator URI wytycznych: „Wytyczne dla dostępności treści internetowych 2.1” pod adresem https://www.w3.org/TR/WCAG21/";
3. Oceniony poziom zgodności: Poziom A, AA lub AAA, jak określono w&nbsp;[kroku 1.b. Określ wymagany poziom zgodności](#krok-1b-określ-wymagany-poziom-zgodności);
4. Definicja strony internetowej, jak określono w [kroku 1.a: Określ zakres witryny;](#krok-1a-określ-zakres-stron-witryny)
5. Technologie internetowe, na których się opiera się, jak określono w&nbsp;[kroku 2.d: Zidentyfikuj użyte technologie internetowe;](#krok-2d-zidentyfikuj-użyte-technologie-internetowe)
6. Podstawowe wsparcie dostępności, jak określono w [kroku 1.c: Określ zestaw technologii bazowych.](#krok-1c-określ-zestaw-technologii-bazowych-obsługujących-dostępność)

Deklaracje ewaluacyjne zgodne z tą metodologią mogą być również sporządzane, gdy osiągnięto jedynie częściową zgodność z&nbsp;WCAG&nbsp;2. W&nbsp;takich przypadkach stwierdzenia ewaluacyjne zawierają również następujące informacje:

- Obszary strony internetowej, które nie są zgodne z&nbsp;WCAG 2;
- Powód, dla którego nie są one zgodne z&nbsp;WCAG 2: „treści stron trzecich”  lub „brak wsparcia dla języków”.

### Krok 5.d: Podaj zagregowany wynik (opcjonalnie)

**Wymaganie metodologiczne 5.d**: Podaj zagregowany wynik (opcjonalnie).

Chociaż zagregowane wyniki stanowią wskaźnik liczbowy, który pomaga komunikować postępy w&nbsp;czasie, obecnie nie ma jednej miary, która uwzględniałaby wymaganą wiarygodność, dokładność i&nbsp;praktyczność. W&nbsp;rzeczywistości zagregowane wyniki mogą wprowadzać w&nbsp;błąd i&nbsp;nie zapewniają wystarczającego kontekstu i&nbsp;informacji, aby zrozumieć rzeczywistą dostępność strony internetowej.

Z tego i innych powodów WCAG 2 nie zapewnia systemu klasyfikacji. Raport badawczy W3C na temat wskaźników dostępności w&nbsp;sieci zawiera więcej informacji na temat bieżących badań, różnych podejść i&nbsp;ograniczeń oceniania wskaźników, które wykraczają poza zakres tego dokumentu. Za każdym razem, gdy podawana jest punktacja, istotne jest, aby sposób punktacji został udokumentowany i&nbsp;udostępniony komisarzowi ds. oceny wraz z&nbsp;raportem, aby ułatwić przejrzystość i&nbsp;powtarzalność.

### Krok 5.e: Sporządź wersję raportu do odczytu maszynowego (opcjonalnie)

**Wymóg metodologiczny 5.e**: Sporządź sprawozdanie z wyników oceny nadające się do odczytu maszynowego (opcjonalnie).

Raporty nadające się do odczytu maszynowego ułatwiają przetwarzanie wyników oceny przez autorów, narzędzia oceny dostępności stron internetowych oraz narzędzia zapewniania jakości. Język oceny i&nbsp;raportowania (EARL) jest formatem do odczytu maszynowego, który został specjalnie zaprojektowany do tego celu. Zaleca się korzystanie z&nbsp;EARL w celu dostarczania raportów do odczytu maszynowego. Aby dowiedzieć się więcej na temat wykorzystania metadanych, w&nbsp;tym raportów odczytywanych maszynowo, takich jak EARL, zobacz: [Understanding Metadata.](http://www.w3.org/TR/UNDERSTANDING-WCAG20/appendixC#understanding-metadata)

## Dodatki

### Dodatek A: Współtwórcy

Dawni i obecni aktywni uczestnicy projektu [WCAG 2.0 Evaluation Methodology Task Force (Eval TF)](http://www.w3.org/WAI/ER/2011/eval/eval-tf): Shadi Abou-Zahra; Frederick Boland; Denis Boudreau; Amy Chen; Vivienne Conway; Bim Egan; Michael Elledge; Gavin Evans; Wilco Fiers; Detlev Fischer; Elizabeth Fong; Vincent François; Alistair Garrison; Emmanuelle Gutiérrez y Restrepo; Katie Haritos-Shea; Martijn Houtepen; Peter Korn; Maureen Kraft; Aurelien Levy; David MacDonald; Mary Jo Mueller; Donald Raikes; Corominas Ramon; Roberto Scano; Samuel Sirois; Sarah J Swierenga; Eric Velleman; Konstantinos Votis; Kathleen Wahlbin; Elle Waters; Richard Warren; Léonie Watson.

### Dodatek B: Bibliografia

**ATAG20**
: Richards J, Spellman J, Treviranus J, eds (2013). Authoring Tool Accessibility Guidelines 2.0. W3C. Dostępne pod adresem: [http://www.w3.org/TR/ATAG20/](http://www.w3.org/TR/ATAG20/)

**Easy Checks**
: Lawton Henry S, ed (2014). Easy Checks - A First Review of Web Accessibility. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/test-evaluate/preliminary/](https://www.w3.org/WAI/test-evaluate/preliminary/)

**Essential Components of Web Accessibility**
: Lawton Henry S, ed (2005). Essential Components of Web Accessibility. Version 1.3. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/fundamentals/components/](https://www.w3.org/WAI/fundamentals/components/)

**How People with Disabilities Use the Web**
: Abou-Zahra S, ed (2012). How People with Disabilities Use the Web. Draft. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/people-use-web/](https://www.w3.org/WAI/people-use-web/)

**Involving Users in Evaluating Web Accessibility**
: Lawton Henry S, ed (2010). Involving Users in Evaluating Web Accessibility. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/test-evaluate/involving-users/](https://www.w3.org/WAI/test-evaluate/involving-users/)

**Selecting Web Accessibility Evaluation Tools**
: Abou-Zahra S, ed (2005). Selecting Web Accessibility Evaluation Tools. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/test-evaluate/tools/selecting/](https://www.w3.org/WAI/test-evaluate/tools/selecting/)

**Using Combined Expertise to Evaluate Web Accessibility**
: Brewer J, ed (2002). Using Combined Expertise to Evaluate Web Accessibility. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/test-evaluate/combined-expertise/](https://www.w3.org/WAI/test-evaluate/combined-expertise/)

**UWEM**
: Velleman E.M, Velasco C.A, Snaprud M (eds) (2007). D-WAB4 Unified Web Evaluation Methodology (UWEM 1.2 Core). Wabcluster. Dostępne pod adresem: [http://www.wabcluster.org/uwem1_2/](http://www.wabcluster.org/uwem1_2/)

**WCAG Overview**
: Lawton Henry S, ed (2012). Web Content Accessibility Guidelines (WCAG) Overview. W3C. Dostępne pod adresem: [https://www.w3.org/WAI/standards-guidelines/wcag/](https://www.w3.org/WAI/standards-guidelines/wcag/)

**WCAG20**
: Caldwell B, Cooper M, Guarino Reid L, Vanderheiden G, eds (2008). Web Content Accessibility Guidelines 2.0. W3C. Dostępne pod adresem: [http://www.w3.org/TR/WCAG20/](http://www.w3.org/TR/WCAG20/)

**WCAG20-TECHS**
: Cooper M, Kirkpatrick A, O Connor J, eds (2014). Techniques and Failures for Web Content Accessibility Guidelines 2.0. W3C. Dostępne pod adresem: [http://www.w3.org/TR/WCAG20-TECHS/](http://www.w3.org/TR/WCAG20-TECHS/)

**Understanding-WCAG20**
: Cooper M, Kirkpatrick A, O Connor J, eds (2014). Understanding WCAG 2.0 - A guide to understanding and implementing Web Content Accessibility Guidelines 2.0. W3C. Dostępne pod adresem: [http://www.w3.org/TR/UNDERSTANDING-WCAG20/](http://www.w3.org/TR/UNDERSTANDING-WCAG20/)
