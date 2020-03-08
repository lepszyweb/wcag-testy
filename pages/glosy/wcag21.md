---
title: Wytyczne dla dostępności internetowej (WCAG) 2.1
summary: "Publikacja jest roboczym tłumaczeniem Wytycznych dla dostepności internetowej (WCAG) 2.1. W tłumaczeniu wykorzystano nieoficjalne polskie tłumaczenie WCAG 2.0."

sidebar: glosy_sidebar
permalink: wcag21
folder: glosy
---

## Streszczenie

„Wytyczne dla dostępności internetowej (WCAG) 2.1” obejmują szeroki wachlarz zaleceń dotyczących zwiększenia dostępności treści internetowych. Wdrożenie tych wytycznych sprawi, że treści będą bardziej dostępne dla szerszego grona osób z niepełnosprawnościami, w tym dla osób niewidomych i&nbsp;słabowidzących, głuchych i niedosłyszących, osób z niepełnosprawnością ruchową, z&nbsp;zaburzeniami mowy, nadwrażliwością na światło, osób z&nbsp;niepełnosprawnościami złożonymi, a także dla niektórych osób mających trudności w uczeniu się i ograniczenia poznawcze; ale nie zaspokoi potrzeb każdego użytkownika z niepełnosprawnością. Niniejsze wytyczne dotyczą dostępności treści internetowych na komputerach stacjonarnych, laptopach, tabletach i urządzeniach przenośnych. Wprowadzenie wytycznych w życie, sprawi również, że treści internetowe będą często bardziej użyteczne dla użytkowników w&nbsp;ogóle.

