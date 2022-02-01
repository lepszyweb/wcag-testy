### Element `<caption>` nie jest zagnieżdżony w elemencie `<table>`

Element `<caption>` musi być umieszczony wewnątrz powiązanego elementu `<table>`

### Dlaczego to jest ważne?

Element `<caption>` jest identyfikatorem i działa jak tytuł lub nagłówek tabeli. Umożliwia czytnikom ekranu przejście bezpośrednio do napisu, aby uzyskać opis tabeli.

### Kogo to dotyczy?

- Osoby niewidome korzystające z czytników ekranu
 
### Co zrobić

- Umieść element `<caption>` wewnątrz elementu `<table>`.

Na przykład:

``` html
<table id="data_table1" border="1" summary="Prosta tabela danych przedstawiająca liczbę chłopców i dziewcząt w każdej klasie szkoły podstawowej">
        <caption>Dziewczęta i chłopcy w klasach szkół podstawowych</caption>
        <tr> ... </tr>
        <tr> ... </tr>
</table>
```

### O tym wymaganiu

[1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
[Techniki WCAG 2.1 - Technika H39](https://www.w3.org/WAI/WCAG21/Techniques/html/H39)