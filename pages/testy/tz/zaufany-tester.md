---
title: O procesie testowym Trusted Tester
summary: "Proces testowy Trusted Tester został pierwotnie stworzony przez Biuro Dostępnych Systemów i Technologii (OAST) w Departamencie Bezpieczeństwa Wewnętrznego (DHS) Stanów Zjednoczonych, a później przyyjęty przez kilka innych amerykańskich agencji federalnych. Jest to zestaw procedur testowych, ktorych celem jest stwierdzenie zgodności treści stron internetowych ze Zmienioną Sekcją 508, która w całości implementuje WCAG 2.1."

sidebar: testy_sidebar
permalink: zaufany-tester
folder: testy/tz
last_updated: 24 maja 2020
---

O dokumencie
===================

Kto powinien korzystać z tego dokumentu
----------------------------

Niniejszy dokument został zaprojektowany i jest przeznaczony do użytku przez Trusted Testerów.

Zaufany Tester to osoba certyfikowana do zapewniania dokładnych i powtarzalnych wyników testów zgodności treści stron internetowych ze Zmienioną Sekcją 508. Zaufany tester postępuje zgodnie ze zmienionym procesem testowania zgodności stron internetowych z sekcją 508, używa zatwierdzonych narzędzi testowych i ocenia aplikacje internetowe pod kątem zgodności ze Zmienionymi  normami 508. Zaufani testerzy to osoby, które zdały egzamin certyfikacyjny Trusted Tester.

Aby uzyskać więcej informacji na temat Zrewidowanego Kursu Szkoleniowego i Egzaminu dla Zaufanych Testerów 508, skontaktuj się z Biurem Pomocy ds. Dostępności Systemów i Technologii Departamentu Bezpieczeństwa Wewnętrznego (OAST), dostępnym pod adresem <accessibility@dhs.gov>.

Harmonizacja z testami podstawowymi
-----------------------------
Ten proces testowy obejmuje wszystkie testy zawarte w wersji 3.0 dokumentu "Zharmonizowane procesy dla Zmienionych testów 508": Podstawowe testy dostępności stron internetowych". Testy podstawowe ustanowiły minimalne kroki wymagane do ustalenia zgodności ze zaktualizowanymi normami Sekcji 508 oraz WCAG 2.0 poziom A i AA. Instrukcje testowe, które są specyficzne tylko dla Trusted Testera, są oznaczone jako *specyficzne dla TT specific* lub "bez linii bazowej". Wyniki tych testów będą odzwierciedlane tylko w wynikach zmienionych testów  508.

Wyniki testów podstawowych będą raportowane osobno i nie będą miały wpływu na wyniki testów specyficznych dla Trusted Testera.



Jak wygląda struktura tego dokumentu
-------------------------------

-   Treść wprowadzająca:

    -   O tym dokumencie - opisuje cel, odbiorców i zakres tego dokumentu Rozdział 1

    -   Środowisko testowe - opisuje środowiska testowe obsługiwane przez ten proces testowy, w tym systemy operacyjne, przeglądarki i narzędzia testujące

    -   Wymagania dotyczące raportowania zgodności - zawiera wytyczne

-   Sekcja 508 Testy zgodności - szczegółowo opisuje procesy testowe. Każdy proces testowy zawiera instrukcje krok po kroku dotyczące tego, jak i co testować, a także instrukcje określania wyników testu dla każdego Warunku testowego.

-   Załączniki - Zawierają tabele referencyjne wskazujące związek między Testów ze Zmienionymi standardami 508 i testami podstawowymi; definicje; dziennik zmian w dokumencie; oraz krótkie podsumowania procesu testowego.

Tylko testy dostępności treści internetowych
----------------------

Ten proces testowy obejmuje tylko treści internetowe.  Zaufany Tester w wersji 4.x i starszych został opracowane dla oryginalnej normy Section 50, która miały osobne wymagania dotyczące sieci i oprogramowania. Wraz ze zmienionymi standardami 508 stosującymi WCAG 2.0 poziom A i AA do sieci, oprogramowania i innych treści elektronicznych, pierwotnym planem było połączenie testów oprogramowania i stron internetowych w jednym procesie testowym.

