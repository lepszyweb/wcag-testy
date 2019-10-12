# Mruganie, miganie, błyskanie, przesuwanie, automatyczna aktualizacja

### Metoda badania: 
Kontrola wzrokowa, testowanie ręczne, testowanie przy użyciu specjalistycznych narzędzi.

### Zastosowanie:
Wszelkie treści, które się poruszają, błyskają, migają, przesuwają, zmieniają automatycznie. 
Uwaga: Miganie oznacza treść, która zmianami swego stanu może rozpraszać uwagę. Miganie jest  dozwolone przez krótki czas, jeśli się zatrzyma lub zostanie zatrzymane.
Błyskanie treści oznacza dwie lub więcej zmian stanów, które różnią się znacznie kontrastem, i odnosi się do treści, które mogą wywołać napady padaczki światłoczułej, gdy są częstsze niż 3 na sekundę oraz wystarczająco duże i jasne. Nie są dozwolone nawet przez sekundę, ponieważ mogą wywołać napad. Nie ma znaczenia, czy można je zatrzymać, ponieważ napad może nastąpić przed wyłączeniem. Mruganie zwykle nie jest częstsze, niż 3 razy na sekundę. Gdyby było częstsze, należy uznawać je za błyski.

### Oczekiwania:
Kryteria sukcesu: [2.2.2. Wstrzymywanie (pauza), zatrzymywanie, ukrywanie](https://wcag.lepszyweb.pl/#pause-stop-hide), [2.3.1 Trzy błyski lub wartości poniżej progu](https://wcag.lepszyweb.pl/#three-flashes-or-below-threshold)
-	Nic nie miga częściej niż trzy razy na sekundę (sytuacja preferowana) ALBO
    - Migający obszar jest wystarczająco mały LUB
    - Miganie nie przekracza dozwolonych wartości granicznych dla błysków ogólnych i czerwonych
-	Użytkownik może wstrzymać, zatrzymać lub ukryć, a także wznowić każdą treść ruchomą i odtwarzaną automatycznie
-	Użytkownik może dostosować częstotliwość aktualizacji treści zmienianej dynamicznie 

### Procedura testowania:
1.	Określ częstotliwość migania. Jeśli częstotliwość migania wynosi 3 Hz lub mniej (trzy błyski w ciągu jednej sekundy), dalsze badanie nie jest konieczne.
2.	Jeśli zawartość miga powyżej 3 Hz lub nie można ustalić częstotliwości, sprawdź, czy spełnia ona jedną z następujących warunków:
    - Łączny obszar błysków pojawiających się jednocześnie nie przekracza „małego bezpiecznego obszaru” w obrębie 10 stopni pola widzenia monitora dla osoby patrzącej na monitor z przeciętnej odległości.
    - Pary przeciwstawnych przejść nie zawierają ostrej/nasyconej czerwieni ORAZ
      - Względna luminancja najciemniejszego obrazu wynosi powyżej 0,80 lub
      - Względna luminancja najciemniejszego obrazu wynosi poniżej 0,80, a maksymalna zmiana względnej luminancji między najciemniejszym i najjaśniejszym obrazem wynosi mniej niż 10%.
3.	Sprawdź, czy istnieje mechanizm umożliwiający użytkownikowi wstrzymanie, zatrzymanie lub ukrycie treści, które się poruszają, przesuwają, migają, są aktualizowane automatycznie.
4.	Sprawdź, czy istnieje mechanizm dostosowania częstotliwości, z jaką następuje automatyczna aktualizacja treści.   

### Pomocne narzędzia:
-	[PEAT](https://trace.umd.edu/peat) - narzędzie do analizy ryzyka padaczki światłoczułej. Bezpłatne narzędzie dla programistów, redaktorów, autorów. PEAT może pomóc autorom ustalić, czy animacje lub wideo w ich treści mogą powodować napady padaczkowe.
-	[Harding FPA](https://www.hardingfpa.com/) - komercyjna aplikacja do badania zgodności z normami dotyczącymi migania w materiałach wideo  