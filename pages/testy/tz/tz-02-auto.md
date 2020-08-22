---
title: 2. Automatyczne odtwarzanie i aktualizacja treści


sidebar: testy_sidebar
permalink: tz-02-auto
folder: testy/tz
---

## Cel procedury testowej
Celem tej procedury testowej jest sprawdzenie, czy użytkownicy mogą kontrolować treści odtwarzane automatycznie, ruchome, przewijane, aktualizowane dynamicznie oraz czy strona zapewnia powiadamianie o każdej automatycznej zmianie treści.

Kontrola nad automatycznym odtwarzaniem, nad treściami ruchomymi oraz zmieniającymi się dynamicznie jest ważna szczególnie dla użytkowników, którzy mają problemy ze skupieniem uwagi. Dzięki temu mogą uzyskać dostęp do całej treści bez rozpraszania treścią przerywającą korzystanie ze strony.

Procedura testowa „Automatyczne odtwarzanie i aktualizacja treści” obejmuje cztery testy:
1.	Test 2.A 1.4.2-sterowanie-dzwiekiem
2.	Test 2.B 2.2.2-tresci-ruchome
3.	Test 2.C 2.2.2-automatyczna-aktualizacja
4.	Test 2.D 4.1.2-powiadamianie-o-automatycznej-zmianie


## Sterowanie dźwiękiem

### Test 2.A 1.4.2-sterowanie-dzwiekiem

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.2-sterowanie-dzwiekiem | 2.A | Użytkownik może wstrzymywać, zatrzymywać lub kontrolować głośność odtwarzanej automatycznie treści audio. |

### Cel testu

Celem tego testu jest sprawdzenie, czy w przypadku, gdy na stronie automatycznie odtwarzana jest treść audio przez ponad 3 sekundy, istnieje w pierwszych trzech napotkanych interaktywnych elementach strony mechanizm umożliwiający użytkownikowi wstrzymanie lub zatrzymanie dźwięku albo kontrolę głośności dźwięku.
 
