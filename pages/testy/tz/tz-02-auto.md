---
title: 2. Automatyczne odtwarzanie i automatyczna aktualizacja treści


sidebar: testy_sidebar
permalink: tz-02-auto
folder: testy/tz
---

### Automatyczne odtwarzanie dźwięku

### Identyfikacja treści

Zidentyfikuj treść audio, która jest odtwarzana automatycznie (bez aktywacji przez użytkownika) przez ponad 3 sekundy.

-   Treści tego typu to alerty, dźwięki i muzyka.

Jeśli nie ma treści nie ma treści audio odtwarzanej automatycznie przez ponad 3 sekundy, wynikiem testu o identyfikatorze 2.A jest **NIE MA ZASTOSOWANIA**.

#### Test 1.4.2-sterowanie-dzwiekiem (sterowanie dźwiękiem)

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.2-sterowanie-dzwiekiem | 2.A | Użytkownik może wstrzymywać, zatrzymywać lub kontrolować głośność odtwarzanej automatycznie treści audio. |

#### Zastosowanie:

Ten test **NIE MA ZASTOSOWANIA**, jeśli nie ma treści audio odtwarzanej automatycznie przez ponad 3 sekundy.

#### Jak testować:

1.	Ustal, czy w *pierwszych trzech napotkanych elementach* znajduje się mechanizm umożliwiający użytkownikowi wstrzymanie lub zatrzymanie dźwięku lub kontrolę głośności dźwięku odtwarzanego automatycznie (tylko).

    1.  Przeglądarka powinna być już skonfigurowana tak, aby wyłączyć autoodwarzanie. (Instrukcje znajdują się w Podręczniku instalacji i konfiguracji narzędzi testowych).

2.  Aktywuj mechanizm.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich wymaganych warunków testowych.


#### Wyniki oceny

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas treść **PRZESZŁA** test:

1.  Istnieje mechanizm, który może wstrzymywać lub zatrzymywać dźwięk lub kontrolować głośność tylko automatycznego odtwarzania dźwięku ORAZ

2.  Mechanizm należy do *pierwszych trzech elementów* napotkanych przez użytkownika, AND

3.  Mechanizm spełnia wszystkie obowiązujące warunki testu w tym procesie testowym.


##### Uwaga:

- Możliwość wyłączenia automatycznego odtwarzania mediów i/lub wyciszenia określonej karty w przeglądarce to akceptowalny mechanizm zatrzymywania lub kontrolowania głośności automatycznie odtwarzanej treści audio. Niestety, nie wszystkie przeglądarki mają możliwość wyłączenia automatycznego odtwarzania multimediów lub wyciszenia określonych okien lub kart.

- Mechanizm kontroli głośności dźwięku musi być niezależny od ogólnego poziomu głośności systemu operacyjnego, ponieważ może to również wpływać na głośność mowy czytnika ekranu.

### Treść przesuwana, migajaca i przewijana

### Identyfikacja treści:

Zidentyfikuj treści wizualne, które:

-   Automatycznie poruszają się, migają lub przewijają (bez aktywacji przez użytkownika) ORAZ

-   Trwają dłużej niż 5 sekund ORAZ

-   Nie jest to jedyna treść na stronie.

Treści tego typu obejmują przewijanie tekstu, filmów i multimediów.

**WYKLUCZ**  treść, w której ruch, miganie lub przewijanie treści jest niezbędne. Niezbędną jest treść lub sposób prezenatacji, których usunięcie, spowodowałoby zasadniczą zmianę informacji lub funkcjonalności, a informacji i funkcjonalności nie można osiągnąć w inny sposób spełniajacy wymogi zgodności.

Jeśli nie ma takiej treści, wynikiem testu o identyfikatorze 2.B jest **NIE MA ZASTOSOWANIA**.

#### Test 2.2.2-migajace-ruchome-przewijane

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.2.2-migajace-ruchome-przewijane | 2.B     | Użytkownik może wstrzymywać, zatrzymywać lub ukrywać ruchome, migające lub przewijane treści. |

#### Zastosowanie:

Ten wymóg testowy NIE MA ZASTOSOWANIA, jeśli nie ma ruchomej, migającej lub przewijanej treści, która jest odtwarzana automatycznie przez ponad 5 sekund  **LUB** jeśli poruszająca się, migająca lub przewijana treść jest **JEDYNĄ** treścią na stronie internetowej.

#### Jak testować:

1.  Ustal, czy istnieje wyraźny mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie treści w *pierwszych trzech elementach*, które użytkownik napotka LUB w obrębie trzech elementów przed i po treści ruchomej, migającej lub przewijanej.

2.  Aktywuj mechanizm.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich wymaganych warunków testowych.

#### Wyniki oceny
Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas treść **PRZESZŁA** test:

1.	Istnieje mechanizm, który może wstrzymywać, zatrzymywać lub ukrywać treść ORAZ
2.	Mechanizm znajdduje się w:
-   *trzech pierwszych elementach* napotykanych przez użytkownika lub
-   trzech elementach znajdujących się przed albo po treści ruchomej, migającej przewijanej,

> ORAZ

3.	Mechanizm **przechodzi** wszystkie odpowiednie warunki testowe w tym procesie testowym.

### Automatyczna aktualizacja

### Identyfikacja treści

Zidentyfikuj treści, które:

-   Aktualizują się automatycznie (bez aktywacji przez użytkownika) ORAZ

-   Nie są jedyną treścia na stronie

Treść tego typu obejmuje zegary, notowania giełdowe i liczniki.


**Uwaga**:

