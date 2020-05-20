---
title: 10. Struktury treści


sidebar: testy_sidebar
permalink: tz-10-struktury
folder: testy/tz
---

## Cel procedury testowej

Celem tej procedury testowej jest sprawdzenie, czy  elementy wizualnej struktury treści - nagłówki i listy - są programowo możliwe do ustalenia i poprawnie zakodowane. Dzięki temu użytkownicy technologii wspomagających mogą zrozumieć strukturę strony i kolejność treści.

Procedura testowania struktury treści obejmuje cztery testy:
- 10.A:	2-4-6-adekwatne-naglowki - Cel nagłówków
- 10.B:	1-3-1-wizualne-naglowki-okreslone-programowo
- 10.C:	1-3-1-logiczna-hierarchia-naglowkow
- 10.D:	1-3-1-odpowiednie-typy-list

## Nagłówki

### Test 10.A: 2.4.6-adekwatne-naglowki

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.4.6-adekwatne-naglowki | 10.A    | Każdy nagłówek opisuje temat lub cel treści, którą tytułuje. |

#### Cel testu 2.4.6-adekwatne-naglowki (Cele nagłowków)

Celem tego testu jest sprawdzenie, czy każdy widoczny nagłówek opisuje odpowiednio temat lub cel treści, którą rozpoczyna. Opisowe nagłówki pomagają użytkownikom zrozumieć, jakie informacje są zawarte na stronach internetowych i jak te informacje są zorganizowane. Ułatwiają użytkownikom łatwe znajdowanie poszukiwanych informacji i zrozumienie relacji między różnymi częściami treści.

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu 2.4.6 Nagłówki i etykiety.

#### Identyfikacja treści

1.  Zidentyfikuj wszystkie wizualnie widoczne nagłówki, które oznaczają sekcje treści.

    1.  Nagłówki mają często większą, pogrubioną czcionkę, są oddzielone od akapitów dodatkowymi odstępami (choć nie zawsze). Zwróć uwagę na hierarchię i strukturę każdego nagłówka w odniesieniu do innych nagłówków na stronie lub ekranie.
	2. Nagłówki nie muszą być długie; słowo, a nawet pojedynczy znak, może wystarczyć, jeśli zapewnia odpowiednią wskazówkę do znajdowania treści i nawigacji.
	3. Ten test polega na inspekcji strony, nie wymaga żadnych narzędzi testowych.
	4. Ten test sprawdza, czy każdy widoczny nagłówek streszcza temat lub cel treści, którą tytułuje.

**Uwaga**: Ten test nie wymaga nagłówków. Ten test wymaga, aby widoczne nagłówki, jeśli istnieją, opisywały temat lub cel treści, którą tytułują. 


#### Zastosowanie:

Test 2.4.6-adekwatne-naglowki **nie ma zastosowania**, jeśli na stronie nie ma żadnych widocznych nagłówków. 


#### Jak testować:

1.  Porównaj tekst każdego wizualnie wyróżnionego nagłówka z treścią pod nagłówkiem.

#### Ocena treści // Wyniki oceny

Oceniasz, czy każdy widoczny nagłówek opisuje temat lub cel treści pod nagłówkiem. Twoim zadaniem nie jest stwierdzenie, czy nagłówek opisuje treść wystarczająco, jasno, zwięźle. Twoim zadaniem jest jedynie stwierdzenie, czy każdy nagłówek trafnie, zgodnie z zawartością, opisuje treść, która znajduje się pod nim. 

Jeśli poniższe stwierdzenie jest prawdziwe, treść (strona) **SPEŁNIA** wymóg testowy, jest **ZGODNA** z KS 2.4.6:

1. Każdy nagłówek opisuje temat lub cel jego treści


### Test 10.B: 1.3.1-naglowki-programowe

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-naglowki-programowe | 10.B    | Każdy nagłówek określony programowo jest nagłówkiem wizualnym, a każdy nagłówek wizualny jest określony programowo. |


