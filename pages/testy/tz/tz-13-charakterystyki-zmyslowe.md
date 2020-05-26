---
title: 13. Charakterystyki zmysłowe i kontrast


sidebar: testy_sidebar
permalink: tz-13-charakterystyki-zmyslowe
folder: testy/tz
---
## Cel scenariusza testowego 
Celem tego scenariusza testowego jest ustalenie, czy informacje są przekazywane w sposób, który nie zależy od jednej cechy sensorycznej. 
Kryterium sukcesu 1.3.3 Właściwości zmysłowe zwraca uwagę na sytuacje, w których od użytkownika oczekuje się, że podejmie działanie lub zareaguje na podstawie wskazania tylko za pomocą cechy odwołującej się do jednego zmysłu, na przykład koloru lub dźwięku. 

Ponadto celem tego scenariusza jest sprawdzenie, czy informacje tekstowe i istotne informacje graficzne są widoczne dla użytkowników poprzez zapewnienie wystarczającego kontrastu między tekstem a tłem. 

Wpływ tego wymogu nie ogranicza się do użytkowników technologii wspomagających.

Scenariusz „Charakterystyki zmysłowe i kontrast” obejmuje trzy testy:
1.	Test 13.A 1.4.1-uzycie-koloru
2.	Test 13.B 1.3.3-charakterystyki-zmyslowe
3.	Test 13.C 1.4.3-kontrast

## Użycie koloru

### Test 13.A 1.4.1-uzycie-koloru

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.1-uzycie-koloru | 13.A    | Kolor nie jest używany jako jedyny wizualny sposób przekazywania informacji, wskazujący działanie, zachęcający do odpowiedzi lub wyróżniający element wizualny. |

### Cel testu 13.A 1.4.1-uzycie-koloru

