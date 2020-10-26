---
title: Punkty orientacyjne
summary: "Treść strony jest podzielona na obszary kluczowe - punkty orientacyjne"
tags: [nawigacja,struktury]
sidebar: testy_sidebar
permalink: H1-02-punkty-orientacyjne
folder: testy/jbt
---
## Opis testu
Ten test służy ocenie struktury strony internetowej.

## Zastosowanie
Wizualne i programowe wyróżnienie kluczowych obszarów strony internetowej. Użycie nowych w HTML5 znaczników strukturalnych oraz atrybutów ARIA.

## Obsługa dostępności
W HTML5 wprowadzono nowe znaczniki strukturalne, które opisują role kluczowych <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obszar}}">obszarów strony</a>
 (`header`, `nav`, `main`, `section`, `aside`, `footer`).

Specyfikacja WAI-ARIA umożliwia określanie kluczowych obszarów strony za pomocą atrybutów `role="banner"`, `role="navigation"`, `role="main"` `role="aside"`, `role="contentinfo"`, `role="search"`, `role="region"`.

## Mapowanie do standardów dostępności
- **WCAG 2.1 - kryterium sukcesu** {% include ks/1-3-1.md %}
- **WCAG 2.1 - kryterium sukcesu** {% include ks/2-4-1.md %}
- **WCAG 2.1 - kryterium sukcesu** {% include ks/2-4-6.md %}
- **WCAG 2.1 - kryterium sukcesu** {% include ks/3-2-3.md %}
- **WCAG 2.1 - kryterium sukcesu** {% include ks/3-2-4.md %}
- **WCAG 2.1 - kryterium sukcesu** {% include ks/4-1-2.md %}

## Oczekiwania:
{% include note.html content="Kryteria sukcesu WCAG nie wymagają, aby oznaczać kluczowe obszary strony i punkty orientacyjne. Czy strona spełnia wymienione poniżej oczekiwania sprawdzamy **tylko wtedy**, gdy stosowane są punkty orientacyjne i oznaczenia sekcji strony." %}

-	Cała zawartość strony znajduje się w kluczowych obszarach strony objętych znacznikami lub atrybutami ARIA definiującymi punkty orientacyjne, odpowiednio do celów tych obszarów:  
    -	znacznikiem `header` lub atrybutem `role="banner"` (nagłówek strony, tylko jeden)
    -	atrybutem `role="search"` (wyszukiwanie)
    -	znacznikiem `footer` lub atrybutem `role="contentinfo"` (stopka strony, tylko jedna)
    -	znacznikiem `nav` lub atrybutem `role="navigation"` (nawigacja, jeżeli więcej niż jedna, każda jest jednoznacznie określona etykietą)
    -	znacznikiem `main` lub atrybutem `role="main"` (obszar treści głównej, tylko jeden)
    -	znacznikiem `aside` lub atrybutem `role="complementary"`  (jeśli więcej niż jeden, każdy jest jednoznacznie określony etykietą)
-	Gdy na stronie istnieje więcej niż jedno wystąpienie typu obszaru, to każdy z&nbsp;nich jest jednoznacznie określony za pomocą:
    -	atrybutu `aria-labelledby` wskazującego na widoczny nagłówek.
    -	atrybutu `aria-label`, jeżeli obszar nie rozpoczyna się od nagłówka.
- Obszar oznaczony głównym punktem orientacyjnym nie zawiera żadnych bloków treści, które powtarzają się na pozostałych stronach witryny, np. powtarzalnego obszaru nawigacyjnego (nie dotyczy ścieżki powrotu – jej treść jest inna na każdej stronie).
- Liczba obszarów jest niewielka.
- Punkt orientacyjny `banner` nie może być zawarty w innym punkcie orientacyjnym.
- Punkt orientacyjny `contentinfo`  nie może być zawarty w innym punkcie orientacyjnym
- Punkt orientacyjny `main`  nie może być zawarty w innym punkcie orientacyjnym
- Na stronie znajduje się tylko jeden punkt orientacyjny `banner`
- Na stronie znajduje się tylko jeden punkt orientacyjny `main`
- Na stronie znajduje się tylko jeden punkt orientacyjny `contentinfo`
- Każdy punkt orientacyjny ma unikalną rolę lub unikalną kombinację roli oraz etykiety lub tytułu
- Obszar `banner` jest na najwyższym poziomie hierachii obszarów funkcjonalnych
- Obszar `main` jest na najwyższym poziomie hierachii obszarów funkcjonalnych
- Obszar `contentinfo` jest na najwyższym poziomie hierachii obszarów funkcjonalnych
- Obszary `complementary` i `aside` są na najwyższym poziomie hierachii obszarów funkcjonalnych


## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Testowanie

### Metoda badania:
Wykorzystanie narzędzia ujawniającego punkty orientacyjne, inspekcja kodu.
### Pomocne narzędzia:

-	[skryptozakładka Ladmarks](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Oznacza punkty orientacyjne. Jeśli zdefiniowane są znacznikiem html – umieszcza etykietę ze znacznikiem na żółtym tle. Jeśli zdefiniowane są atrybutem role, umieszcza etykietę z wartością atrybutu
-	[skryptozakładka Duplicate-landmark-roles](https://github.com/ThePacielloGroup/bookmarklets) z kolekcji Pacciello Group. Oznacza obszary, którym zdefiniowano nadmiarowy niepotrzebny atrybut role.
-	[skryptozakładka Ladmarks](https://accessibility-bookmarklets.org/install.html) z kolekcji Pixo i University of Illinois. Oznacza nakładkami punkty orientacyjne. W etykiecie nakładki komunikuje zastosowany element HTML oraz dostępną nazwę punktu orientacyjnego.
-	[opcja Landmarks w skryptozakładce Tota11y](https://khan.github.io/tota11y/)
-	[skryptozakładka Web Evaluation Tools](https://accessibility.oit.ncsu.edu/tools/web-evaluation-tools/) udostępniona przez IT Accessibility z NC State University
-	[skryptozakładka Active Images](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera. Oznacza punkty orientacyjne. Sprawdza i wyświetla etykiety zdefiniowane przez aria-labelledby, a nawet poprawność ortograficzną nazwy tego atrybutu (częsty błąd = jedno 'l' zamiast dwóch).

### Procedura testowania:
1.	Uruchom podgląd rozmieszczenia punktów orientacyjnych na stronie za pomocą jednego z narzędzi ujawniających punkty orientacyjne (zobacz niżej: *Pomocne narzędzia*).
2.	Sprawdź, czy typy punktów orientacyjnych określone użytymi znacznikami bądź atrybutami role zostały odpowiednio zastosowane do kluczowych obszarów strony (tzn. czy znacznik header bądź rola banner została zastosowana do nagłówka strony, znacznik bądź rola main została zastosowana do obszaru zawierającego główną treść strony, itd.
3.	Jeżeli na stronie występuje więcej niż jeden obszar tego samego typu, sprawdź, czy każdy z nich został oznaczony odróżniającą go etykietą lub nagłówkiem. (*Uwaga*: Jeżeli jakiś obszar nawigacyjny na stronie jest powtórzony, np. w&nbsp;nagłówku i stopce, wówczas może być oznaczony taką samą etykietą).     
4.	Sprawdź czy w obszarze głównego punktu orientacyjnego (`main`), znajdują się tylko niepowtarzalne treści (obszar `main` nie może zawierać żadnych bloków treści, które powtarzają się na stronach).

## Zasoby
### Techniki WCAG 2.1
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:

- {% include techniki/ARIA11.md %}
- {% include techniki/ARIA12.md %}
- {% include techniki/H69.md %}
- {% include techniki/H42.md %}
- {% include techniki/H80.md %}
- {% include techniki/G130.md %}
- {% include techniki/G141.md %}
- {% include techniki/PDF9.md %}

- {% include techniki/G1.md %}
- {% include techniki/G123.md %}
- {% include techniki/G124.md %}

### Opracowania
{% include doglos/131-punkty-orientacyjne-zasoby.md %}

## Przypadki testowe

### Zaliczone
_do opracowania_

### Niezaliczone
_do opracowania_
