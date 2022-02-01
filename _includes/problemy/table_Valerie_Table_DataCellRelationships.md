### Element `<th>` lub `<td>` nie jest skojarzony za pomocą `header` lub `scope`

W złożonej tabeli danych wszystkie elementy <th> i <td> muszą być powiązane za pomocą atrybutów „header” lub „scope”.

### Dlaczego to jest ważne


Nawigacja po komórce poprzez złożoną tabelę danych jest szczególnie trudna, gdy użytkownicy muszą szukać znaczenia każdej komórki. Użycie atrybutów `id` i `header` wychwytuje złożone relacje między komórkami danych a komórkami nagłówkowymi, które mogą być następnie przekazywane użytkownikom, wspierając wydajną nawigację po tabeli.

### Na kogo to wpływa

- Osoby niewidome korzystające z czytników ekranu
- Osoby słabowidzące korzystające z powiększalników ekranu

### Co zrobić

- Jeśli to nie jest tabela danych (brak danych relacyjnych), do rozplanowania treści użyj CSS zamiast elementu `<table>` (wysoce zalecane);
- lub, określ tabelę jako układ za pomocą `role="presentation"` lub `role="none"`;
- lub, gdy jest to tabela danych, użyj atrybutów `id`, aby podać identyfikatory dla komórek nagłówków (np. `<th id="szkola">`);
- oraz  użyj atrybutu `headers` w komórkach danych, aby określić odpowiednie komórki nagłówka (np. `<td headers="szkola nauczyciel poziom">`).

### O tym wymaganiu

[1.3.1 Informacje i relacje]()()
[WCAG 2.1 technique H43](https://www.w3.org/WAI/WCAG21/Techniques/html/H43)


