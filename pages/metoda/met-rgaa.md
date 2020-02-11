---
title: Metoda RGAA
summary: "Metoda RGAA jest przykładem kompleksowej propozycji systemu oceniania zgodności stron internetowych z wymogami dostępności zdefiniowanymi w WCAG 2.0. Jest efektem doświadzeń francuskich."

sidebar: metoda_sidebar
permalink: met-rgaa
folder: metoda
---

## Historia metody
Początki metodyce RGAA dało francuskie stowarzyszenie [BraileNet](https://www.braillenet.org/), które już w 2003 roku opracowało i opublikowałło pod nazwą [AccessiWeb](https://www.braillenet.org/accessibilite-numerique/cadre-technique/), aby zapewnić ujednolicone podejście do kontroli zgodności usług sieciowych dla WCAG. Ta metoda została szeroko rozpowszechniona zastosowana we Francji oraz w&nbsp;świecie francuskojęzycznym.

W 2009 roku francuska administracja rządowa opublikowała pierwszą wersję „ogólnych wytycznych dostępności dla administracji” („Référentiel Général d'Accessibilité des Administrations”, w&nbsp;skrócie RGAA). Wytyczne były adaptacją WCAG 2.0 na potrzeby administracji francuskiej, wzbogaconą o&nbsp;szczegółowe instrukcje oceniania zgodności. W&nbsp;wytycznych wykorzystano dorobek stowarzyszenia BraileNet.

W 2014 roku stowarzyszenie BraileNet z grupą firm wygrało przetarg na aktualizację RGAA, w wyniku którego zostało wykonawca tego rządowego zamówienia. 29 kwietnia 2015 roku udostępniono wersję 3.0 RGAA, która w&nbsp;dużej mierze korzysta z&nbsp;repozytorium AccessiWeb HTML5/ARIA.   

W swej istocie RGAA to nie są tylko „ogólne wytyczne”, jak można by wnosić z&nbsp;nazwy. Jest to bogaty zasób cyfrowy, dostarczający precyzyjnych sposobów badania i&nbsp;oceniania dostępności stron internetowych.

### Polskie tłumaczenie RGAA

W 2018 roku tłumaczenie RGAA wykonane przez pracowników Ministerstwa Cyfryzacji udostępniono na stronie [Dostępność cyfrowa](https://www.gov.pl/web/dostepnosc-cyfrowa/francuska-metodyka-badania-dostepnosci-rgaa). Dzięki temu polskie zasoby poświęcone dostępności cyfrowej wzbogaciły się o&nbsp;niezwykle cenne i&nbsp;jedyne w&nbsp;takim wymiarze źródło metodyki oceniania dostępności.

Na podstawie tłumaczenia udostępnionego przez Ministerstwo Cyfryzacji Pracownia Dostępności Cyfrowej LepszyWeb.pl przygotowała i&nbsp;opublikowała [internetową wersję RGAA](https://rgaa.lepszyweb.pl) systematycznie poprawianą.


## Struktura RGAA

Całe repozytorium metody(ki) RGAA składa się z 6 sekcji:

1. **Kryteria i testy** - uporządkowane w 13 kategorii - tematów,
2. **Słownik** - definiujący i ujednoznaczniający stosowane terminy,
3. **Przypadki szczególne** - prezentacja odstępstw od wymogów zdefiniowanych w kryteriach,
4. **Uwagi techniczne** - wyjaśnienia dotyczące obsługi niektórych elementów HTML5,
5. **Baza referencyjna** - kombinacje technologii, systemów operacyjnych i przeglądarek, które pozwalają stwierdzić, że oprogramowanie oparte na HTML5/ARIA „wspiera dostępność”, jak zdefiniowano w&nbsp;WCAG 2.0.
6. **Referencje** - lista wykorzystanych źródeł i referencji

### Kryteria i testy
Zdefiniowane w WCAG kryteria sukcesu zostały w RGAA przetransponowane na listę kryteriów i testów, które muszą być spełnione, aby zapewnić dostępność.

Specyfikacja RGAA zawiera ogółem blisko 280 testów dla 133 kryteriów uporządkowanych w&nbsp;13 kategorii. RGAA stosuje wprawdzie własne kryteria sukcesu, ale każde z&nbsp;nich jest zmapowane z&nbsp;odpowiednimi kryteriami sukcesu oraz technikami WCAG, co powoduje, że RGAA są **w pełni zgodne** z WCAG. Nie znaczy to - oczywiście - że odwrotne stwierdzenie jest prawdziwe. WCAG nie są w pełni zgodne z RGAA.

Kryteria i testy są zbudowane zgodnie z następującymi zasadami:

- Kryterium lub test zadaje pytanie.
- Kryterium lub test zadaje tylko jedno pytanie i czeka tylko na odpowiedź (uwaga: w przypadku testu ta reguła może mieć pewne wyjątki)
- Jeśli odpowiedź jest pozytywna, oznacza to, że kryterium jest spełnione, że stwierdzono zgodność z wymaganiami dostępności
- Kryterium jest powiązane z co najmniej jednym kryterium sukcesu WCAG, którego poziom jest następnie wywnioskowany z najniższego poziomu WCAG;
- Test lub warunki testu są powiązane przynajmniej z techniką WCAG lub elementem specyfikacji HTML (lub powiązanych uwag).
- Lista kryteriów poprzedzona jest instrukcją obsługi wyjaśniającą, jak korzystać z repozytorium, gdy kod źródłowy nie jest kodem HTML5.

Lista kryteriów składa się z 13 tematów:

- Obrazy
- Ramki
- Kolory
- Multimedia
- Tabele
- Łącza
- Skrypty
- Elementy obowiązkowe
- Informacje o strukturze
- Prezentacja informacji
- Formularze
- Nawigacja
- Przeglądanie

Do każdego tematu dołączono informację wskazującą:

- Powiązane z tematem zasady WCAG (postrzegalność, funkcjonalność, zrozumiałość, rzetelność);
- Ogólne zalecenie dostępności w formie jednego lub dwóch zdań podsumowujących cele tematu.

Następnie pojawia się lista kryteriów sformułowanych w postaci pytań. Każde kryterium posiada swój numer - identyfikator i oznaczone jest poziomem dostępności WCAG (A, podwójne A lub potrójne A) .

Poniżej każdego kryterium znajduje się zestaw testów, definiujących procedury sprawdzania, czy kryterium jest spełnione, oraz łącze do uwag technicznych, jeśli istnieją.

Na końcu znajduje się mapowanie reguł i testów RGAA do międzynarodowego standardu WCAG w następujący sposób:

- Lista kryteriów sukcesu WCAG (normatywny składnik WCAG), których dotyczy mapowane kryterium RGAA
- Lista technik wystarczających do spełnienia kryterium i lista błędów (awarii; nienormatywny składnik WCAG) związanych z mapowanym kryterium RGAA

### Słownik
Aby zapewnić lepsze zrozumienie dokumentacji technicznej, wyjaśnić i ujednoznacznić terminy dodano słownik. Każdy termin zdefiniowany w słowniku jest powiązany bezpośrednio z listą kryteriów. Definicje stanowią integralną część repozytorium i mają wartość normatywną.

Uwaga dotycząca polskiego tłumaczenia: W tłumaczeniu terminów na języku polski starano się z jednej strony zachować w możliwie największym stopniu wierność oryginałowi, a z drugiej uwzględnić wszędzie gdzie to możliwe, rodzimą tradycję językową.

### Przypadki szczególne
Wiele kryteriów RGAA odnosi się do przypadków szczególnych, w których zastosowanie kryterium może podlegać różnym ograniczeniom lub wyjątkom. W dokumencie Przypadki szczególne wymieniono wszystkie przypadki, w których dane kryterium nie ma zastosowania.

### Uwagi techniczne
W uwagach technicznych podano wyjaśnienia dotyczące obsługi niektórych elementów HTML5, których obsługa może być zmienna, oraz sposób, w jaki repozytorium proponuje ich obsługę.

### Baza referencyjna
Wiele kryteriów RGAA odnosi się do testów wykonywanych z użyciem różnych technologii wspomagających, przeglądarek i systemów operacyjnych. Ten dokument określa zestaw technologii, w oparciu o które należy przeprowadzać testy, aby przekonać się o dostępności dla jak najszerszej grupy odbiorców.

### Referencje
Specyfikacja RGAA została sporządzona z wykorzystaniem różnych referencji i źródeł. Dokument referencyjny podaje listę użytych referencji.
