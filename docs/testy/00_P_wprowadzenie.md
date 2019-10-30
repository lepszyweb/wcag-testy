## Baza testów wstępnych
Baza testów wstępnych pomaga rozpocząć ocenę dostępności cyfrowej strony internetowej. Dzięki tym prostym testom można się zorientować, czy dostępność treści strony internetowej została zapewniona w najbardziej elementarny sposób.

### Zakres  
Baza testów wstępnych obejmuje tylko kilka kwestii związanych z dostępnością cyfrową strony internetowej zaprojektowanych tak, aby były łatwe i szybkie, ale nie ostateczne. Może się zdarzyć, że strona internetowa przejdzie pomyślnie przez wszystkie testy wstępne, ale nadal będą na niej występować znaczące bariery dostępności. 

Aby kompleksowo ocenić dostępność strony, potrzebne jest solidniejsze badanie, niż tylko tych kilka testów wstępnych.
 
Baza testów wstępnych została opracowana na podstawie dokumentu W3C WAI zatytułowanego [Easy Checks - A First Review of Web Accessibility](https://www.w3.org/WAI/test-evaluate/preliminary/), co można przetłumaczyć na język polski: Łatwe testy - Pierwszy przegląd dostępności cyfrowej.

Opracowanie W3C ma już swoją blisko 20-letnią historię. Pierwotnie była to jedna sekcja dokumentu Ocena witryn internetowych pod kątem dostępności zredagowana przez Judy Brewera i Chucka Letourneau i opublikowana w październiku 2001 roku. W 2005 roku została ona wyodrębniona jako Wstępny przegląd witryn internetowych pod kątem dostępności. Dokument zredagował Shadi Abou-Zahra. 
Najnowsze aktualizacje pochodzą z roku 2017.

Baza testów wstępnych obejmuje sprawdzenie kilku wymienionych poniżej aspektów strony internetowej oraz zawiera wskazówki dotyczące kolejnych kroków i łącza do dodatkowych zasobów.

- [Tytuł strony](testy/01_P_tytul-strony.md)
- [Teksty altenratywne obrazów](testy/02_P_odpowiedniki-tekstowe-obrazow.md) ( „alternatywy tekstowe” zdjęć, ilustracji, wykresów, etc.)
- **Tekst**:
  - [Nagłówki](testy/03_P_naglowki.md)
  - [Kontrast kolorów](testy/04_P_wspolczynnik_kontrastu.md) ( „współczynnik kontrastu”)
  - [Zmiana rozmiaru tekstu](testy/05_P_zmiana-rozmiaru-tekstu.md)
- **Interakcja**:
  - [Dostęp za pomocą klawiatury i widoczność fokusa](testy/06_P_klawiatura.md)
  - [Formularze, etykiety i błędy](testy/07_P_formularze.md) (w tym pól Szukaj)
- **Ogólne**:
  - [Treść przesuwana, migocąca lub błyskająca](testy/08_P_poruszanie-i-blyski.md)
  - [Odpowiedniki multimediów](testy/09_P_multimedia.md) (wideo, audio)
  - [Podstawowa struktura](testy/10_P_struktura.md)

### Co to jest wstępny przegląd dostępności
Wstępny przegląd dostępności strony internetowej jest formalną, uznaną i zalecaną przez WAI W3C procedurą oceny dostępności strony internetowej, którą można wykorzystać, aby wykryć i naprawić elementarne błędy dostępności cyfrowej witryny, zanim zostanie wykonane badania kompleksowe, obejmujące testy zgodności ze wszystkimi wymaganiami zdefiniowanymi w standardzie WCAG.   

### Cele i efekty wstępnego przeglądu dostępności
Są trzy główne cele wstępnego przeglądu dostępności:
- sprawdzenie, czy witryna spełnia podstawowe wymogi dostępności,
- zidentyfikowanie problemów dostępności, które wymagają pilnego rozwiązania,
- uzyskanie niezbędnych podstaw do sformułowania Deklaracji dostępności. 

Z całą mocą trzeba podkreślić, że nawet jeśli wynik wszystkich testów podczas przeglądu wstępnego będzie pozytywny albo wszystkie wykryte podczas przeglądu wstępnego problemy zostaną rozwiązane, to witryna wciąż może sprawiać różnym osobom poważne problemy z&nbsp;dostępnością. Aby kompleksowo ocenić dostępność witryny, konieczny jest pełny audyt dostępności przeprowadzony zgodnie z&nbsp;metodologią ewaluacji dostępności serwisów internetowych.
 
Efektem wstępnego przeglądu dostępności powinny być:
- lista zidentyfikowanych barier dostępności,
- działania naprawcze usuwające lub przynajmniej ograniczające wykryte problemy dostępności, 
- ogólna ocena dostępności witryny, 
- wnioski wyznaczające aktualne cele polityki dostępności cyfrowej.    

Chociaż nie istnieją żadne formalne wymogi, by wstępny przegląd dostępności kończył się sporządzeniem formalnego raportu czy podsumowania, to nic nie stoi na przeszkodzie, by go solidnie udokumentować.

Na dokumentację czy też raport ze wstępnego przeglądu dostępności witryny powinny się złożyć:
- zwięzły opis przeglądu(kto, kiedy, w jaki sposób dokonał przeglądu),
- wykaz zbadanych stron,
- lista wykrytych problemów dostępności,
- syntetyczna ocena dostępności, 
- wskazówki do poprawy dostępności serwisu, 
- notatki z przeprowadzonych testów.

## Korzystanie z bazy testów wstępnych

Te testy może przeprowadzić każdy, kto korzysta z Internetu. Nie potrzebujesz specjalnej wiedzy ani umiejętności. Niektóre testy wymagają obejrzenia strony internetowej bądź posłuchania dźwięku. Inne zastosowania prostych narzędzi wspomagających testowanie. Ale ogólnie rzecz biorąc są to testy łatwe do przeprowadzenia. 
 
Gdy korzystasz z tej bazy po raz pierwszy, zalecamy uważne zapoznanie się ze  wszystkimi sekcjami.

### Narzędzia: Pasek narzędzi Web Developer i inne (opcjonalnie) 
Większość tych kontroli można przeprowadzić za pomocą dowolnej przeglądarki, tzn. nie trzeba pobierać specjalnych narzędzi.
Jednak niektóre testy będą łatwiejsze, jeśli skorzystasz z odpowiednich narzędzi. Aby zachować prostotę, ograniczyliśmy listę sugerowanych narzędzi do minimum. Wszystkie są narzędziami bezpłatnymi, łatwymi w instalacji i stosowaniu. Niestety, nie zawsze są dostępne w języku polskim. Ale problemowi z rozumieniem komunikatów uda nam się zapewne zaradzić, zapewniając w instrukcjach niezbędne tłumaczenia.

Zwróć uwagę, że nie promujemy tutaj żadnego z narzędzi. Istnieje wiele innych narzędzi, z których można skorzystać. WAI W3C [zestawia ich listę na swojej stronie]( http://www.w3.org/WAI/eval/selectingtools)

### Pasek narzędzi Web Developer
Wiele przydatnych, a czasem niezbędnych podręcznych narzędzi oceny stron internetowych oferuje  pasek narzędzi Web Developer. Autor, Chris Pedrick udostępnia na swojej stronie [trzy wersje paska]( https://chrispederick.com/work/web-developer/) dla najpopularniejszych przeglądarek. Możesz je również pobrać i zainstalować za pomocą poniższych bezpośrednich linków  
-	[Pobierz narzędzie Web Developer dla przeglądarki Chrome](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=pl)
-	[Pobierz narzędzie Web Developer dla przeglądarki Firefox](https://addons.mozilla.org/pl/firefox/addon/web-developer/) 
-	[Pobierz narzędzie Web Developer dla przeglądarki Opera](https://addons.opera.com/pl/extensions/details/web-developer/)

### Usługa internetowa WAVE
WAVE to zestaw narzędzi oferowanych przez WebAim.org i Uniwersytet Stanowy Utah w USA. WAVE wspomaga ocenianie dostępności, pomaga wykryć wiele błędów i możliwych błędów dostępności. Filozofią twórców jest skupić się na problemach, które mają największy wpływ na dostępność stron oraz na edukacji na temat dostępności stron. 
WAVE można zainstalować jako dodatki w przeglądarkach Chrome i Firefox. Ale można również korzystać z WAVE udostępnionego jako usługa internetowa na stronie https://wave.webaim.org/.

### Inne dodatki i rozszerzenia przeglądarek
Oprócz wymienionych powyżej, użyteczne będą inne usługi internetowe bądź rozszerzenia przeglądarek. W testach wstępnych wykorzystujemy także;
- usługę internetową W3C – walidator HTML. Możesz sobie zapewnić szybki dostęp do tej usługi za pomocą skryptozakładek opublikoanych na stronie https://validator.w3.org/favelets.html
- WCAG Color Contrast Checker - rozszerzenie przeglądarek
  - [dla Chrome](https://chrome.google.com/webstore/detail/wcag-color-contrast-check/plnahcmalebffmaghcpcmpaciebdhgdf)
  - [dla Firefox](https://addons.mozilla.org/pl/firefox/addon/wcag-contrast-checker/)
- skryptozakładki Form labels i forms:
  - [Form labels](https://jimthatcher.com/favelets/) 
  - [Forms]( http://pauljadam.com/bookmarklets/index.html)  
(Jeśli nie możesz pobrać tych narzędzi, to jest OK, możesz nadal kontrolować "z dowolnej przeglądarki").

### Odniesienia i łącza do WCAG 
Wszystkie testy opierają się na Wytycznych dotyczących dostępności treści internetowych (WCAG). W Europie i w Polsce standard WCAG stał się normą prawną EN 301 V2.1.2.

Główne punkty w WCAG są nazywane „kryteriami sukcesu”. W sekcjach „Dowiedz się więcej o...” znajdują się łącza do stron wyjaśniających odpowiednie kryteria sukcesu w dokumencie „Zrozumienie WCAG”.

### Ćwiczenia z Demo Przed-Po  
Serwis Demo PrzediPo[] pokazuje dwie wersje tej samej, nieistniejącej w rzeczywistości witryny Światła Miasta: wersję niedostepną i poprawioną wersję dostępną. Możesz użyć stron PrzediPo, aby przećwiczyć wykonywanie niektórych opisywanych tutaj testów. Na przykład najpierw sprawdź dostępną wersję strony, aby zobaczyć, jak powinna wyglądać, a potem sprawdź wersję niedostępną.

Niektóre z testów opisujemy w sekcjach zatytułowanych Ćwiczenia z Demo PrzediPo.

Do stron PrzediPo dołączone są adnotacje, które zawierają bogaty zestaw informacji na temat dostępności i niedostępności na stronach demo. Aby włączyć adnotacje, wybierz w menu opcję Pokaż adnotacje. Problemy dostępności są oznaczone na każdej stronie wyróżnionymi łączami przy lewej krawędzi strony. Wybierz link z numerem notatki, aby wyświetlić okno wyskakujące z informacjami. Wszystkie adnotacje możesz również zobaczyć pod każdą ze stron.  
    
### Kilka ważnych pojęć

Oto kilka rzeczy, które należy wiedzieć, aby dobrze rozumieć instrukcje przedstawione w tym przewodniku:
-	znakowanie – termin odnosi się do kodu strony internetowej, zwanego HTML. Kod strony internetowej można zobaczyć w większości przeglądarek, wybierając z menu: Widok > Źródło. Nie musisz oglądać kodu strony, aby przeprowadzić  testy wstępne. Ale rozumienie słów „znakowanie”, czy „oznakowane” pomaga zrozumieć instrukcje. Znakowanie to najkrócej opisywanie elementów strony specjalnymi znacznikami, czyli słowami ujętymi w nawiasy kątowe.  
-	technologie wspomagające albo asystujące, albo pomocnicze to oprogramowanie lub sprzęt, z którego korzystają osoby z niepełnosprawnościami, aby korzystać ze stron i aplikacji komputerowych, w tym internetowych.
-	czytniki ekranu to rodzaj technologii pomocniczej - oprogramowanie, które umożliwia nawigację po stronie internetowej i odczytuje na głos treści stron. Są używane przez osoby niewidome.
-	sterowanie głosem, nazywane czasem wejściem głosowym, polega na użyciu mowy zamiast klawiatury i myszy.
Aby dowiedzieć się więcej, zobacz:
-	[Wprowadzenie do dostępności sieci](http://dostepny.joomla.pl/dostepnosc/internet-dla-wszystkich/50-wprowadzenie-do-dostepnosci-sieci)
-	[Zasady dostępności](https://www.w3.org/WAI/fundamentals/accessibility-principles/); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.



-------------------------------------
[Testy. Strona główna &lt; Poprzednia strona](README.md) | [Następna strona &gt; Tytuł strony](testy/01_P_tytul-strony.md)




