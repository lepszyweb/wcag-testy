---
title: Współczynnik kontrastu


sidebar: testy_sidebar

permalink: 04-P-wspolczynnik-kontrastu
folder: testy/latwe
---

## Współczynnik kontrastu ( „kontrast kolorów”)
Niektórzy ludzie nie potrafią czytać tekstu, jeśli nie ma wystarczającego kontrastu między tekstem a tłem, na przykład, jasnoszarego tekstu na jasnym tle.

![Szary tekst na jasnym tle](images/andi/04_P_kontrast_01.png)

Wysoki kontrast (na przykład ciemny tekst na jasnym tle lub jasny tekst na ciemnym tle) jest potrzebny niektórym osobom z&nbsp;upośledzeniem wzroku, w tym wielu ludziom starszym, którzy wraz z wiekiem tracą wrażliwość na kontrast.

![Ciemny tekst na jasnym tle, i żółty tekst na czarnym tle](images/andi/04_P_kontrast_02.png)

Chociaż niektórzy ludzie potrzebują wysokiego kontrastu, dla innych - w tym niektórych osób z&nbsp;trudnościami w&nbsp;czytaniu, takimi jak dysleksja - jasne kolory (wysoka luminancja) nie są czytelne. Potrzebują oni niskiej luminancji.

![Brązowy tekst na ciemnym tle, i tekst na brązowym tle.](images/andi/04_P_kontrast_03.png)

Przeglądarki internetowe powinny umożliwić ludziom zmianę koloru tekstu i tła, a&nbsp;strony internetowe muszą działać, gdy ludzie zmieniają kolory.

(Ten wymóg dostępności jest czasem nazywany wystarczającym „kontrastem kolorów”; jednak jest to niepoprawne - technicznie jest to „kontrast luminancji” Na tej stronie używamy „współczynnika kontrastu” jako skrótu od „współczynnika kontrastu luminancji”, ponieważ jest w mniejszym stopniu żargonowy.). O kontraście trzeba wiedzieć znacznie więcej, właśnie wprowadziliśmy tu podstawy.


### Co sprawdzać

- Czy współczynnik kontrastu między zwykłym tekstem a tłem wynosi co najmniej 4,5:1?
- Czy współczynnik kontrastu między dużym tekstem a tłem wynosi co najmniej 3,0:1?
- Czy obiekty na grafikach wymaganych do zrozumienia treści mają współczynnik kontrastu w stosunku do tła co najmniej 3:1?

WCAG 2.1 zawiera dwa kryteria sukcesu, które wskazują, jaki powinien być kontrast między treścią a jej tłem, żeby treść była w&nbsp;pełni zauważalna. Kryterium sukcesu 1.4.3 wyznacza minimalne progi kontrastu, gdy wymagany jest poziom AA zgodności z WCAG 2.1), a kryterium 1.4.6 podwyższone progi kontrastu, gdy wymagany jest poziom AAA.

Według tych kryteriów sukcesu, aby zapewnić, że wizualna prezentacja tekstu i obrazów tekstu będzie rozpoznawalna, współczynnik kontrastu powinien wynosić co najmniej:
- Dla poziomu AA - 1.4.3 Kontrast (minimalny)
  - **4,5** w przypadku małego tekstu,   
  - **3,0** w przypadku dużego tekstu.
- Dla poziomu AAA - 1.4.6 Kontrast (wzmocniony)  
  - **7,0** w przypadku małego tekstu,
  - **4,5** w przypadku dużego tekstu.  

Jako tekst wystarczająco duży, aby wymagać niższego współczynnika kontrastu uznaje się tekst 18-punktowy lub 14-punktowy pogrubiony, czyli:

- **Mały tekst**, według WCAG, jest wtedy, gdy:
  - ma rozmiar mniejszy niż 18 punktów (24 piksele) ALBO
  - ma rozmiar mniejszy niż 14 punktów (19 pikseli) i jest pogrubiona.   
