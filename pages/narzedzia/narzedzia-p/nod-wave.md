---
title: WAVE (Web Accessibility Evaluation Tool)
sidebar: narzedzia_sidebar
permalink: nod-wave
folder: narzedzia-p
---


![Logo WAVE](images/wave/wavelogo.svg) 

[WAVE (Web Accessibility Evaluation Tool)](http://wave.webaim.org/) to internetowy walidator dostępności cyfrowej stron internetowych oferowany przez WebAlM, który można również uruchamiać bezpośrednio w przeglądarce internetowej Chrome lub Firefox. Wystarczy je dodać jako rozszerzenie (dodatek) do swojej przeglądarki, pobierając ze składnicy dodatków Google Chrome WebStore lub Mozilla Firefox Add-Ons albo ze strony http://wave.webaim.org/. WAVE może sprawdzać strony, do których dostęp jest chroniony hasłem.
 
## Instalacja dodatku
Dodatek instalujemy tak, jak inne rozszerzenia przeglądarki Mozilla Firefox. Z podręcznego menu przeglądarki wybieramy opcję **Dodatki/Pobierz dodatki**, a następnie w wyszukiwarce wpisujemy WAVE Toolbar. Po odszukaniu instalujemy dodatek i ponownie uruchamiamy przeglądarkę.
 
Po zainstalowaniu dodatku w pasku narzędziowym przeglądarki pojawi się jego ikona.

![Ikona WAVE w pasku narzędziowym przeglądarki Chrome](images/wave/ikonawave.png)

## Uruchomienie dodatku
Jeśli używasz myszy, możesz uruchomić testowanie dowolnej strony internetowej, klikając w pasku narzędziowym przeglądarki ikonę WAVE.

Jeśli używasz klawiatury, możesz możesz uruchomić testowanie strony otwartej w przeglądarce, naciskając klawisze Ctrl+Shift+U na Windows albo Command+Shift+U na Macu. Możesz również aktywować w menu kontekstowym pozycję „WAVE this page”.

## Funkcje dodatku
W chwilę po uruchomieniu na stronie, którą chcemy zbadać, WAVE dzieli okno przeglądarki na trzy panele. W jednym wyświetla raport z testów, w drugim ocenianą stronę, a w trzecim, zwiniętym, kod ocenianej strony ze swoimi adnotacjami. Trzeci panel można odsłonić, naciskając przycisk **Code** umieszczony przy dolnej krawędzi okna przeglądarki.

![Okno przeglądarki po uruchomieniu WAVE i rozwinięciu panelu Code](images/wave/wave_okno_01.png)

Wykryte na stronie komponenty dostępności oraz błędy i miejsca, które wymagają weryfikacji człowieka, WAVE oznacza różnobarwnymi ikonami. Czerwonymi oznaczone są błędy, pomarańczowymi alerty, zielonymi - cechy zgodne z wymogami dostępności, niebieskimi - elementy struktury, fioletowymi - elementy oznakowane atrybutami ARIA.    



Do wszystkich funkcjonalności WAVE mamy dostęp z panelu sterującego:

![Karty panelu sterującego WAVE](images/wave/wave_okno_03.png)

- przełącznik ***Styles*** wyłącza arkusze stylów (css), wyświetlając stronę bez formatowania, a precyzyjniej mówiąc - tylko z elementarnym formatowaniem przez przeglądarkę (wyróżnienia nagłówków, list). Niektóre osoby (np. niewidome) mają ustawione automatyczne wyłączanie arkuszy stylów. Użycie przełącznika pozwala sprawdzić, czy wszystkie treści są widoczne, gdy wyłączone są arkusze stylów, oraz czy kolejność elementów treści jest logiczna i zrozumiała. 

- przycisk ***Summary*** włącza w panelu sterującym WAVE pierwszą kartę, na której przedstawiona jest statystyka przeprowadzonego badania. Umieszczony na karcie przycisk ***View details*** odkrywa szczegółową statystykę, wyświetlaną na kolejnej karcie.

- przycisk ***Details*** włącza kartę, na której przedstawiono szczegółową statystykę udokumentowaną ikonami symbolizującymi wykryty błąd, problem lub informację. Kliknięcie ikony oznacza na stronie czerwonym przerywanym konturem miejsce wymagające uwagi oraz wyróżnia odpowiedni wiersz kodu, jeśli odsłonięty jest panel *Code*. 

- przycisk ***Reference*** włącza kartę, na której można wyświetlić wszystkie ikony i objaśnienia. Na kartach z&nbsp;objaśnieniami znajdują się informacje, co oznacza ikona (*What It Means*), dlaczego oznaczony aspekt dostępnosci jest ważny (*Why It Matters*), jak naprawić błąd (*How to Fix It*), omówienie zastosowanego algorytmu (*The Algorithm... in English*) oraz odniesienia do kryteriów sukcesu WCAG. Niestety, dla użytkownika, który nie zna języka angielskiego, informacje te nie będą zbytnio przydatne.

- przycisk ***Structure*** włącza kartę, na której prezentowana jest struktura strony - struktura nagłówków i&nbsp;kluczowych obszarów strony, jeśli projektant oznakował punkty orientacyjne. Funkcja ułatwia szybkie sprawdzenie, czy układ strony jest konsekwentny i logiczny. 

- przycisk ***Contrast*** włącza kartę z wynikami testów kontrastu, z narzędziem, za pomocą którego można dobrać poprawnie skontrastowane zestawy barw oraz z przełącznikiem *Desaturate page / Resaturate page* (Zamiana na skalę szarości / Przywrócenie barw. Kliknięcie ikony sygnalizjąjącej bład kontrastu powoduje wyświetlenie w&nbsp;analizatorze kontrastu kodów kolorów, które można chwilowo zmodyfikować, aby dobrać odpowiedniejsze zestawienia. Nowe wartości kolorów można wpisać w&nbsp;polach tekstowych albo ustalić za pomocą próbników i&nbsp;suwaków.   

Kliknięcie każdej z wyświetlanych na analizowanej stronie ikony WAVE wyświetla okno dialogowe z krótkim objaśnieniem problemu oraz z odnośnikami:

- ***Reference***, który włącza w panelu sterującym kartę ze szczegółowymi objaśnieniami problemu
- ***Code***, który przenosi punkt uwagi w panelu *Code* na fragment kodu, z któego generowany jest problematyczny element strony. 

![Okno przeglądarki po uruchomieniu WAVE i rozwinięciu panelu Code](images/wave/wave_okno_02.png)


## Zakres oceny

WAVE potrafi wykryć 13 błędów dostępności i ostrzec w 38 przypadkach o możliwości wystąpienia problemów z dostępności 
38 rodzajów przypadków wymagających. 

### Błędy dostępności

Zgłaszane błędy dotyczą 11 kryteriów sukcesu na poziomie A (KS 1.1.1, 1.3.1, 2.1.1, 2.2.1, 2.2.2, 2.4.1, 2.4.2, 2.4.4, 3.1.1, 3.3.2, 4.1.2) oraz 2 kryteriów sukcesu na poziomie AA (KS 1.4.3 i 2.4.6).

|Ikona|Angielski komunikat błędu |Tłumaczenie komunikatu błędu
|-----|--------------------------|--------------------------------------|
|![](images/wave/errors/alt_missing.svg)|Missing alternative text |Brak tekstu alternatywnego|
|![](images/wave/errors/alt_link_missing.svg)|Linked image missing alternative text |Łącze graficzne bez tekstu alternatywnego|
|![](images/wave/errors/alt_spacer_missing.svg)|Spacer image missing alternative text |Brak tekstu alternatywnego w obrazie rozdzielającym|
|![](images/wave/errors/alt_input_missing.svg)|Image button missing alternative text |Przycisk graficzny bez tekstu alternatywnego|
|![](images/wave/errors/alt_area_missing.svg)|Image map area missing alternative text |Obszar mapy odsyłaczy bez tekstu alternatywnego|
|![](images/wave/errors/alt_map_missing.svg)|Image map missing alternative text |Mapa odsyłaczy bez tekstu alternatywnego|
|![](images/wave/errors/longdesc_invalid.svg)|Invalid longdesc |Niepoprawny atrybut `longdesc`|
|![](images/wave/errors/label_missing.svg)|Missing form label |Brak etykiety kontrolki formularza|
|![](images/wave/errors/label_empty.svg)|Empty form label |Pusta etykieta kontrolki formularza|
|![](images/wave/errors/label_multiple.svg)|Multiple form labels |Wiele etykiet dla jednej kontrolki formularza|
|![](images/wave/errors/aria_reference_broken.svg)|Broken ARIA reference |Niepełne odniesienie ARIA (Istnieje `aria-labelledby` lub `aria-describedby`, ale nie istnieje cel odniesienia.|
|![](images/wave/errors/aria_menu_broken.svg)|Broken ARIA menu |Niepoprawne użycie atrybutu ARIA `role="menu"` (w menu ARIA nie ma pozycji)|
|![](images/wave/errors/title_invalid.svg)|Missing or uninformative page title |Brak lub nieinformacyjny tytuł strony (Brak tytułu strony lub tytuł nie jest on opisowy)|
|![](images/wave/errors/language_missing.svg)|Document language missing |Brak języka dokumentu (Język dokumentu nie jest określony)|
|![](images/wave/errors/meta_refresh.svg)|Page refreshes or redirects | Automatyczne odświeżanie lub przekierowanie strony (za pomocą znacznika `<meta>`)|
|![](images/wave/errors/heading_empty.svg)|Empty heading |Pusty nagłówek (Nagłówek nie ma żadnej treści)|
|![](images/wave/errors/button_empty.svg)|Empty button |Pusty przycisk (Przycisk jest pusty lub nie zawiera tekstu o żadnej wartości)|
|![](images/wave/errors/link_empty.svg)|Empty link  |Puste łącze (Łącze nie ma żadnego tekstu)|
|![](images/wave/errors/link_skip_broken.svg)|Broken skip link |Uszkodzone łącze pomijania (Istnieje łącze pomijania, ale nie istnieje cel dla tego łącza lub łącze nie jest dostępne z klawiatury)|
|![](images/wave/errors/th_empty.svg)|Empty table header |Pusty nagłówek tabeli (W znaczniku nagłówka tabeli`<th>` nie ma żadnego tekstu)|
|![](images/wave/errors/blink.svg)|Blinking content |Migająca treść|
|![](images/wave/errors/marquee.svg)|Marquee |Marquee (Przesuwana treść)|

### Alerty i informacje o komponentach dostępności
Ostrzeżenia odnoszą się do możliwego naruszenia 17 kryteriów sukcesu, w tym 16 dotyczących kryterium sukcesu na poziomie A (KS 1.1.1, 1.2.1, 1.2.2, 1.2.3, 1.3.1, 1.3.2, 1.4.2, 2.1.1, 2.1.2, 2.4.1, 2.4.2, 2.4.3, 2.4.4, 3.2.2, 3.3.2) oraz jednego dotyczącego kryterium sukcesu na poziomie AA (KS 1.2.5).


|Ikona|Angielski komunikat błędu |Tłumaczenie komunikatu błędu
|-----|--------------------------|--------------------------------------|
|![](images/wave/alerts/alt_suspicious.svg)|Suspicious alternative text|Podejrzany tekst alternatywny|
|![](images/wave/alerts/alt_redundant.svg)|Redundant alternative text|Nadmiarowy tekst alternatywny|
|![](images/wave/alerts/alt_duplicate.svg)|A nearby image has the same alternative text|Pobliski obrazek ma ten sam alternatywny tekst|
|![](images/wave/alerts/alt_long.svg)|Long alternative text|Zbyt długi tekst alternatywny|
|![](images/wave/alerts/longdesc.svg)|Long description|Długi opis|
|![](images/wave/alerts/label_orphaned.svg)|Orphaned form label|Osierocona etykieta (nieprzypisana do kontrolki)|
|![](images/wave/alerts/label_title.svg)|Unlabeled form element with title|Kontrolka formularza bez etykiety z `title`|
|![](images/wave/alerts/fieldset_missing.svg)|Missing fieldset|Brak `fieldset`|
|![](images/wave/alerts/legend_missing.svg)|Fieldset missing legend|Brak `legend` dla `fieldset`|
|![](images/wave/alerts/heading_missing.svg)|No heading structure|Brak struktury nagłówków|
|![](images/wave/alerts/h1_missing.svg)|Missing first level heading|Brak nagłówka 1. poziomu|
|![](images/wave/alerts/region_missing.svg)|No page regions|Brak punktów orientacyjnych|
|![](images/wave/alerts/heading_skipped.svg)|Skipped heading level|Pominięty poziom nagłówka|
|![](images/wave/alerts/heading_possible.svg)|Possible heading|Możliwe, że to jest nagłówek|
|![](images/wave/alerts/table_layout.svg)|Layout table|Tabela układu|
|![](images/wave/alerts/table_caption_possible.svg)|Possible table caption|Możliwe, że jest to podpis tabeli|
|![](images/wave/alerts/link_internal_broken.svg)|Broken same-page link|Łącze do tej samej strony|
|![](images/wave/alerts/link_suspicious.svg)|Suspicious link text|Podejrzany tekst łącza|
|![](images/wave/alerts/link_redundant.svg)|Redundant link|Nadmiarowe łącze|
|![](images/wave/alerts/link_word.svg)|Link to Word document|Łącze do dokumentu Word|
|![](images/wave/alerts/link_excel.svg)|Link to Excel spreadsheet|Łącze do arkusza kalkulacyjnego Excel|
|![](images/wave/alerts/link_powerpoint.svg)|Link to PowerPoint document|Łącze do dokumentu PowerPoint|
|![](images/wave/alerts/link_pdf.svg)|Link to PDF document|Łącze do dokumentu PDF|
|![](images/wave/alerts/link_document.svg)|Link to document|Łącze do dokumentu|
|![](images/wave/alerts/audio_video.svg)|Audio/Video|Audio/Video|
|![](images/wave/alerts/html5_video_audio.svg)|HTML5 video or audio|HTML5 wideo lub audio|
|![](images/wave/alerts/flash.svg)|Flash|Flash|
|![](images/wave/alerts/applet.svg)|Java Applet|Aplet Java|
|![](images/wave/alerts/plugin.svg)|Plugin|Plugin|
|![](images/wave/alerts/noscript.svg)|Noscript element|Element `noscript` |
|![](images/wave/alerts/event_handler.svg)|Device dependent event handler|Obsługa zdarzeń zależna od urządzenia|
|![](images/wave/alerts/javascript_jumpmenu.svg)|JavaScript jump menu|Menu Skocz do oparte na JavaScript|
|![](images/wave/alerts/accesskey.svg)|Accesskey|Klawisze dostępu|
|![](images/wave/alerts/tabindex.svg)|Tabindex| `tabindex` |
|![](images/wave/alerts/text_small.svg)|Very small text|Bardzo mały tekst|
|![](images/wave/alerts/text_justified.svg)|Justified text|Tekst wyrównany obustronnie|
|![](images/wave/alerts/underline.svg)|Underlined text|Tekst podkreślony|
|![](images/wave/alerts/title_redundant.svg)|Redundant title text|Nadmiarowy atrybut `title`|


Dodatkowo WAVE zgłasza jeszcze informacje odnośnie 2 kryteriów sukcesu poza wymienionymi dotychczas (KS 3.1.2 i 4.1.2).  

Ogółem WAVE zgłasza błędy, ostrzeżenia i informacje dotyczące 19 spośród 30 kryteriów sukcesu na poziomie A oraz 4 kryteriów sukcesu spośród 20 na poziomie AA (w Polsce obowiązuje wymóg spełnienia 19 z nich). Można uznać z dużym uproszczeniem, że WAVE potrafi nam zwrócić uwagę najwyżej na około 46% możliwych błędów dostępności. 54% pozostałych kryteriów sukcesu WCAG walidator WAVE nie testuje.

|Ikona|Angielska etykieta |Tłumaczenie etykiety |
|-----|--------------------------|--------------------------------------|
|![](images/wave/info/alt.svg)|Alternative text | Tekst alternatywny |
|![](images/wave/info/alt_null.svg)|Null or empty alternative text | Pusty tekst alternatywny |
|![](images/wave/info/alt_spacer.svg)|Null or empty alternative text on spacer | Pusty tekst alternatywny w obrazie rozdzielającym |
|![](images/wave/info/alt_link.svg)|Linked image with alternative text | Łącze graficzne z tekstem  alternatywnym |
|![](images/wave/info/alt_input.svg)|Image button with alternative text | Przycisk graficzny z tekstem alternatywnym |
|![](images/wave/info/alt_map.svg)|Image map with alternative text | Mapa odsyłaczy z tekstem alternatywnym |
|![](images/wave/info/alt_area.svg)|Image map area with alternative text | Obszar mapy odsyłaczy z tekstem alternatywnym |
|![](images/wave/info/label.svg)|Form label | Etykieta kontrolki formularza |
|![](images/wave/info/fieldset.svg)|Fieldset | Zestaw pól (`fieldset`) |
|![](images/wave/info/link_skip.svg)|Skip link | Łącze pomijające |
|![](images/wave/info/link_skip_target.svg)|Skip link target | Cel łącza pomijającego |
|![](images/wave/info/lang.svg)|Element language | Język elementu |
|![](images/wave/info/h1.svg)|Heading level 1 | Nagłówek 1 |
|![](images/wave/info/h2.svg)|Heading level 2 | Nagłówek 2 |
|![](images/wave/info/h3.svg)|Heading level 3 | Nagłówek 3 |
|![](images/wave/info/h4.svg)|Heading level 4 | Nagłówek 4 |
|![](images/wave/info/h5.svg)|Heading level 5 | Nagłówek 5 |
|![](images/wave/info/h6.svg)|Heading level 6 | Nagłówek 6 |
|![](images/wave/info/ol.svg)|Ordered list | Lista uporządkowana |
|![](images/wave/info/ul.svg)|Unordered list | Lista nieuporządkowana |
|![](images/wave/info/dl.svg)|Definition/description list | Lista definicji/opisów |
|![](images/wave/info/header.svg)|Header | Nagłówek |
|![](images/wave/info/nav.svg)|Navigation | Obszar nawigacji |
|![](images/wave/info/search.svg)|Search | Obszar wyszukiwania |
|![](images/wave/info/main.svg)|Main content | Obszar treści głównej |
|![](images/wave/info/aside.svg)|Aside | Obszar uzupełniajacy (`aside`) |
|![](images/wave/info/footer.svg)|Footer | Obszar stopki |
|![](images/wave/info/table_data.svg)|Data table | Tabela danych |
|![](images/wave/info/table_caption.svg)|Table caption | Podpis tabeli |
|![](images/wave/info/th.svg)|Table header cell | Komórka nagłówkowa tabeli |
|![](images/wave/info/th_col.svg)|Column header cell | Komórka nagłówkowa kolumny tabeli |
|![](images/wave/info/th_row.svg)|Row header cell | Komórka nagłówkowa wiersza tabeli |
|![](images/wave/info/iframe.svg)|Inline Frame | Ramki wbudowane (Inline Frame) |
|![](images/wave/info/aria.svg)|ARIA | ARIA|
|![](images/wave/info/aria_label.svg)|ARIA label | Etykieta ARIA (`aria-label`)|
|![](images/wave/info/aria_describedby.svg)|ARIA description | Opis ARIA (`aria-describedby`)|
|![](images/wave/info/aria_live_region.svg)|ARIA alert or live region | Powiadomienie ARIA lub żywy region|
|![](images/wave/info/aria_menu.svg)|ARIA menu | menu ARIA (`role="menu"`) |
|![](images/wave/info/aria_button.svg)|ARIA button | Przycisk ARIA (`role="button"`|
|![](images/wave/info/aria_expanded.svg)|ARIA expanded | ARIA rozwinięte (`aria-expanded`)|
|![](images/wave/info/aria_haspopup.svg)|ARIA popup | ARIA popup (`aria-has-popup`)|
|![](images/wave/info/aria_tabindex.svg)|ARIA tabindex | ARIA tabindex|
|![](images/wave/info/aria_hidden.svg)|ARIA hidden | Ukryte atrybutem ARIA (`aria-has-popup`)|





Każdy z wyświetlonych komunikatów należy przeanalizować.

Wszelkie błędy powinny zostać usunięte. Ostrzeżenia i informacje dodatkowe należy przeanalizować i skorygować, o ile jest taka konieczność.



