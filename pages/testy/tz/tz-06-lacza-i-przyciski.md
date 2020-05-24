---
title: 6. Łącza i przyciski


sidebar: testy_sidebar
permalink: tz-06-lacza-i-przyciski
folder: testy/tz
---

## Cel procedury testowej
Celem tej procedury jest sprawdzenie, czy łącza i przyciski zapewniają wystarczający tytuł do opisania celu każdego przycisku lub łącza. Zapewnienie odpowiednich tytułów łączy i przycisków pomaga użytkownikom ustalić, czy i kiedy należy aktywować łącza i przyciski. Ten zestaw testów obejmuje zmiany treści strony internetowej, które występują w wyniku interakcji z łączami i przyciskami. Gdy aktywacja łącza lub przycisku powoduje zmianę treści strony internetowej, łącze lub przycisk musi opisywać, co nastąpi, lub strona internetowa musi zapewniać inne programowe powiadomienie o zmianach. Zmiany, które są widoczne tylko wizualnie, mogą być trudne do zauważenia i zrozumienia dla użytkowników AT.

Procedura testowa „Łącza i przyciski” obejmuje dwa testy:

- Test 6A: 2.4.4-cele-łączy-przycisków

- Test 6B: 4.1.2-łącza-powiadomienia-o-zmianach


### Test 6A: 2.4.4-cele-łączy-przycisków

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.4.4-cele-łączy-przycisków | 6.A     | Cel każdego łącza lub przycisku można określić na podstawie dowolnej kombinacji tekstu łącza/przycisku, dostępnej nazwy, dostępnego opisu lub programowo określonego kontekstu łącza/przycisku. |


### Cel testu 6A: 2.4.4-cele-łączy-przycisków

Celem tego testu jest ustalenie, czy każde łącze lub przycisk na stronie posiada wystarczający opis celu łącza lub przycisku. Aby zdecydować, czy skorzystać z łącza lub aktywować przycisk, użytkownicy muszą rozumieć, jakie działanie zostanie wykonane po wybraniu łącza lub przycisku. Programiści mogą opisać cel łącza lub przycisku bezpośrednio w tekście łącza lub przycisku (tytule), kojarząc programowo z łączem lub przyciskiem inny tekst opisowy, a także podając kontekstowe wskazówki, które można określić programowo. 

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu WCAG 2.4.4 Cel łącza (w kontekście).

### Metody i narzędzia testowe 

1.	ANDI: łącza/przyciski > łącza

2.	ANDI: łącza/przyciski > przyciski


### Identyfikacja treści

1.	Użyj ANDI: łącza/przyciski, aby zidentyfikować wszystkie łącza i przyciski.

    ANDI łączy identyfikację i analizę łączy i przycisków w jednym module. Rozróżnia dwa typy elementów i konieczne jest zbadanie obu typów.
	
	**Uwaga**: Nie zawsze widać wyraźnie, które elementy to łącza lub przyciski. Łącza można stylizować tak, aby wyglądały jak przyciski i odwrotnie. Dlatego musisz wybrać każdą opcję osobno, aby zidentyfikować wszystkie łącza i przyciski.

2.	Po uruchomieniu modułu łącza/przyciski zbadaj każde „łącze” i „przycisk”.

    Wybierz przyciski „Następny/poprzedni element” w ANDI, aby przejść do każdego łącza lub przycisku. Alternatywnie możesz wybrać przycisk „pokaż listę łączy/przycisków”, aby wyświetlić pełną listę wszystkich przycisków lub łączy na stronie.


### Zastosowanie

Test 6A: 2.4.4-cele-łączy-przycisków **nie ma zastosowania**, jeśli na stronie nie ma łączy ani przycisków. Jeśli ANDI nie zidentyfikuje żadnych łączy ani przycisków, oznacz wynik testu jako **ND**.


### Jak testować

1.  Oceń Wyjście ANDI pod kątem celu łącza/przycisku.

    **Uwaga**: ANDI łączy informacje odczytane z wewnętrznego tekstu łącza lub przycisku z innymi komponentami dostępności, aby uzyskać dostępną nazwę i opis dla każdego łącza lub przycisku. Wyjście ANDI to ciąg tekstowy, który powinien zostać wygenerowany przez technologie pomocnicze, takie jak czytniki ekranu.

