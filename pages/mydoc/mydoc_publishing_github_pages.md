---
title: Publikowanie na stronach Github
sidebar: mydoc_sidebar
permalink: mydoc_publishing_github_pages.html
summary: "Możesz opublikować swój projekt na Github Pages, która jest bezpłatną usługą hostingową udostępnianą przez Github. Wystarczy umieścić treść w gałęzi repozytorium Github zwanej gh-pages i ustawić ją jako domyślną gałąź repo. Z witryną Jekyll, po prostu zatwierdzasz cały projekt w gałęzi gh-pages, a Github Pages zbuduje tę witrynę dla Ciebie."
folder: mydoc
---

## Skonfiguruj swoje repozytorium Github

1. Upewnij się, że masz zainstalowany Git. Możesz pobrać i zainstalować [Git na Windows tutaj](https://git-scm.com/download/win) i [Git na Mac tutaj](https://git-scm.com/download/mac). Jeśli korzystasz z komputera Mac, prawdopodobnie masz już zainstalowany git. Możesz to sprawdzić, otwierając terminal i pisząc `which git`.{{end}}
2. Wejdź na [Github.com](http://github.com) i zarejestruj konto. 
3. Kliknij przycisk  **+** w prawym górnym rogu i wybierz t **New repository**.
4. Nazwij repozytorium czymś w rodzaju **mojmotywdokumentacji**.
5. Wpisz opis.
6. Zaznacz pole wyboru **Initialize this repository with a README** (Zainicjuj to repozytorium z README).
7. W razie potrzeby dodaj licencję.
8. Pozostaw domyślne ustwienia innych opcji i kliknij **Create repository** (Utwórz repozytorium).
9. Kliknij przycisk **Settings** (Ustawienia).
10. Przejdź do strony głównej swojego repozytorium i kliknij menu rozwijane gałęzi..
11. Utwórz nową gałąź o nazwie **gh-pages**.  
12. Kliknij **Settings** i zmień domyślną gałąź na strony **gh-pages**.
13. Wróć do strony głównej swojego repozytorium. Po wybraniu gałęzi gh-pages branch skopiuj adres  **https clone url**:
14. Otwórz terminal, przejdź do dogodnej lokalizacji dla swojego projektu i wpisz `git clone https://github.com/tomjoht/myreponame.git`, zastępując `https://github.com/tomjoht/myreponame.git` adresem URL https klonu repozytorium.
15. Przenieś pliki motywów jekyll do tego nowego folderu, który właśnie utworzyłeś w poprzednim kroku.
16. Otwórz plik \_config.yml i dodaj następujące elementy:

 git clone https://github.com/tomjoht/myreponame.git, zastępując https://github.com/tomjoht/myreponame.gitskopiowany adres URL https klonowania repozytorium.

   ```
   url: tomjoht.github.io
   baseurl: /myreponame
   ```

   Zmień adres URL na nazwę konta github, a baseurl na nazwę repo.


## Zainstaluj Bundler

Bundler to menedżer pakietów dla Ruby, który zainstaluje wszystkie zależności, które mogą być potrzebne do zbudowania twojej witryny lokalnie. Polecam instalację Bundlera przez homebrew. (Przepraszamy, te instrukcje dotyczą tylko komputerów Mac).


1. Zainstaluj [homebrew](http://brew.sh/):

   ```
   /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
   ```
2. Zainstaluj Bundler:

   ```
   gem install bundler
   ```


## Dodaj klejnot stron github (gem)

1. W terminalu przejdź do katalogu projektu Jekyll.
2. Wpisz `bundle init`. Spowoduje to utworzenie plików Gemfile i Gemfile.lock w twoim projekcie.
3. Wpisz `open gemfile`. Spowoduje to otwarcie pliku gemfile w domyślnym edytorze tekstu.
4. Dodaj do pliku gemfile następujący kod  (zastępując istniejącą zawartość):

   ```
   source 'https://rubygems.org'
   gem 'github-pages'
   ```

5. Uruchom`bundle install`.
6. Dodaj nowe pliki Jekyll do git: `git add --all`.
7. Wyślij pliki:  `git commit -m "committing my jekyll theme"`.
8. Push pliki do swojej github repo: `git push`.

Strony Github automatycznie utworzą teraz Twoją witrynę. Zaczekaj minutę lub dwie, a następnie odwiedź tomjoht.github.io/yourreponame, zastępując tę ​​ścieżkę kontem github i głęzią.

## Dostosuj swój adres URL

Możesz także dostosować swój adres URL Github. Więcej instrukcji na ten temat później....

{% include links.html %}
