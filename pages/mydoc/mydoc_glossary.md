---
title: Układ glosariusza
tags: [formatting, special_layouts]
keywords: definitions, glossaries, terms, style guide
last_updated: July 3, 2016
summary: "Twoja strona glosariusza może korzystać z definicji zapisanych w pliku danych. Daje to możliwość ponownego użycia tej samej definicji w wielu miejscach. Dodatkowo, możesz użyć klas Bootstrap do ułożenia listy definicji w poziomie."
sidebar: mydoc_sidebar
permalink: mydoc_glossary.html
toc: false
folder: mydoc
---


Możesz stworzyć glosariusz dla swoich treści. Najpierw stwórz swój glosariusz w pliku danych, takim jak glosariusz.yml.

Następnie stwórz stronę i użyj formatowania listy definicji, jak to opisano powyżej:

a11y
: {{site.data.glossary.a11y}}

afordancje
: {{site.data.glossary.afordancje}}

audio
: {{site.data.glossary.audio}}

ATAG
: {{site.data.glossary.ATAG}}

blok tekstu
: {{site.data.glossary.blok_tekstu}}

sztuka tekstowa
: {{site.data.glossary.sztuka_tekstowa}}

Oto kod:

```
{% raw %}a11y
: {{site.data.glossary.a11y}}

afordancje
: {{site.data.glossary.afordancje}}

audio
: {{site.data.glossary.audio}}

ATAG
: {{site.data.glossary.ATAG}}

blok_tekstu
: {{site.data.glossary.blok_tekstu}}

sztuka tekstowa
: {{site.data.glossary.sztuka_tekstowa}}

cel łącza
: {{site.data.glossary.cel_lacza}}

{% endraw %}

```

Słowniczek działa dobrze jako link w górnym pasku nawigacyjnym.

## Poziomo stylizowane listy definicji

Można również zmienić klasę listy definicji (dl) na dl-horizontal. Jest to klasa specyficzna dla Bootstrap. Jeśli to zrobisz, stylizacja wygląda tak:



<dl class="dl-horizontal">

<dt id="a11y">a11y</dt>
<dd>{{site.data.glossary.a11y}}</dd>

<dt id="afordancje">afordancje</dt>
<dd>{{site.data.glossary.afordancje}}</dd>


<dt id="audio">audio</dt>
<dd>{{site.data.glossary.audio}}</dd>

<dt id="ATAG">ATAG</dt>
<dd>{{site.data.glossary.ATAG}}</dd>

<dt id="blok_tekstu">blok tekstu</dt>
<dd>{{site.data.glossary.blok_tekstu}}</dd>

<dt id="sztuka_tekstowa">sztuka tekstowa</dt>
<dd>{{site.data.glossary.sztuka_tekstowa}}</dd>

<dt id="cel_lacza">cel łącza</dt>
<dd>{{site.data.glossary.cel_lacza}}</dd>


</dl>

Dla tego typu listy, musisz użyć HTML. Lista wyglądałaby wtedy tak:

```html
{% raw %}<dl class="dl-horizontal">

<dt id="a11y">a11y</dt>
<dd>{{site.data.glossary.a11y}}</dd>

<dt id="afordancje">afordancje</dt>
<dd>{{site.data.glossary.afordancje}}</dd>

<dt id="audio">audio</dt>
<dd>{{site.data.glossary.audio}}</dd>

<dt id="ATAG">ATAG</dt>
<dd>{{site.data.glossary.ATAG}}</dd>

<dt id="blok tekstu">blok_tekstu</dt>
<dd>{{site.data.glossary.blok_tekstu}}</dd>

<dt id="sztuka_tekstowa">sztuka_tekstowa</dt>
<dd>{{site.data.glossary.sztuka_tekstowa}}</dd>

<dt id="cel_lacza">cel łącza</dt>
<dd>{{site.data.glossary.cel_lacza}}</dd>

</dl>{% endraw %}

```

Jeśli zgnieciesz swój ekran wystarczająco mały, w pewnym momencie ten styl wraca do zwykłej klasy `dl`.

Chociaż podoba mi się widok "side-by-side" dla krótszych definicji, uważam, że jest on problematyczny z dłuższymi definicjami.


{% include links.html %}