#### Cel testu 
Celem tego testu jest sprawdzenie, czy każdy nagłówek wizualny jest również określony programowo, to znaczy czy został zakodowany jako nagłówek i w związku z tym może być odczytany przez program komputerowy, a każdy nagłówek określony programowo jest również wyróżniony wizualnie. Gdy nagłówki są określone programowo, technologie wspomagające rozpoznają je i mogą przekazać strukturę treści użytkownikowi. Zapewnienie struktury nagłówka nagłówków, że zależności między częściami treści są programowo możliwe do określenia i zapewnia, że informacje ważne dla zrozumienia są dostrzegalne dla wszystkich użytkowników. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu 1.3.1 Informacje  i relacje. 
 

#### Metody i narzędzia testowe 
1.	Inspekcja wzrokowa strony pod kątem wizualnej struktury nagłówków.
2.	ANDI:struktury > nagłówki

#### Identyfikacja treści

1.  Zidentyfikuj wszystkie wizualnie widoczne nagłówki, które oznaczają sekcje treści. (Jak w eście 10A).

2.  Użyj ANDI, aby zidentyfikować wszystkie nagłówki określone programowo za pomocą znaczników od `<h1>` do `<h6>` albo atrybutu ARIA `role="heading"`.

    1.  Uruchom ANDI: struktury.

    2.  Wybierz z menu przycisk „nagłówki”.

    3.  ANDI doda kropkowane kontury wokół każdego oznakowanego nagłówka, który jest widoczny na stronie.


#### Zastosowanie:

Jeśli na stronie nie ma żadnych widocznych nagłówków, ani nagłówków określonych programowo (ANDI nie rozpoznaje nagłówków programowych), test 1.3.1-naglowki-programowe **nie ma zastosowania**. 

Innymi słowy, jeśli występuje którykolwiek typ nagłówka, musisz wykonać ten test.


**Uwaga**: Ten test nie wymaga, by na stronie były nagłówki. Ten test wymaga, aby widoczne nagłówki, jeśli istnieją, opisywały temat lub cel treści, którą tytułują. 


#### Jak testować:

1.  Wybierz ANDI:struktury i przejrzyj Wyjście ANDI dla każdego widocznego nagłówka. ANDI obrysowuje wszystkie nagłówki przerywaną purpurową linią.

    1.  Jeśli ANDI nie zidentyfikuje widocznego nagłówka, oznacza to, że nagłówek nie został określony programowo.
	
	**Uwaga**: Jeśli Wyjście ANDI wyświetla inny tekst niż tekst nagłówka na stronie, wówczas nagłówek nie jest poprawnie określony programowo.

2.  Przejrzyj każdy nagłówek zidentyfikowany przez ANDI, aby ustalić, czy jest to również nagłówek widoczna wizualnie.


#### Ocena treści // Wyniki oceny

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas strona (treść) **SPEŁNIA** wymagania, jest **ZGODNA** z KS 1.3.1:

1.  Każdy programowo określony nagłówek jest również nagłówkiem wizualnym  na stronie **ORAZ**

2.  Każdy nagłówek wizualny jest określony programowo.

#### Uwaga:

Treść, która nie wygląda jak nagłówek (nie jest nagłówkiem wizualnym), nie powinna odgrywać roli nagłówka (np. znaczników nagłówków nie należy używać do wizualnego wyróżniania elementów, które nie są nagłówkami dla treści, które po nich następują). 

I odwrotnie, treść, która jest stylizowana tak, aby wyglądała jak nagłówek i pełnia rolę nagłówka, powinna być programowo określona jako nagłówek (za pomocą znacznika nagłówka, ani za pomocą atrybutu `role="heading"`).

