---
title: 8. Dostosowanie limitów czasu


sidebar: testy_sidebar
permalink: tz-08-limit-czasu
folder: testy/tz
---

## Cel procedury testowej

Celem tej procedury testowej jest sprawdzenie, czy zapewniono użytkownikom z niepełnosprawnościami wystarczająco dużo czasu na interakcję z treścią strony internetowej. Wiele osob może potrzebować więcej czasu na czytanie lub interakcję z treścią. Gdy treść witryny jest zależna od czasu, niektórym użytkownikom może być trudno wykonać wymaganą czynność przed upływem czasu.

Procedura testowa „Dostosowanie limitów czasu” obejmuje jeden test:

1.	8.A - 2.2.1-dostosowanie-czasu


### Test 8A: 2.2.1-dostosowanie-czasu

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.2.1-dostosowanie-czasu | 8.A     | Użytkownik może wyłączyć, dostosować lub przedłużyć limit czasu. |


### Cel testu 8A: 2.2.1-dostosowanie-czasu

Celem testu 8A jest upewnienie się, że gdy strona internetowa zawiera treści z ograniczeniami czasowymi, użytkownik może wyłączyć to ograniczenie albo dostosować lub wydłużyć czas. Daje to każdemu użytkownikowi odpowiedni czas na interakcję ze stroną internetową, na przykład podczas wypełniania formularza, czytania treści lub wykonywania czynności (takich jak zakup przedmiotu, wykonanie przelewu bankowego lub korzystanie z aplikacji). 


Wyniki tego testu pozwalają ustalić, czy spełnione jest kryterium sukcesu 2.2.1 Dostosowanie limitów czasu.

### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa strony.


### Identyfikacja treści

Zidentyfikuj wszelkie przypadki ograniczeń czasowych dotyczących treści.

  **Uwaga**: Limitem czasowym jest każdy proces, który ma miejsce bez inicjacji użytkownika po określonym czasie lub następuje okresowo. Obejmuje to częściowe lub pełne aktualizacje treści, automatyczne odświeżanie strony albo wylogowanie użytkownika po określonym czasie lub pewnym okresie bezczynności), zmiany treści lub wygaśnięcie okna możliwości reakcji użytkownika na prośbę o wprowadzenie danych. Zdarza się, że wprowadzane są ograniczenia czasu na czytanie treści, wypełnianie formularzy, trwanie sesji.

Ograniczenia czasowe można określić poprzez:

-   Sprawdzanie dokumentacji systemu lub witryny

-   Poszukanie wskaźników limitów czasowych na stronie, na której występuje ograniczenie, w tym:

    -  opisów tekstowych,

    -  wyskakujących okienek z komunikatami lub innych wskaźniki ostrzegawczych,	

-   Pozostawienie strony w stanie spoczynku przez dłuższy czas, w którym może zostać wyświetlone powiadomienie o przekroczeniu limitu czasu lub innego ostrzeżenia, że uplywa limit czasu.

**Wskazówki**:

-   Możesz zapytać programistę lub osobę kontaktową, czy na stronie występują limity czasu.

-   Limity czasu występują najczęściej w aplikacjach, która wymagają od użytkownika zalogowania się.


**WYJĄTKI**:

-   **Wyjątek dotyczący czasu rzeczywistego:** Limit czasowy jest wymaganą częścią jakiejś czynności w czasie rzeczywistym (np. aukcji) i nie ma możliwości zmiany limitu, lub:

-   **Wyjątek dotyczący istoty czynności:** Limit czasowy jest istotny i wydłużenie go powodowałoby niespełnienie ważnego kryterium działania lub zaburzałoby daną czynność, a informacji i funkcjonalności nie można uzyskać w inny sposób lub:

-   **Wyjątek 20 godzin:** Limit czasowy przekracza 20 godzin. 

### Zastosowanie
Test 8A: 2.2.1-dostosowanie-czasu **nie ma zastosowania**, jeśli na stronie nie ma ma limitów czasu albo jeśli limit czasu jest uzasadniony jednym wyjątków określonych powyżej w sekcji „Identyfikacja treści”.  

### Jak testować

1.	Ustal, czy istnieje sposób na wyłączenie, dostosowanie lub przedłużenie limitu czasu

### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 2.2.1:

1.  Użytkownik może wyłączyć limit czasu przed jego upływem **lub** 

2.  Użytkownik może dostosować limit czasu przed jego upływem do co najmniej dziesięciokrotności długości ustawienia domyślnego, **lub**

3.  Strona wyświetla ostrzeżenie przed upływem czasu **oraz**:

    1.  Przez co najmniej 20 sekund użytkownik może przedłużyć czas za pomocą prostej czynności (np. naciśnięcie klawisza spacji) **oraz**

    2.  Użytkownik może przedłużyć limit czasu co najmniej dziesięć razy.
	

## Obowiązujące normy

{% include ks/2-2-1.md %}

[21. Limity czasu](ICT-21-limity-czasu)                                                                                                         