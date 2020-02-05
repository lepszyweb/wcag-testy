---
title: Alerty
tags: [formatting]
keywords: notes, tips, cautions, warnings, admonitions
last_updated: July 3, 2016
summary: "Do treści możesz wstawiać notatki, wskazówki, ostrzeżenia i ważne alerty. Te notatki wykorzystują styl Bootstrap i są dostępne w odnośnikach danych, takich jak site.data.alerts.note."
sidebar: mydoc_sidebar
permalink: mydoc_alerts.html
folder: mydoc
---

## O alertach

Alerty to małe ostrzeżenia, informacje lub inne wiadomości, które wywołałeś w specjalnym formacie. Aby użyć tych alertów lub objaśnień, odwołaj się do odpowiedniej wartości przechowywanej w pliku alerts.yml, jak opisano w poniższych sekcjach.



## Alerty

Podobnie jak [w przypadku wstawiania obrazów][mydoc_images], możesz wstawiać alerty za pośrednictwem różnych opracowanych dodatków. Obejmują one szablony, za pomocą których przekazujesz parametry, aby łatwo wypełnić właściwy kod HTML.

```
{%raw%}{% include note.html content="To jest moja notatka. Cała treść, którą tu piszę, jest traktowana jako pojedynczy akapit." %}{% endraw%}
```

Oto wynik:

{% include note.html content="To jest moja notatka. Cała treść, którą tu piszę, jest traktowana jako pojedynczy akapit." %}

W przypadku alertów dostępna jest tylko jedna właściwość:

| Właściwość | Opis |
|-------|--------|
| content | Treść alertu. |

## Używanie znaczników poziomu bloków wewnątrz alertów {#blockleveltags}

Jeśli potrzebujesz wielu akapitów, użyj znaczników `<br/><br/>`. Wynika to z faktu, że tagi blokowe nie są tutaj dozwolone, ponieważ Kramdown przetwarza zawartość jako Markdown, mimo że zawartość jest otoczona tagami HTML. Oto przykład z przerwą:

```
{%raw%}{% include note.html content="To jest moja notatka. Cała treść, którą tu piszę, jest traktowana jako pojedynczy akapit.. <br/><br/> Teraz piszę w nowej linii." %}{% endraw%}
```

Oto wynik:

{% include note.html content="To jest moja notatka. Cała treść, którą tu piszę, jest traktowana jako pojedynczy akapit. <br/><br/> Teraz piszę w nowej linii." %}

To włączenie używa atrybutu  markdown="span", co oznacza, że ​​kramdown przetworzy całość `content` jako element `span`. Nie można używać elementów blokowych takich jak `p`, `div` lub `pre`. Jeśli potrzebujesz tych elementów, możesz ręcznie otoczyć zawartość kodem HTML z dołączenia lub możesz użyć tych tagów:

```
{% raw %}{{site.data.alerts.note}}
<p>To jest moja uwaga.</p>
<pre>
def foo(x):<br>
&nbsp;&nbsp;&nbsp;&nbsp;return x+1
</pre>
{{site.data.alerts.end}}{% endraw %}
```

**Wynik::**

{{site.data.alerts.note}}
<p>To jest moja uwaga.</p>
<pre>
def foo(x):<br>
&nbsp;&nbsp;&nbsp;&nbsp;zwróci x+1
</pre>
{{site.data.alerts.end}}

