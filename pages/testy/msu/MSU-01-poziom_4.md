---
title: Poziom 4


sidebar: testy_sidebar
datatable: true
permalink: MSU-01-poziom-4
folder: testy/msu
---



Zawsze należy wypełnić wszystkie poziomy dokładności (zobacz: [Wprowadzenie](MSU_00_wprowadzenie), aby uzyskać szczegółowe informacje). Zobacz: [Narzędzia audytora dostępności cyfrowej](nod_wprowadzenie#walidatory-kontrastu-i-koloru) - walidatory kontrastu i koloru.

| Test        | Protokoły                    |OK|Źle|ND| Uwagi  |KS WCAG|
|-------------|------------------------------|--|---|--|--------|--------|
|1. Tabele i listy (Czytnik ekranu)|Poruszając się po tabeli za pomocą czytnika ekranu (np. klucz "t" w NVDA), upewnij się, że wszystkie tabele na każdej stronie są identyfikowane przez czytnik ekranu jako tabele oraz że tabele są odpowiednio ustrukturyzowane. Upewnij się, że nagłówki tabel (np. zawartość pierwszego wiersza) są odczytywane dla wszystkich komórek, które organizują (np. wszystkie komórki w tej kolumnie). Poruszając się po tabeli za pomocą czytnika ekranu (np. klucze "L" i "i" w NVDA), upewnij się, że wszystkie listy na każdej stronie są identyfikowane przez czytnik ekranu jako listy oraz że są odpowiednio ustrukturyzowane.| | | | |[1.3.1](https://wcag.lepszyweb.pl/#info-and-relationships)|
|2. Po otrzymaniu fokusa|Użyj klawisza tabulatora na klawiaturze, aby przejść przez każdą stronę i upewnić się, że oznaczenie fokusem któregoś z elementów nie spowoduje automatycznej zmiany zawartości.| | | | |[3.2.1](https://wcag.lepszyweb.pl/#on-focus)|
|3. Podczas wprowadzania danych|Upewnij się, że podczas wprowadzania danych w formularzach (np. zaznaczenie pola wyboru, opcji w menu rozwijanym itp.) nie spowoduje nieoczekiwanej zmiany zawartości, np. przeładowania strony.| | | | |[3.2.2](https://wcag.lepszyweb.pl/#on-input)|
|4. Nawigacja pomijająca|Upewnij się, że na każdej stronie znajduje się tylko jeden nagłówek 1 i że znajduje się on na początku unikalnej zawartości strony (np. zawartość po głównej nawigacji i bannerach witryny), znajdując go za pomocą klawiatury w czytniku ekranu (np. klucz "h" w NVDA) lub że na samym początku każdej strony znajduje się link, który po aktywacji kieruje na początek unikalnej zawartości strony.| | | | |[2.4.1](https://wcag.lepszyweb.pl/#bypass-blocks)|
|5. Kontrast kolorów (CCA)|Użyj narzędzia analizatora kontrastu kolorów, aby upewnić się, że wszystkie teksty i ikony (bez logo i nieaktywnej zawartości) mają wystarczający kontrast w stosunku do tła, na którym się znajdują (4,5:1 dla zwykłego tekstu i 3:1 dla dużego tekstu).| | | | |[1.4.3](https://wcag.lepszyweb.pl/#contrast-minimum)|
|6. Powiększenie|Powiększaj każdą stronę (przy użyciu funkcji powiększenia przeglądarki) do 200% i upewnienie się, że cała zawartość jest nadal widoczna i w pełni funkcjonalna.| | | | |[1.4.4](https://wcag.lepszyweb.pl/#resize-text)|
|7. Cel łącza (w kontekście)|Upewnij się, że miejsca docelowe/funkcje wszystkich łączy/przycisków na każdej stronie są jasno określone przez tekst łącza/przycisku i poprzedzający go kontekst (tzn. użytkownik nie powinien być zaskoczony tym, dokąd zmierza lub co się dzieje).| | | | |[2.4.4](https://wcag.lepszyweb.pl/#link-purpose-in-context)|