Ponieważ jednak Zmienione standardy 508 oprócz WCAG 2.0 mają inne wymagania dotyczące oprogramowania, a narzędzia do testowania oprogramowania nie były jeszcze dostępne, proces testowania oprogramowania będzie odrębny. Chociaż nie jest to tak powszechne ze względu na możliwości HTML5, elementy oprogramowania nadal znajdują się w treści WWW w aplikacjach internetowych. Aby przetestować elementy oprogramowania, skorzystaj z procesu testowania oprogramowania.

Podobnie, wszelkie inne systemy operacyjne, przeglądarki lub platformy, takie jak tablety mobilne, muszą być oceniane przy użyciu innych procedur testowych.


Kolejność testów
-------------

Numeracja testów w ramach procesu testowego niekoniecznie wskazuje kolejność przeprowadzenia testów. Każdy z testerów i każdy z wnioskujących może określić optymalną kolejność testowania pod kątem zasięgu i wydajności.

Zaleca się jednak, aby pierwszym przeprowadzonym testem był Test 1 Zgodne wersje alternatywne. Identyfikacja zgodnych alternatywnych wersji treści pomaga określić zakres testowania i pozwala uniknąć niepotrzebnych testów. Treści niezgodne z wymaganiami, które posiadają zgodną wersję alternatywną, są wyłączane z testów. 

Test 2 Automatyczne odtwarzanie i automatyczna aktualizacja treści oraz Test 3 Miganie są następnie w procesie testowym, a następnie Test 4 Dostęp z klawiatury i fokus. Te testowe kryteria sukcesu WCAG są uwzględnione w [Wymaganie zgodności 5 Brak zakłóceń] (https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html). Niespełnienie tych kryteriów powodzenia może kolidować może kolidować z jakimkolwiek użytkowaniem ze strony i może wskazywać na krytyczne problemy z dostępnością.

Proces testowania został zaprojektowany tak, aby usprawnić sekwencję dla testerów; jednakże testerzy mogą zdecydować się na przeprowadzenie testów (po teście 1) w preferowanej przez siebie kolejności. Każdy warunek testu (po teście 1) jest niezależny od testów poprzedzających, ale niektóre z nich odnoszą się do testów, które następują po nim.

Problemy nieobjęte tym procesem testowym
---------------------------------------

Podczas testów mogą pojawić się problemy, które mogą wpływać na dostępność, ale są to po prostu błędy w kodowaniu i często wpływają na ogólną użyteczność dla wszystkich użytkowników. Przykładem może być łącze, który prowadzi do niewłaściwej strony docelowej. Testerzy mogą powiadomić programistę o tych problemach w formie komentarza do raportu, ale zazwyczaj błedy te nie powodują braku zgodności, ponieważ wykraczają poza zakres zmienionych standardów Sekcji 508.


Uzasadnienie każdego testu
---------------------------

Poprzednie wersje dokumentu procesu Trusted Tester zawierały uzasadnienie dla każdego testu oparte na interpretacji standardów z sekcji 508. Po odświeżeniu standardów w sekcji 508 i przyjęciu kryteriów sukcesu WCAG 2.0, ta wersja procesu testowego opiera się głównie na uzasadnieniu przedstawionym w [*Zrozumieć WCAG 2.0: Przewodnik do zrozumienia i wdrożenia Wytycznych dotyczących dostępności treści WWW 2.0*](https://www.w3.org/TR/UNDERSTANDING-WCAG20/). Proces testowy opiera się również na towarzyszącym szkoleniu Trusted Tester w celu zapewnienia dodatkowego opisu i wskazówek pozwalających zrozumieć logikę, która prowadzi każdy test. Każdy krok zawarty w tym dokumencie zawiera jedynie informacje niezbędne do wykonania testu. Jednakże sekcja "Obowiązujące normy" w każdym teście odnosi się do odpowiedniej normy WCAG 2.0 lub sekcji 508 wraz z łączem do odpowiedniego artykułu z dokumentu *Understanding WCAG 2.0*.


