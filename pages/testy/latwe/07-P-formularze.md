---
title: Formularze, etykiety i błędy


sidebar: testy_sidebar

permalink: 07-P-formularze
folder: testy/latwe
---

## Formularze, etykiety i błędy
**Uwaga**: Ta sekcja jest bardziej złożona niż inne. Jeśli jest zbyt skomplikowana, rozważ na razie pominięcie jej i przejście przez pozostałe testy.

Etykiety, dostęp z klawiatury, jasne instrukcje i skuteczne usuwanie błędów są ważne dla dostępności formularzy.
Pola formularzy i inne formanty formularzy mają zwykle widoczne etykiety, takie jak „Adres e-mail:” jako etykieta pola tekstowego.

![Pole z etykietą Adres e-mail](images/andi/07_P_labels-email.png)

Po prawidłowym [oznakowaniu]() tych etykiet ludzie mogą wchodzić z nimi w interakcje za pomocą klawiatury, poleceń głosowych i&nbsp;czytników ekranu. Również sama etykieta staje się klikalna, co zwiększa obszar docelowy i ułatwia wybieranie małych przycisków opcji lub pól wyboru.

### Co robić:
Znajdź wszystkie formularze na stronie. Formularz może być pojedynczym polem tekstowym, takim jak Wyszukiwanie, lub może być grupą pól tekstowych, przycisków opcji, pól wyboru, list rozwijanych i przycisków.

### Co sprawdzać:

#### Dostęp z klawiatury
-	Sprawdź, czy wszystkie kontrolki formularza są dostępne z klawiatury, wykonując testy [dostępu z klawiatury](images/andi/06_P_klawiatura.md), 
-	Sprawdź, czy możesz dostać się do wszystkich pozycji na dowolnych listach rozwijanych.