- Kryterium sukcesu 2.2.2 nie dotyczy automatycznej aktualizacji informacji, gdy jest ona niezbędna. Jednak automatyczna aktualizacja paska notowań giełdowych, który przekazuje informacje w czasie rzeczywistym, nie byłaby uważana za niezbędną (według WCAG), więc zostałaby uwzględniona w tym teście. 
Jest prawdopodobne, że większość przypadków automatycznej aktualizacji nie byłaby niezbędna (nie miałaby istotnego znaczenia). 
Aby uniknąć nieprawidłowego pominięcia treści w tym teście, tester nie ma za zadanie ustalić, czy automatyczna aktualizacja jest niezbędna i powinien uwzględnić wszystkie treści, które odpowiadają opisowi „Identyfikacja treści”. Wyjątek określony w sekcji 508 może być zastosowany w odniesieniu do istotnej treści podlegającej automatycznej aktualizacji, jednak nie wchodzi to w zakres procesu badania. Wyjątek dla SC 2.2.2 powinien być dokładnie rozważony jako wymaganie zgodności 5: Zakłócenia wymagają jego zgodności.

Jeśli nie ma takiej treści, wynikiem testu o identyfikatorze 2.C jest **NIE MA ZASTOSOWANIA**.

#### Test 2.2.2-automatyczna-aktualizacja

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.2.2-automatyczna-aktualizacja | 2.C     | Użytkownik może wstrzymywać, zatrzymywać, ukrywać lub kontrolować częstotliwość automatycznego aktualizowania treści. | 

#### Zastosowanie:

Ten wymóg testowy **NIE MA ZASTOSOWANIA**, jeśli nie ma ruchomej, migającej lub przewijanej treści, która jest aktualizowana auutomatycznie.


#### Jak testować:

1.  Ustal, czy istnieje wyraźny mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie treści w *pierwszych trzech elementach*, które użytkownik napotka LUB w obrębie trzech elementów przed i po treści, która się automatycznie aktualizuje.

2.  Aktywuj mechanizm.

3.  Po zakończeniu procesu testowania przetestuj mechanizm pod kątem wszystkich wymaganych warunków testowych.

#### Wyniki oceny

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, wówczas treść **PRZESZŁA** test:

1.  Istnieje mechanizm, który może wstrzymywać, zatrzymywać lub ukrywać treść lub kontrolować częstotliwość aktualizacji ORAZ


2.  Mechanizm znajdduje się w:

-   *trzech pierwszych elementach* napotykanych przez użytkownika lub

-   trzech elementach znajdujących się przed albo po treści, która się aktualizuje automatycznie,

> ORAZ

3.	Mechanizm **przechodzi** wszystkie odpowiednie warunki testowe w tym procesie testowym.



### Powiadomienie o zmianie (automatyczna aktualizacja)

### Identyfikacja treści

Zidentyfikuj treść, która zmienia się automatycznie na stronie w ramach automatycznej aktualizacji.
Uwaga : nie uwzględniaj żadnych zmian inicjowanych przez użytkownika, takich jak otwieranie / zamykanie menu.

Jeśli nie ma takiej treści, wynikiem testu o identyfikatorze 2.D jest **NIE MA ZASTOSOWANIA**.

#### Test 4.1.2-powiadamianie-o-automatycznej-zmianie

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 4.1.2-powiadamianie-o-automatycznej-zmianie | 2.D     | Strona zawiera powiadomienia o każdej automatycznej aktualizacji / zmianie treści. |


#### Zastosowanie:

Ten wymóg testowy NIE MA ZASTOSOWANIA, jeśli treść strony nie aktualizuje się ani nie zmienia automatycznie.

#### Jak testować:

1.  Określ, w jaki sposób użytkownik jest powiadamiany o zmianie treści.

    1.  Zidentyfikuj wszystkie okna dialogowe ostrzegające użytkownika o zmianach treści.

        1.  Ustal, czy okna dialogowe zapewniają wystarczające programowe powiadamianie o zmianach treści.

    2.  Zidentyfikuj zmiany treści, które powodują przeniesienie fokusa na treść, która uległa zmianie.

        1.  Ustal, czy przeniesienie fokusa na zmienioną treść jest wystarczające, aby powiadomić użytkownika o zdarzeniu zmiany (np. opisując zmianę bezpośrednio w treści, na którą fokus został przeniesiony).

    3.  Zidentyfikuj zmiany treści występujące w aktywnym &bdquo;żywym&rdquo; obszarze ARIA:

        1.  Uruchom ANDI: struktury

        2.  Kliknij łącze „żywe regiony”, a następnie użyj myszy, aby najechać wskaźnikiem myszy na dowolny zidentyfikowany żywy region (alternatywnie, użyj przycisków poprzedni/następny elementu ANDI, aby przejść do zidentyfikowanych żywych regionów).

        3.  Sprawdź, czy zmieniająca się treść jest zawarta w żywym regionie.

#### Wyniki oceny

Jeśli którekolwiek z poniższych stwierdzeń jest **PRAWDZIWE**, wówczas treść **PRZESZŁA** test:

1.  Strona powiadamia użytkownika o zmianie za pośrednictwem okna dialogowego dostępnego z klawiatury LUB

2.  Strona przenosi fokus na treść, która się zmieniła, ORAZ treść, która się zmieniła, zapewnia wystarczający opis zmiany, LUB

3.  Zmieniona treść jest zawarta w żywym obszarze ARIA

##### Uwaga:

-   Ten test sprawdza powiadamianie o zmianach treści. Testowanie treści przed zmianą i po niej należy przeprowadzić w innych testach. Na przykład elementy formularza, które zmieniły się podczas tego testu, należy przetestować pod kątem testu 5.B.


### Obowiązujące normy

{% include ks/2-2-2.md %}

{% include ks/1-4-2.md %}

[21. Limity czasu](ICT-21-limity-czasu)

{% include ks/4-1-2.md %} 

[5. Treść zmienna](ICT-05-tresc-zmienna) 


