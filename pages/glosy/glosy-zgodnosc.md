---
title: Zgodność
summary: "Zgodność - spełnienie wszystkich wymagań danej normy, wytycznych lub specyfikacji."

sidebar: glosy_sidebar
permalink: glosy-zgodnosc
folder: glosy
---
Ta sekcja pełni funkcję <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.normatywny}}">normatywną</a>.


W tej sekcji znajdują się wymagania dotyczące <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.zgodnosc}}">zgodności</a> z wytycznymi WCAG 2, jak również informacje, w jaki sposób można ogłosić zgodność strony (opcjonalnie). Na końcu wyjaśnione zostało pojęcie wsparcia dla dostępności, gdyż tylko <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc}}">technologie wspierające dostępność</a> mogą stanowić <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.stanowiace_podstawe_zgodnosci}}">wiarygodną podstawę zgodności</a>. Dokument o nazwie [„Understanding Conformance”](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html) zawiera dalsze wyjaśnienie pojęcia <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc}}">wsparcia dla dostępności</a>.

### Wymogi zgodności

Aby strona internetowa była zgodna z wytycznymi WCAG 2.0, wszystkie poniższe wymogi zgodności muszą zostać spełnione:

1. **Poziom zgodności**: Jeden z poniższych poziomów zgodności jest w pełni osiągnięty:
  - **Poziom A**: Aby osiągnąć poziom zgodności A (poziom minimalny), <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa}}">strona internetowa</a> <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.spelnienie_kryterium_sukcesu}}">spełnia</a>   wszystkie kryteria sukcesu na poziomie A, lub też dostępna jest <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.wersja_alternatywna_zapewniajaca_zgodnosc}}">wersja alternatywna spełniająca kryteria sukcesu</a> na poziomie A.
  - **Poziom AA**: Aby osiągnąć poziom zgodności AA, strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A oraz na poziomie AA, lub też dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie AA.
  - **Poziom AAA**: Aby osiągnąć poziom zgodności AAA, strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A, na poziomie AA oraz na poziomie AAA, lub też dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie AAA.

    *Uwaga 1:* Chociaż zgodność może zostać osiągnięta tylko na oznaczonych poziomach, zachęca się autorów, aby podawali (w oświadczeniu zgodności) jakikolwiek postęp na drodze do spełnienia kryteriów sukcesu na poziomach wyższych niż osiągnięty.

    *Uwaga 2:* Odradza się wyznaczania poziomu AAA jako wymaganego dla całych serwisów, gdyż w przypadku niektórych treści, spełnienie wszystkich kryteriów sukcesu na poziomie AAA nie jest możliwe.

2. **Całe strony**: <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.zgodnosc}}">Zgodność</a> (oraz poziomy zgodności) dotyczy całej <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa}}">strony</a> i nie można jej osiągnąć, jeśli jakaś część strony zostanie wyłączona z oceny.

    *Uwaga 1:* W celu ustalenia zgodności, przyjmuje się, iż wersje alternatywne części treści strony są częścią strony, jeśli wersje alternatywne są dostępne bezpośrednio z danej strony, np. długi opis lub alternatywna prezentacja nagrania wideo.

    *Uwaga 2:* Autorzy stron internetowych, którzy nie mogą osiągnąć zgodności ze względu na treść pozostającą poza ich kontrolą, mogą rozważyć [Stwierdzenie częściowej zgodności](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#conformance-partial).

3. **Zakończona procedura**: Jeśli dana <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa}}">strona</a> jest jedną z wielu stron prezentujących jakąś <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa}}">procedurę</a> (tzn. sekwencję kroków, które należy wykonać, aby dokończyć jakąś czynność), to wszystkie te strony osiągają co najmniej ten sam lub wyższy poziom zgodności. (Zgodność na wybranym poziomie nie jest możliwa, jeśli którakolwiek ze stron nie spełnia wybranego poziomu.)

   *Przykład:* Sklep internetowy prezentuje na kilku stronach procedurę wybierania i zakupu produktów. Wszystkie strony w tej procedurze, od początku do końca (do wykonania płatności) są zgodne na tym samym poziomie.

4. **Użycie technologii wspierających dostępność**: Tylko <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.obslugiwana_przez_dostepnosc}}">technologie wspierające dostępność</a> są uwzględniane jako podstawa spełnienia kryteriów sukcesu. Każda informacja czy funkcjonalność, która nie jest dostarczona w postaci wspierającej dostępność, ma swoją alternatywną wersję wspierającą dostępność. (Więcej informacji: [Understanding accessibility suport](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-accessibility-support-head)).

5. **Brak zakłóceń**: Jeśli na stronie wykorzystywane są technologie, które nie wspierają dostępności lub są użyte tak, że nie wspierają dostępności, użytkownicy powinni mieć swobodny dostęp do pozostałej części strony. Dodatkowo, <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.strona_internetowa}}">strona</a> nadal spełnia wymogi zgodności pod każdym z następujących warunków:

    1. kiedy technologia, która nie jest <a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.stanowiace_podstawe_zgodnosci}}">uwzględniana</a>, jest włączona w programie użytkownika,
    2. kiedy technologia, która nie jest uwzględniana, jest wyłączona w programie użytkownika, oraz
    3. kiedy technologia, która nie jest uwzględniana, nie jest wspierana przez program użytkownika.

 Dodatkowo, następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony:

  - 1.4.2 Kontrola odtwarzania dźwięku
  - 2.1.2 Brak pułapki na klawiaturę
  - 2.3.1 Trzy błyski lub wartości poniżej progu
  - 2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie

  *Uwaga:* Jeśli strona nie jest zgodna (na przykład testowa strona zgodności lub strona przykładowa), nie może być włączona w zakres zgodności lub dołączona do oświadczenia zgodności.

Więcej informacji, w tym przykłady, w [Understanding Conformance Requirements](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conformance-requirements-head).