Kryteria sukcesu WCAG 2.1 są formułowane jako twierdzenia możliwe do zweryfikowania i niepowiązane z konkretną technologią. Wytyczne dotyczące spełnienia kryteriów sukcesu dla konkretnych technologii, jak również ogólne informacje dotyczące interpretacji kryteriów sukcesu zawarte są w osobnych dokumentach. Więcej na ten temat przeczytać można w [Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/standards-guidelines/wcag/) (Omówienie Wytycznych dla dostępności treści internetowych (WCAG), gdzie znajduje się wstęp i&nbsp;odnośniki do materiałów edukacyjnych oraz informacji technicznych dotyczących WCAG.

WCAG 2.1 rozszerzają [Web Content Accessibility Guidelines 2.0 (WCAG20)](https://www.w3.org/TR/WCAG20/), które zostały opublikowane w&nbsp;grudniu 2008 roku, jako rekomendacja W3C. Treść zgodna z WCAG 2.1 jest również zgodna z WCAG 2.0. Intencją Grupy Roboczej jest, aby dla polityk wymagających zgodności z WCAG 2.0, WCAG 2.1 mogły zapewnić alternatywne środki zgodności. Publikacja WCAG 2.1 nie deprecjonuje ani nie zastępuje WCAG 2.0. Chociaż WCAG 2.0 nadal pozostają rekomendacją W3C, W3C zaleca stosowanie WCAG 2.1, aby zmaksymalizować możliwości zastosowania w&nbsp;przyszłości działań na rzecz dostępności. W3C zachęca również do korzystania z&nbsp;najbardziej aktualnej wersji WCAG przy opracowywaniu lub aktualizacji polityki dostępności cyfrowej.

## Status dokumentu
Poniższa część opisuje status dokumentu w momencie jego publikacji. Inne dokumenty mogą w przyszłości zastąpić niniejszy. Lista bieżących publikacji W3C oraz zaktualizowany raport techniczny znajdują się na stronie [W3C technical reports index](http://www.w3.org/TR/) pod adresem http://www.w3.org/TR/.

WCAG 2.1 są [Rekomendacją W3C](https://www.w3.org/2018/Process-20180201/#RecsW3C) opracowaną przez [Web Content Accessibility Guidelines Working Group](http://www.w3.org/WAI/GL/) (Grupę Roboczą ds. Wytycznych dla Dostępności).

Niniejszy dokument został zrecenzowany przez członków W3C, programistów, inne grupy W3C oraz inne zainteresowane strony, a następnie zatwierdzony przez Dyrektora W3C, jako Rekomendacja W3C. Jest to wersja finalna dokumentu, która może zostać wykorzystana jako materiał źródłowy lub być cytowana w innych dokumentach W3C. Rolą W3C jest zwrócenie uwagi na tę specyfikację i&nbsp;promowanie jej powszechnego wdrożenia. Stosowanie zaleceń zawartych w tej specyfikacji zwiększa funkcjonalność oraz interoperacyjność sieci.

Publikując tę rekomendację, W3C zakłada, że na funkcjonalność określoną w tej rekomendacji nie będą miały wpływu zmiany w specyfikacjach [CSS Values and Units Module Level 3](https://www.w3.org/TR/css-values-3/) oraz [Pointer Events Level 2](https://www.w3.org/TR/2019/REC-pointerevents2-20190404/). Grupa Robocza będzie nadal śledzić te specyfikacje.

Aby skomentować, [zgłoś problem w repozytorium WCAG W3C na platformie GitHub](https://github.com/w3c/wcag/issues/new). Grupa Robocza prosi, aby komentarze publiczne były składane jako nowe problemy, po jednym w&nbsp;zgłoszeniu. Utworzenie konta GitHub w celu zgłaszania problemów jest bezpłatne. Jeśli zgłaszanie problemów na GitHub jest niemożliwe,  komentarze można też przesyłać na adres [public-comments-wcag20@w3.org](public-comments-wcag20@w3.org). Komentarze na temat rekomendacji WCAG 2.1 nie będą powodować zmian w tej wersji wytycznych. Mogą jednak zostać uwzględnione w erracie lub przyszłych wersjach WCAG. Grupa Robocza nie przewiduje formalnych odpowiedzi na komentarze. Lista [zgłoszonych problemów](https://github.com/w3c/wcag/issues/) oraz [Archiwum dyskusji na listach mailingowych AG WG](http://lists.w3.org/Archives/Public/w3c-wai-gl/) są publicznie dostępne. Grupa Robocza może wziąć pod uwagę komentarze dotyczące niniejszego dokumentu w&nbsp;przyszłości.

Ten dokument został opublikowany przez [Accessibility Guidelines Working Group](https://www.w3.org/WAI/GL/) (Grupę Roboczą Wytycznych dla Dostępności) jako rekomendacja.

Zobacz [raport Grupy Roboczej z wdrożenia](https://www.w3.org/WAI/WCAG21/implementation-report/).

Niniejszy dokument został stworzony zgodnie z [Polityką Patentową W3C](https://www.w3.org/Consortium/Patent-Policy/). W3C prowadzi pełną listę zgłoszonych publicznie patentów odnośnie tego dokumentu. Powyższa strona zawiera również instrukcje zgłaszania patentu. Osoby, które twierdzą, iż posiadają wiedzę na temat patentów zawierających [istotne roszczenia](https://www.w3.org/Consortium/Patent-Policy/#def-essential) (Essential Claim(s)) powinny zgłosić takie informacje, zgodnie z [Rozdziałem 6 Polityki Patentowej Konsorcjum W3C](https://www.w3.org/Consortium/Patent-Policy/#sec-Disclosure).

Niniejszy dokument podlega [dokumentowi procesowemu W3C z 1 lutego 2018 r.](https://www.w3.org/2018/Process-20180201/)

## Wprowadzenie

Niniejsza sekcja pełni funkcję <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.informacyjne | strip_html | replace: '\*', ''}}">informacyjną</a>.

### 0.1 Kontekst WCAG
„Wytyczne dla dostępności treści internetowych (WCAG) 2.1” określają, w jaki sposób zwiększyć dostępność treści internetowych dla osób z&nbsp; niepełnosprawnościami. Mowa tutaj o wielu rodzajach niepełnosprawności: ze względu na wzrok, słuch, kłopoty z mową, trudności w uczeniu się, ograniczenia poznawcze, ruchowe, lingwistyczne czy też neurologiczne.
Chociaż wytyczne poruszają szereg zagadnień, nie jest możliwe, aby odpowiadały szczegółowo na potrzeby wszystkich możliwych rodzajów, stopni niepełnosprawności, czy też niepełnosprawności złożonych. Wytyczne pozwalają jednak tworzyć bardziej użyteczne treści, zarówno dla starszych użytkowników, których sprawność zmienia się wraz z wiekiem, jak i dla każdego innego użytkownika.

WCAG 2.1 zostały opracowane zgodnie z [procedurami W3C](https://www.w3.org/WAI/standards-guidelines/w3c-process/), we współpracy z osobami indywidualnymi oraz różnymi organizacjami z całego świata. Celem było stworzenie wspólnego standardu dostępności treści internetowych, który spełniałby oczekiwania użytkowników, firm czy administracji państwowej w&nbsp;różnych krajach.

WCAG 2.1 opierają się na WCAG 2.0 [[WCAG20](https://www.w3.org/TR/WCAG21/#bib-WCAG20)], które z kolei opierają się na WCAG 1.0 [[WAI-WEBCONTENT](https://www.w3.org/TR/WCAG21/#bib-WAI-WEBCONTENT)] i&nbsp;są przeznaczone do szerokiego zastosowania w różnych technologiach internetowych zarówno teraz, jak i&nbsp;w przyszłości. Są one tak skonstruowane, aby ich spełnienie można było sprawdzić za pomocą kombinacji narzędzi automatycznych i&nbsp;oceny dokonywanej przez człowieka. Na stronie „[Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/standards-guidelines/wcag/)”, znajduje się więcej informacji ogólnych na temat wytycznych WCAG.

Przy określaniu dodatkowych kryteriów dotyczących niepełnosprawności poznawczych, językowych i&nbsp;związanych z uczeniem się, napotkano istotne wyzwania, w tym spowodowane krótkim harmonogramem prac, a&nbsp;także wyzwania w&nbsp;osiągnięciu konsensusu w&nbsp;zakresie testowalności, możliwości wdrożenia i rozpatrzenia propozycji na forum międzynarodowym. Prace w tej dziedzinie będą kontynuowane w przyszłych wersjach WCAG. Zachęcamy autorów do zapoznania się z naszymi dodatkowymi wskazówkami dotyczącymi [poprawy integracji osób z niepełnosprawnościami, w tym osób z trudnościami w uczeniu się i poznawaniu, osób słabowidzących i innych](http://www.w3.org/WAI/standards-guidelines/wcag/#supplement).

Dostępność sieci nie jest uzależniona jedynie od treści stron internetowych, ale również od dostępnych przeglądarek internetowych czy innych programów stosowanych przez użytkownika. Ważną rolę w dostępności spełniają również narzędzia do tworzenia treści. Dalsze informacje na ten temat znajdują się na następujących stronach:

- [Essential Components of Web Accessibility](https://www.w3.org/WAI/fundamentals/components/) (Kluczowe komponenty dostępnosci internetowej),
- [User Agent Accessibility Guidelines (UAAG) Overview)](https://www.w3.org/WAI/standards-guidelines/uaag/) (Omówienie Wytycznych dla dostępności programów użytkownika),
- [Authoring Tool Accessibility Guidelines (ATAG) Overview](https://www.w3.org/WAI/standards-guidelines/atag/) (Omówienie Wytycznych dla dostępności narzedzi do tworzenia treści).

### 0.2 Warstwy wytycznych WCAG 2.1
Osoby indywidualne i organizacje, które korzystają z wytycznych WCAG 2.1 to różnorodna grupa, obejmująca między innymi osoby projektujące serwisy internetowe, decydentów, nabywców usług, nauczycieli czy studentów. Aby sprostać różnym potrzebom tych grup odbiorców, stworzono kilka warstw wytycznych, w tym zasady ogólne, wytyczne, mierzalne kryteria sukcesu, bogaty zbiór wystarczających technik, technik dodatkowych oraz udokumentowane, często występujące błędy, poparte przykładami, odnośnikami do zasobów i&nbsp;fragmentami kodu źródłowego.

- **Zasady** — na szczycie hierarchii znajdują się 4 zasady, które stanowią fundament dostępności internetowej: postrzegalność, funkcjonalność, zrozumiałość i rzetelność. Więcej informacji: ”[Understanding the Four Principles of Accessibility](http://www.w3.org/TR/UNDERSTANDING-WCAG20/intro.html#introduction-fourprincs-head)” (Zrozumienie czterech zasad dostępności).
- **Wytyczne** — na kolejnym poziomie, znajdują się wytyczne. 13&nbsp;wytycznych definiuje podstawowe cele, do których powinni dążyć autorzy, aby treści były bardziej dostępne dla użytkowników z różnymi niepełnosprawnościami. Wytyczne nie są mierzalne, ale stanowią ogólne ramy i&nbsp;cele do osiągnięcia. Mają pomóc autorom zrozumieć kryteria sukcesu i&nbsp;pozwolić na ich skuteczniejsze wdrażanie.
- **Kryteria sukcesu** — dla każdej wytycznej opracowano mierzalne kryteria sukcesu. Pozwala to na zastosowanie WCAG 2.1 wszędzie tam, gdzie konieczne jest sprawdzenie zgodności z wytycznymi, np. przy specyfikacji projektu, zamawianiu usług internetowych, w przepisach prawnych oraz przy umowach. Aby zaspokoić potrzeby różnych grup i&nbsp;różnych sytuacji, zdefiniowano trzy poziomy zgodności: A (najniższy), AA i&nbsp;AAA (najwyższy). Dodatkowe informacje na temat poziomów WCAG można znaleźć na stronie „[Understanding Levels of Conformance](https://www.w3.org/WAI/WCAG21/Understanding/conformance#levels)” (Zrozumieć poziomy zgodności).
- **Techniki wystarczające i dodatkowe** — dla każdej wytycznej oraz kryterium sukcesu WCAG 2.1, grupa robocza zebrała szereg technik (dokument ma charakter informacyjny, ale nie formalny). Podzielono je na dwie kategorie: techniki wystarczające, by spełnić kryteria sukcesu, oraz techniki dodatkowe. Techniki dodatkowe wykraczają poza to, co jest wymagane przez dane kryteria sukcesu i&nbsp;pozwalają wykonawcom i&nbsp;autorom na jeszcze lepszą realizację wytycznych. Niektóre techniki dodatkowe dotyczą barier dostępności, które nie zostały ujęte w mierzalnych kryteriach sukcesu. Często występujące błędy w miarę możliwości również zostały udokumentowane. Więcej informacji w: „[Understanding Techniques for WCAG Success Criteria](https://www.w3.org/WAI/WCAG21/Understanding/understanding-techniques)” (Zrozumieć techniki dla kryteriów sukcesu WCAG).

Wszystkie powyższe warstwy (zasady, wytyczne, kryteria sukcesu, techniki wystarczające i&nbsp;dodatkowe) uzupełniają się wzajemnie i&nbsp;wskazują, w&nbsp;jaki sposób tworzyć bardziej dostępne treści internetowe. Wykonawcom i&nbsp;autorom treści doradza się stosowanie w miarę możliwości wszystkich warstw, w&nbsp;tym także technik dodatkowych, aby zaspokoić potrzeby jak najszerszej grupy użytkowników. Należy pamiętać, że nawet treści, która są zgodne na najwyższym (AAA) poziomie, nie będą dostępne dla osób ze wszystkimi rodzajami i&nbsp;stopniami niepełnosprawności, czy też z&nbsp;niepełnosprawnością złożoną, szczególnie w zakresie problemów z&nbsp;uczeniem się oraz zrozumieniem języka.

Zachęca się wykonawców i autorów treści do zastosowania szerokiego zakresu technik, w tym technik dodatkowych, ale także do poszukiwania najlepszych praktyk stosowanych w&nbsp;danym momencie rozwoju Internetu, aby treści były w możliwie największym stopniu dostępne dla osób z różnymi dysfunkcjami. [Metadane](https://www.w3.org/WAI/WCAG21/Understanding/understanding-metadata) mogą pomóc użytkownikom w&nbsp;znalezieniu treści najbardziej dostosowanych do ich potrzeb.

### 0.3 Dokumenty uzupełniające WCAG 2.1

WCAG 2.1 są sformułowane w taki sposób, aby odpowiedzieć na oczekiwania tych, którzy potrzebują stabilnej dokumentacji technicznej — punktu odniesienia do zasad dostępności. Pozostałe dokumenty, zwane tu dokumentami uzupełniającymi, opierają się na WCAG 2.1 i&nbsp;spełniają inne ważne funkcje. W odróżnieniu od samego WCAG 2.1, mogą być aktualizowane gdy zaistnieje potrzeba wdrażania WCAG 2.1 w&nbsp;nowych technologiach internetowych. Do dokumentów uzupełniających należą:

1. „[**How to Meet WCAG**](http://www.w3.org/WAI/WCAG20/quickref/)” (Jak spełnić WCAG) — Konfigurowalna i aktualizowana na bieżąco lista odniesień (referencji) do WCAG 2.1. zawierająca wszystkie wytyczne, kryteria sukcesu i&nbsp;techniki, z których mogą korzystać autorzy podczas opracowywania i&nbsp;oceny treści internetowych. Obejmuje zarówno treści WCAG 2.0, jak i&nbsp;WCAG 2.1. Można je filtrować na wiele sposobów, aby autorzzy mogli się skupić na odpowiednich treściach.
2. „[**Understanding WCAG**](https://www.w3.org/WAI/WCAG21/Understanding/)” (zrozumienie WCAG 2.1) — przewodnik ułatwiający zrozumienie i wdrożenie WCAG 2.1. Do każdej wytycznej i&nbsp;kryterium sukcesu WCAG 2.1 powstał krótki poradnik pomagający zrozumieć ich kluczowe aspekty.
3. „[**Techniques for WCAG 2.1**](http://www.w3.org/TR/WCAG20-TECHS/)” (Techniki dla WCAG 2.1) — zbiór technik oraz często występujących błędów. Każdy z elementów przedstawiony jest w osobnym dokumencie, zawierającym opis, przykłady, kody źródłowe oraz testy.
4. „[**The WCAG Documents**](https://www.w3.org/WAI/standards-guidelines/wcag/docs/)” (Dokumenty WCAG) — opis dokumentów technicznych WCAG 2.1 w&nbsp;postaci wykresu. Pokazuje, w jaki sposób są one ze sobą powiązane.

W dokumencie „[Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/intro/wcag.php)” (Omówienie Wytycznych dla dostępności internetowej), umieszczono opis materiałów powiązanych z WCAG 2.1, w&nbsp;tym materiały edukacyjne związane z WCAG 2. Materiały dodatkowe, obejmujące takie tematy, jak analiza kosztów i&nbsp;korzyści (business case) w zakresie dostępności, propozycje planowania wdrażania wytycznych dostępności oraz kwestie prawne dotyczące dostępności znajdują się na stronie [WAI Resources](http://www.w3.org/WAI/Resources/Overview) (Omówienie zasobów WAI).

### 0.4 Wymagania dotyczące WCAG 2.1
WCAG 2.1 spełniają [zestaw wymagań dotyczących WCAG 2.1](https://w3c.github.io/wcag21/requirements/), które z kolei odziedziczyły wymagania dotyczące WCAG 2.0. Wymagania tworzą ogólne ramy wytycznych i&nbsp;zapewniają zgodność wsteczną. Grupa Robocza zastosowała również mniej formalny zestaw kryteriów akceptacji dla kryteriów sukcesu, aby zapewnić, że kryteria sukcesu są podobne pod względem stylu i&nbsp;jakości do tych zawartych w WCAG 2.0. Wymagania ograniczały to, co mogło być ujęte w WCAG 2.1. To ograniczenie było konieczne, aby zachować charakter wydania WCAG 2.1 jako <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wydanie_punktowe}}">wydania punktowego</a> WCAG 2.

### 0.5 Porównanie z WCAG 2.0
WCAG 2.1 zostały zainicjowane, aby ulepszyć wytyczne dotyczące dostępności dla trzech głównych grup: użytkowników z&nbsp;zaburzeniami funkcji poznawczych lub uczenia się, użytkowników ze słabym wzrokiem oraz użytkowników z niepełnosprawnościami powodujacymi problemy w&nbsp;korzystaniu z urządzeń przenośnych. Zaproponowano i&nbsp;oceniono wiele sposobów zaspokojenia tych potrzeb, a&nbsp;Grupa Robocza dopracowała ich zestaw. Wymagania strukturalne odziedziczone po WCAG 2.0, jasność i wpływ propozycji, a&nbsp;także przyjęty harmonogram prac, doprowadziły do powstania ostatecznego zestawu kryteriów sukcesu zawartych w niniejszej wersji. Grupa Robocza uważa, że WCAG 2.1 stopniowo rozwija wytyczne dla dostępności treści internetowych we wszystkich tych obszarach, ale podkreśla, że te wytyczne nie zaspokajają wszystkich potrzeb użytkowników.

WCAG 2.1 są oparte na WCAG 2.0 i są z nim kompatybilne wstecznie, co oznacza, że ​​strony internetowe zgodne z WCAG 2.1 są również zgodne z&nbsp;WCAG 2.0. Autorzy, którzy są zobowiązani przez polityki swoich organizacji do zgodności z&nbsp;WCAG 2.0, będą mogli aktualizować treści do WCAG 2.1 bez utraty zgodności z&nbsp;WCAG 2.0. Autorzy przestrzegający obu zestawów wytycznych powinni zdawać sobie sprawę z&nbsp;następujących różnic:

#### 0.5.1 Nowe funkcje w WCAG 2.1

WCAG 2.1 rozszerza WCAG 2.0, dodając nowe kryteria sukcesu,  wspierające je definicje, wytyczną organizującą nowe kryteria sukcesu dodatków oraz kilka dodatków do sekcji zgodności. To podejście addytywne pomaga wyjaśnić, że strony, które są zgodne z WCAG 2.1, są również zgodne z WCAG 2.0, spełniając tym samym wymagania zgodności specyficzne dla WCAG 2.0. Grupa Robocza ds. Wytycznych dla Dostępności zaleca, aby strony przyjęły WCAG 2.1 jako nowy cel zgodności, nawet jeśli formalne zobowiązania wspominają WCAG 2.0, aby zapewnić lepszą dostępność i wyprzedzić przyszłe zmiany polityki.

Następujące kryteria sukcesu są nowe w WCAG 2.1:

- [**1.3.4 Orientacja**](https://wcag.lepszyweb.pl/#sensory-characteristics) (AA)
- [**1.3.5 Określenie pożądanej wartości**](https://wcag.lepszyweb.pl/#sensory-characteristics) (AA)
- [**1.3.6 Określenie przeznaczenia**](https://wcag.lepszyweb.pl/#sensory-characteristics)(AAA)
- [**1.4.10 Dopasowanie do ekranu**](https://wcag.lepszyweb.pl/#reflow) (AA)
- [**1.4.11 Kontrast elementów nietekstowych**](https://wcag.lepszyweb.pl/#non-text-contrast) (AA)
- [**1.4.12 Odstępy w tekście**](https://wcag.lepszyweb.pl/#non-text-contrast) (AA)
- [**1.4.13 Treść spod kursora lub fokusa**](https://wcag.lepszyweb.pl/#content-on-hover-or-focust) (AA)
- [**2.1.4 Skróty klawiaturowe**](https://wcag.lepszyweb.pl/#character-key-shortcuts) (A)
- [**2.2.6 Ostrzeżenie o limicie czasu**](https://wcag.lepszyweb.pl/#timeouts) (AAA)
- [**2.3.3 Animacja po interakcji**](https://wcag.lepszyweb.pl/#animation-from-interactions) (AAA)
- [**2.5.1 Gesty dotykowe**](https://wcag.lepszyweb.pl/#pointer-gestures) (A)
- [**2.5.2 Rezygnacja ze wskazania**](https://wcag.lepszyweb.pl/#pointer-gestures) (A)
- [**2.5.3 Etykieta w nazwie**](https://wcag.lepszyweb.pl/#label-in-name) (A)
- [**2.5.4 Aktywowanie ruchem**](https://wcag.lepszyweb.pl/#motion-actuation) (A)
- [**2.5.5 Rozmiar celu dotykowego**](https://wcag.lepszyweb.pl/#target-size) (AAA)
- [**2.5.6 Równoległe mechanizmy wprowadzania danych**](https://wcag.lepszyweb.pl/#concurrent-input-mechanisms) (AAA)
- [**4.1.3 Komunikaty o stanie**](https://wcag.lepszyweb.pl/#name-role-value) (AA)

Wiele z tych kryteriów sukcesu odnosi się do nowych terminów, które zostały również dodane do słownika i&nbsp;stanowią część normatywnych wymagań kryteriów sukcesu.

W części 5. Zgodność została dodana trzecia uwaga na temat wariantów stron, a&nbsp;w&nbsp;części [Opcjonalne składniki oświadczenia o&nbsp;zgodności](glosy-zgodnosc#opcjonalne-składniki-oświadczenia-o-zgodności)  do odczytu maszynowego została dodana opcja metadanych.

#### 0.5.2 Numeracja w WCAG 2.1
Aby uniknąć zamieszania w narzędziach, dla których ważna jest kompatybilność wsteczna z WCAG 2.0, nowe kryteria sukcesu w WCAG 2.1 zostały dołączone na końcu zestawu kryteriów sukcesu w&nbsp;ramach ich wytycznych. Pozwoliło to uniknąć konieczności zmiany numeracji części kryteriów sukcesu z WCAG 2.0, co byłoby spowodowane wstawianiem nowych kryteriów sukcesu między istniejącymi kryteriami sukcesu w wytycznych. Ale spowodowało to, że kryteria sukcesu w każdej z wytycznych nie są już pogrupowane według poziomu zgodności.Kolejność kryteriów sukcesu w&nbsp;ramach każdej wytycznej nie oznacza informacji o&nbsp;poziomie zgodności; wskazuje to tylko wskaźnik poziomu zgodności (A / AA / AAA) przy samym kryterium sukcesu. W&nbsp;dokumencie [WCAG 2.1 Quick Reference](https://www.w3.org/WAI/WCAG21/quickref/) można przeglądać kryteria sukcesu pogrupowane według poziomu zgodności oraz wielu innych opcji filtrowania i sortowania.

#### 0.5.3 Zgodność z WCAG 2.1
WCAG 2.1 wykorzystują ten sam model zgodności co WCAG 2.0 z kilkoma dodatkami, które opisano w sekcji [5. Zgodność](#5-zgodność). Zakłada się, że witryny zgodne z WCAG 2.1 są również zgodne z&nbsp;WCAG 2.0, co oznacza, że ​​spełniają wymagania wszystkich zasad odnoszących się do WCAG 2.0, a&nbsp;jednocześnie lepiej spełniają potrzeby użytkowników we współczesnej sieci internetowej.

### 0.6 Późniejsze wersje wytycznych dotyczących dostępności
Równolegle z WCAG 2.1 Grupa Robocza ds. Wytycznych dla Dostępności opracowuje kolejną ważną wersję wytycznych dla dostępności. Przewiduje się, że rezultatem tych prac będzie bardziej znacząca restrukturyzacja wytycznych dla dostępności internetowej, niż byłoby to realne w&nbsp;przypadku wydania punktowego WCAG&nbsp;2. Prace prowadzone są zgodnie z&nbsp;ukierunkowaną na badania, skoncentrowaną na użytkownikach metodologią projektowania, aby zapewnić najbardziej efektywny i elastyczny wynik, w&nbsp;tym role związane z&nbsp;tworzeniem treści, obsługą programu użytkownika i obsługą narzędzi tworzenia treści. Jest to wysiłek wieloletni, dlatego też WCAG 2.1 są potrzebne jako tymczasowy środek zapewnienia zaktualizowanych wytycznych dla dostępności internetowej, aby odzwierciedlić zmiany w sieci internetowej od czasu publikacji WCAG 2.0. Grupa Robocza może również opracować dodatkowe wersje tymczasowe, kontynuując prace nad WCAG 2.2, aby zapewnić dodatkowe wsparcie do czasu, zanim zostanie ukończona kolejna główna wersja.

## {% include ks/z-1.md %}

### {% include ks/w-1-1.md %}

{% include ks/1-1-1.md %}

### {% include ks/w-1-2.md %}

{% include ks/1-2-1.md %}

{% include ks/1-2-2.md %}

{% include ks/1-2-3.md %}

{% include ks/1-2-4.md %}

{% include ks/1-2-5.md %}

{% include ks/1-2-6.md %}

{% include ks/1-2-7.md %}

{% include ks/1-2-8.md %}

{% include ks/1-2-9.md %}

### {% include ks/w-1-3.md %}

{% include ks/1-3-1.md %}

{% include ks/1-3-2.md %}

{% include ks/1-3-3.md %}

{% include ks/1-3-4.md %}

{% include ks/1-3-5.md %}

{% include ks/1-3-6.md %}

### {% include ks/w-1-4.md %}

{% include ks/1-4-1.md %}

{% include ks/1-4-2.md %}

{% include ks/1-4-3.md %}

{% include ks/1-4-4.md %}

{% include ks/1-4-5.md %}

{% include ks/1-4-6.md %}

{% include ks/1-4-7.md %}

{% include ks/1-4-8.md %}

{% include ks/1-4-9.md %}

{% include ks/1-4-10.md %}

{% include ks/1-4-11.md %}

{% include ks/1-4-12.md %}

{% include ks/1-4-13.md %}

## {% include ks/z-2.md %}

### {% include ks/w-2-1.md %}
{% include ks/2-1-1.md %}

{% include ks/2-1-2.md %}

{% include ks/2-1-3.md %}

{% include ks/2-1-4.md %}

### {% include ks/w-2-2.md %}
{% include ks/2-2-1.md %}

{% include ks/2-2-2.md %}

{% include ks/2-2-3.md %}

{% include ks/2-2-4.md %}

{% include ks/2-2-5.md %}

{% include ks/2-2-6.md %}

### {% include ks/w-2-3.md %}
{% include ks/2-3-1.md %}

{% include ks/2-3-2.md %}

{% include ks/2-3-3.md %}

### {% include ks/w-2-4.md %}
{% include ks/2-4-1.md %}

{% include ks/2-4-2.md %}

{% include ks/2-4-3.md %}

{% include ks/2-4-4.md %}

{% include ks/2-4-5.md %}

{% include ks/2-4-6.md %}

{% include ks/2-4-7.md %}

{% include ks/2-4-8.md %}

{% include ks/2-4-9.md %}

{% include ks/2-4-10.md %}

### {% include ks/w-2-5.md %}
{% include ks/2-5-1.md %}

{% include ks/2-5-2.md %}

{% include ks/2-5-3.md %}

{% include ks/2-5-4.md %}

{% include ks/2-5-5.md %}

{% include ks/2-5-6.md %}


## {% include ks/z-3.md %}

### {% include ks/w-3-1.md %}
{% include ks/3-1-1.md %}

{% include ks/3-1-2.md %}

{% include ks/3-1-3.md %}

{% include ks/3-1-4.md %}

{% include ks/3-1-5.md %}

{% include ks/3-1-6.md %}

### {% include ks/w-3-2.md %}
{% include ks/3-2-1.md %}

{% include ks/3-2-2.md %}

{% include ks/3-2-3.md %}

{% include ks/3-2-4.md %}

{% include ks/3-2-5.md %}

### {% include ks/w-3-3.md %}
{% include ks/3-3-1.md %}

{% include ks/3-3-2.md %}

{% include ks/3-3-3.md %}

{% include ks/3-3-4.md %}

{% include ks/3-3-5.md %}

{% include ks/3-3-6.md %}


## {% include ks/z-4.md %}

### {% include ks/w-4-1.md %}
{% include ks/4-1-1.md %}

{% include ks/4-1-2.md %}

{% include ks/4-1-3.md %}

## 5. Zgodność

W tej części wymieniono wymagania dotyczące <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.zgodnosc | strip_html | replace: '*', ''}}">zgodności</a> z wytycznymi WCAG 2.1. Zawarto także informacje, w jaki sposób można składać oświadczenia o zgodności (są opcjonalne). Na końcu wyjaśnione zostało pojęcie wspierania (obsługiwania) dostępności, ponieważ tylko technologie <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc | strip_html | replace: '*', ''}}">obsługujące dostępność</a> mogą stanowić <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.stanowiace_podstawe_zgodnosci | strip_html | replace: '*', '' | strip_html | replace: '*', ''}}">wiarygodną podstawę zgodności</a>. Dokument [Understanding Conformance](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html) zawiera dalsze wyjaśnienie pojęcia <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc | strip_html | replace: '*', '' | strip_html | replace: '*', ''}}">obsługi dostępności</a>.

### 5.1 Interpretacja wymagań normatywnych

Główna treść WCAG 2.1 ma charakter <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.normatywny | strip_html | replace: '*', ''}}">normatywny</a> i określa wymagania, które mają wpływ na deklaracje zgodności. Materiał wprowadzający, dodatki, sekcje oznaczone jako „nienormatywne”, diagramy, przykłady i uwagi mają charakter <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.informacyjne | strip_html | replace: '*', ''}}">informacyjny</a> (nienormatywny). Materiały nienormatywne zawierają informacje dodatkowe, które pomagają interpretować wytyczne, ale nie tworzą wymagań, które mają wpływ na deklarację zgodności.

Słowa kluczowe *MOGĄ*, *MUSZĄ*, *NIE MUSZĄ*, *NIE POLECANE*, *POLECANE*, *POWINNY* i *NIE POWINNY* należy interpretować zgodnie z opisem w&nbsp;[RFC2119](https://www.w3.org/TR/WCAG21/#bib-RFC2119).


### 5.2 Wymogi dotyczące zgodności

Aby strona internetowa była zgodna z wytycznymi WCAG 2.1, muszą być spełnione wszystkie poniższe wymagania dotyczące zgodności:

### 5.2.1 Poziom zgodności
Jeden z poniższych poziomów zgodności jest w pełni osiągnięty:

- **Poziom A** (minimalny): <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa | strip_html | replace: '*', ''}}">Strona internetowa</a> <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.spelnienie_kryterium_sukcesu | strip_html | replace: '*', ''}}">spełnia</a>  wszystkie kryteria sukcesu na poziomie A albo dostępna jest <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wersja_alternatywna_zapewniajaca_zgodnosc | strip_html | replace: '*', ''}}">wersja alternatywna spełniająca kryteria sukcesu</a> na poziomie A.
- **Poziom AA**: Strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A oraz na poziomie AA albo dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie A i poziomie AA.
- **Poziom AAA**: Strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A, na poziomie AA oraz na poziomie AAA albo dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie A, poziomie AA i poziomie AAA.

    *Uwaga 1:* Chociaż zgodność może zostać osiągnięta tylko na oznaczonych poziomach, zachęca się autorów, aby podawali (w oświadczeniu zgodności) jakikolwiek postęp na drodze do spełnienia kryteriów sukcesu na poziomach wyższych niż osiągnięty.

    *Uwaga 2:* Odradza się wyznaczania poziomu AAA jako wymaganego dla całych witryn, ponieważ w przypadku niektórych treści spełnienie wszystkich kryteriów sukcesu na poziomie AAA nie jest możliwe.

### 5.2.2 Poziom zgodności
<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.zgodnosc | strip_html | replace: '*', ''}}">Zgodność</a> (i poziom zgodności) dotyczy całej <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa | strip_html | replace: '*', ''}}">strony</a> i nie można jej osiągnąć, jeśli jakaś część strony zostanie wyłączona z oceny.

    *Uwaga 1:* W celu ustalenia zgodności przyjmuje się, że wersje alternatywne części treści strony są częścią strony, jeśli wersje alternatywne są dostępne bezpośrednio z danej strony, np. długi opis lub alternatywna prezentacja nagrania wideo.

    *Uwaga 2:* Autorzy stron internetowych, którzy nie mogą osiągnąć zgodności ze względu na treść pozostającą poza ich kontrolą, mogą rozważyć [Stwierdzenie częściowej zgodności](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#conformance-partial).

    *Uwaga 3:* Cała strona zawiera każdą odmianę strony, która jest automatycznie prezentowana przez stronę dla różnych rozmiarów ekranu (np. odmiany strony responsywnej). Każda z tych odmian musi być zgodna (lub musi mieć zgodną alternatywną wersję), aby cała strona była zgodna.

### 5.2.3 Całe procesy
Jeśli dana <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa | strip_html | replace: '*', ''}}">strona</a> jest jedną z wielu stron prezentujących jakąś <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.procedura | strip_html | replace: '*', ''}}">procedurę</a> (tzn. sekwencję kroków, które należy wykonać, aby dokończyć jakąś czynność), to wszystkie wszystkie strony prezentujące etapy procesu spełniają wymogi co najmniej na tym sammym poziomie zgodności. (Inaczej - zgodność na określonym poziomie nie jest osiągnięta, jeżeli którakolwiek ze stron prezentujących którykolwiek z etapów procesu nie spełnia wszystkich wymogów zgodności na tym poziomie.)

   *Przykład:* Sklep internetowy prezentuje na kilku stronach procedurę wybierania i zakupu produktów. Wszystkie strony w tej procedurze, od początku do końca (do wykonania płatności) są zgodne na tym samym poziomie.

### 5.2.4 Użycie technologii wspierających dostępność
Tylko <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc | strip_html | replace: '*', ''}}">technologie obsługujące dostępność</a> są uwzględniane jako podstawa spełnienia kryteriów sukcesu. Każda informacja czy funkcjonalność, która nie jest dostarczona w postaci obsługującej dostępność, muszą mieć swoją wersję alternatywną obsługującą dostępność. (Więcej informacji: [Understanding accessibility suport](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-accessibility-support-head)).

### 5.2.5 Brak zakłóceń

Jeśli na stronie wykorzystywane są technologie, które nie obsługują dostępności lub są użyte tak, że nie obsługują dostępności, to technologie te nie blokują użytkownikom dostępu do reszty strony. Dodatkowo, <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa | strip_html | replace: '*', ''}}">strona internetowa</a> jako całość nadal spełnia wymogi zgodności pod każdym z następujących warunków:

    1. kiedy technologia, która nie jest <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.stanowiace_podstawe_zgodnosci | strip_html | replace: '*', ''}}">uwzględniana</a>, jest włączona w programie użytkownika,
    2. kiedy technologia, która nie jest uwzględniana, jest wyłączona w programie użytkownika, oraz
    3. kiedy technologia, która nie jest uwzględniana, nie jest wspierana przez program użytkownika.

 Ponadto, następujące kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ niezastosowanie poniższych kryteriów mogłoby uniemożliwiać korzystanie ze strony:

  - **1.4.2 Kontrola odtwarzania dźwięku**
  - **2.1.2 Brak pułapki na klawiaturę**
  - **2.3.1 Trzy błyski lub wartości poniżej progu**
  - **2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie**

  *Uwaga:* Jeśli strona nie może być zgodna (na przykład testowa strona zgodności lub strona przykładowa), to nie można jej uwzględnić w zakresie zgodności ani w oświadczenia o zgodności.

Więcej informacji, w tym przykłady, w [Understanding Conformance Requirements](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conformance-requirements-head).


### 5.3 Oświadczenie o zgodności (opcjonalne)
Zgodność zdefiniowana została tylko dla (pojedynczych) stron internetowych. Można jednak złożyć oświadczenie o zgodności obejmujące pojedynczą stronę, kilka stron lub całe zestawy stron internetowych, np. witrynę.

#### 5.3.1 Wymagane elementy oświadczenia o zgodności
Oświadczenia o zgodności nie są wymagane. Autorzy mogą dostosować się do WCAG 2.1 bez oświadczania zgodności. Jeśli jednak oświadczenie o zgodności zostanie złożone, wówczas musi zawierać następujące informacje:

1. Data złożenia oświadczenia.
2. Tytuł wytycznych, wersja oraz identyfikator URI („Wytyczne dla dostępności treści internetowych 2.1” pod adresem https://www.w3.org/TR/WCAG21/ (wersja anglojęzyczna). W WCAG 2.0 był to datowany URI, który może wymagać korekty.
3. Osiągnięty poziom zgodności (Poziom A, AA lub AAA).
4. Zwięzły opis stron internetowych, taki jak lista adresów URI objętych oświadczeniem, wraz z adnotacją czy włączone są również poddomeny.

    *Uwaga 1:* Strony mogą być opisane oddzielnie, ale może być także użyty jeden opis dla wszystkich adresów URI.

    *Uwaga 2:* Produkty internetowe nie posiadające adresów URI przed instalacją na stronie klienta, mogą zostać opatrzone informacją, że po instalacji będą spełniać wymogi.

5. Lista uwzględnionych technologii tworzenia treści internetowych.

*Uwaga:* Wykorzystywane logo zgodności jest równoznaczne ze złożeniem oświadczenie o zgodności i musi wystąpić razem z&nbsp;wymaganymi, wyżej wymienionymi składowymi oświadczenia o zgodności.

#### 5.3.2 Opcjonalne składniki oświadczenia o zgodności
Poza wymaganymi składowymi oświadczenia o zgodności, które zostały wymienione powyżej, warto rozważyć umieszczenie dodatkowych informacji, przydatnych dla użytkowników. Polecane dodatkowe informacje to na przykład:

- Wykaz kryteriów sukcesu wykraczających poza poziom zgodności zawarty w oświadczeniu. Taką informację należy podać w formie, którą użytkownik mógłby wykorzystać, najlepiej jako metadane, które mogą być odczytywane maszynowo.
- Wykaz poszczególnych technologii, które „są wykorzystywane, ale nie zostały uwzględnione w ocenie zgodności”.
- Wykaz programów użytkownika, w tym technologii pomocniczych, wykorzystanych do testowania treści.
- Wykaz szczególnych cech dostępności, które mogą być odczytywane maszynowo
- Informacje na temat wszelkich kroków podejmowanych w celu zwiększenia dostępności, a które wykraczają poza kryteria sukcesu.
- Lista poszczególnych technologii, które zostały uwzględnione w ocenie, w formie metadanych odczytywalnych maszynowo.
- Wersja metadanych listy technologii uwzględnionych w ocenie, w formie odczytywalej maszynowo.
- Wersja metadanych oświadczenia zgodności, w formie odczytywalej maszynowo.

   *Uwaga 1:* Więcej informacji oraz przykładowe oświadczenia zgodności można znaleźć w dokumencie [Understanding Conformance Claims](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance).

   *Uwaga 2:* Więcej informacji na temat wykorzystania metadanych w oświadczeniach zgodności znajduje się w dokumencie [Understanding Metadata](https://www.w3.org/TR/UNDERSTANDING-WCAG20/appendixC).

### 5.4 Oświadczenie o częściowej zgodności – treść umieszczana przez dostawców zewnętrznych
Czasem strony internetowe tworzone są w taki sposób, aby móc je później uzupełnić dodatkową treścią. Na przykład jest to program do poczty elektronicznej, blog, artykuł, który pozwala użytkownikom na dodanie swoich komentarzy, lub też aplikacja pozwalająca na tworzenie treści przez użytkowników. Kolejny przykład, to strona, taka jak portal lub witryna z wiadomościami, złożona z treści zebranych od wielu autorów lub też witryna, które automatycznie umieszcza treść pobraną z innych źródeł w danym okresie czasu, np. dynamicznie umieszczane reklamy.

W takich przypadkach w momencie opublikowania strony nie można przewidzieć, jaka dodatkowa, niekontrolowana przez autora treść pojawi się w przyszłości. Ważna jest, aby pamiętać, iż niekontrolowana treść może negatywnie wpłynąć także na dostępność treści umieszczonej przez autora. Istnieją dwa rozwiązania:

1. Oświadczenie o zgodności można oprzeć na podstawie najlepszej wiedzy posiadanej na dany moment. Oznacza to, iż strona jest zgodna, jeśli jest monitorowana i korygowana (treść niezgodna jest usuwana lub zmieniona tak, aby strona spełniała wymogi zgodności) w ciągu dwóch dni roboczych; od tego momentu można ustalać zgodność strony, wykluczając błędy w treściach zewnętrznych, które są poprawiane lub usuwane, kiedy się je napotka. Nie można złożyć oświadczenia zgodności, jeśli monitorowanie lub korekta niezgodnej treści nie jest możliwa.

**LUB**:

2. Można złożyć „Oświadczenie częściowej zgodności”, że strona nie jest zgodna, ale spełniałaby wymogi zgodności, gdyby pewne jej części zostały usunięte. Brzmienie takiego oświadczenia jest następujące: „a strona nie jest zgodna, ale byłaby zgodna z WCAG 2.1 na poziomie X, gdyby następujące treści z niekontrolowanych przez autora źródeł zostały usunięte”. Dodatkowo, treść niekontrolowana musi spełnić poniższe kryteria:

   a. Nie jest to treść, która jest pod kontrolą autora.

   b. Jest opisana w sposób umożliwiający identyfikację przez użytkowników (np. nie można stwierdzić jedynie „wszystkie części, których nie kontrolujemy”, muszą być one wyraźnie oznaczone).

### 5.5 Oświadczenie częściowej zgodności – język

„Oświadczenie częściowej zgodności ze względu na język” może zostać złożone w przypadkach, kiedy dana strona nie jest zgodna, jednak mogłaby spełnić wymogi zgodności, gdyby istniało wsparcie dla dostępności wszystkich języków użytych na tej stronie. Brzmienie takiego oświadczenia jest następujące: „Niniejsza strona nie jest zgodna, lecz spełniałaby wymogi WCAG 2.1 na poziomie X, gdyby istniało wsparcie dla dostępności następujących języków:”.

## 6. Słownik
Definicje słownikowe wykorzystane w WCAG 2.1 opublikowane zostay w odrębnym dokumencie pod adresem: [Słownik](slownik).

## 7. Przeznaczenie pól wejściowych w komponentach interfejsu uzytkowników

Ta część zawiera listę typowych celów pól wejściowych w komponentach interfejsu uzytkowników. Terminy poniżej  nie są słowami kluczowymi, których należy użyć, ale reprezentują cele, które muszą zostać ujęte w taksonomii przyjętej przez stronę internetową. W stosownych przypadkach, autorzy oznaczają kontrolki przy pomocy wybranej taksonomii, aby wskazać cel semantyczny. Daje to potencjalnym programom użytkownika i technologiom pomocniczym możliwość stosowania spersonalizowanych prezentacji, które mogą umożliwić większej liczbie osób zrozumienie i wykorzystanie treści.

**UWAGA** Lista  celów typów pól wejściowych jest oparta na celach kontrolek zdefiniowanych w części HTML 5.2 Autofill field, ale ważne jest, aby zrozumieć, że inna technologia może mieć niektóre lub wszystkie z tych samych pojęć zdefiniowanych w jej specyfikacji i wymagane są tylko te pojęcia, które są mapowane do poniższych znaczeń.

Poniższe cele pól wejsciowych mają odnosić się do użytkownika treści i dotyczyć tylko informacji związanych z tą osobą.

- **name** - pełna nazwa
- honorific-prefix - Przedrostek lub tytuł (np. „Pan”, „Pani”, „Dr”, „Prof.”)
- **given-name** - imię (w niektórych kulturach zachodnich, znane również jako „pierwsze imię” )
- **additional-name** - dodatkowa nazwy (w niektórych kulturach zachodnich, znane również jako drugie imię, inne niż pierwsze)

- **family-name** - nazwisko rodowe (w niektórych kulturach zachodnich znane również jako nazwisko)
- **honorific-suffix** - przyrostek (np., „Jr.”, „B.Sc.”, „MBASW”, „II”)
- **nickname** - pseudonim, nazwa ekranowa: zwykle krótka nazwa zamiast pełnej nazwy
- **organization-title** - stanowisko (e.g., "Inżynier oprogramowania", "Wiceprezes", "Zastępca dyrektora generalnego")
- **username** - nazwa użytkownika
- **new-password** - nowe hasło (np. podczas tworzenia konta lub zmiany hasła)
- **current-password** - bieżące hasło do konta określone w polu nazwy użytkownika (np. podczas logowania)
- **organization** - nazwa firmy odpowiadająca osobie, adresowi lub danym kontaktowym w innych polach powiązanych z tym polem
- **street-address** - adres ulicy (wiele linii, zachowuje nowe linie )
- **address-line1** - adres ulicy (jedna linia na pole, linia 1)
- **address-line2** - adres ulicy (jedna linia na pole, linia 2)
- **address-line3** - adres ulicy (jedna linia na pole, linia 3)
- **address-level4** - najbardziej szczegółowy poziom administracyjny, w adresach z czterema poziomami administracyjnymi
- **address-level3** - trzeci poziom administracyjny, w adresach z co najmniej trzema poziomami administracyjnymi
- **address-level2** - drugi poziom administracyjny, w adresach z dwoma lub więcej poziomami administracyjnymi; w krajach o dwóch poziomach administracyjnych zwykle jest to miasto, miejscowość, wieś lub inna miejscowość, w której znajduje się odpowiedni adres
- **address-level1** - najszerszy poziom administracyjny w adresie, tj. prowincja, w której znajduje się miejscowość; na przykład w USA byłby to stan; w Szwajcarii byłby to kanton; w Polsce województwo
- **country** - kod kraju
- **country-name** - nazwa kraju
- **postal-code** - kod pocztowy, kod poczty, kod ZIP, kod CEDEX (jeśli CEDEX, dołącz „CEDEX” oraz, w stosownych przypadkach, pole na address-level2)
- **cc-name** - pełna nazwa w brzmieniu podanym na dokumencie płatniczym
- **cc-given-name** - imię podane na dokumencie płatniczym (w niektórych kulturach zachodnich, znane również jako „pierwsze imię”)
- **cc-additional-name** - dodatkowe nazwy podane na dokumencie płatniczym (w niektórych kulturach zachodnich, znane również jako „drugie imię” inne niż pierwsze)
- **cc-family-name** - nazwisko podane na dokumencie płatniczym (w niektórych kulturach zachodnich, znane również jako nazwisko rodowe)
- **cc-number** - od identyfikujący dokument płatniczy (np. numer karty kredytowej)
- **cc-exp** - data ważności dokumentu płatniczego
- **cc-exp-month** - miesiąc daty ważności dokumentu płatniczego
- **cc-exp-year** - rok daty ważności dokumentu płatniczego
- **cc-csc** - Kod bezpieczeństwa dokumentu płatniczego (znany również jako kod bezpieczeństwa karty (CSC), kod weryfikacji karty (CVC), wartość weryfikacji karty (CVV), kod panelu podpisue (SPC), identyfikator karty kredytowej (CCID), itp.)
- **cc-type** - rodzaj dokumentu płatniczego
- **transaction-currency** - waluta, której użytkownik chce dokonać transakcji
- **transaction-amount** - kwota transakcji (np. przy wprowadzaniu oferty lub ceny sprzedaży)
- **language** - preferowany język
- **bday** - urodziny
- **bday-day** - dzień urodzin
- **bday-month** - miesiąc urodzin
- **bday-year** - rok urodzin
- **sex** - tożsamość płciowa (np. kobieta, mężczyzna, fa’afafine)
- **url** - adres strony głównej lub innej strony internetowej odpowiadająca firmie, osobie, adresowi lub danym kontaktowym w innych polach powiązanych z tym polem
- **photo** - zdjęcie, ikona lub inny obraz odpowiadający firmie, osobie, adresowi lub danym kontaktowym w innych polach powiązanych z tym polem
- **tel** - pełny numer telefonu, w tym kod kraju
- **tel-country-code** - kod kraju w numerze kierunkowym telefonu
- **tel-national** - numer telefonu bez kodu regionu, z prefiksem wewnętrznym kraju, jeśli ma zastosowanie
- **tel-area-code** - element numeru kierunkowego numeru telefonu, w razie potrzeby z prefiksem wewnętrznym kraju
- **tel-local** - numer telefonu bez kodu kraju i numeru kierunkowego
- **tel-local-prefix** - pierwsza część elementu numeru telefonu, która następuje po numerze kierunkowym, gdy ten element jest podzielony na dwa elementy
- **tel-local-suffix** - rruga część elementu numeru telefonu, która następuje po numerze kierunkowym, gdy ten element jest podzielony na dwa elementy
- **tel-extension** - numer telefonu wewnętrznego
- **email** - adres e-mail
- **impp** - adres URL reprezentujący punkt końcowy protokołu wiadomości błyskawicznych (np, "aim:goim?screenname=example" lub "xmpp:fred@example.net")

## A. Poddziękowania
Dodatkowe informacje na temat uczestnictwa w Grupie Roboczej Wytyczne dla Dostępności (AG WG) można znaleźć na [stronie głównej Grupy Roboczej](https://www.w3.org/WAI/GL/).

### A.1 Uczestnicy AG WG aktywni w opracowaniu tego dokumentu
- Jake Abma (Invited Expert)
- Shadi Abou-Zahra (W3C)
- Chuck Adams (Oracle Corporation)
- Amani Ali (Nomensa)
- Jim Allan (Invited Expert)

- Paul Adam (Deque Systems, Inc.)
- Christopher Auclair (VitalSource \| Ingram Content Group)
- Jon Avila (Level Access)
- Tom Babinszki (IBM Corporation)
- Bruce Bailey (U.S. Access Board)
- Renaldo Bernard (University of Southampton)
- Chris Blouch (Level Access)
- Denis Boudreau (Deque Systems, Inc.)
- Judy Brewer (W3C)
- Shari Butler (Pearson plc)
- Thaddeus Cambron (Invited Expert)
- Alastair Campbell (Nomensa)
- Laura Carlson (Invited Expert)
- Louis Cheng (Google)
- Pietro Cirrincione (Invited Expert)
- Vivienne Conway (Web Key IT Pty Ltd)
- Michael Cooper (W3C)
- Romain Deltour (DAISY Consortium)
- Wayne Dick (Knowbility, Inc)
- Chaohai Ding (University of Southampton)
- Kim Dirks (Thompson Reuters)
- Shwetank Dixit (BarrierBreak Technologies)
- Anthony Doran (TextHelp)
- E.A. Draffan (University of Southampton)
- Eric Eggert (W3C)
- Michael Elledge (Invited Expert)
- Wilco Fiers (Deque Systems, Inc.)
- Detlev Fischer (Invited Expert)
- John Foliot (Deque Systems, Inc.)
- Matt Garrish (DAISY Consortium)
- Alistair Garrison (Level Access)
- Michael Gower (IBM Corporation)
- Jon Gunderson
- Markku Hakkinen (Educational Testing Service)
- Katie Haritos-Shea (Knowbility, Inc)
- Andy Heath (Invited Expert)
- Shawn Henry (W3C)
- Thomas Hoffman (Educational Testing Service)
- Sarah Horton (The Paciello Group, LLC)
- Stefan Johansson (Invited Expert)
- Marc Johlic (IBM Corporation)
- Rick Johnson (VitalSource \| Ingram Content Group)
- Crystal Jones (Microsoft Corporation)
- Andrew Kirkpatrick (Adobe)
- John Kirkwood (Invited Expert)
- Jason Kiss (Department of Internal Affairs, New Zealand Government)
- Maureen Kraft (IBM Corporation)
- JaEun Ku (University of Illinois at Urbana-Champaign)
- Patrick Lauke (The Paciello Group, LLC)
- Shawn Lauriat (Google, Inc.)
- Steve Lee (Invited Expert)
- Alex Li (Microsoft Corporation)
- Chris Loiselle (Invited Expert)
- Greg Lowney (Invited Expert)
- Adam Lund (Thomson Reuters)
- David MacDonald (Invited Expert)
- Erich Manser (IBM Corporation)
- Kurt Mattes (Deque Systems, Inc.)
- Scott McCormack (Level Access)
- Chris McMeeking (Deque Systems, Inc.)
- Jan McSorley (Pearson plc)
- Neil Milliken (Unify Software and Solutions)
- Rachael Montgomery (MITRE Corporation)
- Mary Jo Mueller (IBM Corporation)
- Brooks Newton (Thomson Reuters)
- James Nurthen (Oracle Corporation)
- Joshue O Connor (Invited Expert)
- Sailesh Panchang (Deque Systems, Inc.)
- Charu Pandhi (IBM Corporation)
- Kim Patch (Invited Expert)
- Melanie Philipp (Deque Systems, Inc.)
- Mike Pluke (Invited Expert)
- Ian Pouncey (The Paciello Group, LLC)
- Ruoxi Ran (W3C)
- Stephen Repsher (The Boeing Company)
- Jan Richards (Invited Expert)
- John Rochford (Invited Expert)
- Marla Runyan (Invited Expert)
- Stefan Schnabel (SAP SE)
- Ayelet Seeman (Invited Expert)
- Lisa Seeman-Kestenbaum (Invited Expert)
- Glenda Sims (Deque Systems, Inc.)
- Avneesh Singh (DAISY Consortium)
- David Sloan (The Paciello Group, LLC)
- Alan Smith (Invited Expert)
- Jim Smith (Unify Software and Solutions)
- Adam Solomon (Invited Expert)
- Jaeil Song (National Information Society Agency (NIA))
- Jeanne Spellman (The Paciello Group, LLC)
- Makoto Ueki (Invited Expert)
- Jatin Vaishnav (Deque Systems, Inc.)
- Gregg Vanderheiden (Raising the Floor)
- Evangelos Vlachogiannis (Fraunhofer Gesellschaft)
- Kathleen Wahlbin (Invited Expert)
- Can Wang (Zhejiang University)
- Léonie Watson (The Paciello Group, LLC)
- Jason White (Educational Testing Service)
- Mark Wilcock (Unify Software and Solutions)

### A.2 Inni wcześniej aktywni uczestnicy WCAG WG oraz osoby, które miały swój wkład w powstawaniu WCAG 2.0, WCAG 2.1 lub zasobów pomocniczych

Paul Adam, Jenae Andershonis, Wilhelm Joys Andersen, Andrew Arch, Avi Arditti, Aries Arditi, Mark Barratt, Mike Barta, Sandy Bartell, Kynn Bartlett, Chris Beer, Charles Belov, Marco Bertoni, Harvey Bingham, Chris Blouch, Paul Bohman, Frederick Boland, Denis Boudreau, Patrice Bourlon, Andy Brown, Dick Brown, Doyle Burnett, Raven Calais, Ben Caldwell, Tomas Caspers, Roberto Castaldo, Sofia Celic-Li, Sambhavi Chandrashekar, Mike Cherim, Jonathan Chetwynd, Wendy Chisholm, Alan Chuter, David M Clark, Joe Clark, Darcy Clarke, James Coltham, Earl Cousins, James Craig, Tom Croucher, Pierce Crowell, Nir Dagan, Daniel Dardailler, Geoff Deering, Sébastien Delorme, Pete DeVasto, Iyad Abu Doush, Sylvie Duchateau, Cherie Eckholm, Roberto Ellero, Don Evans, Gavin Evans, Neal Ewers, Steve Faulkner, Bengt Farre, Lainey Feingold, Wilco Fiers, Michel Fitos, Alan J. Flavell, Nikolaos Floratos, Kentarou Fukuda, Miguel Garcia, P.J. Gardner, Alistair Garrison, Greg Gay, Becky Gibson, Al Gilman, Kerstin Goldsmith, Michael Grade, Karl Groves, Loretta Guarino Reid, Jon Gunderson, Emmanuelle Gutiérrez y Restrepo, Brian Hardy, Eric Hansen, Benjamin Hawkes-Lewis, Sean Hayes, Shawn Henry, Hans Hillen, Donovan Hipke, Bjoern Hoehrmann, Allen Hoffman, Chris Hofstader, Yvette Hoitink, Martijn Houtepen, Carlos Iglesias, Richard Ishida, Jonas Jacek, Ian Jacobs, Phill Jenkins, Barry Johnson, Duff Johnson, Jyotsna Kaki, Shilpi Kapoor, Leonard R. Kasday, Kazuhito Kidachi, Ken Kipness, Johannes Koch, Marja-Riitta Koivunen, Preety Kumar, Kristjan Kure, Andrew LaHart, Gez Lemon, Chuck Letourneau, Aurélien Levy, Harry Loots, Scott Luebking, Tim Lacy, Jim Ley, Alex Li, William Loughborough, N Maffeo, Mark Magennis, Kapsi Maria, Luca Mascaro, Matt May, Sheena McCullagh, Liam McGee, Jens Oliver Meiert, Niqui Merret, Jonathan Metz, Alessandro Miele, Steven Miller, Mathew J Mirabella, Matt May, Marti McCuller, Sorcha Moore, Charles F. Munat, Robert Neff, Charles Nevile, Liddy Nevile, Dylan Nicholson, Bruno von Niman, Tim Noonan, Sebastiano Nutarelli, Graham Oliver, Sean B. Palmer, Devarshi Pant, Nigel Peck, Anne Pemberton, David Poehlman, Ian Pouncey, Charles Pritchard, Kerstin Probiesch, W Reagan, Adam Victor Reed, Chris Reeve, Chris Ridpath, Lee Roberts, Mark Rogers, Raph de Rooij, Gregory J. Rosmaita, Matthew Ross, Sharron Rush, Joel Sanda, Janina Sajka, Roberto Scano, Gordon Schantz, Tim van Schie, Wolf Schmidt, Stefan Schnabel, Cynthia Shelly, Glenda Sims, John Slatin, Becky Smith, Jared Smith, Andi Snow-Weaver, Neil Soiffer, Mike Squillace, Michael Stenitzer, Diane Stottlemyer, Christophe Strobbe, Sarah J Swierenga, Jim Thatcher, Terry Thompson, Justin Thorp, David Todd, Mary Utt, Jean Vanderdonckt, Carlos A Velasco, Eric Velleman, Gijs Veyfeyken, Dena Wainwright, Paul Walsch, Daman Wandke, Richard Warren, Elle Waters, Takayuki Watanabe, Gian Wild, David Wooley, Wu Wei, Kenny Zhang, Leona Zumbo.

### A.3 Instytucje finansujące
Niniejsza publikacja została częściowo sfinansowana ze środków federalnych USA z Health and Human Services, National Institute on Disability, Independent Living and Rehabilitation Research (NIDILRR), początkowo pw ramach kontraktu numer ED-OSE-10-C-0067, a obecnie w ramach kontraktu numer HHSP23301500054C. Treść niniejszej publikacji niekoniecznie odzwierciedla poglądy lub politykę amerykańskiego Departamentu Zdrowia i Opieki Społecznej lub Departamentu Edukacji USA, a wzmianka o nazwach handlowych, produktach komercyjnych lub organizacjach nie oznacza poparcia ze strony rządu USA.

## B. Literatura

### B.1 Literatura normatywna

[css3-values]
: [CSS Values and Units Module Level 3.](https://www.w3.org/TR/css-values-3/) Tab Atkins Jr.; Elika Etemad. W3C. 29 September 2016. W3C Candidate Recommendation. URL: https://www.w3.org/TR/css-values-3/

[pointerevents]
: [Pointer Events](https://www.w3.org/TR/pointerevents/). Jacob Rossi; Matt Brubeck. W3C. 24 February 2015. W3C Recommendation. URL: https://www.w3.org/TR/pointerevents/

[WCAG20]
: [Web Content Accessibility Guidelines (WCAG) 2.0.](https://www.w3.org/TR/WCAG20/) Ben Caldwell; Michael Cooper; Loretta Guarino Reid; Gregg Vanderheiden et al. W3C. 11 December 2008. W3C Recommendation. URL: https://www.w3.org/TR/WCAG20/

### B.2 Literatura informacyjna
[HARDING-BINNIE]
: *Independent Analysis of the ITC Photosensitive Epilepsy Calibration Test Tape.* Harding G. F. A.; Binnie, C.D..2002.

[IEC-4WD]
: *IEC/4WD 61966-2-1: Colour Measurement and Management in Multimedia Systems and Equipment - Part 2.1: Default Colour Space - sRGB.* May 5, 1998.

[RFC2119]
: [Key words for use in RFCs to Indicate Requirement Levels.](https://tools.ietf.org/html/rfc2119) S. Bradner. IETF. March 1997. Best Current Practice. URL: https://tools.ietf.org/html/rfc2119

[sRGB]
: [A Standard Default Color Space for the Internet - sRGB, Version 1.10.](https://www.w3.org/Graphics/Color/sRGB.html) M. Stokes; M. Anderson; S. Chandrasekar; R. Motta.November 5, 1996. URL: https://www.w3.org/Graphics/Color/sRGB.html

[UAAG10]
: [User Agent Accessibility Guidelines 1.0.](https://www.w3.org/TR/UAAG10/) Ian Jacobs; Jon Gunderson; Eric Hansen. W3C. 17 December 2002. W3C Recommendation. URL: https://www.w3.org/TR/UAAG10/

[UNESCO]
: [International Standard Classification of Education.](http://www.unesco.org/education/information/nfsunesco/doc/isced_1997.htm) 1997. URL: http://www.unesco.org/education/information/nfsunesco/doc/isced_1997.htm

[WAI-WEBCONTENT]
: [Web Content Accessibility Guidelines 1.0.](https://www.w3.org/TR/WAI-WEBCONTENT/) Wendy Chisholm; Gregg Vanderheiden; Ian Jacobs. W3C. 5 May 1999. W3C Recommendation. URL: https://www.w3.org/TR/WAI-WEBCONTENT/
