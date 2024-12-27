---
title: 5. Kontrolki użytkownika
last_updated: 22 października 2024

sidebar: testy_sidebar
permalink: ICT-05-kontrolki-uzytkownika
folder: testy/itc
---
# 5. Kontrolki użytkownika

## Wymagania dostępności
- {% include ks/4-1-2.md %}  

## Uzasadnienie metody testowej
Celem tego testu podstawowego jest sprawdzenie, czy kontrolki mają określone poniższe cechy dostępności:
- Nazwa
- Rola
- Stan
- Wartość

## Ograniczenia, założenia lub wyjątki
- [Komponent interfejsu użytkownika] to część treści, która jest postrzegana przez użytkowników jako pojedynczy element sterowania konkretną funkcją. Komponentami interfejsu użytkownika są elementy formularzy i łącza, a także komponenty generowane przez skrypty. W tym teście dla zwięzłości użyto terminu „kontrolki użytkownika”.
- Cechy dostępności kontrolki użytkownika muszą być poprawne, jeśli kontrolka użytkownika ulegnie zmianie.
- Zgodnie z [Objaśnieniem WCAG KS 1.4.1 Użycie koloru](https://wcag.irdpl.pl/understanding/uzycie-koloru.html) autorzy nie mogą ustawiać stanu odwiedzonych łączy. Element kotwicy nie zawiera atrybutu „odwiedzony”; dlatego autor nie ma możliwości zmiany stanu poprzez ustawienie atrybutu. Wyklucz stany łączy „odwiedzone/nieodwiedzone” z tego testu podstawowego.

- [Sekcja Role widżetów w dokumencie Accessible Rich Internet Applications (WAI-ARIA) 1.2](https://www.w3.org/TR/wai-aria/#attrs_widgets) wymienia role, które mogą być używane w kontrolkach użytkownika. „Widżet” to „dyskretny obiekt interfejsu użytkownika, z którym użytkownik może wchodzić w interakcje. Widżetami są zarówno proste obiekty, które mają jedną wartość lub wykonują jedną operację (np. pola wyboru i elementy menu), jak i złożone obiekty, które zawierają wiele zarządzanych podobiektów (np. drzewa i siatki)”.
- [Sekcja Role widżetów w dokumencie Accessible Rich Internet Applications (WAI-ARIA) 1.2](https://www.w3.org/TR/wai-aria/#attrs_widgets) wymienia atrybuty stanu i właściwości dla elementów interfejsu użytkownika znajdujących się w systemach GUI lub w bogatych aplikacjach internetowych, które odbierają wprowadzane przez użytkownika dane i przetwarzają jego działania. Atrybuty te są wykorzystywane do obsługi ról widżetów. Specyfikacja WAI ARIA wyjaśnia, że „wartości właściwości (takich jak `aria-labelledby`) są często mniej prawdopodobne do zmiany w całym cyklu życia aplikacji niż wartości stanów (takich jak `aria-checked`), które mogą się często zmieniać z powodu interakcji użytkownika”.
- W instrukcjach testu podstawowego, w przypadku wykrycia roli ARIA, jest to pierwsza prawidłowa wartość atrybutu roli ARIA.

## 5.A Procedura testowania nazwy kontrolki
Identyfikator testu podstawowego: *5.A-ControlName*

### Identyfikacja treści
Rozpoznaj kontrolki użytkownika dla każdej odrębnej funkcji. Wyklucz formularze i łącza, ponieważ są one objęte odpowiednio testami podstawowymi [10. Formularze](ICT-10-formularze.md) i testami podstawowymi [14. Łącza](ICT-14-lacza.md).

### Instrukcja testowania
1.	Sprawdź, czy kombinacja dostępnej nazwy i dostępnego opisu nie jest pusta.
2.	Sprawdź, czy niepusta kombinacja dostępnej nazwy i dostępnego opisu opisuje przeznaczenie kontrolki.
3.	Jeśli nazwa kontrolki użytkownika zmieni się podczas interakcji z użytkownikiem, powtórz poprzednie kroki testu i sprawdź, czy dostępna nazwa jest poprawna po zmianie.
    - W zależności od kontrolki, zmiana nazwy może być wywołana przez różne działania, takie jak zmiana wartości lub stanów innych komponentów, przełączenie funkcji, wprowadzenie danych w komponencie, najechanie myszką itp.
    - Przykłady: wprowadzenie odpowiedzi w polu formularza dla kraju zmienia nazwę przycisku na „Zapisz zmiany”, a wybranie kontrolki przełącza jej funkcję z „Rosnąco” na „Malejąco”.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.A-Nazwa-kontrolki_ kończy się niepowodzeniem.

## 5.B Procedura testowania roli kontrolki
Identyfikator testu podstawowego: _5.B-ControlRole_

### Identyfikacja treści
Znajdź kontrolki użytkownika dla każdej odrębnej funkcji, które mają jawny atrybut roli. 
Przykładami są formularze, łącza i przełączniki.

### Instrukcja testowania
1.	Sprawdź, czy rola kontrolki użytkownika jest poprawna i odpowiednia do jej funkcji. 

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.B-ControlRole_ kończy się niepowodzeniem.

## 5.C Procedura testowania stanu kontrolki
Identyfikator testu Podstawowego: _5.C-ControlState_

### Identyfikacja treści
Znajdź kontrolki użytkownika dla każdej odrębnej funkcji, których stan użytkownik może zmienić. Przykładami takich kontrolek użytkownika są te, które można zaznaczać, rozwijać, ukrywać i naciskać. Wyklucz stan odwiedzonych/nieodwiedzonych łączy.

### Instrukcja testowania
1.	Sprawdź, czy stan kontrolki użytkownika jest poprawny.
2.	Jeśli stan kontrolki użytkownika zmienia się w trakcie użycia aplikacji, sprawdź, czy stan kontrolki użytkownika po zmianie stanu jest poprawny.
   - W zależności od kontrolki, zmiana stanu może być wywołana przez różne działania, takie jak zmiana wartości lub stanów innych komponentów, przełączenie funkcji, wprowadzenie danych w komponencie, najechanie myszką itp.
   - Przykładami mogą być: wyłączony przycisk „Prześlij”, który jest włączany po wypełnieniu wszystkich wymaganych pól formularza albo po zakończeniu obliczeń zainicjowanych przez użytkownika, stan pola wyboru, który może się zmieniać z zaznaczonego na niezaznaczone, kontrolka sortowania kolumn tabeli, który może być przełącznikiem z „Rosnąco” na „Malejąco”.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.C-ControlState_ kończy się niepowodzeniem.

## 5.D Procedura testowania wartości kontrolki
Identyfikator testu bazowego: _5.D-ControlValue_

### Identyfikacja treści
Znajdź kontrolki użytkownika, których wartość użytkownik może zmienić.  Przykładami są pola formularzy i suwaki.

### Instrukcja testowania
1.	Sprawdź, czy wartość kontrolki użytkownika jest poprawna.
2.	Sprawdź, czy wartość kontrolki może być zmieniana. W zależności od kontrolki, zmiana wartości może być wykonana poprzez wprowadzenie liczby, wybór z listy opcji itp.
3.	Sprawdź, czy wartość kontrolki użytkownika jest poprawna po zmianie wartości zainicjowanej przez użytkownika.

### Wynik testów
Jeśli którykolwiek z powyższych testów zakończy się niepowodzeniem, test podstawowy _5.D-ControlValue_ kończy się niepowodzeniem.

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-  Zmiany w kontrolkach mogą również obejmować zmiany koloru w celu przekazania informacji. Jeśli tak, ten test powinien sprawdzić, czy nazwa została zaktualizowana, aby odzwierciedlić znaczenie zmienionego koloru. Jeśli kolor zostanie użyty jako jedyny wizualny sposób przekazywania informacji (lub zmian informacji), wówczas treść nie spełnia wymagań KS 1.4.1 Użycie koloru (omówione w punkcie [7. Właściwości zmysłowe](ICT_07_wlasciwosci-zmyslowe.md)).
- Dostępna nazwa i dostępny opis niektórych kontrolek użytkownika są testowane w innych testach podstawowych, takich jak testy podstawowe [10. Formularze](ICT-10-formularze.md), testy podstawowe [14. Łącza](ICT-14-lacza.md).
- W przypadku kontrolek użytkownika, które mają dedykowane testy podstawowe, zamapuj je na te testy dla dostępnej nazwy, a nie _5.A-ControlName_.
- Ten test może wymagać interakcji z kontrolkami w celu oceny zmian w nazwie, roli, stanie, wartości. Pomocne mogą być instrukcje dotyczące interakcji, takie jak plan testów.

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/F20.md %}