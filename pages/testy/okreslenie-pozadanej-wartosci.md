---
title: Określenie pożądanej wartości
last_updated: 22 października 2024
toc: false
sidebar: testy_sidebar
permalink: okreslenie-pozadanej-wartosci
folder: testy
---

## Wymagania dostępności
- {% include ks/1-3-5.md %} 

## Test Określenie pożądanej wartościa
Identyfikator testu podstawowego: _okreslenie-pozadanej-wartosci_ / _testID-012_ 

| Nazwa testu | ID testu | Warunek testowy |
|------------------------|---------|---------------------------------------|
| okreslenie-pozadanej-wartosci | 10.H | Pole formularza zbierające dane użytkownika  podpowiada oczekiwaną wartość|

## Cel testu
Celem testu jest sprawdzenie, czy programy użytkownika mogą rozpoznać i przedstawić użytkownikom cel i rodzaj informacji oczekiwanej w polu formularza, które gromadzi dane o użytkowniku.  

## Oczekiwania, ograniczenia lub wyjątki
- Atrybut `autocomplete` HTML umożliwia bardziej szczegółową definicję lub oznaczenie celu niż atrybut `type`, na przykład umożliwia autorowi określenia konkretnego typu nazwy: `given-name` - imię `additional-name` - drugie imię, `family-name` - nazwisko (nazwisko rodowe).
- Wartością atrybutu `autocomplete` może być albo słowo kluczowe `off`, albo `on`, albo uporządkowana lista oddzielonych spacją tokenów wybranych spośród wskazanych w [części 7  WCAG 2.2](https://www.w3.org/TR/WCAG22/#input-purposes). Kryterium sukcesu 1.3.5 wymaga wskazania konkretnych wartości opisujących cel zbieranych danych. Użycie słowa kluczowego `on` nie spełnia KS 1.3.5. 
- **Uwaga do wykazu typów pól danych**. Lista celów typów pól danych jest oparta na celach kontrolek zdefiniowanych w części [HTML 5.2 Autofill field](https://www.w3.org/TR/html52/sec-forms.html#sec-autofill), ale ważne jest, aby zrozumieć, że inna technologia może mieć niektóre lub wszystkie z tych samych pojęć zdefiniowanych w swojej specyfikacji i wymagane są tylko te pojęcia, które są mapowane do poniższych znaczeń.  

## Procedura testowa Orientacja wyświetlania

### Identyfikacja treści
Znajdź wszystkie pola formularzy zbierające dane użytkownika, takie jak imię, nazwisko, dane kontaktowe

### Zastosowanie:
Test _okreslenie-pozadanej-wartosci_ **nie ma zastosowania** do pól formularza, które zbierają dane innych osób niż użytkownik strony.

### Jak testować:
1. Sprawdź, czy w każdym polu formularza, którego temat dotyczy informacji o użytkowniku, cel wprowadzania danych został przekazany programowo, np. za pomocą atrybutu `autocomplete`.
2. Sprawdź, czy wartość lub wartości atrybutu `autocomplete` są poprawne (znajdują się w [wykazie dozwolonych wartości](https://www.w3.org/TR/WCAG22/#input-purposes) lub są mapowane do wartości w tym wykazie.
3. Sprawdź, czy wartość atrybutu `autocomplete` jest odpowiednia w odniesieniu do typu oczekiwanej informacji wskazanej przez etykietę pola.


### Ocena wyników
Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** warunki testowe i test podstawowy _okreslenie-pozadanej-wartosci_ kończy się wynikiem **zaliczony**.
Jeśli którekolwiek twierdzenie poniżej jest **fałszywe**, wówczas strona (treść) **nie spełnia** warunków testowych i test podstawowy _okreslenie-pozadanej-wartosci_ kończy się wynikiem **niezaliczony**.

1. Pole formularza zbierające dane o użytkowniku ma atrybut `autocomplete`.
2. Wartości atrybutu  `autocomplete` są poprawne.
3. Wartości atrybutu `autocomplete` oznaczają typ informacji wskazanej w etykiecie pola.

## Wskazówki praktyczne
brak

## Techniki WCAG 2.2
Przy opracowywaniu tej procedury testowej, wzięto pod uwagę następujące wystarczające techniki i typowe błędy:

- {% include techniki/H98.md %}
- {% include techniki/F107.md %}