#### Etykiety
-	Sprawdź, czy do każdej kontrolki formularza jest przypisana etykieta:
 - za pomocą `label`, `for` i `id` , jak pokazano poniżej w sekcji [Sprawdzanie etykiet formularza](#/testy/07_P_formularze?id=sprawdzanie-etykiet-formularza-za-pomoc%c4%85-skryptozak%c5%82adki-form-labels). (Jest to najlepsza praktyka w większości przypadków, choć nie jest to wymóg, ponieważ etykietę kontroli formularza można powiązać na inne sposoby).
 - umieszczenie pola formularza wewnątrz znacznika `label`

-	Sprawdź, czy etykiety są prawidłowo umieszczone. W przypadku języków z kierunkiem pisma od lewej do prawej etykiety powinny zwykle być umieszczone:
 - Po lewej stronie pól tekstowych i list rozwijanych (lub bezpośrednio nad nimi). <br/> ![Pole z etykietą Adres e-mail](images/andi/07_P_labels-email.png)
 - Po prawej stronie przycisków opcji i pól wyboru. <br/> ![Etykiety w grupie pól](images/andi/07_P_labels-grupapol.png )

#### Wymagane pola i inne instrukcje
-	Sprawdź, czy wszystkie pola wymagane (obowiązkowe) są wyraźnie wskazane.
-	Sprawdź, czy wskaźnik pola wymaganego nie opiera się wyłącznie na kolorze, na przykład jeśli wymagane pola były oznaczone tylko czerwonymi etykietami, nie byłyby one dostępne dla osób, które nie widzą różnych kolorów.
-	Sprawdź, czy wskaźniki pól wymaganych (takie jak gwiazdki '\*' albo słowo „wymagane”) są zawarte w zaznaczonej etykiecie w&nbsp;przypadku pól tekstowych i list rozwijanych lub w legendzie przycisków opcji i pól wyboru, jak pokazano poniżej w sekcji [Sprawdzanie etykiet formularza](#sprawdzanie-etykiet-formularza).
-	Sprawdź, czy instrukcje wypełniania formularza znajdują się w bezpośrednim sąsiedztwie formularza, na przykład:
 - Ogólne instrukcje powinny zwykle znajdować się na górze formularza lub w sekcji, której dotyczą.
 - Instrukcje dotyczące wypełniania pól powinny się znajdować tuż obok pola, nad polem lub pod polem (powinny być również powiązane programowo z polem, aby czytnik ekranu mógł je przekazać osobom niewidomym lub słabowidzącym)
 - Wymagane formaty, takie jak daty (rok-miesiąc-dzień w formacie RRRR-MM-DD), powinny być zawarte oznakowanej etykiecie (to jest najlepsza praktyka, ale mogą być również zawarte w odpowiednio oznakowanej wskazówce, która będzie czytana przez czytnik ekranu.

#### Obsługa błędów
Obsługa niektórych prostych formularzy, takich jak pojedyncze pole wyszukiwania, może nie wiązać się z możliwością popełnienia błędu. Jeśli uważasz, że formularze na sprawdzanej stronie powinny zgłaszać komunikaty o błędach, spróbuj pozostawić wymagane pola puste lub wprowadzić nieprawidłowo sformatowane informacje (takie jak numer telefonu lub adres e-mail), a następnie prześlij formularz i:
-	Upewnij się, że formularz z niewypełnionym wymaganym polem albo polem błędnie wypełnionym nie został przesłany.
-	Sprawdź, czy zapewniono jasne i szczegółowe wskazówki, które pomogą ludziom zrozumieć i naprawić błąd. Jeśli błąd dotyczy formatu, takiego jak data, godzina lub adres, sprawdź, czy poprawny format został jasno przedstawiony.
-	Sprawdź, czy błędy można łatwo znaleźć. Ogólnie najlepiej jest, jeśli komunikaty o błędach znajdują się przed formularzem, a nie po nim.
-	Sprawdź, czy pola bez błędów są nadal wypełnione wprowadzonymi danymi. (Jest to najlepsza praktyka, choć nie jest to wymóg.) Ludzie nie powinni ponownie wprowadzać wszystkich informacji w formularzu, z wyjątkiem niektórych poufnych danych, takich jak numery kart kredytowych.


### Sprawdzanie etykiet formularza
Nie ma prostego sposobu sprawdzenia powiązania etykiet z kontrolkami formularzy. Ale istnieją dwa bardzo dobre i przy tym nietrudne w uruchomieniu i obsłudze, które pomagają sprawdzić, czy formularze posiadają etykiety poprawnie powiązane z polami. Ponieważ umieszczamy je w przeglądarkach na paskach zakładek i uruchamiamy, posługując się linkiem na pasku zakładek nazywane są skryptozakładkami, a po angielsku „bookmarkletami” albo „favletami”.
-	[Form labels](https://jimthatcher.com/favelets/) autorstwa Jima Thatchera,
-	[Forms](http://pauljadam.com/bookmarklets/index.html)  autorstwa Paula J. Adama.

„Instalacja” tych skryptów jest bardzo prosta. Wystarczy je dodać do przeglądarek jako zakładki, co można zrobić co najmniej na dwa sposoby:
-	**sposób pierwszy**: przeciągnąć link skryptozakładki na pasek zakładek w przeglądarce
-	**sposób drugi**: użyć opcji *Dodaj do zakładek*. Najłatwiej użyć tego sposobu w przeglądarce Firefox, w której wystarczy wskazać link do zakładki prawym przyciskiem myszki i wybrać opcję Dodaj odnośnik do zakładki (błędne tłumaczenie, powinno być – *Dodaj zakładkę do odnośnika*).

**Uwaga**: Pasek narzędziowy WebDeveloper posiada w zestawie opcji dotyczących formularzy opcję *Outline Form Fields Without Labels* (Obrysuj pola formularzy bez etykiet), ale jej użycie nie uwidacznia informacji niezbędnych do oceny.
#### Sprawdzanie etykiet formularza za pomocą skryptozakładki Form labels:
Aby sprawdzić dostępność etykiet za pomocą skryptozakładki Form labels:  
1.	Otwórz stronę z formularzem, który chcesz sprawdzić.
2.	Wybierz z paska lub menu zakładek zakładkę Form labels.
3.	W oknie dialogowym zostanie wyświetlony komunikat z informacją, ile znaleziono kontrolek formularzy, w ilu wśród znalezionych stwierdzono błędy oraz ile wymaga przeglądu testera.   

   ![Komunikat o liczbie elementów formularza i etykiet](images/andi/07_P_labels-komunikat.png)
   Okno dialogowe informuje o liczbie zidentyfikowanych błędów, całkowitej liczbie kontrolek formularza i liczbie kontrolek, które należy sprawdzić „ręcznie”. W kolejnych krokach musisz spojrzeć na tekst wokół etykiet. Jeśli jest to trudne, możesz pominąć kolejne kroki.
4.	Sprawdź, czy obok każdej kontrolki znajduje się etykieta wskazująca w atrybucie for na ID kontrolki. Na dwóch ilustracjach poniżej pokazano kilka poprawnych przykładów. Zobacz, że np. w pierwszym przed etykietą „Pole  1” znajduje się wyróżniony kod `<label for id="id-pole1">`, a w kodzie pola masz dokładnie ten sam identyfikator: `<input id="id-pole1">`. Identyfikatory mogą być dowolne, ale muszą do siebie pasować.

   ![Wynik testu - etykiety powiązane poprawnie](images/andi/07_P_form_labels-bez-bledu1.png)

   ![Wynik testu - etykiety powiązane poprawnie](images/andi/07_P_form_labels-bez-bledu2.png)

   - Jeśli brakuje etykiety, obok pola pojawi się tylko informacja o polu z komunikatem, jak np. w pierwszym przypadku na ilustracji poniżej:  `<No Match id="bez-etykiety" Error>`.
   - Jeśli identyfikator wskazany w FOR nie będzie taki sam, jak identyfikator kontrolki, komunikat poinformuje jak w przykładzie 2 na ilustracji poniżej:  `No ID Match` i `<input No Match id="id-zle" Error>`
   - Jeśli znacznik etykiety nie będzie mieć atrybutu FOR, komunikat poinformuje jak w trzecim przykładzie poniżej: `<label No for>` oraz `<input No Match id="brak-id" Error>`

   ![Wynik testu z błędami](images/andi/07_P_form_labels-z-bledami1.png)

**Uwaga**: Może się jednak zdarzyć, że etykieta zostanie powiązana z polem w inny sposób, niż za pomocą `FOR`, a test skryptozakładki Form Labels zgłosi błąd. Takie przypadki wymagają głębszej analizy. Dwie ilustracje poniżej pokazują różnice w interpretacji tego samego przypadku przez skryptozakładkę Forms i Forms Labels. Pole zostało w tym przypadku powiązane z etykietą dopuszczalnym i zapewniającym dostępność sposobem polegającym, na umieszczeniu pola między początkowym i końcowym znacznikiem label. Na pierwszej ilustracji widzimy, że skryptozakładka oznaczyła etykietę i pole zielonym obrysem wskazującym, że to rozwiązanie jest poprawne i dostępne.

Ale na drugiej ilustracji z testu za pomocą skryptozakładki Form labels mamy komunikat błędu.        

   ![Wynik testu według Form labels](images/andi/07_P_labels-interpret1.png)

   ![Wynik testu według Forms](images/andi/07_P_labels-interpret2.png)  

5.	Sprawdź, czy wskaźnik pola wymaganego (np. gwiazdka lub słowo „wymagane” znajduje się na etykiecie pola albo – w przypadku grupy przycisków wyboru lub opcji znajduje się w legendzie grupy pól.
    - Prawidłowo: gwiazdka  (\*) znajduje się na etykiecie.
    - Nieprawidłowo: gwiazdka  (\*) znajduje się za etykietą (przed lub za polem). Niestety, test skryptozakłdek nie sygnalizuje tego błędu:
    - Prawidłowo: tekst „wymagane” znajduje się na etykiecie.
    - Nieprawidłowo: tekst „wymagane” znajduje się za etykietą (przed lub za polem). Niestety, test skryptozakładek nie sygnalizuje tego błędu:

![Poprawne i błedne oznaczenie pól wymaganych](images/andi/07_P_form_labels-wymagane.png)  

6.	Sprawdź położenie etykiet względem kontrolek. Ogólna zasada – etykieta powinna znajdować się w bezpośrednim sąsiedztwie i przed kontrolką, z wyjątkiem pól wyboru i pól opcji – tu powinna się znajdować za każdym polem wyboru bądź opcji. Ponadto w przypadku grupy pól wyboru i pól opcji musi istnieć etykieta całej grupy (zwykle w znaczniku legend) oraz etykiety każdego pola.

Zobacz na ilustracji poniżej, że test skryptozakładki nie oznacza jako błędnych etykiet umieszczonych w nieoczekiwanych miejscach.  

![Połózenie etykiet](images/andi/07_P_labels-polozenie.png)

**Uwaga**: Niekiedy niezbędne jest podzielenie etykiety na 2 lub więcej części. Programiści mogą w takich przypadkach, z myślą o osobach korzystających z czytników ekranu, posłużyć się rozwiązaniem oferowanym przez ARIA. Atrybut labelledby umożliwia wskazanie więcej niż jednego elementu z etykietą dla jednego pola.  

![Jedno pole, ale dwie etykiety](images/andi/07_P_form_labels-wieleetykiet.png)

### Sprawdzenie formularza na stronie demo PrzediPo  

Aby poćwiczyć sprawdzanie etykiet formularzy i błędów na stronie demo PrzediPo:

#### Etykiety:
1.	Otwórz dostępną wersję strony Ankieta: https://przedipo.lepszyweb.pl/after/survey.html, na której jest kilka formularzy. Sprawdź poprawność etykiet. Zwróć uwagę na występowanie znacznika `label`, atrybutu `for` oraz zgodność atrybutów `id` ze wskazywanym w atrybucie `for`.

   ![Widok wyników testu na stronie PrzediPo](images/andi/07_P_przedipo_ok.png)

2.	Otwórz niedostępną wersję strony Ankieta: https://przedipo.lepszyweb.pl/before/survey.html i powtórz test. Najpierw pojawi się okna dialogowe z informacją, że w 13 formularzach wykryto 13 błędów. Po zamknięciu okna dialogowego zobaczysz oznaczone błędy.  

   ![Widok wyników testu na stronie PrzediPo](images/andi/07_P_przedipo_bledy.png)

#### Błędy
1.	Otwórz dostępną wersję strony Ankieta: https://przedipo.lepszyweb.pl/after/survey.html. Pozostaw pola puste i prześlij formularz. Zwróć uwagę na komunikat o błędach u góry formularza i wyróżnienie wymaganych pól. Sprawdź również [Tytuł strony](01_P_tytul-strony.md). Tytuł zawiera informację, że „Wysyłka nieudana”.

   ![Widok wyników testu na stronie PrzediPo](images/andi/07_P_przedipo_bledy-ok.png)

2.	Otwórz niedostępną wersję strony Ankieta: https://przedipo.lepszyweb.pl/before/survey.html i powtórz test. Zauważ, że błędy są wskazywane tylko przez czerwoną kolor etykiet  i nie są wyjaśnione.

   ![Widok wyników testu na stronie PrzediPo](images/andi/07_P_przedipo_bledy-na-niedostepnej.png)

### Dowiedz się więcej o formularzach

-	[Zrozumieć kryterium sukcesu 3.3.2 Etykiety lub instrukcje](https://www.w3.org/WAI/WCAG21/Understanding/labels-or-instructions.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 1.3.1 Informacje i relacje](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 3.3.1 Identyfikacja błędu](https://www.w3.org/WAI/WCAG21/Understanding/error-identification.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 3.3.3 Sugestie korekty błędów](https://www.w3.org/WAI/WCAG21/Understanding/error-suggestion.html)(poziom A); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 3.3.4 Zapobieganie błędom&hellip;](https://www.w3.org/WAI/WCAG21/Understanding/error-prevention-legal-financial-data.html)(poziom AA); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.


--------------------
[&lt; Dostęp do klawiatury i widoczny fokus](06-P-klawiatura) | [Łatwe testy - spis treści](00-P-spis-tresci) | [Treść ruchoma, migająca lub błyskająca >](08-P-poruszanie-i-blyski)