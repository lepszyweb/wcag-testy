---
title: O bazie prostych testów


sidebar: testy-proste_sidebar
permalink: 00_P_wprowadzenie
folder: testy-proste
last_updated: 2 lutego 2020
---

## Baza prostych testów dostępności
Baza prostych testów pomaga oceniać dostępność cyfrową stron internetowych. Dzięki prostym testom można się zorientować, czy dostępność treści na stronie internetowej została zapewniona w najbardziej elementarny sposób.

Testy zostały dobrane i zaprojektowane tak, aby mógł je przeprowadzić każdy, kto posiadł wykształcenie ogólne i korzysta ze stron internetowych. 

Wcześniej nabyta wiedza o dostępności cyfrowej czy projektowaniu stron na pewno będzie pomocna w przeprowadzeniu przeglądu, ale nie jest konieczna. 

Przeprowadzenie prostego przeglądu dostępności wymaga od oceniających jedynie zapoznania się z opisami testów i zastosowania przedstawionych w nich instrukcji. 

Oznacza to, że komplet informacji potrzebnych do przeprowadzenia testów i oceny dostępności w sprawdzanym zakresie znajduje się w opisach testów.
  
Jedynym technicznym wymogiem jest umiejętność zainstalowania w przeglądarce dodatków rozszerzających jej możliwości. 


