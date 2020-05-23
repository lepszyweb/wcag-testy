---
title: 3. Migotanie


sidebar: testy_sidebar
permalink: tz-03-migotanie
folder: testy/tz
---



## Treść migająca

Celem tej procedury testowej jest ustalenie, czy strony internetowe zawierają treść, która migocze. Jasne migotanie z gwałtowną zmianą luminancji, zmiany koloru od lub do nasyconej czerwieni, animacje wzorów geometrycznych składajacych się z naprzemiennie występujących jasnych i ciemnych elementów znacznie zwiększają ryzyko wystąpienia napadu epileptycznego nie tylko u osób cierpiących na padaczki fotogenne, ale taże u osób zdrowych.

Ponieważ dotychczas nie określono narzędzia, które może odpowiednio ułatwić walidację zgodności dla tresci migoczącej, w procesie Trusted tester proponuje się oznaczyć przypadki takiej treścic jako nietestowane.

### Test 3.A 2.3.1-migotanie

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 2.3.1-migotanie | 3.A     | Na stronie internetowej nie ma treści migających, które mogą wywołać napady epileptyczne |


### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa.

2.	[PEAT](https://trace.umd.edu/peat) - narzędzie do analizy ryzyka padaczki światłoczułej. Bezpłatne narzędzie dla programistów, redaktorów, autorów. PEAT może pomóc autorom ustalić, czy animacje lub wideo w ich treści mogą powodować napady padaczkowe.

### Identyfikacja treści
Wzrokowo określ treść, która migocze. Treść migająca to treść, która szybko zmienia się między dwoma lub więcej stanami, różniącymi się znacznie kontrastem.


Miganie oznacza gwałtowne zmiany jasności, koloru od lub do nasyconej czerwieni, jasnych i ciemnych wzorów geometrycznych, które mogłyby spowodować napad epileptyczny, gdyby byłyby wystarczająco jasne lub utrzymywały się wystarczająco długo.


### Zastosowanie

Test 3.A 2.3.1-migotanie  **nie ma zastosowania**, jeśli na stronie nie zostanie wykryta treść migocząca. W takim przypadku oznacz wynik testu jako **ND**. 

### Jak testować
Możesz zastosować narzędzie [PEAT](https://trace.umd.edu/peat).


### Ocena wyników
Jeśli korzystasz z narzędzia [PEAT](https://trace.umd.edu/peat), ustal ocenę wyników na podstawie rpzeprowadzonego testu.

**Uwaga**: Określono wiele wymagań dla zgodności treści błyskających i migoczących. Aby ustalić, czy wymagania są spełnione, potrzebne jest automatyczne narzędzie testujące, ale w systemie oceniania  Trusted tester uznano, że obecnie takie narzędzie nie jest dostępne. Dlatego, dopóty nie zostanie okreśłone konkretne narzędzie testowe, nalezy ocenić wynik testu 3.A 2.3.1-migotanie jako **nie testowano**. 

Do czasu określenia odpowiedniego narzędzia testującego wynik **Nie testowano** będzie wskazywał, że na stronie znaleziono treść błyskającą (migoczącą).

**Ważne**: Ten test jest wyjatkowy. Ponieważ w procesie Trusted tester nie określono odpowiedniego narzędzia testującego i w zwiazku z tym nie ma uznanej metody, która pozwalałaby stwierdzić, czy treść migocząca spełnia dopuszczalne normy, to jedynymi opcjami oceny wyników są: 

-	**Nie ma zastosowania**, jeśli nie ma tresci migoczącej (błyskjacej), **lub**
-	**Nie testowano**, jeśli na stronie internetowej istnieje treść migocząca (błyskjaca).

### Zastosowane standardy

{% include ks/2-3-1.md %}

[9. Błyskanie](ICT-09-blyskanie.md)                                                                                               
