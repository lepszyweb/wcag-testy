---
title: Accessibility Insights – ocenianie dostępności  cyfrowej

sidebar: narzedzia_sidebar
tags: [rozszerzenia_przeglądarek, skryptozakładka,narzędzia_oceny_dostępności]

permalink: nod-insights
folder: narzedzia-p
---


Accessibility Insights for Web to rozszerzenie dla Chrome i Microsoft Edge Insider [stworzone przez Microsoft](https://accessibilityinsights.io/en/), które pomaga programistom znaleźć i naprawić problemy z dostępnością w aplikacjach i witrynach internetowych.

Narzędzie obsługuje dwa podstawowe scenariusze:
- **FastPass**: lekki, dwuetapowy proces, który pomaga programistom w wykrywaniu typowych problemów związanych z dostępnością w niecałe pięć minut.
   - **Automated checks** (Testy automatyczne) – automatycznie sprawdza zgodność z około 50 wymaganiami dostępności.
   - **Tab stops** (Punkty tabulacji) – narzędzie zapewnia przejrzyste instrukcje i wizualną pomoc, która ułatwia identyfikację krytycznych problemów dostępności związanych z obsługą za pomocą klawiatury, pułapki na klawiaturę i nieprawidłowa kolejność tabulacji.
- **Assessment** (Ocena wspomagana) pozwala każdemu, kto zna się na HTML, na sprawdzenie, czy aplikacja internetowa jest zgodna z WCAG 2.1 na poziomie AA:
   - **Automated checks** (Testy automatyczne) – automatycznie sprawdza zgodność z około 50 wymaganiami dostępności.
   - **Manual tests** (Testy ręczne) – narzędzie zawiera instrukcje krok po kroku, przykłady i wskazówki dotyczące około 20 testów; wiele testów jest &bdquo;wspomaganych&rdquo;, co oznacza, że narzędzie identyfikuje przypadki testowe lub zapewnia pomoc wizualną, a oceniający dokonuje osądu i wskazuje wynik oceny


## Jak wykonać ocenę

### Przygotuj się do testu

W przeglądarce Chrome lub Microsoft Edge przejdź do strony, którą chcesz przetestować (czyli strony docelowej).
1. Otwórz Accessibility Insights for Web:
2. Wybierz ikonę rozszerzenia.
   - lub naciśnij Ctrl + Shift + K (⌘ + Shift + K dla MacOS) ([Dostosuj ten skrót klawiaturowy](https://accessibilityinsights.io/docs/en/web/reference/keyboard)).
   - lub użyj następujących poleceń klawiatury:
   a) **Windows lub Linux**:
      - Naciśnij Shift + Alt + T lub F10, aby ustawić fokus na pasku adresu przeglądarki.
      - Naciśnij strzałkę w lewo, aby ustawić koncentrację na statystykach dostępności dla rozszerzenia sieci Web.
      - Naciśnij klawisz spacji, aby otworzyć rozszerzenie.
   b) **System operacyjny Mac**:
      - Naciśnij ⌘ + L, aby ustawić ostrość na pasku adresu przeglądarki.
      - Naciśnij klawisz Tab, aby ustawić koncentrację na statystykach dostępności dla rozszerzenia sieci Web.
      - Naciśnij klawisz spacji, aby otworzyć rozszerzenie.
Rozszerzenie Accessibility Insights for Web otworzy **pasek uruchamiania**.

{% include image.html file="insights/insights01.png" alt="W panelu startowym dostępne są trzy opcje: FastPass, Assessment, narzędzia ad hoc" %}

3. Na pasku uruchamiania wybierz **Assessment** (Ocenianie).
Zostanie otwarte dodatkowe okno przeglądarki zawierające przegląd procesu oceny i wyników. W tym momencie ocena jest w 100% niepełna, więc nie będą dostępne żadne wyniki.

{% include image.html file="insights/insights02.png" alt="Badana strona i przegląd testów wyświetlany obok siebie" %}

### Uruchom automatyczne sprawdzanie
1.	W okienku nawigacji wybierz opcję Automatyczne sprawdzanie – **Automated checks**.
W ciągu kilku sekund funkcja Accessibility Insights for Web sprawdzi stronę docelową pod kątem zgodności z dziesiątkami wymagań dostępności. Wymagania te pojawią się na liście z wymaganiami, które nie zostały spełnione. Instancje błedów pojawią się w panelu po liście.

{% include image.html file="insights/insights03.png" alt="Wyświetlanie wyników kontroli automatycznej, pogrupowanych według testów"  %}

2.	Przejrzyj wyniki:
- Aby zobaczyć wystąpienia awarii dla danego wymagania, wybierz wymaganie.
- Aby dowiedzieć się więcej o wymaganiu, wybierz **See more info here** (Zobacz więcej informacji tutaj). Aplikacja przekieruje cię na stronę Uniwersytetu Deque, na której znajdziesz szczegółowe informacje dotyczące badanego aspektu (w języku angielskim)  
- Aby zobaczyć wystąpienia awarii wyróżnione bezpośrednio na stronie docelowej:
- Włącz przełącznik pomocnika wizualnego, **Visual helper**, aby jednocześnie zaznaczyć wszystkie wystąpienia awarii
lub
- Zaznacz jedno lub więcej pól wyboru, aby wyróżnić określone wystąpienia awarii.

{% include image.html file="insights/insights04.png" alt="Przypadki defektu wyróżnione na badanej stronie"  %}

### Wykonaj testy wspomagane i ręczne
Każdy z pozostałych testów obejmuje zestaw powiązanych wymagań. Zalecamy wykonanie tych testów w kolejności, w jakiej pojawiają się w okienku nawigacji.
1.	Wybierz test w okienku nawigacji.
a.	Aby dowiedzieć się więcej o temacie testowym, wybierz ikonę **Guidance** (Wskazówki) obok tytułu testu. Wskazówki na poziomie testu obejmują:
- Dlaczego jest to ważne
- Wskazówki: Co robić, czego nie robić
- Linki do odpowiednich kryteriów sukcesu WCAG, wystarczających technik i typowych błędów.
**Uwaga**: Po przeczytaniu sekcji Rozpoczynamy (**Geting started**) możesz ją zwinąć.
Wskazówki dotyczące poziomu testu pojawią się na nowej karcie przeglądarki.

{% include image.html file="insights/insights05.png" alt="Wskazówki otwarte na nowej karcie przeglądarki." %}

2.	Wybierz element z **listy wymagań**. Informacje związane z wymaganiem pojawią się w panelu po liście.
a.	Aby dowiedzieć się więcej o wymaganiu, wybierz  **Info & examples** (Informacje i przykłady). Wytyczne na poziomie wymagań obejmują:
- Dlaczego jest to ważne
- Z perspektywy użytkownika (jeśli dotyczy). To jest wkład z wytycznych Design for People.
- Jak naprawić
- Przykłady
- Fragmenty kodu (w stosownych przypadkach)
- Linki do odpowiednich kryteriów sukcesu WCAG, wystarczających technik i typowych błędów.
Wskazówki dotyczące poziomu wymagań pojawią się w nakładce.

{% include image.html file="insights/insights05.png" alt="Wskazówki dotyczące wymagań otwarte w nakładce."  %}

3. Przeczytaj instrukcje w części **Jak testować**.
**Uwaga**: Po przeczytaniu instrukcji możesz zwinąć sekcję Jak testować.

4. Oceń instancje testowe i zapisz wyniki:

W przypadku wymagań, które automatycznie generują listę instancji testowych do oceny, wybierz Pass lub Fail dla każdej instancji.

Uwaga: Możesz zresetować instancję do oryginalnego stanu nieokreślonego, wybierając Cofnij.

Uwaga: Po zaznaczeniu wszystkich niepowodzeń możesz przekazać pozostałe instancje, wybierając Prześlij niezaznaczone instancje.

Gdy wszystkie wystąpienia awarii zostaną oznaczone jako **Pomiń** lub **Niepowodzenie**, wymaganie pokaże wynik zagregowany.

{% include image.html file="insights/insights06.png" alt="Nie spełniono wymogów zwiażanych z obrazami z powodu wykrycia co najmniej 1 defektu"  %}

W przypadku wymagań, które nie generują instancji testowych:

a) Wybierz **Pass** lub **Fail** dla wymagania.

