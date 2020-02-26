---
title: Korzystanie z łatwych testów
summary: "Łatwe testy może przeprowadzić każdy, kto korzysta z Internetu. Nie potrzebujesz specjalnej wiedzy ani umiejętności. Niektóre testy wymagają obejrzenia strony bądź posłuchania dźwięku. Inne wymagają zastosowania prostych narzędzi. Ale ogólnie rzecz biorąc są to testy łatwe do przeprowadzenia."
sidebar: testy_sidebar
permalink: 00-P-wprowadzenie3
folder: testy/latwe
---

{% include note.html content="**Gdy korzystasz z tej bazy po raz pierwszy, zalecamy uważne zapoznanie się ze  wszystkimi sekcjami**." %}

## Narzędzia: Pasek narzędzi Web Developer i inne (opcjonalnie)
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
Oprócz wymienionych powyżej, użyteczne będą inne usługi internetowe bądź rozszerzenia przeglądarek. W łatwych testach wykorzystujemy także;
- usługę internetową W3C – walidator HTML. Możesz sobie zapewnić szybki dostęp do tej usługi za pomocą skryptozakładek opublikowanych na stronie https://validator.w3.org/favelets.html
- WCAG Color Contrast Checker - rozszerzenie przeglądarek
  - [dla Chrome](https://chrome.google.com/webstore/detail/wcag-color-contrast-check/plnahcmalebffmaghcpcmpaciebdhgdf)
  - [dla Firefox](https://addons.mozilla.org/pl/firefox/addon/wcag-contrast-checker/)
- skryptozakładki Form labels i Forms:
  - [Form labels](https://jimthatcher.com/favelets/)
  - [Forms]( http://pauljadam.com/bookmarklets/index.html)  

(Jeśli nawet nie możesz pobrać i zainstalować tych narzędzi, to nadal możesz wykonać łatwe testy za pomocą dowolnej przeglądarki).

## Odniesienia i łącza do WCAG
Wszystkie testy opierają się na Wytycznych dotyczących dostępności treści internetowych (WCAG). W Europie i w Polsce standard WCAG stał się normą prawną EN 301 V2.1.2.

Główne punkty w WCAG są nazywane „kryteriami sukcesu”. W sekcjach „Dowiedz się więcej o...” znajdują się łącza do stron wyjaśniających odpowiednie kryteria sukcesu w dokumencie „Zrozumienie WCAG”.

## Ćwiczenia z Demo Przed-Po  
Serwis Demo PrzediPo[https://przedipo.lepszyweb.pl/] pokazuje dwie wersje tej samej, nieistniejącej w rzeczywistości witryny Światła Miasta: wersję niedostepną i poprawioną wersję dostępną. Możesz użyć stron PrzediPo, aby przećwiczyć wykonywanie niektórych opisywanych tutaj testów. Na przykład najpierw sprawdź dostępną wersję strony, aby zobaczyć, jak powinna wyglądać, a potem sprawdź wersję niedostępną.

Niektóre z testów opisujemy w sekcjach zatytułowanych Ćwiczenia z Demo PrzediPo.

Do stron PrzediPo dołączone są adnotacje, które zawierają bogaty zestaw informacji na temat dostępności i niedostępności na stronach demo. Aby włączyć adnotacje, wybierz w menu opcję Pokaż adnotacje. Problemy dostępności są oznaczone na każdej stronie wyróżnionymi łączami przy lewej krawędzi strony. Wybierz link z numerem notatki, aby wyświetlić okno wyskakujące z informacjami. Wszystkie adnotacje możesz również zobaczyć pod każdą ze stron.  

## Kilka ważnych pojęć

Oto kilka rzeczy, które należy wiedzieć, aby dobrze rozumieć instrukcje przedstawione w tym przewodniku:
-	znakowanie – termin odnosi się do kodu strony internetowej, zwanego HTML. Kod strony internetowej można zobaczyć w większości przeglądarek, wybierając z menu: Widok > Źródło. Nie musisz oglądać kodu strony, aby przeprowadzić łatwe testy. Ale rozumienie słów „znakowanie”, czy „oznakowane” pomaga zrozumieć instrukcje. Znakowanie to najkrócej opisywanie elementów strony specjalnymi znacznikami, czyli słowami ujętymi w nawiasy kątowe.  
-	technologie wspomagające albo asystujące, albo pomocnicze to oprogramowanie lub sprzęt, z którego korzystają osoby z niepełnosprawnościami, aby korzystać ze stron i aplikacji komputerowych, w tym internetowych.
-	czytniki ekranu to rodzaj technologii pomocniczej - oprogramowanie, które umożliwia nawigację po stronie internetowej i odczytuje na głos treści stron. Są używane przez osoby niewidome.
-	sterowanie głosem, nazywane czasem wejściem głosowym, polega na użyciu mowy zamiast klawiatury i myszy.
Aby dowiedzieć się więcej, zobacz:
-	[Wprowadzenie do dostępności sieci](http://dostepny.joomla.pl/dostepnosc/internet-dla-wszystkich/50-wprowadzenie-do-dostepnosci-sieci)
-	[Zasady dostępności](https://www.w3.org/WAI/fundamentals/accessibility-principles/); artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