2.  Ustal, czy Wyjście ANDI, w połączeniu z określonym programowo kontekstem łącza/przycisku (tekst, który znajduje się w tym samym akapicie, liście lub komórce tabeli, co łącze/przycisk, czy w komórce nagłówka tabeli powiązanej z komórką tabeli zawierającą łącze/przycisk) odpowiednio opisuje cel lub funkcję łącza/przycisku.

    1.  W przypadkach, gdy cel łącza/przycisku jest celowo niejasny lub niejednoznaczny (np. treść, która zostanie ujawniona po wybraniu łącza do „Drzwi 1”, „Drzwi 2” lub „Drzwi 3” ma być niespodzianką), może być wystarczające, aby kombinacja tekstu łącza/przycisku, dostępnej nazwy, dostępnego opisu oraz kontekstu łącza/przycisku odnosiła się do celu łącza/przycisku niejasno lub niejednoznacznie.


ANDI oferuje funkcję „pokaż listę łączy/przycisków”, a także prezentuje ostrzeżenia pozwalające zidentyfikować nieunikatowe przyciski i niejednoznaczne łączą, które mają taką samą nazwę lub opis jak inne łącze czy przycisk, wskazują inny cel (atrybut `href`). Ale ponieważ KS 2.4.4 Cel łączy (w kontekście) pozwala na wykorzystanie do poinformowania o celu łącza lub przycisku kontekstu, który może być określony programowo, konieczne może być dokonanie oceny każdego łącza lub przycisku w kontekście, a nie tylko przeglądanie i ocena listy łączy czy przycisków.

Aby określić inne powiązania programowe, konieczne może być użycie jednego z pozostałych modułów ANDI. Na przykład użyj ANDI: tabele, aby ocenić, czy nagłówek wiersza lub kolumny może informować o celu łącza lub przycisku. Użyj ANDI:struktury, aby ocenić, czy pozycja łącza lub przycisku na liście może informować o celu łącza lub przycisku.



### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 2.4.4:

1.  Cel każdego łącza lub przycisku można określić na podstawie dowolnej kombinacji tekstu łącza/przycisku, dostępnej nazwy, dostępnego opisu lub programowo określonego kontekstu łącza/przycisku.


### Uwaga:

-   Łącza i przyciski mogą zmieniać się automatycznie lub w wyniku interakcji z treścią strony. Takie zmiany powinny zostać uwzględnione w tym teście. Za każdym razem, gdy zmienia się tekst łącza lub przycisku lub otaczający je kontekst, należy ponownie ocenić łącze lub przycisk, aby ustalić, czy nadal odpowiednio opisują swój cel.


### Test 6B: łącza-powiadomienia-o-zmianach

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4.1.2-łącza-powiadomienia-o-zmianach | 6.B     | Użytkownik jest powiadamiany o każdej zmianie treści, która jest wynikiem interakcji z łączem lub przyciskiem.  |


### Cel testu 6B: 4.1.2-łącza-powiadomienia-o-zmianach
Celem tego testu jest ustalenie, czy strona internetowa zapewnia wystarczające powiadomienie i opis o wszelkich zmianach treści na stronie internetowej, które nastąpiły w wyniku interakcji z łączem lub przyciskiem. Programiści mogą użyć łącza lub przycisku i innego powiązanego tekstu zidentyfikowanego w poprzednim teście, aby powiadomić o zmianach związanych z łączem/przyciskiem. Programiści mogą również stosować inne techniki w celu powiadamiania o zmianach związanych z łączami/przyciskami. 

Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu WCAG 4.1.2 Nazwa, Rola, Wartość.


### Metody i narzędzia testowe 

1.	ANDI: łącza/przyciski > łącza

2.	ANDI: łącza/przyciski > przyciski

3.	ANDI: struktury > żywe regiony.


### Identyfikacja treści

1. Użyj ANDI: łącza/przyciski, aby zidentyfikować wszystkie łącza i przyciski.

2. Zidentyfikuj wszelkie zmiany treści strony, które nastąpią w wyniku interakcji z łączami lub przyciskami. Zmiany treści mogą obejmować zmiany innych łączy i przycisków, informacji tekstowych, struktury strony, obrazów, wykresów, schematów kolorów itp.


### Zastosowanie

Test 6B: 4.1.2-łącza-powiadomienia-o-zmianach **nie ma zastosowania**, jeśli na stronie nie ma łączy ani przycisków ORAZ jeśli treść strony nie zmienia się w efekcie interakcji z łączem lub przyciskiem.

Ten test dotyczy tylko treści zmieniających się na danej stronie internetowej w wyniku wybrania łącza lub przycisku.
 
Innymi słowy, jeśli klikniesz łącze lub przycisk i:

-	kliknięcie spowoduje na stronie zmianę treści, ale adres URL pozostanie taki sam, wykonaj instrukcje testowania, aby ocenić zmiany.

-	kliknięcie **nie spowoduje** zmian treści na stronie, oznacz wynik testu jako **ND** (**nie ma zastosowania**).

