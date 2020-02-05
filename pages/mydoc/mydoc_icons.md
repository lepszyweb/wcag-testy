---
title: Icons
tags: [formatting]
keywords: font icons, buttons, images, vectors, font awesome, glyphicons
last_updated: July 16, 2016
summary: "Możesz zintegrować ikony czcionek za pomocą bibliotek Font Awesome i Glyphical Halflings. Te biblioteki umożliwiają osadzanie ikon w ich bibliotekach dostarczonych jako odnośnik do linku. Nie potrzebujesz żadnych bibliotek obrazów pobranych do twojego projektu."
sidebar: mydoc_sidebar
permalink: mydoc_icons.html
folder: mydoc
---

## Opcje fontów ikonicznych
Motyw ma zintegrowane dwa zestawy ikon czcionek: Font Awesome i Glyphicons Halflings. Ten ostatni jest częścią Bootstrap, podczas gdy ten pierwszy jest niezależny. Ikony czcionek pozwalają wstawiać ikony narysowane jako wektory z CDN (więc nie masz żadnych lokalnych obrazów na swojej stronie).

## Ikony zewnętrzne

Kiedy link do strony zewnętrznej, takiej jak [Jekyll](http://jekyllrb.com), po linku pojawi się ikona. Jeśli chcesz usunąć tę ikonę, skomentuj ten styl w pliku css / customstyles.css.

```css
/* ta część dodaje ikonę po każdym zewnętrznym linku, używajac, using FontAwesome*/
a[href^="http://"]:after, a[href^="https://"]:after {
    content: "\f08e";
    /*font-family: FontAwesome;
    font-weight: normal;*/
    content: '\e164';
    font-family: Glyphicons Halflings;		
    font-style: normal;
    display: inline-block;
    text-decoration: none;
    padding-left: 3px;
}
```

{% include note.html content="Uwaga, zastąpione Glyphicons." %}

## See Font Awesome icons available

Zobacz dostępne ikony w  [bibliotece Font Awesome](http://fortawesome.github.io/Font-Awesome/icons/).

Ikony Font Awesome pozwalają dostosować ich rozmiar, po prostu dodając `fa-2x`, `fa-3x` tak dalej, jako klasę do ikony, aby dopasować ich rozmiar do dwukrotności lub trzykrotności oryginalnego rozmiaru. Jako ikony wektorowe skalują się wyraźnie w dowolnym rozmiarze.

Oto przykład powiększania ikony kamery:

```html
<i class="fa fa-camera-retro"></i> normal size (1x)
<i class="fa fa-camera-retro fa-lg"></i> fa-lg
<i class="fa fa-camera-retro fa-2x"></i> fa-2x
<i class="fa fa-camera-retro fa-3x"></i> fa-3x
<i class="fa fa-camera-retro fa-4x"></i> fa-4x
<i class="fa fa-camera-retro fa-5x"></i> fa-5x
```

Oto, co renderują:

<i class="fa fa-camera-retro"></i> 1x
<i class="fa fa-camera-retro fa-lg"></i> fa-lg
<i class="fa fa-camera-retro fa-2x"></i> fa-2x
<i class="fa fa-camera-retro fa-3x"></i> fa-3x
<i class="fa fa-camera-retro fa-4x"></i> fa-4x
<i class="fa fa-camera-retro fa-5x"></i> fa-5x


Dzięki Font Awesome zawsze używasz  znacznika `i` z odpowiednią klasą. Najpierw implementujesz `fa` jako klasę podstawową. Możesz używać Font Awesome w innych elementach. Tutaj używam klasy Font Awesome wewnątrz alertu Bootstrap:

```html
<div class="alert alert-danger" role="alert"><i class="fa fa-exclamation-circle"></i> <b>Ostrzeżenie: </b>To jest specjalny komunikat ostrzegawczy.
```

Poniżej jest rezultat:

<div class="alert alert-danger" role="alert"><i class="fa fa-exclamation-circle fa-lg"></i> To jest specjalny komunikat ostrzegawczy.</div>

Notatki, porady, ostrzeżenia itp. Są wstępnie zakodowane w programie Font Awesome i przechowywane w pliku alerts.yml. Plik ten obejmuje następujące elementy:

{% raw %}
```yaml
tip: '<div class="alert alert-success" role="alert"><i class="fa fa-check-square-o"></i> <b>Tip: </b>'
note: '<div class="alert alert-info" role="alert"><i class="fa fa-info-circle"></i> <b>Note: </b>'
important: '<div class="alert alert-warning" role="alert"><i class="fa fa-warning"></i> <b>Important: </b>'
warning: '<div class="alert alert-danger" role="alert"><i class="fa fa-exclamation-circle"></i> <b>Warning: </b>'
end: '</div>'

callout_danger: '<div class="bs-callout bs-callout-danger">'
callout_default: '<div class="bs-callout bs-callout-default">'
callout_primary: '<div class="bs-callout bs-callout-primary">'
callout_success: '<div class="bs-callout bs-callout-success">'
callout_info: '<div class="bs-callout bs-callout-info">'
callout_warning: '<div class="bs-callout bs-callout-warning">'

hr_faded: '<hr class="faded"/>'
hr_shaded: '<hr class="shaded"/>'
```
{% endraw %}

Oznacza to, że możesz wstawić wskazówkę, notatkę, ostrzeżenie lub ważny alert, używając tych tagów.


```liquid
{% raw %}{% include note.html content="Dodaj tutaj swoją uwagę." %}{% endraw %}
```


```liquid
{% raw %}{% include tip.html content="Dodaj tutaj swoją poradę." %}{% endraw %}
```


```liquid
{% raw %}{% include important.html content="Dodaj tu informację uzupełniajacą." %}{% endraw %}
```


{% raw %}
```liquid
{% include warning.html content="Dodaj tu ostrzeżenie." %}
```
{% endraw %}

Oto wynik:

{% include note.html content=" Dodaj swoją notatkę tutaj." %}

{% include tip.html content="Tu jest porada" %}

{% include important.html content="To jest ważna informacja." %}

{% include warning.html content="Jeśli to przeoczysz, możesz umrzeć." %}

Schemat kolorów to domyślne kolory z Bootstrap. W razie potrzeby możesz modyfikować ikony lub kolory.

## Tworzenie własnych kombinacji

Możesz wprowadzać innowacje dzięki własnym kombinacjom. Oto podobne podejście z ikoną pobierania pliku:

```html
<div class="alert alert-success" role="alert"><i class="fa fa-download fa-lg"></i> To specjalna wskazówka na temat pliku do pobrania....</div>
```

A wynik::

<div class="alert alert-success" role="alert"><i class="fa fa-download fa-lg"></i> To specjalna wskazówka na temat pliku do pobrania....</div>


Weź właściwą nazwę klasy z biblioteki  [Font Awesome library](http://fortawesome.github.io/Font-Awesome/icons/), a następnie zaimplementuj ją, postępując zgodnie z pokazanym wcześniej wzorem.

Jeśli chcesz, aby Twoje czcionki były jeszcze większe niż styl 5x, dodaj niestandardowy styl do swojego arkusza stylów w następujący sposób:

```css
.fa-10x{font-size:1700%;}
```

Wtedy dowolny element z atrybutem `fa-10x` zostanie powiększony o 1700%.


## Dostępne ikony glifikonu

Glifikony działają podobnie do Font Awesome. Przejdź do [biblioteki Glyphicons](http://getbootstrap.com/components/#glyphicons), aby zobaczyć dostępne ikony.

Chociaż biblioteka Glyphicon Halflings nie zapewnia skalowalnych klas, takich jak Font Awesome, istnieje[sztuczka StackOverflow](http://stackoverflow.com/questions/24960201/how-do-i-make-glyphicons-bigger-change-size), która sprawia, że ​​ikony zachowują się w podobny sposób. Arkusz stylów tego motywu (customstyles.css) zawiera następujące elementy do arkusza stylów:



```css
.gi-2x{font-size: 2em;}
.gi-3x{font-size: 3em;}
.gi-4x{font-size: 4em;}
.gi-5x{font-size: 5em;}
```

Teraz wystarczy dodać `gi-5x` lub cokolwiek, aby zmienić rozmiar ikony czcionki:

```html
<span class="glyphicon glyphicon-globe gi-5x"></span>
```

A oto wynik::

<span class="glyphicon glyphicon-globe gi-5x"></span>

Glypikony używają elementu `span` zamiast `i` aby dołączać swoje klasy.

Oto inny przykład:



```html
<span class="glyphicon glyphicon-download"></span>
```

<span class="glyphicon glyphicon-download"></span>

I powiększony:

```html
<span class="glyphicon glyphicon-download gi-3x"></span>
```

<span class="glyphicon glyphicon-download gi-3x"></span>

Możesz także umieścić glifiki w innych elementach::

```html
<div class="alert alert-danger" role="alert">
  <span class="glyphicon glyphicon-exclamation-sign" aria-hidden="true"></span>
  <b>Błąd:</b> Wprowadź prawidłowy adres e-mail

</div>
```

<div class="alert alert-danger" role="alert">
  <span class="glyphicon glyphicon-exclamation-sign" aria-hidden="true"></span>
  <b>Błąd:</b> Wprowadź prawidłowy adres e-mail
</div>

## Objaśnienia

Wcześniej wyświetlane alerty mogą być odpowiednie dla krótkich wiadomości, ale w przypadku dłuższych notatek jednolity kolor zajmuje trochę miejsca. W tym temacie masz również opcję używania objaśnień, które są dość powszechne w dokumentacji Bootstrap, ale zaskakująco nie są oferowane jako wyraźny element. Ich style zostały skopiowane do tego motywu w sposób podobny do alertów:


```html
<div class="bs-callout bs-callout-info">
 To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. </div>
```

<div class="alert alert-info" role="alert"><span class="glyphicon glyphicon-question-sign"></span> To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. To jest specjalna wiadomość informacyjna. </div>

A oto krótki kod:

{% raw %}
```
{{site.data.alerts.callout_info}To jest specjalny komunikat informacyjny.{{site.data.alerts.end}}
{% endraw %}
```

Oto wynik:

{{site.data.alerts.callout_info}}To jest specjalny komunikat informacyjny.{{site.data.alerts.end}}

Możesz użyć dowolnego z poniższych:
{% raw %}
```
{{site.data.alerts.callout_default}}
{{site.data.alerts.callout_primary}}
{{site.data.alerts.callout_success}}
{{site.data.alerts.callout_info}}
{{site.data.alerts.callout_warning}}
```
{% endraw %}

Jedyną różnicą jest kolor lewego paska.

Objaśnienia zostały wyjaśnione bardziej szczegółowo w [Alerty][mydoc_alerts].

{% include links.html %}
