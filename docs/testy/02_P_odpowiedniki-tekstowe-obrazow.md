## Teksty alternatywne obrazów ( „odpowiedniki tekstowe”)

Współczesne technologie nie potrafią jeszcze odczytać i przekazać odpowiednio treści obrazów osobom, które ich z różnych względów nie mogą zobaczyć. Dlatego każdy obraz w dokumencie i na stronie internetowej musi posiadać odpowiednik tekstowy, inaczej zwany tekstem alternatywnym lub alternatywą tekstową.

Odpowiedniki tekstowe przekazują cel obrazów, w tym zdjęć, ilustracji, wykresów, itp. Odpowiedniki tekstowe są przeznaczone dla osób, które nie widzą obrazu. Na przykład osoby niewidome, które używają czytników ekranu, usłyszą tekst alternatywny. A osoby, które wyłączyły zdjęcia, aby przyspieszyć pobieranie stron, mogą zobaczyć i odczytać teksty alternatywne.

Odpowiednik tekstowy powinien spełniać tę samą rolę, co obraz i zapewnić użytkownikom, którzy nie widzą obrazu, równoważne doświadczenie, a niekoniecznie opisać obraz. Na przykład właściwym odpowiednikiem tekstowym dla przycisku wyszukiwania ![Szukaj](/img/02_P_przycisk-szukaj.png)  będzie słowo  „Szukaj”, a nie „lupa” czy „Szkło powiększające”.  

Tekstu alternatywnego zwykle nie widać na stronie, znajduje się on jednak w kodzie strony jako atrybut znaczników, które osadzają obraz na stronie, np.

```<img src = "nazwa-pliku-obrazu.png" alt = "Tutaj znajduje się tekst alternatywny">```

Każdy obraz osadzony na stronie powinien zawierać atrybut w osadzającym go znaczniku atrybut alt.
-	Jeśli obraz przekazuje jakiekolwiek informacje istotne w interakcji z treściami strony internetowej lub niezbędne do jej zrozumienia, to informacje te powinny być przekazane tekstem alternatywnym.
-	Jeżeli obraz spełnia tylko funkcję dekoracyjną i użytkownicy nie muszą wiedzieć o obrazie, żeby poznać treść strony i wykonać zadania na stronie, to obraz powinien mieć pusty atrybut alt ( `alt=""`), czyli bez żadnego tekstu.
Testy automatyczne mogą cię poinformować, jedynie o tym, w których znacznikach brakuje atrybutu `alt`. Aby ustalić, czy tekst alternatywny jest odpowiedni, trzeba zobaczyć obraz i oceniać go w kontekście.

### Co sprawdzać:
-	Czy każdy obraz ma atrybut alt z odpowiednim tekstem alternatywnym.

### Wskazówki
Formułowanie odpowiednich tekstów alternatywnych adekwatnych do treści i funkcji obrazów nie opiera się na ścisłych regułach, które prowadziłyby do sytuacji, że bez względu na to, kto opracowuje tekst alternatywny, to zawsze ten tekst będzie taki sam (w przypadku tego samego obrazu. Ponadto, niektórzy ludzie wolą, aby obrazy posiadały szczegółowe opisy; a inni wolą zwięzłe, znacznie mniej dokładne opisy.

#### Odpowiedni tekst alternatywny: 
-	Tekst alternatywny musi przekazać to samo znaczenie co obraz. Oznacza to, że jeśli ktoś nie widzi obrazu, to ważne informacje wyrażane obrazem otrzymuje w tekście alternatywnym.
-	Tekst alternatywny zależy od kontekstu. Na przykład tekst alternatywny dla obrazu psa na stronie klubu hodowców psów może zawierać rasę psa; ale ten sam obraz na stronie internetowej o parku psów może tylko sprawiać, że strona będzie bardziej atrakcyjna, ale obraz nie wnosi do niej żadnej treści. W takim przypadku obraz może nie potrzebować żadnego tekstu alternatywnego, a wiec powinien mieć pusty atrybut alt. Jednym ze sposobów pomagającym ustalić odpowiedni tekst atrybutu alt jest odpowiedź na pytanie: co można by powiedzieć o obrazie, gdy komuś pomagasz czytać i wchodzić w interakcje ze stroną internetową, której nie może zobaczyć?
-	Obrazy „funkcjonalne” - na przykład inicjujące akcje (takie jak przyciski Wyślij) czy obrazy linkujące (np. ikony w nawigacji) - potrzebują tekstu alternatywnego, który przekazuje funkcję obrazu, a więc nie tekstu, który opisuje obraz, lecz tekstu, który wskazuje cel łącza albo funkcję przycisku. 
-	Jeśli na obrazie znajduje się tekst - na przykład w logo - ten tekst musi zostać uwzględniony w tekście alternatywnym.
-	Jeśli obraz przekazuje złożone informacje - np. wykres lub graf – to w tekście alternatywnym należy umieścić zwięzłe określenie roli obrazu, a w treści zawierającej obraz umieścić szczegółowe informacje przekazywane przez obraz (na prrzykład w tabeli danych).

#### Co nie jest potrzebne w tekście alternatywnym: 
-	**opis wyglądu obrazu**: jeśli obraz nie jest istotny dla zrozumienia treści - na przykład jest to tylko ozdoba  - powinien mieć pusty atrybut alt (alt = ""). Jednym ze sposobów na określenie, czy obraz powinien mieć pusty alt jest zadać sobie pytanie: Czy użytkownik nadal otrzyma wszystkie informacje ze strony, jeśli obraz zostanie usunięty?
-	**zbędne słowa takie jak „obraz”, „przycisk”, „link”**. Czytniki ekranu zapewniają te informacje automatycznie.
-	**powtórzenia opisu zawartego w treści**: jeśli obraz jest wystarczająco opisany w tekście - na przykład prosty diagram ilustrujący to, co jest napisane w tekście strony - może zawierać krótki tekst alt, taki jak " Schemat przepływu pracy opisany powyżej.”

### Atrybut alt,  a nie "znacznik alt " 
W kodzie HTML strony internetowej, zwanym też znakowaniem, `alt` jest **atrybutem** elementów osadzających obrazy, elementu `img` i elementów `applet`, `area` oraz elementu `input` typu `image`. Określenie „znacznik alt” jest nieprawidłowe technicznie, poprawną terminologią jest **atrybut alt** albo **tekst alternatywny**). 
Atrybut alt wygląda w kodzie strony np. tak: 

