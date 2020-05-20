---
title: 11. Język


sidebar: testy_sidebar
permalink: tz-11-jezyk
folder: testy/tz
---

## Cel procedury testowej

Celem tej procedury testowej jest sprawdzenie, czy naturalny język lub języki używane na stronie internetowej zostały poprawnie programowo określone.

Poprawne programowe określenie języka lub języków naturalnych używanych na stronie zapewnia, że technologie wspomagające, np. czytniki ekranu, będą poprawnie  interpretować i prezentować informacje.  

**Uwaga**: „Język naturalny” odnosi się do języka, którego ludzie używają do komunikowania się ze sobą, w przeciwieństwie do języków kodowania używanych do tworzenia oprogramowania i treści internetowych.

Procedura testowa „Języki” obejmuje dwa testy:

1.	Test 11.A 3.1.1-okreslono-jezyk-strony
2.	Test 11.B 3.1.2-okreslono-jezyk-części



### Język strony

#### Test 11.A 3.1.1-okreslono-jezyk-strony

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.1.1-okreslono-jezyk-strony | 11.A    | Domyślny ludzki język każdej strony można ustalić programowo. |

#### Cel testu 11.A 3.1.1-okreslono-jezyk-strony

Celem tego testu jest ustalenie, czy naturalny język użyty w tekście na stronie jest programowo określony, aby technologie wspomagające mogły odczytać treść w sposób zrozumiały dla użytkownika. 

Ten test sprawdza naturalny język używany domyślnie na stronie. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 3.1.1 Język strony.


#### Metody i narzędzia testowe 
1.	ANDI: struktury > więcej szczegółów > język strony.
2.	[Rejestr Podznaczników Języka (IANA, Internet Assigned Numbers Authority)](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry) do sprawdzania poprawności dwu- lub trzyliterowych kodów języka używanych na stronie.


#### Identyfikacja treści
Aby określić, co należy przetestować:

1.  Określ domyślny naturalny język strony (język, w którym prezentowana jest większość strony).

2.  Jeśli tekst nie jest widoczny , określ język na podstawie napisów kodowanych dla multimediów, transkrypcji tylko dla dźwięku lub tekstu alternatywnego dla obrazów.

**Uwaga**: „Język naturalny” odnosi się do języka, którego ludzie używają do komunikowania się ze sobą, w przeciwieństwie do języków kodowania używanych do tworzenia oprogramowania i treści internetowych.	

#### Zastosowanie:
Nie możesz uznać (ocenić) wyniku tego testu jako **nie ma zastosowania** (**ND**). Wszystkie strony powinny zawierać pewną treść tekstową, nawet jeśli ta treść jest dostępna tylko programowo. Jeśli tekst nie jest od razu widoczny, sprawdź język związany z napisami kodowanymi dla multimediów, transkrypcję tylko dla dźwięku lub alternatywny tekst dla obrazów.

#### Jak testować:

1.  Uruchom ANDI: struktury.

2.  2.	Kliknij łącze „więcej szczegółów”, a następnie „język strony”.

    1.  ANDI wyświetli okno dialogowe z listą wartości atrybutu `lang` przypisanego do elementu `<html>` strony.

    2.  Jeśli nie ma `lang` lub atrybut jest pusty, ANDI wyświetli w  oknie dialogowym ostrzeżenie.