## Pierwowzór bazy prostych testów
Baza prostych testów została opracowana na podstawie dokumentu W3C WAI zatytułowanego [Easy Checks - A First Review of Web Accessibility](https://www.w3.org/WAI/test-evaluate/preliminary/), co można przetłumaczyć na język polski: Łatwe testy - Pierwszy przegląd dostępności cyfrowej.

Opracowanie W3C ma już swoją blisko 20-letnią historię.
 
Pierwotnie była to jedna sekcja opublikowanego w październiku 2001 roku dokumentu *Evaluating Web Sites for Accessibility* (Ocenianie witryn internetowych pod kątem dostępności), zatytułowana Preliminary Review (Przegląd wstępny). Zredagowali ją Judy Brewer i Chucka Letourneau. 

W 2005 roku część poświęcona przeglądowi wstępnemu została wyodrębniona, rozbudowana i opublikowana pod tytułem *Preliminary Review of Web Sites for Accessibility* (Wstępny przegląd witryn internetowych pod kątem dostępności). Redaktorem tej odsłony był Shadi Abou-Zahra. 
Szkic roboczy najnowszej odsłony dokumentu został opublikowany w czerwcu 2013 roku pod przywołanym już tutaj tytułem *Easy Checks - A First Review of Web Accessibility*. Najnowsze aktualizacje pochodzą z roku 2017.

## Zakres  
Baza prostych testów obejmuje tylko kilka kluczowych aspektów dostępności stron internetowych. Może się zdarzyć, że strona internetowa przejdzie pomyślnie przez wszystkie te testy, ale nadal będą na niej występować znaczące bariery dostępności.

Aby kompleksowo ocenić dostępność cyfrową strony internetowej, potrzebne jest solidniejsze badanie, niż kilka prostych testów.

Stwierdzenie to nie podważa w najmniejszym stopniu sensu przeprowadzania prostych przeglądów dostępności. 
 
Wręcz przeciwnie. Proste testy dostępności są miarodajne i godne zaufania.

Przeprowadzanie przeglądów dostępności w oparciu o bazę prostych testów i podjęcie w ich następstwie odpowiednich czynności naprawczych może znacząco poprawić dostępność witryny. Szacunkowo prosty przegląd dostępności umożliwia wykrycie około 75-80% barier występujących na stronach internetowych. Gdyby ze stron internetowych usunąć tylko tych 75-80% najłatwiejszych do wykrycia barier, uczynilibyśmy milowy krok ku dostępności cyfrowej.


Baza prostych testów obejmuje sprawdzenie 10 wymienionych poniżej aspektów witryny oraz zawiera wskazówki dotyczące kolejnych kroków i łącza do dodatkowych zasobów.


- [Tytuł strony](01_P_tytul-strony)
- [Teksty alternatywne obrazów](02_P_odpowiedniki-tekstowe-obrazow) ( „alternatywy tekstowe” zdjęć, ilustracji, wykresów, etc.)
- **Tekst**:
  - [Nagłówki](03_P_naglowki)
  - [Kontrast kolorów](04_P_wspolczynnik_kontrastu) („współczynnik kontrastu”)
  - [Zmiana rozmiaru tekstu](05_P_zmiana-rozmiaru-tekstu)
- **Interakcja**:
  - [Dostęp za pomocą klawiatury i widoczność fokusa](06_P_klawiatura)
  - [Formularze, etykiety i błędy](07_P_formularze) (w tym pól Szukaj)
- **Ogólne**:
  - [Treść przesuwana, migocąca lub błyskająca](08_P_poruszanie-i-blyski)
  - [Odpowiedniki multimediów](09_P_multimedia.md) (wideo, audio)
  - [Podstawowa struktura](10_P_struktura)

## Proste testy a WCAG

WCAG obejmują ogółem 78 kryteriów sukcesu wyznaczających wymagania dostępności, w tym 30 na poziomie A (minimalnym), 20 na poziomie AA (zalecanym), a 28 na poziomie AAA (komfortowym). 

Ustawa o dostępności cyfrowej stron internetowych i aplikacji mobilnych wymaga spełnienia wszystkich kryteriów sukcesu na poziomie A oraz 19 kryteriów sukcesu na poziomie AA, a więc wymaga spełnienia minimum 49 kryteriów sukcesu. 

Natomiast proste testy umożliwiają sprawdzenie spełnienia tylko 22 kryteriów sukcesu, w tym 15 kryteriów sukcesu na poziomie A, a więc zaledwie połowy ze wszystkich kryteriów na najniższym poziomie oraz 7 kryteriów na poziomie AA, a więc nawet nie połowy wszystkich wymagań na tym poziomie. 

W tabeli poniżej znajduje się zestawienie prostych testów i kryteriów sukcesu, z  którymi te testy są powiązane.

| Test        | Kryterium sukcesu WCAG                   |
|-------------|------------------------------|
| Tytuły stron | 2.4.2 Tytuły stron (A) |
| Teksty alternatywne obrazów | 1.1.1 Treść nietekstowa (A) |
| Współczynnik kontrastu | 1.4.3: Kontrast minimalny (AA) |
| Zmiana rozmiaru tekstu | 1.4.4 Zmiana rozmiaru tekstu (AA) |
| Nagłówki | 1.3.1 Informacje i relacje (A), 2.4.6 Nagłówki i etykiety  (AA), 2.4.10 Nagłówki sekcji (AAA), 1.4.5 Obrazy tekstu (AA) |
| Dostęp za pomocą klawiatury i widoczność fokusa | 2.1.1 Klawiatura (A), 2.1.2 Bez pułapki na klawiaturę (A), 2.4.3 Kolejność zaznaczania (A), 2.4.7 Widoczny fokus (AA) |
| Formularze, etykiety i błędy | 3.3.2 Etykiety lub instrukcje (A), 1.3.1 Informacje i relacje (A), 3.3.1 Identyfikacja błędu (A), 3.3.3 Sugestie korekty błędów (A), 3.3.4 Zapobieganie błędom… (AA) |
| Treść przesuwana, migocąca lub błyskająca | 2.2.2 Wstrzymywanie (pauza), zatrzymywanie, ukrywanie (A), 2.3.1 Trzy błyski lub wartości poniżej progu (A) |
| Odpowiedniki multimediów | 1.2.2 Napisy (rozszerzone) (A), 1.2.3 Audiodeskrypcja lub alternatywa dla mediów (nagranie) (A), 1.2.5 Audiodeskrypcja (nagranie) (AA), 1.4.2 Kontrola odtwarzania dźwięku  (A), 1.2.8 Alternatywa dla mediów (nagranie) (AAA) |


