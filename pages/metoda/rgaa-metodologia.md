---
title: "Metodyka testów - RGAA"
description: "Polskie tłumaczenie RGAA 4.0, Francuskie oficjalne wytyczne dostępności. Bibliografia."
keywords: "RGAA, RGAA 4.0, francuskie wytyczne dostępności, tłumaczenie polskie, bibliografia"
permalink: rgaa-metodyka-testow
toc: false
sidebar: metoda_sidebar
---

### Wstęp

Ten dokument został opracowany jako część zasobów towarzyszących wprowadzeniu  wersji 4 ogólnego standardu poprawy dostępności (RGAA 4).

Przeznaczony jest dla każdego, kto zajmuje się weryfikacją zgodności treści internetowych z RGAA 4. Jest to metodologia testowania dokumentująca kroki weryfikacji, czy kryterium RGAA 4 są spełnione, czy nie. 

Metodologię tę należy zatem traktować jako uzupełnienie technicznych ram odniesienia RGAA i nie można jej stosować samodzielnie. Nie zwalnia więc z dokładnej lektury repozytorium technicznego lub szkolenia w zakresie RGAA.

Dla każdego z testów danego kryterium istnieje odpowiednia procedura testowa; realizacja tej procedury może niekiedy wymagać użycia specjalnych narzędzi, w przeciwnym razie do przeprowadzenia większości testów wystarczy przeglądarka internetowa.

Podano również listę narzędzi pomocnych w przeprowadzeniu testów. Zostały wybrane zarówno dlatego, że są często używane przez ekspertów w tej dziedzinie, jak i dlatego, że ułatwiają uzyskanie określonych wyników.


### Narzędzia

Najbardziej użytecznym narzędziem jest inspektor kodu, jaki oferuje każda przeglądarka. Pozwala w prosty sposób wyszukać elementy i atrybuty wymagane do testowania dostępności.

Pomoce techniczne wymienione w wybranym środowisku testowym stanowią drugi zestaw niezbędnych narzędzi (patrz sekcja [Środowisko testowe](srodowisko.md/#content)). Są one w istocie wymagane do zapewnienia poprawnego renderowania dostępnych treści  (alternatywy obrazów, nagłówki linków, nagłówki tabel itp.), szczególnie w przypadku, gdy gdy samo sprawdzenie kodu nie byłoby wystarczające. 


Dostępne są inne narzędzia pomagające w wyszukiwaniu elementów treści. Są to często rozszerzenia przeglądarki. Pozwalają zbadać jednego lub więcej aspektów dostępności.

Paski narzędzi to rozszerzenia przeglądarki, które ułatwią wizualne zlokalizowanie określonych elementów w dokumencie:

- [Web Accessibility Toolbar - dla Internet Explorer](https://developer.paciellogroup.com/resources/wat/): pasek narzędzi do sprawdzania określonych punktów dostępności dokumentu.
- [Web Developer Toolbar - dla Firefox](https://addons.mozilla.org/fr/firefox/addon/web-developer/): pasek narzędzi dla programistów, który może pomóc wizualnie znaleźć określone w dokumencie elementy w celu sprawdzenia ich dostępności.
- [Web Developer Toolbar - dla Chrome](https://chrome.google.com/webstore/detail/web-developer/): ten sam pasek narzędzi, co poprzednio, ale dla Chrome.


Poza prostym paskiem narzędzi inne narzędzia zapewniają pełną analizę dokumentu, sygnalizując wizualnie błędy dostępności na stronie lub odwrotnie - elementy, które są dla niej korzystne. Filtry często pozwalają wyświetlać tylko niektóre z tych aspektów. Właśnie to oferuje [Wave](http://wave.webaim.org) -  rozwiązanie dostępne zarówno internetowo, jak i jako [rozszerzenie przeglądarki] (https://wave.webaim.org/extension/).

Do sprawdzania poprawności kodu źródłowego dokumentu HTML wykorzystywany jest [walidator W3C](https://validator.w3.org/). Należy pamiętać, że do walidacji kodu źródłowego generowanego przez przeglądarkę, musisz użyć opcji  *<span lang="en">Validate by Direct Input</span>* („Sprawdź poprawność przez bezpośrednie wprowadzanie”), kopiując źródło HTML generowane przez inspektora kodu przeglądarki. 

Dostępne są również rozszerzenia do przeglądarek, ale w korzystaniu z nich należy zachować ostrożność, ponieważ algorytmy walidacji tych rozszerzeń niekoniecznie są aktualne w stosunku do walidatora W3C i dlatego uzyskane wyniki mogą być inne.

Weryfikacji kontrastów kolorów można dookonać za pomocą kilku różnych narzędzi:

- [WCAG Contrast Checker](https://addons.mozilla.org/fr/firefox/addon/wcag-contrast-checker/): rozszerzenie Firefox, które umożliwia automatyczną kontrolę kontrastów kolorów tekstu w dokumencie ;
- [Color Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/): aplikacja dla systemu Windows lub Mac, która umożliwia kontrolę kontrastu kolorów.

Do weryfikacji drzewa dokumentu i hierarchii tytułów bardzo przydatnesą dwa  rozszerzenia:
- [HeadingsMap dla Firefoksa](https://addons.mozilla.org/fr/firefox/addon/headingsmap/): rozszerzenie Firefoksa, które daje przegląd planu dokumentu i strukturę drzewa dokumentu.
- [HeadingsMap dla Chrome](https://chrome.google.com/webstore/detail/headingsmap/flbjommegcjonpdmenkdiocclhjacmbi): to samo rozszerzenie, co poprzednie dla Chrome.

Analizę plików biurowych można przeprowadzić przy użyciu różnych narzędzi w zależności od formatu pliku:

- [PAC (PDF Accessibility Checker) wersja 3 dla Windows](https://www.access-for-all.ch/en/pdf-lab/pdf-accessibility-checker-pac.html): oprogramowanie umożliwiające sprawdzenie określonych punktów dostępności dokumentów PDF;
- [Word Accessibility Plug-in dla Microsoft Office Windows](http://accessibility.zhaw.ch/index.php?id=6&L=1): rozszerzenie programu Microsoft Word, które umożliwia edycję i sprawdzanie dostępności edytowalnego dokumentu biurowego w formacie .doc; należy pamiętać, że ostatnie wersje narzędzi biurowych firmy Microsoft oferują wbudowaną funkcję sprawdzania dostępności.
- [AccessODF dla LibreOffice](https://extensions.libreoffice.org/extensions/accessodf): rozszerzenie do sprawdzania dostępności dokumentu LibreOffice Writer; należy pamiętać, że to rozszerzenie nie jest już kompatybilne z najnowszymi wersjami LibreOffice (powyżej wersji 4.0);
- [Ace autorstwa DAISY App](https://inclusivepublishing.org/toolbox/ace-by-daisy-app/) jest narzędziem do sprawdzania dostępności plików EPUB.

Wreszcie, stare, ale wciąż przydatne oprogramowanie do oceny potencjału niektórych treści internetowych do wywoływania napadów: PEAT [Photosensitive Epilepsy Analysis Tool) dla systemu Windows](https://trace.umd.edu/peat).


{% include komponenty/rgaa-testy.html %}