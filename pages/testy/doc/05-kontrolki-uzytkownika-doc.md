---
title: 5. Kontrolki użytkownika (dokumenty)
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: 05-kontrolki-uzytkownika-doc
folder: testy/doc
---

# 5. Kontrolki użytkownika

## Wymagania dostępności
- {% include ks/4-1-2.md %}  

## Uzasadnienie metody testowej
Celem tego testu podstawowego jest sprawdzenie, czy w przypadku kontrolek użytkownika określono poniższe cechy dostępności:
- Nazwa
- Rola
- Stan
- Wartość

## Ograniczenia, założenia lub wyjątki
- [Komponent interfejsu użytkownika] to część treści, która jest postrzegana przez użytkowników jako pojedynczy element sterowania konkretną funkcją. Komponentami interfejsu użytkownika są elementy formularzy i łącza, a także komponenty generowane przez skrypty. W tym teście dla zwięzłości użyto terminu „kontrolki użytkownika”.
- Cechy dostępności kontrolki użytkownika muszą być poprawne, jeśli kontrolka użytkownika ulegnie zmianie.
- Zgodnie z [Objaśnieniem WCAG KS 1.4.1 Użycie koloru](https://wcag.irdpl.pl/understanding/uzycie-koloru.html) autorzy nie mogą ustawiać stanu odwiedzonych łączy. Element kotwicy nie zawiera atrybutu „odwiedzony”; dlatego autor nie ma możliwości zmiany stanu poprzez ustawienie atrybutu. Wyklucz stany łączy „odwiedzone/nieodwiedzone” z tego testu podstawowego.

## 5.A Procedura testowania nazwy kontrolki
Identyfikator testu podstawowego: *5.A-ControlName*

### Identyfikacja treści

<p id="d5aIC">Rozpoznaj kontrolki użytkownika dla każdej odrębnej funkcji. Wyklucz formularze i łącza, ponieważ są one objęte odpowiednio testami podstawowymi [10. Formularze (dokumenty)](ICT-10-formularze-dokumenty.md) i testami podstawowymi [14. Łącza (dokumenty)](ICT-14-lacza-dokumenty.md).</p>

#### Test Instructions

<ol id="d5aTI">
    <li id="d5aTI-1">Check that the combination of the accessible name and accessible description is not empty. [SC 4.1.2]</li>
    <li id="d5aTI-2">Check that the non-empty combination of the accessible name and accessible description describes the control's purpose. [SC 4.1.2]</li>
    <li id="d5aTI-3">If the name of the user control changes on user interaction, repeat the previous test steps and check that the accessible name is correct after the change.
        <ul>
            <li>Depending on the control, a change of name may be triggered by various actions, such as changing values or states of other components, toggling a function, entering data in the component, mouseover, etc.</li>
            <li>Examples include entering a response in a form field for country changes the name of a button to "Save Changes", and selecting a control toggles its functionality from sorting ascending to descending.</li>
        </ul>
    </li>
</ol>


### Instrukcja testowania
1.	Sprawdź, czy kombinacja dostępnej nazwy i dostępnego opisu nie jest pusta. [KS 4.1.2]
2.	Sprawdź, czy niepusta kombinacja dostępnej nazwy i dostępnego opisu opisuje przeznaczenie kontrolki. [KS 4.1.2]
3.	Jeśli nazwa kontrolki użytkownika zmieni się podczas interakcji z użytkownikiem, powtórz poprzednie kroki testu i sprawdź, czy dostępna nazwa jest poprawna po zmianie.
    - W zależności od kontrolki, zmiana nazwy może być wywołana przez różne działania, takie jak zmiana wartości lub stanów innych komponentów, przełączenie funkcji, wprowadzenie danych w komponencie, najechanie myszką itp.
    - Przykłady: wprowadzenie odpowiedzi w polu formularza dla kraju zmienia nazwę przycisku na „Zapisz zmiany”, a wybranie kontrolki przełącza jej funkcję z „Rosnąco” na „Malejąco”.

### Wynik testów

<p id="d5aTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.A-Nazwa-kontrolki_ kończy się niepowodzeniem.</p>

## 5.B Procedura testowania roli kontrolki
Identyfikator testu podstawowego: _5.B-ControlRole_

### Identyfikacja treści

<p id="d5bIC">Znajdź kontrolki użytkownika dla każdej odrębnej funkcji, które mają jawny atrybut roli. 
Przykładami są kontrolki formularzy, łącza i przełączniki.</p>

### Instrukcja testowania

<ol id="d5bTI">
    <li id="d5bTI-1">Sprawdź, czy rola kontrolki użytkownika jest prawidłowa i odpowiednia dla jej funkcji.  [KS 4.1.2]</li>
</ol>

### Wynik testów

<p id="d5bTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.B-ControlRole_ kończy się niepowodzeniem.</p>

## 5.C Procedura testowania stanu kontrolki
Identyfikator testu Podstawowego: _5.C-ControlState_

### Identyfikacja treści

<p id="d5cIC">Znajdź kontrolki użytkownika dla każdej odrębnej funkcji, których stan użytkownik może zmienić. Przykładami takich kontrolek użytkownika są te, które można zaznaczać, rozwijać, ukrywać i naciskać. Wyklucz stan odwiedzonych/nieodwiedzonych łączy.</p>

### Instrukcja testowania
1.	Sprawdź, czy stan kontrolki użytkownika jest poprawny.  [KS 4.1.2]
2.	Jeśli stan kontrolki użytkownika zmienia się w trakcie użycia aplikacji, sprawdź, czy stan kontrolki użytkownika po zmianie stanu jest poprawny. [KS 4.1.2]
   - W zależności od kontrolki, zmiana stanu może być wywołana przez różne działania, takie jak zmiana wartości lub stanów innych komponentów, przełączenie funkcji, wprowadzenie danych w komponencie, najechanie myszką itp.
   - Przykładami mogą być: wyłączony przycisk „Prześlij”, który jest włączany po wypełnieniu wszystkich wymaganych pól formularza albo po zakończeniu obliczeń zainicjowanych przez użytkownika, stan pola wyboru, który może się zmieniać z zaznaczonego na niezaznaczone, kontrolka sortowania kolumn tabeli, który może być przełącznikiem z „Rosnąco” na „Malejąco”.

### Wynik testów

<p id="d5cTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.C-ControlState_ kończy się niepowodzeniem.</p>

## 5.D Procedura testowania wartości kontrolki
Identyfikator testu bazowego: _5.D-ControlValue_

### Identyfikacja treści

<p id="d5dIC">Znajdź kontrolki użytkownika, których wartość użytkownik może zmienić.  Przykładami są pola formularzy i suwaki.</p>

### Instrukcja testowania
1.	Sprawdź, czy wartość kontrolki użytkownika jest poprawna.  [KS 4.1.2]
2.	Sprawdź, czy wartość kontrolki może być zmieniana. W zależności od kontrolki, zmiana wartości może być wykonana poprzez wprowadzenie liczby, wybór z listy opcji itp.
3.	Sprawdź, czy wartość kontrolki użytkownika jest poprawna po zmianie wartości zainicjowanej przez użytkownika. [KS 4.1.2]

### Wynik testów
<p id="d5dTR">Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.D-ControlValue_ kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-  Zmiany w kontrolkach mogą również obejmować zmiany koloru w celu przekazania informacji. Jeśli tak, ten test powinien sprawdzić, czy nazwa została zaktualizowana, aby odzwierciedlić znaczenie zmienionego koloru. Jeśli kolor zostanie użyty jako jedyny wizualny sposób przekazywania informacji (lub zmian informacji), wówczas treść nie spełnia wymagań KS 1.4.1 Użycie koloru (omówione w punkcie [7. Właściwości zmysłowe (dokumenty)](ICT_07_wlasciwosci-zmyslowe-dokumenty.md)).
- Dostępna nazwa i dostępny opis niektórych kontrolek użytkownika są testowane w innych testach podstawowych, takich jak testy podstawowe [10. Formularze (dokumenty)](ICT-10-formularze-dokumenty.md), testy podstawowe [14. Łącza (dokumenty)](ICT-14-lacza-dokumenty.md).
- W przypadku kontrolek użytkownika, które mają dedykowane testy podstawowe, zamapuj je na te testy dla dostępnej nazwy, a nie _5.A-ControlName_.
- Ten test może wymagać interakcji z kontrolkami w celu oceny zmian w nazwie, roli, stanie, wartości. Pomocne mogą być instrukcje dotyczące interakcji, takie jak plan testów.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/F20.md %}