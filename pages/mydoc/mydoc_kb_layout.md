---
title: Układ bazy wiedzy
tags: [special_layouts]
keywords: knowledge base, support portal, grid, doc portal
last_updated: July 3, 2016
summary: "To pokazuje przykładowy układ bazy wiedzy. Każdy kwadrat może prowadzić do strony archiwum znaczników. W tym przykładzie ikony czcionek z Font Awesome są używane do grafiki, a układ jest pobierany z motywu Modern Business."
sidebar: mydoc_sidebar
permalink: mydoc_kb_layout.html
toc: false
folder: mydoc
---


Oto przykładowy układ stylu bazy wiedzy:


<div class="row">
         <div class="col-lg-12">
             <h2 class="page-header">Kategorie bazy wiedzy</h2>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-tree fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Pierwsze kroki</h4>
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_getting_started.html" class="btn btn-primary">Czytaj więcej</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-car fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Nawigacja</h4>
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_navigation.html" class="btn btn-primary">Czytaj więcej</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-support fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Pojedyncze źródło</h4>
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_single_sourcing.html" class="btn btn-primary">Czytaj więcej</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-database fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Formatowanie</h4>
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_formatting.html" class="btn btn-primary">Czytaj więcej</a>
                 </div>
             </div>
         </div>
</div>


## Generowanie listy wszystkich stron z określonym znacznikiem

Jeśli nie chcesz linkować do indeksu archiwum tagów, ale zamiast tego chcesz wyświetlić listę wszystkich stron, które mają określony tag, możesz użyć tego kodu:

```html
{% raw %}Getting started pages:
<ul>
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
{% for tag in page.tags %}
{% if tag == "getting_started" %}
<li><a href="{{ page.url | remove: "/" }}">{{page.title}}</a></li>
{% endif %}
{% endfor %}
{% endfor %}
</ul>{% endraw %}
```

Oto wynik:

Tworzymy pierwsze strony:

<ul>
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
{% for tag in page.tags %}
{% if tag == "getting_started" %}
<li><a href="{{ page.url | remove: "/"}}">{{page.title}}</a></li>
{% endif %}
{% endfor %}
{% endfor %}
</ul>

{% include links.html %}
