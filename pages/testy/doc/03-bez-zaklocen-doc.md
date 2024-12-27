---
title: 3. Bez zakłóceń (dokumenty)
last_updated: 22 grudnia 2024

sidebar: testy_sidebar
permalink: 03-bez-zaklocen-doc
folder: testy/doc
---

## 3. Bez zakłóceń

## Wymagania dostępności

-   [5.2 Wymagania zgodności: Bez zakłóceń](https://wcag.irdpl.pl/guidelines/22/#cc5) - Poniższe kryteria sukcesu dotyczą wszystkich treści na stronie, włącznie z treściami, które w&nbsp;innych przypadkach nie są podstawą spełnienia wymogów zgodności, ponieważ ich niespełnienie może zakłócać korzystanie ze strony:
    -   1.4.2 - Kontrola odtwarzania dźwięku,
    -   2.1.2 - Bez pułapki na klawiaturę,
    -   2.3.1 - Trzy błyski lub wartości poniżej progu, oraz
    -   2.2.2 - Pauza, zatrzymanie, ukrycie.

## Uzasadnienie metody testowej
Wyniki tego testu podstawowego ustala się na podstawie wyników testów dla KS 1.4.2 (21.4-AudioControl), KS 2.1.2 (1.B-NoKeyboardTrap), KS 2.3.1 (9.A-Flashes) i KS 2.2.2 (21.B-MovingInfo i 21.C-AutoUpdate).

## Ograniczenia, założenia lub wyjątki

Brak.

## 3.A Procedura testu dla Wymagania zgodności 5

Identyfikator testu bazowego: *3.A-Bez-zaklocen*

### Identyfikacja treści

<p id="d3aIC">Wyniki testów podstawowych <a href="{{site.baseurl}}/document-baselines/21TimedEventsDocs/#21d-test-procedure-for-audio-control">21.D-AudioControl</a>, <a href="{{site.baseurl}}/document-baselines/01KeyboardDocs/#1b-test-procedure-for-no-keyboard-trap">1.B-NoKeyboardTrap</a>, <a href="{{site.baseurl}}/document-baselines/09FlashingDocs/#9a-test-procedure-for-three-flashes-or-below-threshold">9.A-Flashes</a>, <a href="{{site.baseurl}}/document-baselines/21TimedEventsDocs/#21b-test-procedure-for-moving-information">21.B-MovingInfo</a>, and <a href="{{site.baseurl}}/document-baselines/21TimedEventsDocs/#21c-test-procedure-for-auto-updating-information">21.C-AutoUpdate</a>.</p>

### Instrukcja testowania
1.  

<ol id="d3aTI">
    <li id="d3aTI-1">Sprawdź, czy wszystkie powyższe testy zakończyły się powodzeniem (zostały zaliczone). [CR5]</li>
</ol>

#### Test Results

<p id="d3aTR">Jeżeli którakolwiek z testów zakończył się niepowodzeniem, wówczas test podstawowy *3.A-Bez-zaklocen* kończy się niepowodzeniem.</p>

##  Poradnik: Wskazówki dotyczące usprawniania procesu testowego
-   Wszystkie testy wskazane w tym teście podstawowym muszą się zakończyć pomyślnie, aby cały test został uznany za zaliczony.
-   Narzędzie do raportowania może być wykorzystane do wygenerowania wyniku dla wymagania zgodności 5.

### Techniki WCAG 2.2
Nie dotyczy