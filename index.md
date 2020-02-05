---
title: "Rozpoczęcie pracy z motywem dokumentacji dla Jekyll"
keywords: sample homepage
tags: [getting_started]
sidebar: mydoc_sidebar
permalink: index.html
summary: Te krótkie instrukcje pomogą Ci szybko rozpocząć pracę z tematem. Pozostałe tematy w tej pomocy zawierają dodatkowe informacje i szczegółowe informacje na temat pracy z innymi aspektami tego tematu i Jekyll..
---

{% include note.html content="Jeśli klonujesz ten motyw, prawdopodobnie piszesz jakieś dokumenty. Mam tutaj blog poświęcony pisaniu technicznemu, który nazywa się <a alt='technical writing blog' href='http://idratherbewriting.com'>I'd Rather Be Writing</a>. Jeśli chcesz być na bieżąco z najnowszymi trendami, najlepszymi praktykami i innymi metodami pisania dokumentacji, rozważ <a href='https://tinyletter.com/tomjoht'>subskrypcję</a>. Mam też stronę poświęconą <a href='http://idratherbewriting.com/learnapidoc'>pisaniu dokumentacji API</a>." %}

## Zbuduj motyw

Postępuj zgodnie z tymi instrukcjami, aby zbudować motyw.

### 1. Download the theme