(

**Uwagi**: Jeśli do treści odnoszą się następujące opisy, należy ją ocenić, że **NIE SPEŁNIA** wymagań kryterium sukcesu 1.3.1:

- Treść, która nie wygląda jak nagłówek (nie jest nagłówkiem wizualnym), ale pełni rolę nagłówka, **nie spełnia wymagań tego testu**.   
- Treść, która wygląda jak nagłówek, i została programowo określona jako nagłówek, ale nie pełni roli nagłówka, **nie spełnia wymagań tego testu** (znaczników nagłówków nie należy używać do wizualnego wyróżniania elementów, które nie są nagłówkami).  
- Treść, która wygląda jak nagłówek i pełni rolę nagłówka, ale nie jest programowo określona jako nagłówek ani za pomocą znacznika nagłówka, ani za pomocą atrybutu `role="heading"`, **nie spełnia wymagań tego testu** 
)


### Test 10.C: 1.3.1-poziom-naglowka

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-poziom-naglowka | 10.C    | Programowy poziom każdego nagłówka jest logicznie dopasowany do wizualnej prezentacji (stylizacji) nagłówka w strukturze nagłówków. |

#### Cel testu 10.C 1.3.1-poziom-naglowka

Celem tego testu jest sprawdzenie, czy programowy poziom każdego nagłówka odpowiada jego prezentacji wizualnej. Ułatwia to widzącym użytkownikom szybką orientację i zrozumienie relacji między różnymi częściami treści, dzięki czemu rozumieją strukturę treści. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu 1.3.1 Informacje  i relacje.

#### Metody i narzędzia testowe 
1.	Inspekcja wzrokowa strony pod kątem wizualnej struktury nagłówków.
2.	ANDI:struktury > nagłówki oraz widok Konspekt struktury 

#### Zastosowanie:

Jeśli coś wizualnie wydaje się być nagłówkiem, ale ANDI nie rozpoznaje tej treści jako nagłówka, test 1.3.1-poziom-naglowka **nie ma zastosowania**.

Jeśli na stronie nie ma żadnych widocznych nagłówków, ani nagłówków określonych programowo (ANDI nie rozpoznaje nagłówków programowych), test 1.3.1-poziom-naglowka **nie ma zastosowania**. 

Innymi słowy, ten test musisz wykonać tylko wtedy, jeśli na stronie występuje którykolwiek typ nagłówka..

#### Jak testować:

1.	Uruchom ANDI:struktury i wybierz przycisk „pokaż konspekt”, aby wyświetlić konspekt struktury strony.

2.  Najeżdżaj myszką lub tabuluj poszczególne nagłówki w konspekcie struktury ANDI, aby przejrzeć wyniki ANDI dla każdego nagłówka.

    1.  ANDI zidentyfikuje konflikty w określeniu poziomów nagłówków, jeśli zostaną znalezione. Np. „Poziom elementu nagłówka `<h1>` powoduje konflikt z `aria-level="2"`” albo „`aria-level` nie jest liczbą całkowitą większą niż zero; domyślnie zostanie zastosowany poziom 2.”, albo „Użyto `role=heading` bez `aria-level`; domyślnie zostanie zastosowany poziom 2”.
	