- **Duży tekst**, według WCAG, jest wtedy, gdy:
  - ma rozmiar co najmniej 18 punktów (24 piksele) ALBO
  - ma rozmiar co najmniej 14 punktów (19 pikseli) i jest pogrubiona.    

### Sposoby sprawdzania współczynnika kontrastu
Istnieją zasadniczo trzy sposoby sprawdzania kontrastu. Każdy ma mocne i słabe strony.

1. **Tabela współczynników kontrastu** - narzędzie wyświetla tabelę wszystkich współczynników kontrastu, jakie można uzyskać z kombinacji użytych na stronie kolorów. Niektóre narzędzia pokazują, gdzie na stronie internetowej znajduje się wskazana kombinacja kolorów.
   - *Zalety*: Kompleksowe.
   - *Wady*: Może być niedokładne, może pokazywać także kombinacje kolorów, których nie ma stronie.
2. **Próbnik koloru (zakraplacz)** - narzędzie pozwala wybrać kolor tekstu i kolor tła, a następnie pokazuje współczynnik kontrastu.
   - *Zalety*: Dokładne.
   - *Wady*: Naraz można przetestować tylko jedną kombinację kolorów. Użytkownicy muszą widzieć i używać myszy.
3. **Wyłączenie kolorów**. Narzędzie wyświetla stronę w skali szarości.
   - *Zalety*: Zapewnia bezpośrednie doświadczenie.
   - *Wady*: Nieprecyzyjne, nie przedstawia wartości współczynnika kontrastu.


### Sprawdzanie kontrastu
Istnieje wiele narzędzi umożliwiających sprawdzanie kontrastu. Lista kilku narzędzi, z których można skorzystać, została podana w ostatniej sekcji tego poradnika.  

Poniżej znajdują się instrukcje dotyczące sprawdzania kontrastu za pomocą rozszerzenia WCAG Color Contrast Checker przeznaczonego dla przeglądarek Chrome i Firefox.  

#### Sprawdzanie kontrastu za pomocą WCAG Color Contrast Checker

