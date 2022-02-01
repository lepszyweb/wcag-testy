### Element {0} z rolą WAI-ARIA `presentation` lub `none` ma element(y) i atrybut(y) strukturalny(e) {1}

Elementy tabeli z `role=presentation` lub `role=none` nie powinny mieć strukturalnych elementów lub atrybutów

### Dlaczego to jest ważne

Technologie wspomagające wykorzystują elementy strukturalne (`<th>`, `<caption>`) i atrybuty (`summary`, `scope`, `header`), aby pomóc użytkownikom w nawigacji i zrozumieniu tabel danych. Włączenie tych funkcji do tabelu powoduje, że cel tabeli jest niejasny.

### Na kogo to wpływa

- Osoby niewidome korzystające z czytników ekranu
- Osoby słabowidzące korzystające z czytników ekranu

### Co zrobić

- Jeśli tabela jest tabelą danych, usuń atrybut `role`;
- jeśli tabela jest używana do rozmieszczenia elementów, użyj zamiast tego układów opartych na CSS;
- LUB, jeśli musi być zastosowana tabela układu, usuń elementy, `<th>`, `<caption>` oraz atrybuty `summary`, `scope` lub `header` z elementów `<td>`.
 

### O tym wymaganiu

[1.3.1 Informacje i relacje]()
[Technika WCAG 2.1 F46](https://www.w3.org/WAI/WCAG21/Techniques/failures/F46)
[Technika WCAG 2.1 F92](https://www.w3.org/WAI/WCAG21/Techniques/failures/F92)