3.	Porównaj poziomy nagłówków wymienione w konspekcie struktury z treścią strony. Ustal, czy poziom każdego nagłówka logicznie pasuje do wizualnej prezentacji nagłówka.

    **Uwaga**: Wizualna prezentacja nagłówka odnosi się zarówno do wizualnego stylu nagłówków, dzięki czemu ważniejsze nagłówki są wyświetlane większe czcionką, odmiennym krojem, a mniej ważne nagłówki są mniejsze ORAZ kontekstowa prezentacja nagłówków jest logiczna (nagłówek tytułujący część większej sekcji wydaje się być być niższego poziomem nagłówka niż nagłówek tej większej sekcji).

    1.  Na stronach, które mają tylko jeden nagłówek, nagłówek ten może mieć dowolny poziom nagłówka, ponieważ struktura strony jest zdefiniowana tylko przez ten jeden nagłówek.

    2.  Najważniejsze nagłówki powinny mieć najwyższy poziom priorytetu. Na przykład poziom nagłówka 1 jest wyższy niż poziom nagłówka 2, który jest wyższy niż poziom nagłówka 3.

    3.  Nagłówki z jednakowym lub wyższym poziomem rozpoczynają nową sekcję; nagłówki z niższym poziomem rozpoczynają nowe podsekcje, które są częścią sekcji o wyższym poziomie.

    4.  Poziom nagłówka 1:

        -   Nie jest wymagany

        -   Może być używany więcej niż raz na stronie

        -   Nie jest wymagane, aby pasował do tytułu strony

    5.  Kolejność poziomów nagłówków nie zawsze musi być zgodna z porządkiem liczenia, a mimo to będzie prawidłowa ponieważ odnosi się do struktury wizualnej/ważności przekazywanej za pomocą widocznych nagłówków na stronie. Na przykład nagłówek `<h2>` może być zastosowany dla oznaczenia struktury nawigacyjnej poprzedzającej tytuł `<h1>` rozpoczynający główną treść na stronie. Podobnie po `<h1>` może następować `<h3>` bez `<h2>` między nimi. Dopuszczalne jest również występowanie `<h3>`, a następnie `<h5>` bez `<h4>` pomiędzy nimi.

#### Wyniki oceny // Ocena treści

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas strona (treść) **SPEŁNIA** wymagania, jest **ZGODNA** z KS 1.3.1:

1.	Każdy programowo zidentyfikowany poziom nagłówka logicznie odpowiada wizualnej strukturze nagłówka na stronie **ORAZ**

2.	Programowe określenia poziomu nagłówka, jeśli użyto znacznika H i atrybutu ARIA, są takie same (poziom nagłówka jest poprawnie określony - nie ma konfliktów w okreśłeniu poziomów nagłóków) 

?????????

3.  Każdy nagłówek wizualny jest określony programowo.


## Listy

### Test 10.D: 1.3.1-typy-list

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.1-typy-list | 10.D    | Wszystkie wizualnie widoczne listy są określone programowo zgodnie z ich typem. |


#### Cel testu 10.D: 1.3.1-typy-list

Celem tego testu jest sprawdzenie, czy wszystkie listy wyróżnione wizualnie są również określone programowo zgodnie z typem listy.

Listy, w których elementy mogą się pojawiać w dowolnej kolejności, są zwykle, ale nie zawsze, formatowane wizualnie za pomocą jakiejś formy symbolu wypunktowania (np. ● lub -). Listy, w których elementy muszą być wymienione w określonej kolejności, mają pozycje na liście opatrzone numerem porządkowym albo kolejnymi literami alfabetu.  

Niezależnie od zastosownego sposoby wyróżnienia, elementy listy muszą być ze sobą poprawnie powiązane - listy muszą być odpowiednio zakodowane, aby relacja między elementami listy mogła być przekazana użytkownikom technologii wspomagajacej, by ułatwić im nawigację i zrozumienie prezentowanych informacji. 

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu 1.3.1 Informacje i relacje.

#### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa strony pod kątem wizualnej struktury list.

2.	ANDI:struktury > listy.

#### Identyfikacja treści

Znajdź na stronie wszystkie widoczne listy.

Listy to struktury zgrupowanych elementów, które przekazują informacje i relacje (związki) między informacjami. Listy mogą występować w różych postaciach, takich jak pozioma lista pozycji menu nawigacyjnego, pionowa lista powiązanych zasobów, lista zakupów, zespołów, definicji, itp. 

**Uwaga:**

-   Programiści mogą używać elementów listy do prezentacji pogrupowanych elementów, takich jak menu i&nbsp;podmenu, usuwając z nich punktowanie lub numerację. Takie użycie elementów listy jest dopuszczalne i zgodne z warunkami testu określonymi poniżej.

-   Zwróć szczególną uwagę na listy, które wyglądają jak grupa elementów, ale nie mają przed elementami listy symbolów wypunktowania lub numeracji. 

