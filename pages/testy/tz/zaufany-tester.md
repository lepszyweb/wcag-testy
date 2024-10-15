---
title: O procesie testowym Trusted Tester
summary: "Proces testowy Trusted Tester to zestaw procedur testowych, ktorych celem jest stwierdzenie zgodności treści stron internetowych ze Zmienioną Sekcją 508, która w całości implementuje WCAG 2.0. Pierwotnie został  stworzony przez Biuro Dostępnych Systemów i Technologii (OAST) w Departamencie Bezpieczeństwa Wewnętrznego (DHS) Stanów Zjednoczonych, a później przyjęty przez kilka innych amerykańskich agencji federalnych."

sidebar: testy_sidebar
permalink: zaufany-tester
folder: testy/tz
last_updated: 4 października 2024
---

O dokumencie
===================

Kto powinien korzystać z tego dokumentu
----------------------------

Oryginalny dokument został opracowany i jest przeznaczony do użytku przez Zaufanych Testerów (ang. <span lang ="en">Trusted Tester</span>).

Zaufany tester to osoba, która zdała egzamin certyfikacyjny Trusted Tester i w związku z tym posiada certyfikat uprawniający do dostarczania dokładnych i powtarzalnych wyników testu zgodności treści internetowych ze standardami dostępności.

Zaufany tester postępuje zgodnie ze zmienionym procesem testowania zgodności z sekcją 508 dla Internetu, korzysta z zatwierdzonych narzędzi testowych i ocenia aplikacje internetowe pod kątem zgodności ze zaktualizowanymi standardami 508. 

Aby uzyskać więcej informacji na temat Poprawionego Kursu Szkoleniowego i Egzaminu 508 Trusted Tester, skontaktuj się z Działem Pomocy Technicznej Departamentu Bezpieczeństwa Wewnętrznego (DHS) pod adresem accessibility@dhs.gov.

Harmonizacja z testami podstawowymi
-----------------------------


Zharmonizowane dostosowanie linii podstawowej
Ten proces testowy obejmuje wszystkie testy opisane w "Harmonized Processes for Revised 508 Testing: Baseline Tests for Web Accessibility" (<q>Ujednolicone procesy dla zmienionych testów 508: Podstawowe testy dostępności stron internetowych</q>) w wersji 3.0. Testy podstawowe ustanowiły minimalne kroki wymagane do określenia zgodności ze zaktualizowanymi normami Sekcji 508 oraz WCAG 2.0 poziom A i AA. 

Instrukcje testowe, które są specyficzne tylko dla Zaufanego testera, są oznaczone jako *specyficzne dla TT* lub "[brak punktu odniesienia]". Wyniki tych testów zostaną odzwierciedlone tylko w wynikach poprawionych testów 508.

Wyniki testów podstawowych będą raportowane oddzielnie i nie mają na nie wpływu testy specyficzne dla procesu Trusted Tester.

Jak wygląda struktura tego dokumentu
-------------------------------

-   Treść wprowadzająca:

    -   O tym dokumencie - opisuje cel, odbiorców i zakres tego dokumentu Rozdział 1

    -   Środowisko testowe - opisuje środowiska testowe obsługiwane przez ten proces testowy, w tym systemy operacyjne, przeglądarki i narzędzia testujące

    -   Wymagania dotyczące raportowania zgodności - zawiera wskazówki dotyczące raportowania

-   Sekcja 508 Testy zgodności - szczegółowo opisuje procesy testowe. Każdy proces testowy zawiera instrukcje krok po kroku dotyczące tego, jak i co testować, a także instrukcje określania wyników testu dla każdego Warunku testowego.

-   Załączniki - Zawierają tabele referencyjne wskazujące związek między Testów ze Zmienionymi standardami 508 i testami podstawowymi; definicje; dziennik zmian w dokumencie; oraz krótkie podsumowania procesu testowego.

Tylko testy treści internetowych
----------------------

Ten proces testowy obejmuje tylko treści internetowe.  Zaufany Tester w wersji 4.x i starszych został opracowany dla oryginalnej normy Section 508, która miały osobne wymagania dotyczące stron internetowych i oprogramowania. Ze względu na to, że zaktualizowane standardy 508 stosują WCAG 2.0 poziom A i AA do stron internetowych, oprogramowania i innych treści elektronicznych, pierwotnym planem było połączenie testów oprogramowania i stron internetowych w jednym procesie testowym.