Uwaga: Możesz zresetować wymaganie do pierwotnego stanu nieokreślonego, wybierając **Cofnij**.

- Jeśli wymaganie nie powiedzie się, dodaj wystąpienie błędu. (Jeśli wymóg zostanie spełniony, nie są potrzebne dalsze dane).
- Gdy wymóg zostanie oznaczony jako **Pass** lub zostaną dodane wystąpienia awarii, wymaganie pokaże wynik zagregowany.

{% include image.html file="insights/insights07.png" alt="Nie spełniono wymogu nawigacji za pomocą klawiatury z powodu wykrycia co najmniej 1 defektu"  %}

- Gdy każde wymaganie w każdym teście jest oznaczone jako **Pass** lub **Fail**, twoja ocena jest zakończona.

### Wyświetl podsumowanie wyników oceny

Wybierz Przegląd w okienku nawigacji.

Podziel się szczegółowym raportem z wyników oceny
1. W pasku poleceń **Widok szczegółów** wybierz **Eksportuj wynik**.
  a. Opcjonalne: podaj opis do uwzględnienia w raporcie.
2. Użyj paska pobierania przeglądarki, aby otworzyć raport lub wyświetlić lokalizację pliku.

### Rozpocznij nową ocenę
**Uwaga**: Dane zebrane podczas oceny będą trwać do momentu rozpoczęcia nowej oceny.

1. W pasku poleceń **Widok szczegółów** wybierz **Rozpocznij od > Rozpocznij od oceny**.
2. Wybierz w oknie dialogowym **Start over** (Zacznij od nowa).


{% include note.html content="Poradnik jest tłumaczeniem: [Assessment in Accessibility Insights for Web](https://accessibilityinsights.io/docs/en/web/getstarted/assessment)  "  %} 