-   Nie wszystkie listy wymagają znaczników. Na przykład lista pozycji w zdaniu, oddzielona przecinkami, nie musi być oznakowana (zakodowana) jako lista wypunktowana lub numerowana.


**Uwaga**: Ten test nie wymaga, aby grupy elementów miały strukturę list. Ten test wymaga, elementy prezentowane wizualnie jako listy były programowo określone jako listy odpowiedniego typu. 


#### Zastosowanie:

Test 1.3.1-typy-list **nie ma zastosowania**, jeśli na stronie nie widać żadnych elementów, które  wyglądają jak listy. 

#### Jak testować:

1.  Uruchom ANDI:struktury i wybierz przycisk „listy”.

2.	Przejrzyj informacje w części „Elementów list”, zwracając uwagę na liczbę znalezionych list i ich typy.


3.  W odniesieniu do każdej listy określ, czy wygląda na uporządkowaną, nieuporządkowaną czy listę opisów (asocjacji).
	
	-  **Lista uporządkowana** - lista ponumerowana sekwencyjnie, a jeśli to konieczne, także hierarchicznie (np. 1, 2, 2a, 2ai, itd.). List uporządkowanych używa się tam, gdzie ważna jest kolejność albo konieczne jest odwoływanie się do konkretnych pozycji na liście według liczby/litery.

    -   **Lista nieuporządkowana** - lista nie jest numerowana. List nieuporządkowanych używa się w przypadkach, gdy kolejność elementów nie jest istotna, ani nie ma konieczności odwoływania się do konkretnych pozycji na liście według liczby/litery.

    -   **List opisów** (asocjacji, dawniej definicji) - używa się ich do grupowania dowolnych danych w&nbsp;zestawy nazwa-wartość. Rolę grupy nazwa-wartość mogą spełniać terminy i ich definicje, elementy metadanych i ich wartości oraz dowolne inne grupy danych, na przykład autorzy i tytuły ich książek.

4.  Przeanalizuj wizualną reprezentację relacji na liście, w tym kolejność, hierarchię i zagnieżdżanie, porównując do przedstawionej powyżej definicji poszczególnych typów list wykryte przez ANDI programowe określenie typu każdej listy.

    1.  Możliwe jest podanie dowolnej liczby kombinacji list zagnieżdżonych przy użyciu list uporządkowanych, nieuporządkowanych i list definicji. ANDI identyfikuje każdą listę zagnieżdżoną osobno. Przejrzyj każdą listę za pomocą przycisku „Sprawdź następny element”, aby ustalić, czy wizualne zagnieżdżanie i relacje są zgodne z programowym zagnieżdżaniem i relacjami.
	

#### Wyniki oceny // Ocena treści

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas strona (treść) **SPEŁNIA** wymagania, jest **ZGODNA** z KS 1.3.1:

1.  Wszystkie treści, które mają wygląd listy, są określone programowo jako listy, zgodnie z typem listy.

    1.  Każda lista nieuporządkowana (z punktorami lub bez) jest oznaczona jako lista nieuporządkowana (`ul`).

    2.  Każda lista uporządkowana jest oznaczona jako lista uporządkowana (`ol`).

    3.  Każda lista terminów i ich opisów albo innych zestawów nazwa-wartość jest oznaczona jako lista opisów (`dl`) 

        **ORAZ**

2.  Wszystkie programowe relacje list, w tym zagnieżdżanie i hierarchie, są spójne z relacjami list przedstawionymi wizualnie.

**Uwaga**:

-	Nie wszystkie listy wymagają znaczników. Na przykład lista pozycji w zdaniu, oddzielona przecinkami, nie musi być oznakowana (zakodowana) jako lista wypunktowana lub numerowana.


## Standardy dostępności

{% include ks/2-4-5.md %}

{% include ks/1-3-1.md %}

[13. Struktura treści](ICT-13-struktura-tresci)


