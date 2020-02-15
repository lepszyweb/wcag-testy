---
title: Skuteczność testowani dostępności lub dlaczego testy użyteczności powinny być ostatnie
summary: "Te testy może przeprowadzić każdy, bez żadnej wiedzy na temat dostępności i wiedzy na temat projektowania stron."
sidebar: testy_sidebar
permalink: met-skutecznosc-testowania
folder: metoda
toc: true
datatable: true
---


**Źródło**: [Karl Groves: Efficiency in Accessibility Testing or, Why Usability Testing Should be Last](http://www.karlgroves.com/2012/04/27/efficiency-in-accessibility-testing-or-why-usability-testing-should-be-last/) opublikowane 27 kwietnia 2012  

Testowanie dostępności to testowanie systemu w celu ustalenia, jak system będzie działał, w przypadku dostępu osób z niepełnosprawnościami. Testowanie wszystkich produktów i usług ICT jest ważne dla określenia, jakie problemy istnieją i jakie ryzyko stwarzają jakiekolwiek problemy związane z dostępnością dla organizacji. Z mojego doświadczenia wynika, że [większość prób testowych podejmowanych jest po fakcie](http://www.karlgroves.com/2011/06/12/prioritizing-remediation/).  W związku z tym ważne jest, aby wysiłek włożony w testowanie był skuteczny w znajdowaniu jak najdokładniejszych danych w najszybszy sposób – innymi słowy, tanio i szybko. Może to oznaczać, że zespół programistów również szybko naprawi błędy.

Wielu zwolenników dostępności argumentuje, że skoro dostępność tak naprawdę dotyczy wyłącznie użytkownika, najlepszym sposobem sprawdzenia, czy system jest dostępny, jest przetestowanie go z prawdziwymi ludźmi. Jest to oczywiste, ale moim zdaniem nie oznacza, że testowanie użyteczności jest jedynym (lub nawet preferowanym) sposobem testowania dostępności.  W rzeczywistości jestem zdania, że testowanie użyteczności powinno być ostatnim rodzajem testowania przeprowadzanego na systemie. Wynika to z czasu i kosztów testowania użyteczności oraz z faktu, że tańsze i szybsze metody mogą być stosowane przed testowaniem użyteczności, co może sprawić, że ewentualny test użyteczności stanie się jeszcze bardziej wartościowy. Przyjrzyjmy się różnym metodom testowania i omówimy każdą.

## Automatyczne testy dostępności

Automatyczne testowanie dostępności polega na użyciu aplikacji komputerowej lub internetowej albo usługi internetowej, wtyczki do przeglądarki lub wtyczki IDE, która może uzyskać dostęp do źródła testowanej strony internetowej. Źródło jest następnie oceniane na podstawie wbudowanych przez producenta narzędzia testów heurystycznych  w celu ustalenia, czy istnieją jakieś błędy.

**Co mogę znaleźć**? Zautomatyzowane testowanie umożliwia ostateczne przetestowanie około 25% najlepszych praktyk dotyczących dostępności. Kolejne około 35% może być sprawdzone przez testowanie maszynowe, ale wyniki wymagają weryfikacji przez człowieka. Wiele z automatycznie Wiele z automatycznie wykrywanych problemów ma duży wpływ na dostępność
**Czego będzie mi brakowało**? W przybliżeniu 40% najlepszych praktyk dotyczących dostępności nie można w ogóle przetestować za pomocą narzędzia do automatycznego testowania, ponieważ są one albo zbyt subiektywne, albo zbyt skomplikowane, aby testować je automatycznie.
**Ile to kosztuje**? Tyle, ile narzędzie i czas testera na jego użycie i wykrycie problemów oraz ich segregację.

Mimo że duża liczba najlepszych praktyk w zakresie dostępności nie może być automatycznie przetestowana, **faktem jest, że w ujęciu ilościowym można automatycznie znaleźć dużą liczbę błędów dostępności**. 

Z moich danych wynika, że średnio na witrynach organizacji rozpoczynającej pracę nad dostępnością występuje około 40 błędów na stronie, które można wykryć za pomocą testów automatycznych. Jeśli narzędzie, którego używasz, ma możliwość mapowania strony i przekazywania znalezisk za pomocą odniesień do kodu, automatyczne testowanie będzie zdecydowanie najbardziej wydajnym sposobem gromadzenia danych dotyczących dostępności.

## Ręczne testy dostępności

Ręczne techniki testowania dostępności mogą się znacznie różnić. Ręczne testy dostępności mogą obejmować inspekcję kodu, manipulowanie sprzętem, zmiany ustawień oprogramowania lub użycie technologii wspomagających w celu sprawdzenia najlepszych praktyk dotyczących dostępności.

**Co mogę znaleźć**? Zwykle wszystko. Jeśli tylko masz wystarczające umiejętności i wystarczająco dużo czasu.

**Czego będzie mi brakowało**? Tego, czego nie potrafisz znaleźć lub nie masz czasu znaleźć.

Ile to kosztuje? Wynagrodzenie pracownika wraz ze wszystkimi obciążeniami albo wynagrodzenie konsultanta przeprowadzającego testy  według stawki rozliczeniowej.

Testowanie ręczne ma tę zaletę, że jest wysoce dokładne, pod warunkiem że osoba przeprowadzająca testy jest wystarczająco wykwalifikowana. [Zarówno skuteczność, jak i rzetelność sędziów ekspertów są znacznie wyższe niż sędziów niebędących ekspertami](http://dl.acm.org/citation.cfm?doid=1639642.1639678), co może oznaczać znaczne różnice w jakości wyników takich testów. Ponadto, testowanie ręczne może być bardzo czasochłonne. W zależności od funkcji strony oraz złożoności i dokładności testów, testowanie ręczne może zająć od 1 do 3 godzin na stronę. Wynika z tego, że przetestowanie każdej strony na dużej witrynie tylko przy użyciu testów ręcznych raczej nie będzie możliwe. Takie postępowanie byłoby zbyt kosztowne i czasochłonne. Nie ma również większego sensu wykorzystywanie ludzi do testowania rzeczy, które mogą zostać wykryte przez zautomatyzowane narzędzie. Właśnie dlatego zalecam [najpierw przeprowadzanie testów automatycznych](http://www.karlgroves.com/2012/02/02/web-accessibility-testing-do-automatic-testing-first/).


## Testy przypadków użycia
W inżynierii oprogramowaniu i systemów [przypadek użycia](http://en.wikipedia.org/wiki/Use_case) to lista kroków, określająca zazwyczaj interakcje między rolą a systemem, aby osiągnąć cel. Testowanie przypadków użycia polega zatem na sprawdzeniu, jak system reaguje na te interakcje. W przypadku testowania przypadków użycia pod kątem dostępności, praktyką jest wykonanie przypadku testowego przy użyciu technologii wspomagających aby określić, jak działa system, gdy jest używany przez osobę korzystającą z tej technologii wspomagającej.

**Co mogę znaleźć**? Zazwyczaj to, co można znaleźć, to ścisła reprezentacja rzeczywistego poziomu dostępności systemu i, co najważniejsze, tego, jak poważne są wszelkie błędy dostępności.

**Czego bym brakowało**? Często pomijane są konkretne wady w kodzie, które powodują niepowodzenie testu.

**Ile to kosztuje**? Wynagrodzenia pracownika wraz ze wszystkimi obciążeniami albo wynagrodzenie konsultanta według stawki rozliczeniowej. Będzie to również koszt uzyskania niezbędnych licencji na technologie wspomagające, które są testowane.

Uwielbiam testowanie przypadków użycia. Podstawowym problemem z testowaniem przypadków jest to, że jakość wyników może się dość znacząco różnić. Podobnie jak w przypadku testów ręcznych, rzeczywista wartość tego rodzaju testów zależy w dużej mierze od umiejętności osób wykonujących testy. Należy również zauważyć, że testowanie przypadków użycia nie jest testowaniem użyteczności. Ponieważ testowane przypadki są scenariuszowane, a testery mogą być dokładnie zaznajomieni z systemem (i prawdopodobnie z technologiami pomocniczymi, z którymi się testują), dobre wyniki testów przypadków użycia nie będą korelować z dobrymi wynikami testów użyteczności. Wreszcie sukces z jednym konkretnym typem, marką i wersją technologii wspomagającej niekoniecznie będzie korelował z powodzeniem we wszystkich technologiach wspomagających. Jest to jednak bardzo cenny rodzaj testowania, zwłaszcza gdy wykonuje go wykwalifikowany tester.

## Testowanie użyteczności
[Testy użyteczności](http://en.wikipedia.org/wiki/Usability_testing) to technika stosowana w projektowaniu interakcji zorientowanym na użytkownika w celu oceny produktu poprzez przetestowanie go na użytkownikach. Tradycyjnie wykonywane testy są metodą analizy poznawczej ([Cognitive walkthrough](http://en.wikipedia.org/wiki/Usability_testing)) z wykorzystaniem  [protokołu głośnego myślenia](http://en.wikipedia.org/wiki/Think_aloud_protocol), chociaż istnieją również inne metody. W przypadku testów użyteczności pod kątem dostępności testy polegają na wykorzystaniu osób z niepełnosprawnościami jako uczestników testu.

**Co mogę znaleźć**? Dowiesz się dokładnie, jak łatwe (lub trudne) jest korzystanie z systemu dla prawdziwych użytkowników z niepełnosprawnościami. Podobnie jak przy testowaniu przypadków użycia, można znaleźć konkretne interakcje, które są problematyczne a nawet niemożliwe do zrealizowania.

**Czego bym brakowało**? Podobnie jak w przypadku testów użycia, często brakuje określonych błędów w kodzie powodującym problemy.

**Ile to kosztuje**? Wynagrodzenia pracownika wraz ze wszystkimi obciążeniami albo wynagrodzenie konsultanta według stawki rozliczeniowej.  Także koszt wynajmu / wyposażenia laboratoriów lub zakupu sprzętu oraz wszelkie niezbędne koszty transportu i honorarium dla uczestników.

Testy użyteczności zapewniają jeden kluczowy punkt danych, którego nie może zapewnić żaden inny typ testowania: mówią nam, jak poważne są nasze problemy. Chociaż prawdą jest, że wysoko wykwalifikowany recenzent lub tester przypadków użycia może dać pogląd na to, jak poważny jest problem (i często mają rację), nie ma nic tak dokładnego jak prawdziwi użytkownicy mający realne problemy. Niestety, przeprowadzanie testów użyteczności (w zakresie dostępności) zbyt wcześnie może być marnowaniem czasu i pieniędzy, jeśli testy użyteczności są utrudnione przez oczywiste błędy dostępności.

## Jak i kiedy wykonać poszczególne rodzaje testów 

Uważam, że wszelkie testy dostępności, niezależnie od metodologii, muszą być ukierunkowane na jeden główny cel: zebranie danych niezbędnych do zrozumienia, co należy naprawić, aby ulepszyć system. Końcowy wynik każdego testu musi być czymś więcej niż tylko mglistym raportem stwierdzającym, że coś jest zepsute. Aby naprawdę zapewnić wartość, musisz dostarczyć kadrze zarządzającej i programistom jasno nakreśloną listę niezbędnych ulepszeń, aby programiści systemu mogli pobrać informacje z raportu i naprawić system. Im bardziej nasze wyniki testu odbiegają od tego celu, jakim jest jasno określona lista problemów, tym mniejsza jest wartość dostarczana przez twoje testy. Jest to podstawowa zasada działania SQA. Raport [dla każdego problemu](http://blogs.msdn.com/b/productfeedback/archive/2004/09/27/235003.aspx) musi być dokładny, opisowy i pomocny. Elementy, które są niejasne i nie są (oczywiście) możliwe do wykonania, mogą zostać zignorowane lub, co najmniej, potrzeba więcej czasu, aby je zweryfikować i naprawić.

Nie tylko musimy być w stanie wygenerować bardzo szczegółową listę problemów, ale jestem zdania, że powinniśmy być w stanie zrobić to jak najszybciej. Naszym szefom (lub klientom) najbardziej zależy na tym, aby praca była wykonana prawidłowo, szybko i tanio. Musisz zebrać dane niezbędne do bardzo dokładnego określenia, co należy naprawić, i musisz to zrobić przy możliwie całkiem znacznych ograniczeniach czasu i pieniędzy. Każda metoda ma swoje mocne i słabe strony.  Każda z nich ma czas, kiedy są odpowiednia i czas, w którym nie jest odpowiednia.

## Porównanie czterech różnych typów testów

{% include note.html content="Powyższe stwierdzenia dotyczące jakości, czasu i kosztów opierają się na jakości, czasie i koszcie każdego wydania." %}

<div class="datatable-begin"></div>
| Rodzaj testu	| Raport o jakości problemów | Czas | Koszt | Reprezentuje użytkowników
| ---------- | ------------------- | -------- | ------ | ------- |
| Testy automatyczne | Najwyższa objętość;<br />duża szczegółowość | Najszybszy | Najtańsze | Najniższe |
| Testowanie ręczne | Duża objętość<br />najwyższa szczegółowość | Powolny | Umiarkowany | Umiarkowany |
| Testy przypadków użycia | Niska objętość<br />niska szczegółowość | Umiarkowany | Umiarkowany | Wysoki |
| Testowanie użyteczności | Najniższa objętość<br />najniższa szczegółowość | Najwolniejszy | Najwyższy | Najwyższy |
<div class="datatable-end"></div>

Powyżej oceniłem wszystkie typy testów na podstawie kilku czynników, które należy rozważyć przy wyborze rodzaju testu (i kiedy):

**Raport o jakości problemów**: czy raport będzie zawierał pełną listę konkretnych  problemów (wolumen) i czy poszczególne zgłoszone problemy będą zawierać wystarczającą ilość informacji (szczegółów), aby zweryfikować i naprawić problem?
**Czas**: ile czasu zajmie znalezienie problemu lub ukończenie testów?
**Koszt**: ile kosztuje znalezienie problemu (-ów) i ukończenie testów?
**Reprezentuje użytkowników**: czy ten typ testów reprezentuje doświadczenie prawdziwych użytkowników systemu?

Powyższe informacje nie są pozbawione zastrzeżeń i poczyniłem pewne założenia:
Jakość i cechy zautomatyzowanych narzędzi testujących mogą się znacznie różnić.
Przydatność zautomatyzowanego narzędzia zależy w dużej mierze od jego prawidłowej konfiguracji.

Poziom umiejętności osoby (osób) wykonującej testy ręczne i testy przypadków użycia ma zasadnicze znaczenie dla zapewnienia wysokiej jakości wyników.

Istnieje szereg technik oceny użyteczności. Mówię głównie o testach laboratoryjnych, w których uczestnicy wykonują analizę poznawczą za pomocą protokołu głośnego myślenia. Więcej na ten temat poniżej.

Ze względu na wszystko, co powiedziałem powyżej, zwykle polegam na każdej metodzie w kolejności, w której je wymieniłem: automatyczne, ręczne, przypadków użycia, użyteczności. Mocno wierzę, że [najpierw](http://www.karlgroves.com/2012/02/02/web-accessibility-testing-do-automatic-testing-first/) powinniśmy [przeprowadzić testy automatyczne](http://www.karlgroves.com/2012/02/02/web-accessibility-testing-do-automatic-testing-first/). W rzeczywistości nie sądzę, że powinniśmy przeprowadzać jakiekolwiek inne testy systemu, jeśli nie sprawdzono go automatycznie. Nigdy nie powinniśmy płacić ludziom za informację, że brakuje nam tekstu i etykiet formularza. Takie rzeczy można przetestować maszynowo, a automatyczne testowanie jest tanie, szybkie i skuteczne w znajdowaniu bardzo konkretnych elementów wymagających naprawy. Jest to jednak dalekie od ideału i często można pominąć niektóre bardzo ważne kwestie. Nie można po prostu poprzestać na testach automatycznych. 

W tym momencie pojawia się ręczne testowanie. Wykwalifikowany recenzent, wykorzystujący dobrze zdefiniowaną i ustrukturyzowaną metodologię, może wypełnić większość luk nieodkrytych przez automatyczne testowanie. Wysoce wykwalifikowany recenzent może również określić wskaźniki niezbędne [do ustalenia priorytetów w usuwaniu stwierdzonych problemów](http://www.karlgroves.com/2011/06/12/prioritizing-remediation/). 

A kiedy już zautomatyzowane testy i testy ręczne zostaną wykonane, co wtedy?

W tym miejscu wkracza testowanie przypadków użycia i / lub testowanie użyteczności. Takie testy, moim zdaniem, są idealnym sposobem na uzupełnienie zautomatyzowanych i ręcznych testów dostępności.

## Dlaczego testy użyteczności powinny być ostatnie

Tradycyjne testowanie użyteczności typu, który opisałem wcześniej, jest z mojego doświadczenia najbardziej czasochłonnym i kosztownym sposobem gromadzenia danych o dostępności:

- Musisz mieć niezbędny sprzęt laboratoryjny i miejsce do testowania
- Musisz rekrutować odpowiednich uczestników. Jest to łatwe do zrobienia dla pojedynczego testu, ale znacznie trudniejsze, jeśli robisz to często, co może wymagać zatrudniania rekrutera.
- Musisz zapłacić uczestnikom.  Typowe honoraria to $50-$100 na uczestnika, a testy często mają od 8 do 12 uczestników.
- Musisz posiadać system testowy, który będzie odzwierciedlał systemy testowe uczestników. Czy używają JAWS, Window-Eyes, ZoomText lub MAGic? Jaka wersja? Jaki system operacyjny? Jaka przeglądarka? Itp.

Jak doprowadzić uczestników do miejsca testu – zwłaszcza jeśli nie mogą jeździć, a nie mieszkasz w dużym obszarze metropolitalnym? Być może będziesz musiał pojechać do nich, co wymagałoby przenośnego laboratorium.

Pewnego razu, gdy wspomniałem o powyższym, ktoś złośliwie skomentował, że to wszystko wyglądało jak [Reductio ad absurdum](https://pl.wikipedia.org/wiki/Dow%C3%B3d_nie_wprost). W większości mają rację, przyznaję. Istnieje wiele sposobów na [tanie testowanie użyteczności](https://www.google.com/search?q=cheap+usability+testing). Jakob Nielsen mówił o [Guerilli HCI](http://www.useit.com/papers/guerrilla_hci.html) w 2004 roku. Nie musisz mieć laboratorium ani sprzętu. Nie musisz sprowadzać uczestnika, ani iść do niego, możesz to zrobić za pośrednictwem konferencji internetowych, takich jak GoToMeeting lub WebEx. Ale jeśli zamierzasz przeprowadzić testy użyteczności na dużą skalę (co oznacza wiele razy w roku), musisz za każdym razem dowiedzieć się, jak rekrutować nowych uczestników, musisz zapłacić uczestnikom, musisz zaprojektować swoje testy, przeprowadzać sesje testowe oraz zestawiać i analizować dane z notatek. Wszystko to wymaga czasu i pieniędzy – często sporo czasu i pieniędzy, jeśli są wykonywane często.

Zrozumienie, jak testować, kiedy testować i co sprawdzać pod kątem dostępności, wydaje mi się, że często umyka nawet osobom, które były zaangażowane w dostępność Internetu. Dzieje się tak, ponieważ ich celem jest (i słusznie) użytkownik, a zatem testowanie z prawdziwymi użytkownikami wydaje się logicznym najlepszym wyborem do sprawdzania dostępności. Twierdzę jednak, że w porównaniu z innymi rodzajami testów dostępności, testy użyteczności są nieefektywnym sposobem osiągnięcia naszego celu końcowego. Naszym celem końcowym nie są wyniki testu, ale raczej dostępny system. Ze względu na znaczenie dostępności powinniśmy dążyć do dokładnego i skutecznego znalezienia danych. Tylko z tego powodu testy użyteczności powinny być wykonywane później w całym cyklu życia – po automatycznym, ręcznym, a nawet testowaniu przypadków użycia.


{% include links.html %}
