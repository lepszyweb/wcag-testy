---
title: 3-3-3 Sugestie korekty błędów


sidebar: testy_sidebar
permalink: 3-3-3-Sugestie-korekty-bledow
folder: testy/adept
---

## Test
**Czy po wykryciu błędu we wprowadzanych przez użytkownika danych serwis podpowiada mu możliwe odpowiedzi?**

## Wyjaśnienie
Serwisy internetowe często zawierają formularze, w których użytkownik wprowadza dane. Zazwyczaj implementuje się wtedy mechanizmy wykrywania błędów popełnianych przez użytkownika i wtedy system powinien podpowiedzieć prawidłową odpowiedź, o ile jest to tylko możliwe. Serwis może dysponować biblioteką nazw miejscowości i na podstawie wpisanej błędnie nazwy sugerować podobne. Może też rozpoznawać nieprawidłowo wprowadzone formaty daty lub czasu i sugerować prawidłowe wpisy. Można też zaproponować listę wyboru zamiast pola edycyjnego. System nie może podpowiadać prawidłowych wartości w sytuacji, gdy narusza to zasady bezpieczeństwa, a zatem nie powinien podpowiadać loginu lub hasła.

## Testowanie
Sprawdź opublikowane w serwisie formularze wpisując błędne dane. Jeżeli serwis zwraca tylko uwagę na fakt popełnienia błędu, zastanów się, czy mógłby bardziej wspierać użytkownika. Sam musisz zdecydować, czy proponowanie podpowiedzi jest możliwe i sensowne.