- Pobierz i zainstaluj WCAG Color Contrast Checker [w przeglądarce Chrome](https://chrome.google.com/webstore/detail/wcag-color-contrast-check/plnahcmalebffmaghcpcmpaciebdhgdf)
- Pobierz i zainstaluj WCAG Color Contrast Checker [w przeglądarce Firefox](https://addons.mozilla.org/pl/firefox/addon/wcag-contrast-checker/)

1.	Otwórz stronę, którą chcesz sprawdzić.
2.	Uruchom narzędzie WCAG Color Contrast Checker. Kontroler zostanie wyświetlony w panelu po lewej stronie ekranu. Niestety, nie można manipulować jego położeniem, a  często zasłania część sprawdzanej strony. Kontroler domyślnie sprawdza poprawność kontrastu na poziomie wymagań AA. Jeśli wymagana jest zgodność z WCAG 2.1 na poziomie AAA, można zmienić ustawienie domyślne na liście rozwijanej w górnej części kontrolera, opisanej etykietą *Level* (Poziom).   
	- **Tabela współczynników kontrastu.** W głównej części panelu wyświetlana jest tabela wykrytych kombinacji kolorów tekstu i&nbsp;tła oraz danych dotyczących kontrastu. **Zielona fiszka** oznacza wystarczający kontrast, czerwony znak **x** oznacza niewystarczający kontrast. Obok ikony podawany jest wyliczony współczynnik kontrastu. Następnie rozmiar tekstu – słowo *small* oznacza mały tekst, a słowo *large* duży tekst. Dla małego tekstu wymagany jest wyższy współczynnik kontrastu, dla dużego – niższy. W następnej kolumnie wyświetlana jest próbka kombinacji kolorów, a w ostatniej kolumnie liczba wykrytych elementów strony i znaczniki HTML, w których dany współczynnik kontrastu został rozpoznany. Aby zobaczyć dokładniejszą statystykę, wystarczy za pomocą przełącznika z lewej strony współczynnika kontrastu rozwinąć szczegółowe informacje. Jeśli wskażesz w&nbsp;tabeli dowolną pozycję, wszystkie wystąpienia elementów z&nbsp;wybranym współczynnikiem kontrastu zostaną otoczone czerwonym obrysem. Niestety, niekiedy trudno go znaleźć, bo może być ukryty pod panelem kontrolera.

	![Tabela wyników testu współczynników kontrastu w panelu narzędzia WCAG Color Contrast Checker](images/andi/04_P_kontrast_WCAG_1.png)

	- **Próbnik koloru (zakraplacz)**: Kontroler umożliwia również zbadanie współczynnika kontrastu dowolnej pary kolorów i&nbsp;odczytanie wartości użytych kolorów.  Aby zbadać współczynnik kontrastu  między treścią i tłem dowolnego elementu strony:
	  1. W sekcji *Color tool* (Narzędzia koloru) zaznacz próbnik koloru obok pola zatytułowanego *Foreground color hex* (Kolor pierwszego planu w formacie szesnastkowym).
	  2. Następnie wskaż na stronie treść, którą chcesz sprawdzić. W polu tekstowym pojawi się szesnastkowy kod wskazanego koloru.
	  3. Powtórz tę czynność, by zbadać kolor tła. Tym razem użyj próbnika koloru obok pola zatytułowanego *Background color...* (Kolor tła). W polu tekstowym pojawi się szesnastkowy kod wskazanego koloru tła, a poniżej zostanie wyświetlona próbka małego i dużego tekstu na tle we wskazanych kolorach.
	  4. Sprawdź w tabeli poniżej wyniki wyliczenia współczynnika  kontrastu  dla małego i dużego tekstu na poziomie AA i AAA.  

	![Testowanie współczynnika kontrastu za pomocą próbnika kolorów](images/andi/04_P_kontrast_WCAG_2.png)	  

	- **Wyłączenie kolorów**: WCAG Color Contrast Checker zapewnia również możliwość sprawdzenia kontrastów za pomocą symulatora widzenia przez osoby z różnymi odmianami ślepoty barw, w tym achromatopsji, czyli osoby widzące tylko w odcieniach szarości:
	  1. Z listy rozwijanej *color-blindness* (ślepota barw) – wybieraj kolejne opcje.
	  2. Sprawdź na stronie dla każdej wybranej opcji, czy wszystkie treści są czytelne i mają wystarczający kontrast. Uwaga:  Możesz sprawdzić współczynniki kontrastu dla wszystkich wykrytych oryginalnych kombinacji kolorów po przekształceniu ich do skali barw charakterystycznej dla danego typu ślepoty barw.   

	![Testowanie współczynnika kontrastu z wykorzystaniem symulatora ślepoty barw](images/andi/04_P_kontrast_WCAG_3.png)


#### Testy w dowolnej przeglądarce  

Aby sprawdzić kontrasty w dowolnej przeglądarce:

1. Otwórz stronę internetową [narzędzia oceny dostępności WAVE](http://wave.webaim.org).
2. W polu *Web page address* ('Adres strony internetowej') wpisz adres strony internetowej, którą chcesz ocenić.
3. Kliknij przycisk strzałki *WAVE this page!* ('Testuj tę stronę'). Twoja strona internetowa pojawi się w przeglądarce z mnóstwem małych ikon na jej temat. Po lewej stronie w ramce pojawi się panel zarządzania narzędziem WAVE.
4. W panelu kontrolnym narzędzia WAVE wybierz z paska menu opcję *Contrast*. Widok sprawdzanej strony zostanie przełączony. W miejscach, w których narzędzie stwierdzi niewystarczający kontrast, znajdują się ikony ![błędu kontrastu](images/andi/04_P_contrast.png).

   ![Lokalizacja opcji Kontrast w narzędziu WAVE](images/andi/04_P_kontrast_WAVE_1.png)

   1. Kliknij ikonę, aby wyświetlić komunikat błędu z łączem do szczegółowych objaśnień (w języku angielskim).

   ![Testowanie kontrastu za pomocą narzędzia WAVE](images/andi/04_P_kontrast_WAVE_2.png)

   2. Sprawdź w panelu kontrolnym WAVE w sekcji *Contrast Tools* (Narzędzia kontrastu) szczegółowe informacje o wykrytych niewystarczających współczynnikach kontrastu.
      - w polu *Foreground color* wyświetlany jest szesnastkowy kod koloru pierwszego planu (tekstu),
	  - w polu *Background color* wyświetlany jest szesnastkowy kod koloru tła,
	  - obok etykiety *Contrast ratio* wyświetlany jest wyliczony współczynnik kontrastu
	  - poniżej podane jest podsumowanie dla normalnego i dużego tekstu z rozbiciem na poziommy zgodność AA i AAA. Słowo *fail* oznacza niewystarczający kontrast. Słowo *Pass* oznacza wystarczający kontrast.

   ![Wyniki testu kontrastu w narzędziu WAVE](images/andi/04_P_kontrast_WAVE_3.png)

**Uwaga**: WAVE umożliwia również wzrokowe sprawdzenie kontrastu za pomocą opcji wyświetlenia strony w skali szarości. W tym celu wybierz w panelu kontrolnym łącze: *Desaturate page*.    

## Ćwiczenie sprawdzania kontrastów na stronie demo PrzediPo  
W ramach ćwiczeń przygotowawczych do powyższych testów możesz sprawdzić problemy z kontrastem w naszym [Demo PrzediPo: Niedostępna strona główna](https://przedipo.lepszyweb.pl/before/home.html).

### Wskazówki

1. Otwórz niedostępną wersję strony Bilety https://przedipo.lepszyweb.pl/before/tickets.html
2. Użyj jednego z opisanych powyżej sposobów sprawdzania kontrastu:
   - Zwróć uwagę na tabelkę zatytułowaną „daty koncertu”. W nagłówku tabeli znajduje się czarny tekst na szarym tle. Współczynnik kontrastu tego tekstu wynosi 3,88, a tekst, choć pogrubiony, jest zbyt mały, by uznać ten współczynnik kontrastu za wystarczający.
   - Sprawdź również współczynniki kontrastu w komórkach nagłówkowych w tabeli poniżej, przedstawiającej ceny biletów. Tu również współczynnik kontrastu wynosi 3,88.
3. Otwórz dostępną wersję strony Bilety https://przedipo.lepszyweb.pl/after/tickets.html.
4. Sprawdź, czy w poprawionej wersji strony został zwiększony współczynnik kontrastu.  

## Dowiedz się więcej o współczynniku kontrastu
-	[Zrozumieć kryterium sukcesu 1.4.3: Kontrast minimalny)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html) - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 1.4.6: Wzmocniony kontrast](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html)   - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.

## Narzędzia sprawdzające kontrast

- [Color Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/): aplikacja działająca w systemie Windows i MacOS. Kilka sposobów ustawiania kolorów, obsługa przezroczystości alfa w kolorach pierwszego planu, symulator ślepoty barw
- [Tota11y](https://khan.github.io/tota11y/): zestaw narzędzi sprawdzających kilka aspektów dostępności cyfrowej, w tym kontrast. Wskazuje elementy z niewystarczającym kontrastem, pokazuje fragment kodu z problematycznym elementem, sugeruje dobór kolorów zapewniających odpowiedni kontrast.
- [Vischeck](http://www.vischeck.com/vischeck/): symulator ślepoty barw, który może być używany online lub jako wtyczka programu Photoshop, która pojawia się w menu „Filtr”. Narzędzie online symuluje ślepotę kolorów na przesyłanym obrazie lub na określonej stronie internetowej.