```<img alt="Logo WAI" src="/wai/logo.png">```

###  Tekst alternatywny, alternatywa tekstowa czy odpowiednik tekstowy

Każdy z tych terminów jest poprawny i każdy z nich można zastosować do opisywanych tutaj przypadków. Gdy mówimy o tekście umieszczanym w atrybucie `alt`, najlepszym terminem jest „tekst alternatywny”. Gdy mówimy o równoważnym teście w treści obok obrazu właściwszymi terminami są „odpowiednik tekstowy” albo „alternatywna tekstowa”.    


###  Sprawdzanie tekstów alternatywnych
Istnieją kilka możliwości, aby sprawdzić tekst alternatywny. Dwie przedstawiamy poniżej
### Użyj narzędzi paska Web Developer
**Uwaga**: Jeśli nie masz zainstalowanego w swojej przeglądarce paska narzędzi Web Developer:
-	[Pobierz narzędzie Web Developer dla przeglądarki Chrome](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=pl)
-	[Pobierz narzędzie Web Developer dla przeglądarki Firefox](https://addons.mozilla.org/pl/firefox/addon/web-developer/) 
-	[Pobierz narzędzie Web Developer dla przeglądarki Opera](https://addons.opera.com/pl/extensions/details/web-developer/)
  
**Aby sprawdzić tekst alternatywny za pomocą narzędzia Web Developer:**  
-	Otwórz stronę internetową, którą sprawdzasz.
-	Rozwiń pasek Web Developer i wybierz opcję *Images* ('Obrazy'), a następnie opcję  *Outline Images Without Alt Atttributes* ('Obrysuj wszystkie obrazy bez atrybutu alt'). Wokół wszystkich obrazów bez atrybutu alt pojawią się czerwone obrysy. 
	![Menu paska narzędzi Web Developer i czerwone kontury obrazków bez atrybutu alt](/img/02_P_alt_web-developer-bez-alt.png)
-	Zanotuj informację o wszystkich obrazach, które nie posiadają tekstu alternatywnego. Najlepiej wykonaj zrzut ekranu, aby dysponować zestawieniem obrazów, które nie posiadają tekstu alternatywnego.  Możesz również wskazać kolejno każdy z obrazków i wybrać z menu kontekstowego przeglądarki opcję Zbadaj element, a następnie skopiować z panelu kod osadzający obrazek:

	![Kod obrazka w kodzie strony](/img/02_P_alt_skopiuj_kod_obrazka.png) 
	
-	Następnie wyłącz opcję *Outline Images Without Alt Atttributes*, a włącz opcję *Outline All Images* ('Obrysuj wszystkie obrazy') oraz *Display Alt Attributes* ('Wyświetlaj atrybuty alt')  
Wokół wszystkich obrazów pojawią się czerwone obrysy. Obok obrazów z atrybutem alt pojawią teksty alternatywne (białe na czerwonym tle).  

	![Menu paska narzędzi Web Developer z wybranymi opcjami Obrysuj wszystkie obrazy i Wyświetl atrybuty alt oraz fragment strony z obrysowanymi obrrazami i tekstami alternatywnymi](/img/02_P_alt_web-developer-z-alt.png)
	
-	Rozważ, czy tekst alternatywny każdego obrazu właściwie przekazuje informacje o obrazie, zgodnie ze wskazówkami powyżej. Zanotuj uwagi.
-	Na koniec włącz opcję *Outline Images With Empty Alt Attributes* ('Obrysuj wszystkie obrazy z pustym atrybutem alt'). Opcję *Outline Alt Images* możesz wyłączyć. 

	![Menu paska narzędzi Web Developer i oznaczone obrazy z pustym atrybutem alt](/img/02_P_alt_web-developer-z-alt.png)

-	Rozważ, czy pozostawienie pustego atrybutu alt w przypadku każdego obrazu jest uzasadnione, czy rzeczywiście w każdym przypadku jest to obraz dekoracyjny, a treść będzie kompletna i zrozumiała bez obrazu. Zanotuj uwagi.

**Aby sprawdzić tekst alt w dowolnej przeglądarce**
-	Otwórz stronę internetową [narzędzia oceny dostępności WAVE](http://wave.webaim.org).

	![Strona WAVE z polem na adres strony, którą chcesz zbadać](/img/02_P_alt_wave_wpisz_adres.png)
	
-	W polu *Web page address* ('Adres strony internetowej') wpisz adres strony internetowej, którą chcesz ocenić.
-	Kliknij przycisk strzałki *WAVE this page!* ('Testuj tę stronę'). 
Twoja strona internetowa pojawi się w przeglądarce z mnóstwem małych ikon na jej temat. Po lewej stronie w ramce pojawi się panel zarządzania narzędziem WAVE. 
-	**Aby sprawdzić, czy brakuje alt**: wyszukaj czerwoną ikonę alt (![Ikona Brak alta](/img/02_P_alt_missing.png)) lub poszukaj tekstu alt *ERROR: Missing alt text*. Jeśli go znajdziesz, oznacza to, że poniższy obraz nie ma atrybutu `alt`. Być może na starszych witrynach znajdziesz także ikonę (![Ikona Obraz odstępu bez alta](/img/02_P_alt_spacer_missing.png)) oznaczającą obrazy użyte do formatowania odstępów między elementami (ERRORS: Spacer image missing alternative text)  
-	**Aby sprawdzić, czy nie brakuje atrybutu alt dla obrazków „funkcjonalnych”**: wyszukaj ikonę (![Ikona Obraz odstępu bez alta](/img/02_P_alt_link_missing.png)) lub poszukaj tekstu alternatywnego ERRORS: Linked image missing alternative text.
-	**Aby sprawdzić, czy tekst alt jest odpowiedni**: 
Poszukaj ikony zielonej alt (![Tekst alternatywny](/img/02_P_alt_alt.png)). Obok jest tekst na jasnozielonym tle; tekst alt jest między gwiazdkami (*). czy tekst alt przekazuje informacje o obrazie stosownie do wskazówek powyżej.
 
## Przećwicz sprawdzanie tekstu alternatywnego w demo PrzediPo  
 
W ramach ćwiczeń przygotowawczych do powyższych testów możesz sprawdzić problemów z dostępnością obrazów w naszym [Demo PrzediPo: Niedostępna strona główna](https://przedipo.lepszyweb.pl/before/home.html). 

### Wskazówki:
-	**Brakujący alt**:
	-	Na stronie jest wiele obrazów bez tekstu alternatywnego. (Wiele z nich jest tylko dekoracyjnych, więc powinny mieć pusty tekst alternatywny, zgodnie ze wskazówkami powyżej.)
	-	Obraz pogodynki przedstawiający chmurę i słońce nie ma atrybutu alt.
-	**Niewłaściwy tekst alternatywny**:
	-	Nieco poniżej górnej krawędzi znajduje się długi tekst alternatywny dla obrazu logo strony, zaczynający się od słów: Logo. Niebieska kropka z białą literą 'M'. Opis ten jest zbyt szczegółowy i zawiera nieistotne informacje. Odpowiedni tekst alternatywny na stronie dostępnej stronie brzmi: "Światła Miasta: Twoje okno na miasto.".
	-	Na dole, w obszarze treści głównej znajduje się obraz tekstu (1)269 K-A-R-C-Z-O-C-H” (numer telefonu w systemie amerykańskim). Alternatywą dla tego tekstu jest ciąg cyfr: „123456789”, który nie jest równoważny tekstowi na obrazku.  
-	**Odpowiedni tekst alternatywny**:
	-	W nagłówku strony wyświetlane jest logo pracowni LepszyWeb. Tekstem alternatywnym dla logo jest „LepszyWeb.pl. Pracownia Dostępności Cyfrowej”.
 
## Dowiedz się więcej o tekście alternatywnym 
-	[Text alternatives for non-text content](http://www.w3.org/WAI/intro/people-use-web/principles#alternatives) (Tekst alternatywny dla terści nietekstowych)  - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 1.1.1 Treść nietekstowa](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html)  - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[An alt text decision tree](https://www.w3.org/WAI/tutorials/images/decision-tree/) (Drzewo decyzji o atrybucie alt) - artykuł w języku angielskim, skorzystaj z tłumaczenia Google. 
-------------------------------------
[Tytuł strony &lt; Poprzednia strona](testy/01_P_tytul-strony.md) | [Następna strona &gt; Nagłówki](testy/03_P_naglowki.md)