Najpierw pobierz lub sklonuj motyw z [repozytorium Github](https://github.com/tomjoht/documentation-theme-jekyll). Najprawdopodobniej nie będziesz pobierał aktualizacji po rozpoczęciu dostosowywania motywu, więc pobranie motywu (zamiast klonowania) prawdopodobnie ma sens. W Github kliknij przycisk **Clone or download**, a następnie kliknij **Download ZIP**.



### 2. Zainstaluj Jekyll

Jeśli nigdy nie zainstalowałeś lub nie uruchomiłeś witryny Jekyll lokalnie na twoim komputerze, postępuj zgodnie z tymi instrukcjami, aby zainstalować Jekyll:

* [Zainstaluj Jekyll na Macu][mydoc_install_jekyll_on_mac]
* [Zainstaluj Jekyll w systemie Windows][mydoc_install_jekyll_on_windows]


### 3. Zainstaluj pakiet

Jeśli nie zainstalowałeś Bundlera, zainstaluj go:

```
gem install bundler
```

Będziesz chciał, aby [Bundler](http://bundler.io/) upewnił się, że wszystkie potrzebne klejnoty (gemy) Ruby działają dobrze z twoim projektem. Bundler rozwiązuje zależności i instaluje brakujące klejnoty lub dopasowuje klejnoty do odpowiednich wersji w oparciu o zależności klejnotów.

### 4. Opcja 1: zbuduj motyw (*bez klejnotu* na stronach github) {#opcja1}

Użyj tej opcji, jeśli nie planujesz publikować swojej witryny Jekyll przy użyciu [stron Github](https://pages.github.com/).

Gemfile Bundlera określa sposób zarządzania zależnościami projektu. Chociaż ten projekt zawiera Gemfile, ten motyw nie ma żadnych zależności poza podstawowym Jekyll. Gemfile służy do wyświetlania listy klejnotów potrzebnych do publikowania na stronach Github.  **Jeśli nie planujesz, aby strony Github tworzyły projekt Jekyll, usuń te dwa pliki z katalogu głównego kompozycji:**

* Gemfile
* Gemfile.lock

Jeśli nigdy nie korzystałeś z Jekyll na swoim komputerze (możesz to sprawdzić jekyll --version), być może będziesz musiał zainstalować klejnot Jekyll:

```
gem install jekyll
```

Teraz uruchom usługę jekyll służyć (najpierw zmień katalogi (`cd`) do miejsca, do którego pobrałeś projekt):

```
jekyll serve
```

### 4. Option 2: Build the Theme (*with* the github-pages gem) {#option2}

If you *are* in fact publishing on Github Pages, leave the Gemfile and Gemfile.lock files in the theme.The Gemfile tells Jekyll to use the github-pages gem. **However, note that you cannot use the normal `jekyll serve` command with this gem due to dependency conflicts between the latest version of Jekyll and Github Pages** (which are noted [briefly here](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)).

You need Bundler to resolve these dependency conflicts. Use Bundler to install all the needed Ruby gems:

```
bundle update
```

Then *always* use this command to build Jekyll:

```
bundle exec jekyll serve
```

If you want to shorten this long command, you can put this code in a file such as jekyll.sh (on a Mac) and then simply type `. jekyll.sh` to build Jekyll.

## Running the site in Docker

You can also use Docker to directly build and run the site on your local machine. Just clone the repo and run the following from your working dir:
```
docker-compose build --no-cache && docker-compose up
```
The site should now be running at [http://localhost:4000/](http://localhost:4000/).

This is perhaps the easiest way to see how your site would actually look.

## Skonfiguruj pasek boczny

W tym temacie znajduje się kilka produktów. Każdy produkt używa innego paska bocznego. To jest istota tego, co czyni ten motyw wyjątkowym - różne paski boczne dla różnych dokumentacji produktu. Chodzi o to, że gdy użytkownicy czytają dokumentację dla określonego produktu, nawigacja na pasku bocznym powinna być specyficzna dla tego produktu. (Możesz przeczytać więcej moich przemyśleń na temat tego, dlaczego wiele pasków bocznych jest ważnych w tym [poście na blogu](http://idratherbewriting.com/2016/03/23/release-of-documentation-theme-for-jekyll-50/).)

Górna nawigacja zwykle pozostaje taka sama, ponieważ pozwala użytkownikom nawigować między produktami. Ale nawigacja na pasku bocznym dostosowuje się do produktu.

W nagłówku każdej strony ('frontmatter') musisz określić pasek boczny, którego ma używać ta strona. Oto przykład frontmatter strony pokazujący właściwość paska bocznego:


<pre>
---
title: Alerty
tags: [formaowanie]
keywords: uwagi, porady, przestrogi, ostrzeżenia, napomnienia
last_updated: 3 lipca 2016
summary: "Możesz wstawiać notatki, porady, ostrzeżenia i ważne powiadomienia w swoich treściach, przechowywane jako skróty udostępnione przez linksrefs.hmtl obejmują."
<span class="red">sidebar: mydoc_sidebar</span>
permalink: mydoc_alerts
---
</pre>

Opcja `sidebar: mydoc_sidebar` odnosi się do pliku \_data/sidebars/mydoc_sidebar.yml.

Pamiętaj, że pasek boczny może mieć tylko 2 poziomy (rozwiń opcję **Tag archives**, aby zobaczyć przykład drugiego poziomu). Biorąc pod uwagę, że każdy produkt ma własny pasek boczny, ta głębokość powinna być wystarczająca (to naprawdę 3 poziomy). Głębsze zagnieżdżanie jest sprzeczne z zaleceniami użyteczności.

Opcjonalnie możesz wyłączyć pasek boczny na dowolnej stronie (np. Stronach docelowych). Aby wyłączyć pasek boczny strony, ustaw znacznik frontmatter strony jako `hide_sidebar: true`.

Jeśli nie zadeklarujesz paska bocznego, plik `home_sidebar`  zostanie użyty jako domyślny, ponieważ jest to domyślny parametr określony w pliku konfiguracyjnym `_config.yml`:

```yaml
-
  scope:
    path: ""
    type: "pages"
  values:
    layout: "page"
    comments: true
    search: true
    sidebar: home_sidebar
    topnav: topnav
```

Jeśli chcesz ustawić różne ustawienia domyślne paska bocznego na podstawie różnych folderów dla swoich stron, określ ustawienia domyślne w następujący sposób:

```
-
  scope:
    path: "pages/mydoc"
    type: "pages"
  values:
    layout: "page"
    comments: true
    search: true
    sidebar: mydoc_sidebar
    topnav: topnav
```

Spowoduje to załadowanie pliku `mydoc_sidebar` na wszystkich stronach na stronach **pages/mydoc**. Możesz ustawić różne wartości domyślne dla różnych zakresów ścieżek.

Aby uzyskać więcej informacji na temat paska bocznego, zobacz [Boczna nawigacja][mydoc_sidebar_navigation].

## Górna nawigacja

Górna nawigacja działa tak jak pasek boczny. Możesz określić, który plik danych topnav ma zostać załadowany, dodając `topnav` właściwość na swojej stronie, w następujący sposób:

```yaml
topnav: topnav
```

Tutaj topnav odnosi się do pliku `_data/topnav.yml`.

Ponieważ większość opcji topnav będzie taka sama, plik `_config.yml` określa plik topnav jako domyślny:



```yaml
-
  scope:
    path: ""
    type: "pages"
  values:
    layout: "page"
    comments: true
    search: true
    sidebar: home_sidebar
    topnav: topnav
```

## Składnia paska bocznego

Plik danych paska bocznego używa określonej składni YAML, której należy przestrzegać. Postępuj zgodnie z wzorcem pokazanym w motywie, a konkretnie na przykładzie `mydoc_sidebar.yml`: Oto przykładowy kod pokazujący wszystkie poziomy:


```yaml
entries:
- title: sidebar
  product: Motyw dokumentacji Jekyll
  version: 6.0
  folders:
  - title: Przegląd
    output: web, pdf
    folderitems:

    - title: Pierwsze kroki
      url: /index.html
      output: web, pdf
      type: homepage

    - title: Wprowadzenie
      url: /mydoc_introduction.html
      output: web, pdf

  - title: Uwagi o wydaniach
    output: web, pdf
    folderitems:

    - title: Uwagi o wydaniu 6.0
      url: /mydoc_release_notes_60.html
      output: web, pdf

    - title: Uwagi o wydaniu 5.0
      url: /mydoc_release_notes_50.html
      output: web, pdf

  - title: Archiwum tagów
    output: web
    folderitems:

    - title: Przegląd archiwum tagów
      url: /mydoc_tag_archives_overview.html
      output: web

      subfolders:
      - title: Strony archiwum tagów
        output: web
        subfolderitems:

        - title: Formatowanie stron
          url: /tag_formatting.html
          output: web

        - title: Nawigacja po stronach
          url: /tag_navigation.html
          output: web

        - title: Typy treści stron
          url: /tag_content_types.html
          output: web
```

Każda `folder` lub `subfolder` musi zawierać właściwości `title` oraz `output`. Każdy `folderitem` albo `subfolderitem` musi zawierać właściwości `title`, `url` oraz `output`.

Dwa dostępne wyjścia to `web` oraz `pdf`. (Nawet jeśli nie publikujesz plików PDF, nadal musisz je określić `output: web`).

Składnia YAML zależy od dokładnych spacji (odstepów), więc upewnij się, że stosujesz się do wzoru pokazanego na przykładowych paskach bocznych. Zobacz mój [samouczek YAML](mydoc_yaml_tutorial) , aby uzyskać więcej informacji na temat działania YAML.

{% include note.html content="Jeśli masz tylko jeden brakujący znak spacji, Jekyll nie zbuduje się z powodu błędu składniowego YAML. W konsoli zobaczysz komunikat o błędzie: \"Error ... did not find expected key while parsing a block mapping at line 22 column 5. Error: Run jekyll build --trace for more information.\" („Błąd… nie udało się znaleźć oczekiwanego klucza podczas analizowania odwzorowania bloku w wierszu 22 kolumna 5. Błąd: Uruchom polecenie jekyll build --trace, aby uzyskać więcej informacji.”) Jeśli się z tym spotkasz, zazwyczaj odnosi się to do nieprawidłowego wcięcia lub odstępu w pliku YAML. Zobacz przykład mydoc_sidebar.yml , aby zobaczyć, gdzie źle poszło formatowanie." %}

Każdy poziom musi mieć co najmniej jeden temat, zanim rozpocznie się następny poziom. Nie można mieć drugiego poziomu, który zawiera wiele poziomów trzecich, bez posiadania co najmniej jednego samodzielnego tematu na drugim poziomie. Jeśli potrzebujesz hierarchii, która zawiera folder zawierający inne foldery i bez luźnych tematów, użyj pustego elementu `-` tak, jak poniżej:

```yaml
entries:
- title: sidebar
  product: Motyw dokumentacji Jekyll
  version: 6.0
  folders:
  - title: Przegląd
    output: web, pdf
    folderitems:

    -

  - title: Uwagi o wydaniach
    output: web, pdf
    folderitems:

    - title: Uwagi o wydaniu 6.0
      url: /mydoc_release_notes_60.html
      output: web, pdf

    - title: Uwagi o wydaniu 5.0
      url: /mydoc_release_notes_50.html
      output: web, pdf

  - title: Instalacja
    output: web, pdf
    folderitems:

    - title: O Ruby, Gemach, Bundler, etc.
      url: /mydoc_about_ruby_gems_etc.html
      output: web, pdf

    - title: Zainstaluj Jekyll na Macu
      url: /mydoc_install_jekyll_on_mac.html
      output: web, pdf

    - title: Zainstaluj Jekyll na Windows
      url: /mydoc_install_jekyll_on_windows.html
      output: web, pdf
```

Aby zmieścić stronę tytułową i spis treści w generowanychplikach PDF, każdy pasek boczny produktu musi zawierać najpierw listę tych stron:

```yaml
- title:
  output: pdf
  type: frontmatter
  folderitems:
  - title:
    url: /titlepage
    output: pdf
    type: frontmatter
  - title:
    url: /tocpage
    output: pdf
    type: frontmatter
```

Leave the output as `output: pdf` for these frontmatter pages so that they don't appear in the web output.

Aby uzyskać więcej informacji na temat paska bocznego, zobacz [Nawigacja boczna][mydoc_sidebar_navigation] oraz [samouczek YAML ][mydoc_yaml_tutorial].

## Komentarze

Motyw integruje [Commento.io](https://commento.io/) dla komentarzy pod stronami i postami. (Ta usługa komentowania nie wprowadza kontrowersyjnych reklam śledzących, tak jak robi to Disqus.) Musisz mieć konto Commento.io + plan (5 USD / miesiąc) , aby autoryzować Commento w swojej domenie (nie jest wymagana żadna inna konfiguracja). Jeśli nie chcesz komentarzy, w pliku \_config.yml file, zmień właściwość `comments: true`  (poniżej `defaults`) na `comments: false` w każdym przypadku. W efekcie logika zawarta  w pliku włączającym commento.html  (wewnątrz \_includes), `{% raw %}{% unless page.comments == false %} ... {% endunless %}{% endraw %}` nie wstawi formularza komentarza.

## Linki względne i przeglądanie offline

W tym motywie używane są względne linki, dzięki czemu można przeglądać witrynę offline i nie martwić się o serwer lub katalog, w którym ją hostujesz. Dokumenty techniczne często wypychają zawartość na wewnętrzny serwer w celu przejrzenia przed przesłaniem zawartości na zewnętrzny serwer w celu publikacji. Ze względu na potrzebę bezproblemowego przenoszenia z jednego hosta na drugi, strona musi używać linków względnych.

Aby wyświetlić strony lokalnie na twoim komputerze (bez serwera podglądu Jekyll), muszą mieć  rozszerzenie `.html`. Właściwość `permalink` w nagłówku strony (frontmatter , bez otaczających ukośników), co popycha pliki do katalogu głównego, gdy strona buduje..

## Nagłówek strony

Kiedy piszesz strony, włączaj te same właściwości w nagłówku każdej strony:

```yaml
---
title: "Jakiś tytuł"
tags: [przykład1, przykład2]
keywords: słowokluczowe1, słowokluczowe2, słowokluczowe3
last_updated: Dzień miesiąc rok
summary: "opcjonalnie streszczenie"
sidebar: nazwa_sidebar
permalink: filename.html
---
```

(Oczywiście dostosujesz wartości dla każdej z tych właściwości).

W przypadku tytułów otaczanie tytułu w cudzysłowie jest opcjonalne, ale jeśli w tytule znajduje się dwukropek, musisz otoczyć tytuł cudzysłowami. Jeśli w tytule znajduje się cudzysłów, uniknij go, używając ukośnika `\`.

Wartości dla `keywords` zapisywane są w metadanych strony dla SEO.

Wartości dla `tags` muszą być zdefiniowane na liście \_data/tags.yml. Potrzebny jest również odpowiedni plik znaczników w folderze znaczników, który ma ten sam wzór, co inne pliki znaczników pokazane w folderze znaczników. (Jekyll nie utworzy automatycznie tych plików znaczników).

Jeśli nie chcesz, aby mini-TOC wyświetlał się na stronie (na przykład na stronie głównej lub stronach docelowych), dodaj `toc: false` w nagłówku strony.

Wartość  `permalink` być taka sama jak nazwa pliku i obejmować rozszerzenie pliku ".html".

Aby uzyskać więcej informacji, zobacz [Strony][mydoc_pages].

## Gdzie przechowywać tematy dotyczące dokumentacji

Możesz przechowywać swoje pliki dla każdego produktu w podfolderach zgodnie ze wzorem pokazanym w motywie. Na przykład produkt1, produkt2 itp. Można przechowywać we własnych podfolderach w katalogu \_pages. Wewnątrz \_pages, możesz przechowywać swoje tematy w podfolderach lub pod-podfolderach. Kiedy Jekyll buduje twoją witrynę, przenosi tematy do katalogu głównego i użyje linku bezpośredniego do adresu URL.

Pamiętaj, że product1, product2 i mydoc to tylko przykładowa zawartość, aby pokazać, jak dodać wiele produktów do kompozycji. Możesz dowolnie usuwać te treści..

Aby uzyskać więcej informacji, zobacz[Strony][mydoc_pages] oraz [Posty][mydoc_posts].


## Skonfiguruj górną nawigację

Elementy menu górnego paska nawigacyjnego ustawia się w pliku \_data/topnav.yml. Użyj górnego paska nawigacyjnego, aby udostępnić łącza do przechodzenia między produktami lub do zasobów zewnętrznych.

W przypadku zewnętrznych adresów URL użyj właściwości `external_url` , jak pokazano w przykładowym pliku topnav.yml. W przypadku łączy wewnętrznych użyj tego samego `url`, co w plikach danych paska bocznego.

Zauważ, że topnav ma dwie sekcje: `topnav` i `topnav_dropdowns`. Sekcja topnav zawiera pojedyncze linki, a sekcja  topnav_dropdowns zawiera menu rozwijane. Dwie sekcje są od siebie niezależne.

## Generowanie pliku PDF

Jeśli chcesz wygenerować plik PDF, potrzebujesz licencji na [Prince XML](http://www.princexml.com/). Będziesz także musiał [zainstalować Prince](http://www.princexml.com/doc/installing/).  Możesz generować pliki PDF według produktu (ale nie dla każdego produktu w witrynie łącznie w jednym ogromnym pliku PDF). Prince będzie działał nawet bez licencji, ale na pierwszej stronie nadrukuje mały obrazek Prince, a ty musisz kupić licencję, aby z niego korzystać.

Jeśli korzystasz z systemu Windows [Git Bash client](https://git-for-windows.github.io/) zamiast domyślnego wiersza polecenia systemu Windows.

Otwórz plik css css/printstyles.css i dostosuj podany tam adres (`youremail@domain.com`). Ten adres e-mail jest wyświetlany w lewym dolnym rogu stopki pliku PDF. Konieczne będzie również utworzenie pliku konfiguracyjnego PDF zgodnie z przykładami pokazanymi w folderze pdfconfigs, a także dostosowanie niektórych skryptów kompilacji według tego samego wzorca pokazanego w katalogu głównym: pdf-product1.sh

Zobacz sekcję [Generowanie plików PDF][mydoc_generating_pdfs], aby uzyskać więcej informacji na temat konfigurowania motywu dla tego formatu wyjściowego.

## Blogi / Aktualności

W przypadku postów na blogu utwórz pliki markdown w folderze \_posts folder following the sample formats. zgodnie z przykładowymi formatami. Nazwy plików postów zawsze zaczynają się od daty (RRRR-MM-DD-tytul).

Plik news/news.html wyświetla posty, a plik  news_archive.html pokazuje roczną historię wpisów. W dokumentacji możesz użyć wiadomości do wyróżnienia funkcji produktu poza dokumentacją lub do dostarczenia informacji o wersji i innych aktualizacji.

Zobacz [Posty][mydoc_posts], aby uzyskać więcej informacji.

## Markdown

Ten motyw wykorzystuje [kramdown markdown](http://kramdown.gettalong.org/). jest podobny do Markdown o smaku Github, z tą różnicą, że gdy masz tekst, który przechwytuje elementy listy, odstępy między tekstem przechwytującym muszą być wyrównane z odstępami pierwszego znaku po spacji numerowanego elementu listy. Zasadniczo, korzystając z numeracji elementów listy, użyj dwóch spacji po kropce w liczbie, w następujący sposób:

```
1.  Pierwsza pozycja
2.  Druga pozycja
3.  Trzecia pozycja
```

Jeśli chcesz wstawić akapity, notatki, fragmenty kodu lub inne elementy pomiędzy elementami listy, użyj czterech spacji do wcięcia. Cztery spacje będą wyrównane z pierwszą literą elementu liście (the <b>P</b>ierwszy lub <b>D</b>rugi albo <b>T</b>rzeci).

```
1.  Pierwsza pozycja

    ```
    alert("hello");
    ```

2.  Druga pozycja

    Some pig!

3.  Trzecia pozycja
```

Aby uzyskać więcej informacji, zobacz tematy w sekcji „Formatowanie” na pasku bocznym.


## Automatyczne linki

Jeśli chcesz używać automatycznego systemu do zarządzania linkami, zobacz [Automatyczne łącza][mydoc_hyperlinks.html#automatedlinks]. Takie podejście automatycznie tworzy listę odniesień Markdown w celu uproszczenia łączenia.

## Inne instrukcje

Treść tutaj jest tylko przewodnikiem dla początkujących. Więcej informacji na temat pracy z motywem znajduje się w różnych sekcjach na pasku bocznym.

{% include links.html %}
