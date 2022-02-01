### Złożona tabela danych nie ma 'summary' lub 'aria-describedby', które daje przegląd tabeli

Złożone tabele danych powinny mieć `summary` lub `aria-describedby`, które daje przegląd tabeli

### Dlaczego to jest ważne

Podsumowanie tabeli zawiera krótkie omówienie sposobu zorganizowania danych w tabeli danych i jest szczególnie przydatne, gdy tabela jest duża i zawiera wiele wierszy i kolumn lub gdy tabela ma złożoną strukturę (wiele nagłówków wierszy lub kolumn). Podsumowanie tabeli nie powinno treści podpisu tabeli.

### Na kogo to wpływa

- Osoby niewidome korzystające z czytników ekranu
- Osoby słabowidzące korzystające z czytników ekranu

### Co zrobić

- Dodaj atrybut `aria-labelledby` do elementu `<table>`. Atrybut `aria-labelledby` musi wskazywać na element, w którym znajduje się widoczny na stronie tekst, opisujący organizację danych w tabeli (podsumowujący tabelę)
- lub  dodaj atrybut `aria-describedby`, aby zapewnić krótki przegląd tabeli danych;
- lub dodaj atrybut `aria-label`, aby zapewnić krótki przegląd tabeli danych.

Uwaga: w HTML5 atrybut `summary` jest przestarzały i należy go unikać.

Na przykład, w poniższym przykładzie przedstawiono podsumowanie tabeli, korzystając z atrybutu `aria-labelledby`:

``` html
<p id="tblSummary">The following table shows the number of boys and girls in each grade of an elementary school.</p>
    
    <table border="1" aria-labelledby="tblSummary">
     <tr>
       <th id="klasa">Klasy</th>
       <th id="nauczyciel">Nauczyciel</th>
       <th id="chlopcy"># chłopców</th>
       <th id="dziewczeta"># dziewcząt</th>
     </tr>
     <tr>
       <th rowspan="2" id="1klasa">1. klasa</th>
        <th headers="1klasa nauczyciel" id="mgrKowalski">mgr Kowalski</th>
        <td headers="1klasa mgrKowalski chlopcy">5</td>
        <td headers="1klasa mgrKowalski dziewczeta">4</td>
     </tr>
    ...
   </table>
 ```  

### O tym wymaganiu

[IBM 1.3.1 Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content)
[Techniki WCAG 2.1 - Technika HTML H73](https://www.w3.org/WAI/WCAG21/Techniques/html/H73)