-	kliknięcie otwiera nową stronę internetową, oznacz wynik testu dla testu **ND** (**nie ma zastosowania**) (to nie jest zmiana treści na samej stronie internetowej).




### Jak testować

1.  Aktywuj każde łącze lub przycisk, które wywołuje zmiany w treści strony (np. usunięcie treści, dodanie treści itp.).

2.  Określ, w jaki sposób użytkownik jest powiadamiany o zmianie treści.

    1.  Ustal, czy łącze lub przycisk, który wyzwala zmianę, ma dostępną nazwę, dostępny opis lub kontekst, który zapewnia wystarczający opis celu komponentu interfejsu.

        1.  Jeśli zmiany treści są bezpośrednim wynikiem działania użytkownika podczas interakcji z treścią ORAZ komponent interfejsu, który wyzwala zmianę, zapewnia wystarczający opis zmiany, wówczas dodatkowe powiadomienie o zdarzeniu programowym nie jest konieczne.
		
		Wiele zmian treści na stronie internetowej może wystąpić w tym samym kontekście i jako oczekiwany wynik typowej interakcji z łączami i przyciskami. Element menu, który wyświetla dodatkowe elementy podmenu, dodatkowe pola formularza, które pojawiają się na stronie, ponieważ użytkownik odpowiada na pytanie z określoną odpowiedzią, lub dodatkowa treść strony po wybraniu przycisku „rozwiń” zazwyczaj nie wymaga dodatkowego powiadomienia oprócz tekst łącza/ przycisku i powiązane atrybuty. Już ustaliłeś, czy link lub przycisk wystarczająco opisuje jego przeznaczenie (w teście 6.A). Jednak fakt, że element menu zawiera podmenu, może nie być oczywisty z samego tekstu linku. W takim przypadku, jeśli programista dodał atrybut `aria-expanded=[true/false]`, wówczas tekst łącza wraz z atrybutem `aria-expanded` wystarcza do opisania, że wybranie pozycji menu powoduje wyświetlenie dodatkowych pozycji podmenu.

    2.  Zidentyfikuj wszystkie okna dialogowe ostrzegające użytkownika o zmianach treści.

        1.  Ustal, czy okna dialogowe zapewniają wystarczające programowe powiadamianie o zmianach treści.
		
		**Uwaga**: Niektóre zmiany treści mogą nie wystąpić w bezpośredniej bliskości łącza lub przycisku lub mogą nie być możliwe do bezpośredniej identyfikacji za pomocą programowych atrybutów łącza lub przycisku. Takie zmiany treści mogą wymagać dodatkowego powiadomienia, na przykład w oknie dialogowym. Okna dialogowe mogą służyć do różnych celów, takich jak przekazywanie komunikatów ostrzegawczych, czy  udostępnianie opcji akceptowania lub anulowania zmian, które mogą wystąpić w wyniku wybrania przycisku lub łącza.

    3.  Zidentyfikuj zmiany treści, które powodują przeniesienie fokusa na treść, która uległa zmianie.

        1.  Ustal, czy przeniesienie fokusa na zmienioną treść jest wystarczające, aby powiadomić użytkownika o wystąpieniu zmiany (np. opisując zmianę bezpośrednio w treści, na którą fokus został przeniesiony).

    4.  Zidentyfikuj zmiany treści występujące w dynamiczym (żywym) regionie ARIA:

        1.  Uruchom ANDI: struktury

        2.  Kliknij łącze „żywe regiony”, a następnie użyj myszy, aby najechać wskaźnikiem myszy na dowolny zidentyfikowany „żywy region” (alternatywnie, użyj przycisków poprzedni/następney element ANDI, aby nawigować do zidentyfikowanych „żywych regionów”).

        3.  Sprawdź, czy zmieniająca się treść jest zawarta w „żywym regionie”.


### Ocena wyników

Jeśli którakolwiek z poniższych sytuacji, to **prawda**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 4.2.1:

1.  Działanie użytkownika bezpośrednio skutkuje zmianą treści, a komponent interfejsu, który wywołał zmianę, zapewnił wystarczający opis zdarzenia zmiany, **lub**

2.  Strona powiadamia użytkownika o zmianie za pośrednictwem okna dialogowego dostępnego z klawiatury **lub**

3.  Strona przenosi fokus na treść, która się zmieniła, **a** treść, która się zmieniła, zapewnia wystarczający opis zmiany, **lub**

4.  Zmieniona treść jest zawarta w „żywym regionie” ARIA.


### Obowiązujące normy

{% include ks/2-4-4.md %}

- [14. Łącza i przyciski](ICT-14-lacza-przyciski)

{% include ks/4-1-2.md %}

- [5. Treść zmienna](ICT-05-tresc-zmienna)                                                                                                                                 
