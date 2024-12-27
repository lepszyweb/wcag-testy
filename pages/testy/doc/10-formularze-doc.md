---
title: 10. Formularze (dokumenty)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 10-formularze-doc
folder: testy/doc
---

# 10. Formularze

## Wymagania dostępności
- {% include ks/1-1-1.md %}
- {% include ks/1-3-1.md %}
- {% include ks/2-4-6.md %}
- {% include ks/3-2-2.md %}
- {% include ks/3-3-1.md %}
- {% include ks/3-3-2.md %}
- {% include ks/3-3-3.md %}
- {% include ks/3-3-4.md %}
- {% include ks/4-1-2.md %}

## Uzasadnienie metody testowej
Zapoznaj się z instrukcjami dotyczącymi formularza pod kątem kompletności i programowego powiązania z wprowadzanymi danymi. Wprowadź błędne dane i przejrzyj powiadomienia o błędach dostarczane użytkownikowi.

## Ograniczenia, założenia lub wyjątki
-   Pola formularza tylko do odczytu (np. wstępnie wypełnione) otrzymują fokus klawiatury i można je wybierać, ale nie można ich modyfikować. Pola te muszą być oznaczone i [programowo określone](https://www.w3.org/TR/WCAG21/#dfn-programmatically-determinable). Są testowane zgodnie z KS 1.3.1.
-   Wyłączone pola formularza nie otrzymują fokusu klawiatury, nie można ich wybrać ani modyfikować. Nie są one uwzględniane w tym teście.
-   Połączenie dostępnej nazwy elementu i dostępnego opisu jest jego alternatywą tekstową.
-   Kliknięcie opcji lub wybranie opcji w formularzu powinno spowodować zaznaczenie opcji, ale nie powinno inicjować zmiany  kontekstu.
-   [Zmiana kontekstu](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html#dfn-zmiana-kontekstu) została zdefiniowana na stronie [Objaśnienie KS 3.2.1: Po oznaczeniu fokusem](https://wcag.irdpl.pl/understanding/po-otrzymaniu-fokusu.html#dfn-zmiana-kontekstu) jako: poważna zmiana treści \[strony internetowej\], która, jeśli zostanie dokonana bez świadomości użytkowników, może dezorientować osoby, które nie są w stanie jednocześnie wyświetlić całej strony. Zmiany kontekstu obejmują zmiany:
    1.  W programie użytkownika (przeglądarce, itp.)
    2.  okno ekranu
    3.  Fokusu
    4.  Treści, która zmienia znaczenie dokumentu.
    -   **Uwaga:** Zmiana treści nie zawsze oznacza zmianę kontekstu. Zmiany nie zawsze oznacza zmianę kontekstu. Zmiany treści, na przykład rozwinięcie drzewa, dynamicznego menu lub karty niekoniecznie zmieniają kontekst, dopóki nie zmienią jednego z powyższych (np. fokusu).
    -   **Przykłady**: Otwarcie nowego okna, przeniesienie fokusu na inny obiekt, przejście do innego dokumentu (w tym wszystko, co dla użytkownika może wyglądać tak, jakby przeszedł do innego dokumentu) lub przekształcenie wyglądu dokumentu.
-   Zgodnie z [Objaśnieniem KS 3.3.2: Etykiety lub instrukcje](https://wcag.irdpl.pl/understanding/podczas-wprowadzania-danych.html), to kryterium sukcesu nie ma zastosowania do łączy lub innych kontrolek (takich jak widżet rozwijania/zwijania lub podobne komponenty interaktywne), które nie są powiązane z wprowadzaniem danych.

## 10.A Procedura testowania nazw formularzy 

Identyfikator testu podstawowego: _10.A-FormName_

### Identyfikacja treści
1.  Znajdź wszystkie komponenty formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne), które są powiązane ze składnikami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania
1.  Sprawdź, czy kombinacja [dostępnej nazwy i dostępnego opisu](https://lepszyweb.pl/blog2/dostepne-nazwy-i-dostepne-opisy) nie jest pusta. [KS 4.1.2]
2.	Sprawdź, czy niepusta kombinacja dostępnej nazwy i dostępnego opisu opisuje cel formularza. [KS 4.1.2] [Komponenty formularza zawierające treść inną niż tekst powinny być również mapowane na KS 1.1.1]. 
3.	Sprawdź, czy wszystkie istotne instrukcje i wskazówki (tekstowe i graficzne) są powiązanie programowe (np. powiązania nagłówków kolumn i/lub wierszy tabeli) ze składnikiem formularza. [KS 1.3.1]

### Wynik testów
<p id="d10aTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _10.A-FormName_ również kończy się niepowodzeniem.</p>

## 10.B Procedura testowania opisowości etykiet
Identyfikator testu podstawowego: _10.B-FormDescriptiveLabel_

### Identyfikacja treści
1.  Znajdź wszystkie komponenty formularza (komponenty zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne), które są powiązane ze składnikami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania
<ol id="d10bTI">
    <li id="d10bTI-1">Sprawdź, czy etykiety (instrukcje i wskazówki) każdego komponentu formularza opisują jego cel, informują użytkowników, jakie dane są oczekiwane i, jeśli ma to zastosowanie, jaki format jest wymagany. [KS 2.4.6]</li>
</ol>

### Wynik testów
<p id="d10bTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy 10.B-FormDescriptiveLabel również kończy się niepowodzeniem.</p>

## 10.C Procedura testowania wprowadzania danych
Identyfikator testu podstawowego: _10.C-OnInput_

### Identyfikacja treści
<p id="d10cIC">Wszystkie aktywne komponenty formularzy.</p>

### Instrukcje testowania
1.  Wprowadź dane w każdym polu formularza i opuść pole (klawiszem <kbd>Tab</kbd>).
2.  Zmień wybór lub wartości w komponentach formularza, takich jak przyciski opcji, pola wyboru, listy wyboru itp.
3.  Sprawdź, czy opuszczenie komponentu lub zmiana wartości/wyboru w komponencie (np. wprowadzanie danych w polu tekstowym, zmiana wyboru przycisku opcji)  **NIE**  powoduje zmiany kontekstu, chyba że użytkownik został poinformowany o takim zachowaniu przed użyciem komponentu [KS 3.2.2]. Przykłady zmiany kontekstu:
    -   Automatyczne przesłanie formularza po opuszczeniu pola,
    -   Automatyczne przesłanie formularza po opuszczeniu ostatniego pola w formularzu,
    -   Uruchomienie nowego okna, gdy zostanie zmienione zaznaczenie w grupie przycisków opcji
    -   Przeniesienie fokusu na inny komponent interfejsu po zaznaczeniu elementu na liście wyboru
	
### Wynik testów
<p id="d10cTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _10.C-OnInput_ również kończy się niepowodzeniem.</p>

## 10.D Procedura testowania identyfikacji błędów
Identyfikator testu podstawowego: _10.D-ErrorIdentification_

### Identyfikacja treści
<p id="d10dIC">Znajdź komponenty formularzy z automatycznym wykrywaniem błędów i powiadamianiem o nich.</p>

### Instrukcja testowania
1.	Wprowadź niepoprawne wartości w komponentach zbierających dane, aby wyzwolić automatyczne wykrywanie błędów, które skutkuje powiadomieniami o błędach, np. 
    -   w polach oznaczonych jako wymagane
    -   w polach daty (format)
    -   w polach adresów internetowych (URL, e-mail)
    -   w polach przeznaczonych na hasło
2.  Jeśli  automatycznie zostanie wykryty błąd we wprowadzaniu danych, sprawdź, czy powiadomienie o błędzie spełnia wszystkie poniższe warunki:
    -   użytkownik jest informowany o błędzie (albo natychmiast po opuszczeniu błędnie wypełnionego pola, albo przy próbie przesłania formularza) **oraz**
    -   błąd jest opisany użytkownikowi w formie tekstowej, **oraz**
    -   element, w którym występuje błąd, jest oznaczony tekstem.

### Wynik testów
<p id="d10dTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, wówczas test podstawowy _10.D-ErrorIdentification_ również kończy się niepowodzeniem.</p>

## 10.E Procedura testowania widoczności etykiet i instrukcji
Identyfikator testu podstawowego: _10.E-FormHasLabel_

### Identyfikacja treści
1.  Znajdź wszystkie komponenty formularza (zbierające dane), takie jak pola tekstowe, przyciski opcji, pola wyboru, pola tylko do odczytu i listy wielokrotnego wyboru.
2.  Znajdź wszystkie instrukcje i wskazówki (tekstowe i graficzne), które są powiązane ze składnikami formularza, w tym dotyczące elementów pogrupowanych, kolejności wypełniania, specjalnych warunków lub kwalifikatorów, instrukcji formatowania itp.

### Instrukcja testowania

1.	Sprawdź, czy każdy komponent formularza zbierający dane ma widoczne etykiety lub instrukcje, gdy otrzymuje fokus. [KS 3.3.2]

### Wynik testów
<p id="d10eTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _10.E-FormHasLabel_ również kończy się niepowodzeniem</p>

## 10.F Procedura testowania sugestii korekty błędów
Identyfikator testu podstawowego: _10.F-ErrorSuggestion_

### Identyfikacja treści
<p id="d10fIC">Znajdź komponenty formularzy z automatycznym wykrywaniem błędów i powiadamianiem o nich.</p>

### Instrukcja testowania
1.	Wprowadź niepoprawne wartości w komponentach zbierających dane, aby wywołać automatyczne wykrywanie błędów, które skutkuje powiadomieniami o błędach, np. 
    -   w polach oznaczonych jako wymagane
    -   w polach daty (format)
    -   w polach adresów internetowych (URL, e-mail)
    -   w polach przeznaczonych na hasło
2.	Przejrzyj wszystkie powiadomienia o błędach.
3.	Sprawdź, czy podano dodatkowe wskazówki, jak poprawić błędy w polach formularza, które nie zagroziłyby bezpieczeństwu ani przeznaczeniu treści (np. przykłady poprawnych danych, wskazówki, jak poprawić dane wprowadzone przez użytkownika). [KS 3.3.3]

### Wynik testów
<p id="d10fTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _10.F-ErrorSuggestion_ również kończy się niepowodzeniem.</p>

## 10.G Procedura testowania zapobiegania błędom (prawnym, finansowym, w danych)
Identyfikator testu podstawowego: _10.G-ErrorPrevention_

### Identyfikacja treści
<p id="d10gIC">Dokument, który powoduje powstanie zobowiązań prawnych lub transakcji finansowych dla użytkownika, który modyfikuje lub usuwa dane kontrolowane przez użytkownika w systemach przechowywania danych lub który przesyła odpowiedzi testowe użytkownika.</p>

### Instrukcja testowania
1.	Wypełnij pola formularza niezbędne do przesłania, wpisz błędne dane albo poleć usunięcie danych.
2.	Sprawdź, czy spełniony jest co najmniej jeden z poniższych warunków [KS 3.3.4]:
    a.  **Odwracalność**: Wprowadzenie danych jest odwracalne.
    b.  **Sprawdzanie**: Dane wprowadzone przez użytkownika są sprawdzane pod kątem błędów, a użytkownik ma możliwość wprowadzenia poprawek.
    c.  **Potwierdzenie**: Istnieje mechanizm sprawdzania, potwierdzania i korygowania informacji przed jej ostatecznym wysłaniem.

### Wynik testów
<p id="d10gTR">Jeżeli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _10.G-ErrorPrevention_ również kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesów testowych
-   W przypadku KS 3.3.1 dopuszczalne techniki obejmują: (a) przeniesienie fokusu na komunikat o błędzie informujący użytkownika, że ​​poprzednie pole wymaga korekty i opisujące błąd, (b) odświeżenie strony po przesłaniu formularza i wyświetlenie na górze strony opisów i lokalizacji błędów. **Uwaga**: Ponowne wyświetlenie formularza i wskazanie pól zawierających błędy w formularzu nie jest wystarczające, aby spełnić ten wymóg. Użytkownik nie powinien być zmuszony do przeszukiwania formularza, aby znaleźć miejsca, w których popełniono błędy.
-   W przypadku KS 3.3.4: ponieważ użytkownik może przejrzeć prosty, jednostronicowy formularz przed naciśnięciem przycisku „Prześlij” na stronie, inny specjalny mechanizm weryfikacji poprawności nie jest wymagany.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/G13.md %}
- {% include techniki/G80.md %}
- {% include techniki/G83.md %}
- {% include techniki/G85.md %}
- {% include techniki/G115.md %}
- {% include techniki/G131.md %}
- {% include techniki/H44.md %}
- {% include techniki/H65.md %}
- {% include techniki/H71.md %}
- {% include techniki/PDF5.md %}
- {% include techniki/PDF10.md %}
- {% include techniki/PDF12.md %}
- {% include techniki/PDF15.md %}
- {% include techniki/PDF22.md %}
- {% include techniki/SCR19.md %}
- {% include techniki/F36.md %}
- {% include techniki/F37.md %}
- {% include techniki/F82.md %}

