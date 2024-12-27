---
title: "Podstawa testowania TIK dla dokumentów elektronicznych"
last_updated: 26 grudnia 2024

sidebar: testy_sidebar
permalink: doc-wprowadzenie
folder: testy/doc
---

# Podstawa testowania TIK dla dokumentów elektronicznych

## Wprowadzenie

Definicja [documentu](https://www.access-board.gov/ict/#defDocument) według sekcji 508:

> Logicznie odrębny zbiór treści (taki jak plik, zestaw plików lub media strumieniowe), który: funkcjonuje jako pojedyncza jednostka, a nie zbiór; nie jest częścią oprogramowania; i nie zawiera własnego oprogramowania do pobierania i prezentowania treści dla użytkowników. Przykłady dokumentów obejmują między innymi listy, wiadomości e-mail, arkusze kalkulacyjne, prezentacje, podcasty, obrazy i filmy.

Podstawa testowania dla dokumentów elektronicznych odnosi się wszystkie dokumentów [niebędących dokumentami internetowymi](https://www.access-board.gov/ict/#defNonWebDocument). (Dokument niebędący stroną internetową, zdefiniowany w sekcji 508, to dokument, który nie jest: stroną internetową, osadzony na stronie internetowej lub używany do renderowania lub funkcjonowania stron internetowych). Wersja 1.0 została wydana 30 września 2024 roku.

## Wymagania sekcji 508 dotyczące dokumentów

W tej sekcji przedstawiono [wymagania sekcji 508](https://www.access-board.gov/ict/#E205-content) dotyczące treści elektronicznych.

### E205 - Treść elektroniczna

#### E205.2 Treść publiczna

Treści elektroniczne skierowane do ogółu społeczeństwa muszą być zgodne z wymogami dostępności określonymi w [E205.4](#e205.4-accessibility-standard).

#### E205.3 Oficjalna komunikacja agencji

Treści elektroniczne, które nie są publicznie dostępne, są zgodne z wymogami dostępności określonymi w [E205.4](#e205.4-accessibility-standard), gdy takie treści stanowią oficjalną działalność i są przekazywane przez agencję za pośrednictwem co najmniej jednego z poniższych::

<ol type="A">
    <li>Powiadomienie alarmowe</li>
    <li>Wstępna lub ostateczna decyzja rozstrzygająca roszczenie lub postępowanie administracyjne.</li>
    <li>Wewnętrzne lub zewnętrzne ogłoszenie programu lub polityki.</li>
    <li>Powiadomienie o korzyściach, uprawnieniach do programu, możliwościach zatrudnienia lub działaniach personalnych.</li>
    <li>Formalne potwierdzenie odbioru.</li>
    <li>Kwestionariusz ankiety.</li>
    <li>Szablon lub formularz.</li>
    <li>Materiały edukacyjne lub szkoleniowe; lub</li>
    <li>Zawartość intranetowa zaprojektowana jako strona internetowa.</li>
</ol>

#### E205.4 Standard dostępności

Treść elektroniczna powinna być zgodna z kryteriami sukcesu i wymaganiami zgodności na poziomie A i AA w WCAG 2.2 (włączone przez odniesienie, [patrz 702.10.1](https://www.access-board.gov/ict/#702.10.1)).

**WYJĄTEK:**Dokumenty niebędące stronami internetowymi nie muszą być zgodne z następującymi czterema kryteriami sukcesu WCAG 2.2:

-   2.4.1 Możliwość pomijania bloków
-   2.4.5 Wiele dróg
-   3.2.3 Spójna nawigacja oraz
-   3.2.4 Spójna identyfikacja.

##### E205.4.1 Zastępowanie słów przy stosowaniu WCAG do dokumentów niebędących dokumentami internetowymi


W przypadku dokumentów niebędących dokumentami internetowymi, wszędzie tam, gdzie w kryteriach sukcesu i wymaganiach zgodności WCAG 2.2 poziomu A i AA pojawia się termin „strona internetowa” lub „strona”, terminy te zastępuje się terminem „dokument”. Ponadto w Kryterium sukcesu w punkcie 1.4.2 wyrażenie „na danej stronie” zastępuje się wyrażeniem „w dokumencie”.

## Niezależność od formatu pliku dokumentu i narzędzi testowych

Podobnie jak Podstawa testowania TIK dla Internetu, Podstawa testowania TIK dla dokumentów elektronicznych jest niezależna od narzędzi testowych. Każdy test bazowy identyfikuje testowany wymóg dostępności, zawartość dokumentu podlegającą ocenie oraz instrukcje krok po kroku dotyczące określania wyników testu. Agencje mogą stosować dowolne narzędzia, które są zgodne z tym poziomem bazowym, aby zapewnić spójne i wiarygodne wyniki testów.

## Autorzy Podstawy testowania

Autorem tej podstawy testowania jest Federalna Wspólnota Praktyk Dostępnych Dokumentów Elektronicznych (AED COP) i Techniczny Komitet Doradczy ds. Wykorzystuje on ramy Baseline for Web, mając na celu poprawę zgodności dostępności dokumentów elektronicznych.

## Docelowi odbiorcy
Podstawa testowania dla dokumentów elektronicznych jest najlepiej wykorzystywany przez twórców metodologii testowania. Jest mało prawdopodobne, aby pojedyncza metodologia testowania mogła skutecznie testować wiele formatów plików. Na przykład, metodologia testowa dla PDF może nie być przydatna dla Worda lub innego formatu pliku. Aby upewnić się, że metodologia testowania testuje wszystkie wymagania sekcji 508, należy uwzględnić każdy test podstawowy w metodologii testowania. 