Celem tego testu jest ustalenie, gdzie kolor jest używany do przekazania znaczenia i sprawdzenie, czy oprócz koloru do przekazania informacji wykorzystane są również inne środki. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-4-1 Użycie koloru](https://wcag.lepszyweb.pl/#use-of-color).

### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa treści strony.

### Identyfikacja treści
Treść, która uzależnia znaczenie informacji od koloru, która 

- tylko kolorem sygnalizuje bądź wskazuje czynności, np. „Wymagane pola są oznaczone na czerwono”, 
- podpowiada reakcję, 
- wyświetl odpowiedzi, np. „Wybierz niebieski tekst, aby zobaczyć definicję terminu”
- wyróżnia element wizualny, np. „Elementy oznaczone na czerwono są nieaktualne”,
 lub identyfikuje błędy.

### Zastosowanie

Test 13.A 1.4.1-uzycie-koloru **nie ma zastosowania**, jeśli na stronie

-	kolor jest stosowany tylko do celów dekoracyjnych (kolor nie przekazuje znaczenia).

W takim przypadku oznacz wynik testu jako **ND**. 

### Jak testować

1.  Ustal, czy kolor jest jedyną metodą stosowaną do przekazywania informacji (np. przejrzyj tekst na ekranie, aby uzyskać pełny opis i poszukaj innych wskazówek wizualnych).

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.4.1:

1.  Gdy kolor jest używany do przekazywania informacji, wskazywania czynności, monitowania o odpowiedź lub wyróżniania elementu wizualnego, do przekazywania informacji, która nie używa koloru, stosowana jest inna wizualna metoda ekranowa.

### Uwaga

-   Tekst alternatywny, który pojawia się po najechaniu myszką na element wizualny; nie jest traktowany jako „tekst na ekranie”.

-   Wskazanie błędu nie może używać samego koloru jako wskaźnika.

-   Zmiany koloru zastosowano w celu wskazania odwiedzanego łącza; jest to uważane za ustawienie przeglądarki.


## Użycie właściwości zmysłowych

### Test 13.B 1.3.3-charakterystyki-zmyslowe

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.3.3-sensory-info | 13.B    | Instrukcje dotyczące zrozumienia i obsługi treści nie opierają się wyłącznie charakterystykach odwołujących się do zmysłów, takich jak kształt, rozmiar, lokalizacja wizualna, orientacja lub dźwięk. |

### Cel testu 13.B 1.3.3-charakterystyki-zmyslowe
Celem tego testu jest sprawdzenie, czy instrukcje obsługi i objaśnienia treści nie opierają się wyłącznie na właściwościach zmysłowych, takich, jak kształt, rozmiar, lokalizacja wzrokowa, orientacja w przestrzeni lub dźwięk. 

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-3-3 Włąściwości zmyslowe](https://wcag.lepszyweb.pl/https://wcag.lepszyweb.pl/#sensory-characteristics).


### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa treści strony.
2.	Kontrola pod kątem sygnałów dźwiękowych.


### Identyfikacja treści

Wskazówki umożliwiające zrozumienie instrukcji i obsługi treści, które wykorzystują informacje sensoryczne do przekazywania informacji, np. odniesienia do kształtu, rozmiaru, wizualnej lokalizacji, orientacji lub dźwięku.

### Zastosowanie

Test 13.B 1.3.3-charakterystyki-zmyslowe **nie ma zastosowania**, jeśli strona nie przekazuje informacji ważnych dla zrozumienia instrukcji lub obsługi treści poprzez zastosowanie:

-	dźwięku
-	lokalizacji lub orientacji obiektów,
-	charakterystyki elementu, takiej jak kształt lub rozmiar.

### Jak testować

1.  Ustal, czy instrukcje wykorzystujące cechy sensoryczne zawierają szczegóły, które pozwalają na lokalizację, identyfikację, zrozumienie i obsługę treści bez wiedzy o jej kształcie, rozmiarze, orientacji lub względnej pozycji.

2.  Sprawdź, czy nie ma żadnych wskazówek dźwiękowych dotyczących instrukcji lub treści operacyjnej.

    1.  Upewnij się, że dźwięk nie jest wyciszony podczas testowania.

    2.  Ustal, czy są dostępne także inne wskazówki wizualne i / lub tekstowe.

**Uwaga**: użycie słów „dalej” („następne”) i „poniżej” jest często używane w odniesieniu do sekwencji kroków, a nie do konkretnej lokalizacji. W takich przypadkach nie jest to uważane za cechę sensoryczną.

### Ocena wyników

Jeśli twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.3.3:

1.  Gdy instrukcje używają kształtu, rozmiaru, położenia, orientacji lub dźwięku do przekazania znaczenia, zapewniona jest inna metoda, która nie opiera się na cechach sensorycznych.

### Uwaga

Część testu 13.A 1.4.1-uzycie-koloru polega na upewnieniu się, że sam kolor nie jest używany do przekazywania informacji. Dotyczy to również tego, czy sam kolor jest używany do dostarczania instrukcji lub procedur operacyjnych. Aby spełnić ten wymóg, kolor może być stosowany w połączeniu z kształtem, rozmiarem, położeniem wizualnym, orientacją lub dźwiękiem. Jeżeli instrukcje lub procedury operacyjne opierają się wyłącznie na:

- kolorze, wtedy treść **nie spełnia** warunku testowego 13.A 1.4.1-uzycie koloru.
- innych informacjach sensorycznych (takich jak kształt, rozmiar, wizualna lokalizacja, orientacja lub dźwięk), wtedy treć **nie spełnia** warunku testowego 13.B 1.3.3-charakterystyki-zmyslowe.


## Kontrast kolorów

### Test 13.C 1.4.3-kontrast

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.3-kontrast   | Wizualna prezentacja tekstu i obrazy tekstu mają wystarczający kontrast. |

### Cel testu 13.C 1.4.3-kontrast
Celem tego testu jest zapewnienie wystarczającego kontrastu między tekstem pierwszego planu i jego tłem, aby był czytelny. Dotyczy to tekstu i obrazów tekstu. Wyniki tego testu są wykorzystywane do ustalenia, czy kontrast WCAG SC 1.4.3 (minimum) jest spełniony.

### Metody i narzędzia testowe 

1.	Inspekcja wzrokowa treści strony.
2.	Kontrola pod kątem sygnałów dźwiękowych.

### Identyfikacja treści
Cały widoczny znaczący tekst ORAZ obrazy tekstu.

**Uwaga:**

- Niektóre teksty mogą być początkowo niewidoczne na stronie, w tym teksty, który stają się widoczny po wskazaniu kursorem myszki lub gdy element otrzymuje fokus. Niemniej jednak, tekst musi spełniać wymagania dotyczące kontrastu kolorów, niezależnie od miejsca jego występowania.

### Zastosowanie

Test 13.C 1.4.3-kontrast **nie ma zastosowania**, jeśli:

- Na stronie nie ma widocznego tekstu ani obrazów tekstu lub strona zawiera tylko alternatywy tekstowe, 
- Zidentyfikowany tekst to:
   - Logotyp: logo lub nazwa marki,
   - Nieaktywne (wyłączone) komponenty interfejsu użytkownika,
   - Element czysto dekoracyjny i nieistotny, bez żadnej funkcjonalności,
   - Tekst zawarty w obrazach, które zawierają inną znaczącą treść wizualną.
   - Tekst zmieniony, aby wskazać, że jest to łącze „odwiedzone”.

### Jak testować

1.  Uruchom ANDI: kontrast kolorów..

2.  Przejrzyj wszystkie „Alerty kontrastu” w sekcji „Alerty dostępności” ANDI, aby określić, który tekst nie spełnia minimalnego współczynnika kontrastu.

    1. Wybierz tekst „Alerty kontrastu”, aby wyświetlić określone alerty.
	2. Wybierz kolejno każdy alert, aby przejść do alertu.
	3. Przejrzyj szczegółowe wyniki dla każdego alertu. Wyniki wskazują.

       - Element, w którym znaleziono błąd.
       - Współczynnik kontrastu tekstu na pierwszym planie do tła, słowo „FAIL” i wymagany współczynnik.
       - Szczegóły stylu dotyczące stosunku:
       - Kolory tekstu i tła oraz wartości szesnastkowe.
       - Rozmiar czcionki (używany do ustalenia odpowiedniego wymaganego współczynnika).
       - Sugerowany kolor tekstu, który zmieni odcień na tyle, aby spełnić wymaganie (pomoc dla programistów).
       - Tekst wybranego alertu.

3.  W sekcji „Alerty dostępności” ANDI znajdź łącza „Potrzebne testy ręczne” i rozwiń je.

    1.  Jeśli tekstu nie można wybrać lub pojawia się na obrazie tła, określ kontrast za pomocą narzędzia *Colour Contrast Analyser* (Analizator kontrastu kolorów).

    2.  Otwórz narzędzie Analizator kontrastu kolorów , wybierz przycisk kroplomierza koloru pierwszego planu i kliknij piksel w czcionce tekstowej.

    3.  Wybierz kroplomierz koloru tła i kliknij piksel w tle blisko tekstu. Jeśli tło ma inny wygląd lub kolor, wybierz piksel zapewniający najmniejszy kontrast.

    4.  Określ współczynnik kontrastu

    5.  Porównaj współczynnik kontrastu z minimalnym wymaganym współczynnikiem kontrastu określonym w danych wyjściowych współczynnika kontrastu ANDI.
	
	**Uwaga**: Wyjście ANDI dostosowuje minimalny współczynnik kontrastu do 3:1, jeśli ma zastosowanie wymóg dotyczący dużej czcionki.

4.  Jeśli strona zawiera obraz samego tekstu lub obraz z tekstem i bez innych istotnych treści, przetestuj obraz tekstu za pomocą Analizatora kontrastu kolorów, aby określić współczynnik kontrastu między pierwszym planem (tekstem) a tłem.

    **Uwaga**: Dotyczy to przypadków, w których moduł kontrastu kolorów ANDI nie jest w stanie wykryć obecności tekstu.

    1.  Wybierz w ANDI moduł grafiki/obrazy.

    2.  Użyj przycisków strzałek ANDI, aby określić wszelkie obrazy tekstu lub obrazy z tekstem i bez innych istotnych treści.
	
    3.  Otwórz CCA i sprawdź kontrast tekstu na obrazie.

        1.  Wybierz kroplomierz koloru pierwszego planu i kliknij piksel w czcionce tekstowej. Jeśli kolor tekstu jest zróżnicowany pod względem wyglądu lub koloru, wybierz piksel, który zapewnia najmniejszy kontrast.

        2.  Wybierz kroplomierz koloru tła i kliknij piksel w tle blisko tekstu. Jeśli tło ma inny wygląd lub kolor, wybierz piksel zapewniający najmniejszy kontrast.

        3.  Ustal, czy uzyskany współczynnik kontrastu wynosi co najmniej 4,5:1.

Określ współczynnik kontrastu na podstawie testu:
-	Możesz ocenić treść, po prostu odnotowując wynik podany przez ANDI  **zgodny** (**pass**) lub **niezgodny** (**fail**), aby ustalić, czy spełniony jest wymóg testowy (od kroku 2 w Jak testować).
-	Jeśli konieczne było ręczne testowanie, należy porównać współczynnik kontrastu podany przez CCA z minimalnym wymaganiem określonym przez ANDI (od kroku 3 w Jak testować ).
-	Jeśli obraz tekstu został przetestowany, współczynnik kontrastu musi wynosić co najmniej 4,5:1, ponieważ rozmiar tekstu nie jest ustawiany programowo (od kroku 4 w Jak testować).


### Ocena wyników

Jeśli którekolwiek twierdzenie poniżej jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.4.3

1.	Kontrast między tekstem a tłem jest równy lub większy niż minimalny wymagany współczynnik kontrastu określony w danych wyjściowych współczynnika kontrastu ANDI, **lub**
2.	Jeśli tekst jest obrazem tekstu, kontrast między obrazem tekstu a jego tłem jest równy lub większy niż 4,5:1, jak określono za pomocą Analizatora kontrastu kolorów.


## Obowiązujące normy

- {% include ks/1-4-1.md %}
- {% include ks/1-3-3.md %}
- {% include ks/1-4-3.md %}
- [07. Właściwości zmysłowe](ICT-07-wlasciwosci-zmyslowe)
- [08. Kontrast](ICT-08-kontrast)


