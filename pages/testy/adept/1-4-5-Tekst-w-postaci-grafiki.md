---
title: 1-4-5 Tekst w postaci grafiki


sidebar: testy_sidebar
permalink: 1-4-5-Tekst-w-postaci-grafiki
folder: testy/adept
---

## Test
**Czy publikowane w serwisie teksty są zamieszczane w postaci jawnego tekstu, z wyjątkiem sytuacji, gdy jest to absolutnie niezbędne?**

## Wyjaśnienie
Dosyć często zdarza się, że dokumenty są publikowane w serwisie internetowym jako grafika przedstawiająca tekst. Najczęściej problem ten pojawia się w wypadku plików PDF, ale także wówczas, gdy projektant chce zaprezentować jakiś układ typograficzny trudny do uzyskania w HTML i CSS. Taka graficzna prezentacja jest całkowicie niedostępna dla osób niewidomych i częściowo dla słabowidzących. Pierwsi nie są w stanie w ogóle odczytać takiej informacji, a drudzy nie mogą jej dostosować do własnych potrzeb. Specyfikacja WCAG 2.0 na poziomie AA robi wyjątek dla sytuacji, gdy taka prezentacja tekstu jest kluczowa i niemożliwa do osiągnięcia w inny sposób. Przykładem mogą być tu starodruki, mapy, czy logotypy. Jednak uzasadnieniem nie mogą już być względy estetyczne.

## Testowanie
Przyjrzyj się publikowanym w serwisie internetowym plikom PDF, czy zawierają jawny tekst, czy może tylko zeskanowane obrazy dokumentów papierowych. Możesz też spróbować zapisać taki plik do formatu tekstowego, na co pozwala przeglądarka Adobe Reader. Spróbuj zaznaczyć fragment tekstu i wykopiować go do innego dokumentu. Przyjrzyj się też elementom graficznym (przyciski, bannery), które zawierają informację tekstową. Sprawdź, czy można ten tekst zaznaczyć i przekopiować w inne miejsce. Możesz też użyć bezpłatnego czytnika ekranu NVDA, by sprawdzić jaką informację uzyska niewidomy użytkownik.

-	czytnik ekranu NVDA http://www.nvaccess.org/