3.  Zapoznaj się z [Rejestrem Podznaczników Języka (IANA, Internet Assigned Numbers Authority)](https://www.iana.org/assignments/language-subtag-registry),  aby ustalić, czy język jest poprawnie zdefiniowany i odpowiada domyślnemu  naturalnemu językowi strony.

    1. Naciśnij klawisze CTRL + F, aby otworzyć funkcję wyszukiwania w przeglądarce, i wpisz domyślny język strony.
	
	1. Przejrzyj podznacznik, aby określić kod powiązany z językiem.

#### Wyniki oceny  // Ocena treści

Jeśli **oba** twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 3.1.1:

1.  Domyślny język podstawowy jest poprawnie określony według [IANA](https://www.iana.org/assignments/language-subtag-registry), **oraz**

2.  Język określony w atrybucie `lang` pasuje do domyślnego języka naturalnego używanego na stronie.

##### Uwaga:

- Podznacznik języka podstawowego jest pierwszym dwu- lub trzyznakowym kodem w wartości atrybutu `lang`. (Nie należy testować dodatkowych specyfikacji językowych dla dialektów, które mogą występować po podznaczniku języka podstawowego).

-   Podznacznik języka podstawowego musi być zgodny z [Rejestrem Podznaczników Języka (IANA, Internet Assigned Numbers Authority.](https://www.iana.org/assignments/language-subtag-registry)


### Język części

#### Test 11.B 3.1.2-okreslono-jezyk-części

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 3.1.2-okreslono-jezyk-części | 11.B    | The human language for any content segment that differs from the default human language of the page can be programmatically determined. |

Język naturalny każdego segmentu treści, napisanego w innym niż domyślny język strony, może być określony programowo.


#### Cel testu 11.B 3.1.2-okreslono-jezyk-części

Celem tego testu jest sprawdzenie, czy technologia wspomagająca  będzie prawidłowo wymawiać słowa, fragmenty lub frazy, które zostały zapisane w innym języku niż reszta strony. Język naturalny używany w części lub częściach musi być określony programowo. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 3.1.2 Język części.


#### Metody i narzędzia testowe 
1.	ANDI: struktury > więcej szczegółów > atrybuty języka.
2.	[Rejestr Podznaczników Języka (IANA, Internet Assigned Numbers Authority)](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry) do sprawdzania poprawności dwu- lub trzyliterowych kodów języka używanych na stronie.

### Identyfikacja treści
Aby określić, co należy przetestować:

1.  Określ wszelkie treści tekstowe zapisane w innym niż domyślny naturalny język strony, w tym teksty alternatywne.

2.  Określ naturalny język treści tekstowej, który różni się od domyślnego naturalnego języka strony.

**Uwaga:**

-   Nazwy własne, , terminy techniczne, słowa o nieokreślonym języku oraz słowa lub zwroty, które stały się częścią słownika bezpośrednio sąsiadującego tekstu, nie wymagają atrybutu `lang` innego niż domyślny język strony i nie są objęte tym testem.

#### Zastosowanie:
Test 11.B 3.1.2-okreslono-jezyk-części  **nie ma zastosowania**, jeśli 

- Na stronie jest tylko jeden język.
- Segment tekstu to bełkot.
- Tekst jest nazwą własną.
- Tekst jest terminem technicznym.
- Segment tekstu jest powszechnie rozumianym słowem lub frazą.

**Wskazówki**:

- Jednym ze sposobów ustalenia, czy słowo w innym języku naturalnym jest powszechnie rozumiane, jest określenie, czy pojawi się ono w słowniku dla podstawowego języka strony.
- Określenie języka dla części powszechnie rozumianej nie jest zabronione. Jeśli jednak zostanie to zrobione, wartość języka musi być poprawna.

#### Jak testować:

1.  Uruchom ANDI: struktury; kliknij łącze „więcej szczegółów”, a następnie „[#] atrybuty języka”. Jeśli [#] wynosi zero, żadna treść nie została oznaczona atrybutem `lang`.

2.  Znajdź znacznik, który definiuje element, do którego zastosowano atrybut `lang`, oraz język zdefiniowany w wartości atrybutu `lang` (np. „en” dla języka angielskiego).

    1.  Najedź myszką lub tabulatorem, aby odsłonić początek i koniec elementu.

    2.  ustal, czy cały innojęzyczny segment znajduje się wewnątrz elementu z atrybutem `lang`.

3.  Zapoznaj się z [Rejestrem Podznaczników Języka (IANA, Internet Assigned Numbers Authority)](https://www.iana.org/assignments/language-subtag-registry),  aby ustalić, czy język jest poprawnie zdefiniowany i odpowiada domyślnemu naturalnemu językowi innojęzycznego segmentu treści.

    1. Naciśnij klawisze CTRL + F, aby otworzyć funkcję wyszukiwania w przeglądarce, i wpisz domyślny język strony.
	
	2. Przejrzyj podznacznik, aby określić kod powiązany z językiem.


#### Wyniki oceny  // Ocena treści

Jeśli **oba** twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 3.1.2:

1.  Język segmentu treści, który różni się od podstawowego domyślnego języka strony, jest poprawnie określony według [IANA](https://www.iana.org/assignments/language-subtag-registry), **oraz** 
2.	Język określony w atrybucie `lang` pasuje do domyślnego języka naturalnego użytego w innojęzycznym segmencie strony na stronie.


##### Uwaga:

- Podznacznik języka podstawowego jest pierwszym dwu- lub trzyznakowym kodem w wartości atrybutu `lang`. (Nie należy testować dodatkowych specyfikacji językowych dla dialektów, które mogą występować po podznaczniku języka podstawowego).

-   Podznacznik języka podstawowego musi być zgodny z [Rejestrem Podznaczników Języka (IANA, Internet Assigned Numbers Authority.](https://www.iana.org/assignments/language-subtag-registry)

### Zastosowane standardy
- {% include ks/3-1-1.md %}
- {% include ks/3-1-2.md %}
- [15. Język](ICT-15-jezyk)