Ten sam kod Bootstrap dla alertu jest przechowywany w plikach yaml w folderze _data. (W ten sposób wcześniej zaimplementowałem ten kod, ale ponieważ ta metoda była podatna na błędy i nie wyzwalała żadnych ostrzeżeń kompilacji lub błędów, gdy została nieprawidłowo zakodowana, zmieniłem zamiast tego metodę użycia.

## Dostępne typy alertów

Istnieją cztery rodzaje alertów, które możesz wykorzystać:

* note.html
* tip.html
* warning.html
* important.html

Działają tak samo, ale mają inny kolor, ikonę i słowo ostrzegawcze. Możesz włączyć do treści różne typy alertów, wybierając odpowiedni szablon dołączania. Oto przykłady każdego alertu:

{% include note.html content="To jest uwaga." %}

{% include tip.html content="To jest wskazówka." %}

{% include warning.html content="To jest ostrzeżenie." %}

{% include important.html content="To jest ważna informacja." %}

Mechanizm obsługi alarmów obejmuje przechowywanie w folderze  \_include. Opcja `content` jest parametrem przekazywanym do dołączenia. W dołączeniu parametr jest przekazywany w następujący sposób:


```
{% raw %}<div markdown="span" class="alert alert-info" role="alert"><i class="fa fa-info-circle"></i> <b>Uwaga:</b> {{include.content}}{% endraw %}</div>
```

Treść w `content="To jest uwaga."` zostanie wstawiona do części szablonu `{% raw %}{{include.content}}}{% endraw %}`. Możesz zastosować ten sam wzorzec, aby zbudować dodatkowe dołączenia. Zobacz ten [screencast Jekyll](http://jekyll.tips/jekyll-casts/includes/) lub [ten screencast](https://www.youtube.com/watch?v=TJcn_PJ2100), aby uzyskać więcej informacji.

## Objaśnienia

Dostępny jest też inny rodzaj objaśnień, zwany objaśnieniami. Ten format jest zwykle używany w przypadku dłuższych objaśnień obejmujących więcej niż jeden lub dwa akapity, ale tak naprawdę to tylko stylistyczna preferencja, czy używać alertu, czy objaśnień.

Oto składnia objaśnienia:

```
{% raw %}{% include callout.html content="To jest moje objaśnienie. Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type. Zazwyczaj używam tego stylu objaśnień, gdy mam więcej informacji, które chcę udostępnić, często obejmujących wiele akapitów. " type="primary" %} {% endraw %}
```

Oto wynik:

{% include callout.html content="To jest moje objaśnienie. Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type. Zazwyczaj używam tego stylu objaśnień, gdy mam więcej informacji, które chcę udostępnić, często obejmujących wiele akapitów." type="primary" %}

Dostępne właściwości objaśnień są następujące:

| Właściwość | opis |
|-------|--------|
| content | The content for the callout. |
| type | Styl objaśnienia. Dostępne są następujące opcje `danger`, `default`, `primary`, `success`, `info`, and `warning`.|

Typy po prostu określają kolor lewej krawędzi. Każdy z tych typów objaśnień jest wstawiany jako nazwa klasy w szablonie objaśnień. Te nazwy klas odpowiadają stylom w Bootstrap. Klasy te są popularnymi nazwami klas Bootstrap, których atrybuty stylu różnią się w zależności od motywu Bootstrap i definicji stylu.

Oto przykład każdego rodzaju objaśnienia:

{% include callout.html content="To jest objaśnienie typu **danger** (zagrożenie). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="danger" %}

{% include callout.html content="To jest objaśnienie typu **default** (domyślny). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="default" %}

{% include callout.html content="To jest objaśnienie typu **primary** (podstawowy). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="primary" %}

{% include callout.html content="To jest objaśnienie typu **success** (powodzenie). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="success" %}

{% include callout.html content="To jest objaśnienie typu **info**  (informacja). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="info" %}

{% include callout.html content="To jest objaśnienie typu **warning**  (ostrzeżenie). Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type." type="warning" %}

Teraz, w przeciwieństwie do alertów, objaśnienia nie zawierają słowa alertu (uwaga, wskazówka, ostrzeżenie lub ważne). Jeśli chcesz, musisz ręcznie umieścić go w środku `content`.

Aby uwzględnić podziały akapitów wewnątrz objaśnienia, użyj `<br/><br/>`


```
{% raw %}{% include callout.html content="**Ważna informacja**: To jest moje objaśnienie. Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type. Zazwyczaj używam tego stylu objaśnień, gdy mam więcej informacji, które chcę udostępnić, często obejmujących wiele akapitów. <br/><br/>Tutaj zaczynam nowy akapit, ponieważ mam wiele informacji do przekazania. Możesz się zastanawiać, dlaczego używam podziałów linii zamiast znaczników akapitu. Jest tak, ponieważ Kramdown przetwarza tutaj Markdown jako `span`, a nie 'div' (z jakiegoś powodu). Bądź wdzięczny, że możesz używać Markdown w ogóle w HTML. Zwykle nie jest to dozwolone w składni Markdown, ale jest dozwolone tutaj." type="primary" %} {% endraw %}
```

Oto wynik:

{% include callout.html content="**Ważna informacja**: To jest moje objaśnienie. Ma po lewej stronie ramkę, której kolor określasz, przekazując parametr type. Zazwyczaj używam tego stylu objaśnień, gdy mam więcej informacji, które chcę udostępnić, często obejmujących wiele akapitów. <br/><br/>Tutaj zaczynam nowy akapit, ponieważ mam wiele informacji do przekazania. Możesz się zastanawiać, dlaczego używam podziałów linii zamiast znaczników akapitu. Jest tak, ponieważ Kramdown przetwarza tutaj Markdown jako `span`, a nie 'div' (z jakiegoś powodu). Bądź wdzięczny, że możesz używać Markdown w ogóle w HTML. Zwykle nie jest to dozwolone w składni Markdown, ale jest dozwolone tutaj." type="primary" %}


## Użyj zmiennych Liquid w parametrach z włączeniami

Załóżmy, że masz nazwę produktu lub inną właściwość, którą przechowujesz jako zmienną w pliku konfiguracyjnym (\_config.yml) i chcesz użyć tej zmiennej w parametrze `content` dla alertu lub objaśnienia. Błąd pojawi się, jeśli użyjesz składni Liquid w parametrze include. Na przykład ta składnia spowoduje błąd:

```
{%raw%}{% include note.html content="{{site.company}} ma przyjemność ogłosić nadchodzącą premierę." %}{%endraw%}
```

Błąd powie coś takiego:

```
Liquid Exception: Invalid syntax for include tag. File contains invalid characters or sequences: ... Valid syntax: {%raw%}{% include file.ext param='value' param2='value' %}{%endraw%}
```

Aby użyć zmiennych w parametrach dołączania, musisz zastosować podejście „parametru zmiennego”. Najpierw użyj znacznika `capture`, aby przechwycić część treści. Następnie odwołujesz się do tego przechwyconego tagu w swoim dołączeniu. Oto przykład.


W moim pliku konfiguracji witryny (\_congfig.yml), mam właściwość o nazwie `company_name`.

```yaml
company_name: Nazwa Twojej firmy
```

Chcę użyć tej zmiennej w mojej dołączonej notatce.

Po pierwsze, przed notatką przechwytuję treść notatek:


```liquid
{%raw%}{% capture company_note %} {{site.company_name}} ma przyjemność ogłosić nadchodzącą premierę.{% endcapture %}{%endraw%}
```

Teraz odwołujesz się do `company_note` w parametrze `include` jak poniżej:

```
{%raw%}{% include note.html content=company_note}{%endraw%}
```
Oto wynik:

{% capture company_note %}The {{site.company_name}} ma przyjemność ogłosić nadchodzącą premierę.{% endcapture %}
{% include note.html content=company_note %}

Zwróć uwagę na pominięcie cudzysłowów ze zmiennymi parametrami.


Pamiętaj również, że zamiast przechowywać zmienną w pliku konfiguracyjnym witryny, możesz również umieścić zmienną w nagłówku strony (frontmatter). Następnie zamiast używać `{%raw%}{{site.company_name}}{%endraw%}`, `{%raw%}{{page.company_name}}{%endraw%}`.


## Markdown w objaśnieniach i alertach

Możesz używać Markdown w objaśnieniach i alertach, nawet jeśli ta zawartość jest faktycznie wstawiana do HTML w dołączeniu. Jest to jedna z zalet kramdown Markdown. Szablon dołączania ma atrybut `markdown="span"`, który pozwala procesorowi analizować Markdown wewnątrz HTML..

## Sprawdzanie poprawności

Jeśli masz część składni niepoprawną w przypadku alertu lub objaśnienia, zobaczysz błąd, gdy Jekyll będzie próbował zbudować witrynę. Błąd może wyglądać następująco:

```
{% raw %}Liquid Exception: Invalid syntax for include tag: content="This is my **info** type callout. It has a border on the left whose color you define by passing a type parameter. type="info" Valid syntax: {% include file.ext param='value' param2='value' %} in mydoc/mydoc_alerts.md {% endraw %}
```

Te błędy są dobre, ponieważ pozwalają stwierdzić, że w składni wystąpił błąd. Bez błędów możesz nie zdawać sobie sprawy z tego, że kodujesz coś niepoprawnie, dopóki nie zobaczysz braku ostrzeżenia lub stylu objaśnień na wydruku.

W takim przypadku cudzysłowy nie są ustawione poprawnie. Zapomniałem zamykającego cudzysłowu dla parametru content include.

## Wysyłanie ostrzeżenia do użytkowników na każdej stronie

Jeśli chcesz wysyłać ostrzeżenie do użytkowników na każdej stronie, dodaj alert lub objaśnienie do \_layouts/page.html page tuż pod nagłówkiem. Każda strona korzystająca z układu strony (domyślnie wszystkie) wyświetla ten komunikat.

{% include links.html %}