Ponieważ jednak Zaktualizowane standardy 508 oprócz WCAG 2.0 mają inne wymagania dotyczące oprogramowania, a narzędzia do testowania oprogramowania nie były jeszcze dostępne, proces testowania oprogramowania będzie odrębny. Chociaż nie jest to tak powszechne ze względu na możliwości HTML5, elementy oprogramowania nadal nadal można znaleźć w treściach internetowych w aplikacjach internetowych. Aby przetestować elementy oprogramowania, skorzystaj z procesu testowania oprogramowania.

Podobnie, wszelkie inne systemy operacyjne, przeglądarki lub platformy, takie jak tablety mobilne, muszą być oceniane przy użyciu innych procedur testowych.


Kolejność testów
-------------

Numeracja testów w ramach procesu testowego niekoniecznie wskazuje kolejność, w jakiej testy muszą być wykonywane. Każdy tester i każda aplikacja może określić optymalną kolejność testowania pod kątem zasięgu i wydajności.

Zaleca się jednak, aby pierwszym przeprowadzonym testem był Test 1 Zgodne wersje alternatywne. Identyfikacja zgodnych alternatywnych wersji treści pomaga określić zakres testowania i uniknąć niepotrzebnych testów. Treści niezgodne z wymaganiami, która ma zgodną wersję alternatywną, są wyłączane z testowania.

Test 2 Automatyczne odtwarzanie i automatyczna aktualizacja treści oraz Test 3 Miganie są następne w procesie testowym, a kolejnym Test 4 Dostęp z klawiatury i fokus. Testują one kryteria sukcesu WCAG, które są objęte wymogiem zgodności [Wymaganie zgodności 5 Brak zakłóceń](https://wcag.irdpl.pl/understanding/zgodnosc#conf-req5). Niespełnienie tych kryteriów sukcesu może zakłócić korzystanie ze strony i wskazywać na krytyczne problemy z dostępnością.

Proces testowania został zaprojektowany tak, aby usprawnić kolejność dla testerów; Testerzy mogą jednak zdecydować się na wykonanie testów (po Testach 1) w preferowanej przez siebie kolejności. Każdy warunek testowy (po teście 1) jest niezależny od poprzedzających go testów, ale niektóre z nich będą odwoływać się do kolejnych testów.

Problemy nieobjęte tym procesem testowym
---------------------------------------

Podczas testowania mogą zostać znalezione problemy, które mogą wpływać na dostępność, ale są to po prostu błędy w kodowaniu i często wpływają na ogólną użyteczność dla wszystkich użytkowników. Przykładem może być łącze, który prowadzi do niewłaściwej strony docelowej. Testerzy mogą powiadomić programistę o tych problemach w formie komentarza do raportu, ale zazwyczaj błędy te nie powodują braku zgodności, ponieważ wykraczają poza zakres zmienionych standardów Sekcji 508.


Objaśnienie każdego testu
---------------------------

Poprzednie wersje dokumentu procesu Trusted Tester zawierały objaśnienie dla każdego testu oparte na interpretacji norm z Sekcji 508. Po odświeżeniu standardów w sekcji 508 i przyjęciu kryteriów sukcesu WCAG 2.0, ta wersja procesu testowego opiera się głównie na objaśnieniach przedstawionych w [*Objaśnienia WCAG 2.0: Przewodnik do zrozumienia i wdrożenia Wytycznych dla dostępności treści internetowych 2.0*](https://www.w3.org/TR/UNDERSTANDING-WCAG20/). Proces testowania opiera się również na towarzyszącym szkoleniu dla zaufanych testerów, które zapewnia dodatkowy opis i wskazówki dotyczące zrozumienia logiki, która prowadzi każdy test. Każdy krok zawarty w tym dokumencie procesu testowego zawiera tylko informacje niezbędne do wykonania testu. Jednakże sekcja <q>Obowiązujące wymagania</q>" każdego testu odwołuje się do odpowiedniej normy WCAG 2.0 lub sekcji 508 wraz z łączem do odpowiedniego artykułu z dokumentu *Objaśnienia WCAG 2.0*.