Jeśli taki mechanizm istnieje, musi również spełniać wszystkie pozostałe wymagania testowe w ramach tej procedury testowej. Dzięki temu użytkownicy korzystający z czytników ekranu nie będą doświadczać nieoczekiwanych przerw w odtwarzaniu mowy, a użytkownicy, którzy mogą być rozproszeni treściami audio podczas próby skupienia się na treści strony, będą mogli wchodzić w interakcję ze stroną internetową bez zakłóceń. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1.4.2 Kontrola odtwarzania dźwięku](https://wcag.lepszyweb.pl/#audio-control).

### Metody i narzędzia testowe 
1.	Inspekcja ręczna.
2.	Wszystkie odpowiednie moduły ANDI dla mechanizmu używanego do sterowania treścią audio.

### Identyfikacja treści
Każda treść dźwiękowa, ktora jest odtwarzana automatycznie (bez aktywacji przez użytkownika) przez ponad 3 sekundy. 

Mogą to być treści typu alerty, muzyka, odgłosy przyrody,  

**Wskazówka**: Zanim określisz, czy istnieje treść audio odtwarzana automatycznie, sprawdź, czy w przeglądarce zostało wyłączone autoodtwarzanie.

**Uwaga**: Przeglądarka powinna być już skonfigurowana tak, aby wyłączyć autoodtwarzanie. (Instrukcje znajdują się w Podręczniku instalacji i konfiguracji narzędzi testowych).

### Zastosowanie

Test 2.A 1.4.2-sterowanie-dzwiekiem **nie ma zastosowania**, jeśli nie ma treści audio odtwarzanej automatycznie przez ponad 3 sekundy. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.	Ustal, czy w *pierwszych trzech napotkanych elementach* znajduje się mechanizm umożliwiający użytkownikowi wstrzymanie lub zatrzymanie dźwięku lub kontrolę głośności dźwięku odtwarzanego automatycznie (tylko).

   Chodzi o to, aby użytkownicy mogli szybko znaleźć mechanizm i wyłączyć automatycznie odtwarzane treści audio. Oto niektóre przykłady mechanizmu kontrolnego:
   - Tekst w lewym górnym rogu strony wyjaśniający, jak używać klawiszy skrótów aktywujących mechanizm.
   - Przycisk pauzy/zatrzymania/kontroli głośności to drugi element na stronie po nagłówku.
   - Łącze do odtwarzacza audio w prawym górnym rogu strony internetowej, które jest jednym z trzech pierwszych napotkanych na stronie elementów.
   - Okno dialogowe instruujące użytkownika, że może użyć kombinacji klawiszy skrótu, aby aktywować mechanizm u dołu strony.
   - Funkcje ułatwienia dostępu do platformy (np. przeglądarki). Niektóre przeglądarki umożliwiają wyłączanie automatycznego odtwarzania multimediów i / lub wyciszanie określonych kart lub okien.
   
   Prostym sposobem ustalenia, czy mechanizm mieści się w pierwszych trzech elementach, jest użycie klawisza Tab do poruszania się po stronie od lewej do prawej, od góry do dołu.

2.  Aktywuj mechanizm. Sprawdź, czy mechanizm skutecznie wstrzymuje, zatrzymuje odtwarzanie dźwięku lub kontroluje głośność.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich pozostałych wymagań testowych w tym procesie.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.4.2:

1.  Istnieje mechanizm, który może wstrzymywać lub zatrzymywać dźwięk lub kontrolować głośność dźwięku odtwarzanego automatycznie (bez wpływu na dźwięki systemu operacyjnego) **oraz**

2.  Mechanizm należy do *pierwszych trzech elementów* napotkanych przez użytkownika, **oraz**

3.  Mechanizm spełnia wszystkie pozostałe obowiązujące warunki testu w tym procesie testowym.


### Uwaga
- Możliwość wyłączenia automatycznego odtwarzania mediów lub wyciszenia określonej karty w przeglądarce to akceptowalny mechanizm zatrzymywania lub kontrolowania głośności automatycznie odtwarzanej treści audio. Niestety, nie wszystkie przeglądarki mają możliwość wyłączenia automatycznego odtwarzania multimediów lub wyciszenia określonych okien lub kart. Jeśli testerzy polegają na funkcjonalności przeglądarki w celu zatrzymania lub kontrolowania głośności automatycznego odtwarzania treści audio, powinni udokumentować wyniki testów dla wszystkich przeglądarek, które mogą być użyte do uzyskania dostępu do treści w środowisku produkcyjnym.

- Mechanizm kontroli głośności dźwięku musi być niezależny od sterowania poziomem głośności systemu operacyjnego, aby nie wpływać na głośność mowy czytnika ekranu. 



## Treść mrugająca, przesuwana i przewijana

### Test 2.B 2.2.2-tresci-ruchome

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.2.2-tresci-ruchome | 2.B     | Użytkownik może wstrzymywać, zatrzymywać lub ukrywać treść, która  miga, przesuwa się lub przewija przez ponad 5 sekund |

### Cel testu

Celem tego testu jest sprawdzenie, czy w przypadku, gdy na stronie znajduje się treść, która automatycznie miga, przesuwa się lub przewija przez ponad 5 sekund, istnieje w pierwszych trzech napotkanych interaktywnych elementach strony mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie tej treści.

Ruchoma treść może rozpraszać niektórych użytkowników i utrudniać im interakcję z innymi sekcjami treści strony. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie](https://wcag.lepszyweb.pl/#pause-stop-hide).

### Metody i narzędzia testowe 
1.	Inspekcja ręczna.
2.	Wszystkie odpowiednie moduły ANDI w zależności od rodzaju mechanizmu używanego do kontrolowania ruchomych, migających lub przewijanych treści.

### Identyfikacja treści
Każda treść na stronie, która:

- porusza się, przesuwa lub mruga automatycznie (bez aktywacji użytkownika) **oraz**
- jeśli trwa ruch trwa dłużej niż 5 sekund, **oraz** 
- nie jest to jedyna treść na stronie

Treści tego typu obejmują przewijanie tekstu, filmów i multimediów.

**Z wyjątkiem**  treści, w której ruch, miganie lub przewijanie jest niezbędne. Niezbędną jest treść lub sposób prezentacji, których usunięcie, spowodowałoby zasadniczą zmianę informacji lub funkcjonalności, a informacji i funkcjonalności nie można osiągnąć w inny sposób spełniający wymogi zgodności.

### Zastosowanie

Test 2.B 2.2.2-tresci-ruchome **nie ma zastosowania**, jeśli na stronie nie ma treści ruchomej, migającej lub przewijanej treści, która jest odtwarzana automatycznie przez ponad 5 sekund **albo**
jeśli poruszająca się, migająca lub przewijana treść jest jedyną treścią na stronie internetowej


### Jak testować

1.  Ustal, czy istnieje wyraźny mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie treści w *pierwszych trzech elementach*, które użytkownik napotka **lub** w obrębie trzech elementów przed i po treści ruchomej, migającej lub przewijanej.

   Ponieważ chodzi o to, aby użytkownicy mogli szybko wyłączyć ruch lub miganie treści, mechanizm ten musi być widoczny w pierwszych trzech elementach, które użytkownik napotka u góry strony lub w obrębie trzech elementów przed i po treści ruchomej, migającej lub przewijanej. Przykładami takich mechanizmów są: instrukcje tekstowe, łącze, przycisk, okno dialogowe z instrukcją.
   
2.  Aktywuj mechanizm. Sprawdź, czy mechanizm skutecznie wstrzymuje, zatrzymuje lub ukrywa ruchomą treść.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich pozostałych wymagań testowych w tym procesie.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.2.2:

1.	Istnieje mechanizm, który może wstrzymywać, zatrzymywać lub ukrywać ruchomą treść **oraz**
2.	Mechanizm znajduje się w:
-   *trzech pierwszych elementach* napotykanych przez użytkownika **lub**
-   trzech elementach znajdujących się przed albo po treści ruchomej, migającej przewijanej.

**oraz**

3.  Mechanizm spełnia wszystkie pozostałe obowiązujące warunki testu w tym procesie testowym.

## Automatyczna aktualizacja

### Test 2.C 2.2.2-automatyczna-aktualizacja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.2.2-automatyczna-aktualizacja | 2.C     | Użytkownik może wstrzymywać, zatrzymywać, ukrywać lub kontrolować częstotliwość automatycznego aktualizowania treści. | 

### Cel  testu 

Celem tego testu jest sprawdzenie, czy w przypadku, gdy treść aktualizuje się automatycznie i nie jest jedyną treścią na stronie, istnieje w pierwszych trzech napotkanych interaktywnych elementach strony albo w obrębie trzech elementów przed lub po automatycznie aktualizującej się treści mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie aktualizującej się treści lub mechanizm kontrolowania częstotliwości aktualizacji. 

Treść, która aktualizuje się automatycznie, może stanowić barierę dla każdego, kto ma problemy z szybkim czytaniem, a także dla osób, które mają problemy ze śledzeniem ruchomych obiektów i osób, które się łatwo rozpraszają  


Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie](https://wcag.lepszyweb.pl/#pause-stop-hide).

### Metody i narzędzia testowe 
1.	Inspekcja ręczna.
2.	Wszystkie odpowiednie moduły ANDI w zależności od rodzaju mechanizmu używanego do kontrolowania   automatycznej aktualizacji treści.

### Identyfikacja treści

Wszelkie treści, które:

-   aktualizują się automatycznie (bez aktywacji przez użytkownika) **oraz**

-   nie są jedyną treścią na stronie

Treść tego typu obejmuje zegary, notowania giełdowe i liczniki.


**Uwaga**:

- Kryterium sukcesu WCAG 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie nie dotyczy automatycznej aktualizacji treści, których automatyczna aktualizacja jest niezbędna. Jednak automatyczna aktualizacja paska notowań giełdowych, który przekazuje informacje w czasie rzeczywistym, nie byłaby uważana za niezbędną (według WCAG), więc zostałaby uwzględniona w tym teście. 

Jest bardzo prawdopodobne, że większość przypadków automatycznej aktualizacji treści nie jest niezbędna.

Aby uniknąć nieprawidłowego pominięcia treści w tym teście, zadaniem tester nie jest ustalenie, czy automatyczna aktualizacja jest niezbędna. Powinien więc objąć testem wszystkie treści, które odpowiadają opisowi w sekcji „Identyfikacja treści”. 

W odniesieniu do istotnej treści podlegającej automatycznej aktualizacji  może być zastosowany wyjątek określony w sekcji 508, jednak nie wchodzi to w zakres procesu badania. Wyjątek dla kryterium sukcesu 2.2.2 powinien być dokładnie rozważony jako wymaganie zgodności 5: Bez zakłóceń.

### Zastosowanie

Test 2.C 2.2.2-automatyczna-aktualizacja **nie ma zastosowania**, jeśli na stronie nie ma treści, która aktualizuje się automatycznie **lub** jeśli treść, która aktualizuje się automatycznie, jest jedyną treścią na stronie. 

### Jak testować:

1.  Ustal, czy istnieje wyraźny mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie treści albo kontrolowanie częstotliwości aktualizacji w *pierwszych trzech elementach*, które użytkownik napotka **albo**  w ramach trzech elementów przed lub po treści, która się automatycznie aktualizuje.


   Ponieważ chodzi o to, aby użytkownicy mogli szybko wyłączyć automatyczne aktualizowanie informacji, mechanizm ten musi być widoczny w pierwszych trzech elementach, które użytkownik napotka u góry strony lub w obrębie trzech elementów przed i po treści, która się automatycznie aktualizuje. Przykładami takich mechanizmów są: instrukcje tekstowe, skróty klawiaturowe, łącze, przycisk, okno dialogowe z instrukcją.

2.  Aktywuj mechanizm. Sprawdź, czy mechanizm działa poprawnie.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich pozostałych wymagań testowych w tym procesie.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 2.2.2:

1.  Istnieje mechanizm, który może wstrzymywać, zatrzymywać lub ukrywać treść albo kontrolować częstotliwość aktualizacji **oraz**
2.	Mechanizm znajduje się w:
-   *trzech pierwszych elementach* napotykanych przez użytkownika **lub**
-   trzech elementach znajdujących się przed albo po treści, która się aktualizuje automatycznie.

**oraz**

3.  Mechanizm spełnia wszystkie pozostałe obowiązujące warunki testu w tym procesie testowym.


### Powiadomienie o zmianie (automatyczna aktualizacja)

### Test 2.D 4.1.2-powiadamianie-o-automatycznej-zmianie

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4.1.2-powiadamianie-o-automatycznej-zmianie | 2.D     | Strona zawiera powiadomienia o każdej automatycznej aktualizacji / zmianie treści. |

### Cel testu 

Celem tego testu jest sprawdzenie, czy po każdej automatycznej zmianie treści (bez odświeżania strony lub aktywacji użytkownika), użytkownik otrzyma powiadomienie o tej zmianie i może skorelować zmianę z równoważnymi informacjami programowymi lub tekstowymi.

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 4.1.2 Nazwa, rola, wartość](https://wcag.lepszyweb.pl/#name-role-value).

### Metody i narzędzia testowe 
1.	Inspekcja ręczna.
2.	ANDI: struktury > przycisk „żywe regiony”.

### Identyfikacja treści

Wszelkie treści na stronie, które zmieniają się lub aktualizują się automatycznie (bez aktywacji przez użytkownika)

**Uwaga**: nie uwzględniaj żadnych zmian inicjowanych przez użytkownika, takich jak np. otwieranie i zamykanie menu.

### Zastosowanie

Test 2.D 4.1.2-powiadamianie-o-automatycznej-zmianie **nie ma zastosowania**, jeśli na stronie nie ma treści, która aktualizuje się automatycznie **lub** zmienia się automatycznie. 


### Jak testować

1.  Określ, w jaki sposób użytkownik jest powiadamiany o zmianie treści.

    1.  Zidentyfikuj wszystkie okna dialogowe ostrzegające użytkownika o zmianach treści.

        1.  Ustal, czy okna dialogowe zapewniają wystarczające programowe powiadamianie o zmianach treści.

    2.  Zidentyfikuj zmiany treści, które powodują przeniesienie fokusu na treść, która uległa zmianie.

        1.  Ustal, czy przeniesienie fokusu na zmienioną treść jest wystarczające, aby powiadomić użytkownika o zdarzeniu zmiany (np. opisując zmianę bezpośrednio w treści, na którą fokus został przeniesiony).

    3.  Zidentyfikuj zmiany treści występujące w aktywnym „żywym” obszarze ARIA:

        1.  Uruchom ANDI: struktury

        2.  Kliknij przycisk „żywe regiony”, a następnie użyj myszy, aby najechać wskaźnikiem myszy na dowolny zidentyfikowany żywy region (alternatywnie, użyj przycisków poprzedni/następny elementu ANDI, aby przejść do zidentyfikowanych żywych regionów).

        3.  Sprawdź, czy zmieniająca się treść jest zawarta w żywym regionie.

### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 4.1.2:

1.  Strona powiadamia użytkownika o zmianie za pośrednictwem okna dialogowego dostępnego z klawiatury **lub**

2.  Strona przenosi fokus na treść, która się zmieniła, **oraz** treść, która się zmieniła, zapewnia wystarczający opis zmiany, **albo**

3.  Zmieniona treść jest zawarta w „żywym regionie” ARIA.

### Uwaga:

-   Ten test sprawdza powiadamianie o zmianach treści. Testowanie treści przed zmianą i po niej należy przeprowadzić w innych testach. Na przykład elementy formularza, które zmieniły się podczas tego testu, należy przetestować pod kątem testu 5.B.


### Obowiązujące normy

{% include ks/2-2-2.md %}

{% include ks/1-4-2.md %}

[21. Limity czasu](ICT-21-limity-czasu)

{% include ks/4-1-2.md %} 

[5. Treść zmienna](ICT-05-tresc-zmienna) 


