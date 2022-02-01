### Element `<table>` ma pusty element `<caption>`

Element `<caption>` w elemencie `<table>` musi zawierać opisowy tekst 

### Dlaczego to jest ważne?

Element `<caption>` jest identyfikatorem i działa jak tytuł lub nagłówek tabeli. Umożliwia czytnikom ekranu przejście bezpośrednio do napisu, aby uzyskać opis tabeli.

### Kogo to dotyczy?

- Osoby niewidome korzystające z czytników ekranu


### Co zrobić

- Dodaj tekst opisowy do elementu `<caption>`.

Na przykład:

``` html
<table id="data_table1" border="1">
<caption>Dziewczęta i chłopcy w klasach szkół podstawowych</caption>
	<tr>
		<th scope="col">Klasy</th>
		<th scope="col"># dziewcząt</th>
		<th scope="col"># chłopców</th>
	</tr>
</table>
```

### O tym wymaganiu

[1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
[Techniki WCAG 2.1 - Technika H39](https://www.w3.org/WAI/WCAG21/Techniques/html/H39)


