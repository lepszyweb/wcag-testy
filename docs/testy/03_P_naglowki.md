## Nagłówki
Strony internetowe często posiadają sekcje informacji oddzielone wyróznionymi wizualnie nagłówkami, na przykład nagłówek jest większy i pogrubiony (jak "Nagłówki" tuż nad tym zdaniem :-). Aby te nagłówki były skuteczne dla wszystkich, muszą być oznakowane (określone jako nagłówki w kodzie). Dzięki temu użytkownicy będą mogli wykorzystać nagłowki do nawigacji po stronie, zwłaszcza osoby, które nie mogą używać  myszy i korzystają tylko z klawiatury, oraz osoby, które korzystają z czytnika ekranu.

Poziomy nagłówków powinny mieć sensowną hierarchię, np:
1. Nagłówek poziomu 1 `<h1>`
   2. Nagłówek poziomu 2 `<h2>`
      3. Nagłówek poziomu 3 `<h3>`
      3. Nagłówek poziomu 3 `<h3>`
   2. Nagłówek poziomu 2 `<h2>`
      3. Nagłówek poziomu 3 `<h3>`
         4. Nagłówek poziomu 3 `<h4>`
         4. Nagłówek poziomu 3 `<h4>`
   2. Nagłówek poziomu 2 `<h2>`

### Co sprawdzać:
-	Czy strona ma nagłówki? Na każdej stronie powinien być co najmniej jeden nagłówek.
-	Czy napisy, które wyglądają jak nagłówki są oznaczone jako nagłówki.
-	Czy napisy, które są oznaczone jako nagłówki, powinny rzeczywiście być tytułami sekcji.
-	Czy hierarchia nagłówków jest sensowna. Idealnie jest, gdy strona zaczyna się nagłówkiem `h1`, który jest zwykle podobny do tytułu strony, oraz nie pomija się na stronie poziomów nagłówków. Nie są to jednak wymagania bezwzględne.

### Sprawdzanie nagłówków
Poniższe testy zawierają instrukcje, w jaki sposób w różnych przeglądarkach uzyskać podgląd konspektu nagłówków lub znakowania nagłówków.

**Konspekt nagłówków**: przykład konspektu nagłówków na stronie:

![Konspekt nagłówków na stronie](/img/03_P_naglowki-konspekt.png) 

**Oznakowanie nagłówków**: przykład widoku strony z oznakowanymi nagłówkami:

![Oznakowanie nagłówków](/img/03_P_naglowki-znaczniki.png) 

#### Test z użyciem paska narzędzi Web Developer
Aby sprawdzić nagłówki za pomocą paska narzędzi Web Devoloper

**Konspekt nagłówków:**

1.	Otwórz stronę internetową, którą sprawdzasz.
2.	Rozwiń pasek Web Developer i wybierz opcję *Information* (Informacje), a następnie *View Document Outline* (Wyświetl konspekt dokumentu. Zostanie otwarta nowa strona z konspektem dokumentu.
3.	Testy bezwzrokowe (?):
    - Czy wykryto na stronie nagłówki? Jeśli nie, zobaczysz tekst *0 headings*.
    - Czy konspekt zaczyna się od nagłówka `[H1]`, a hierarchia nagłówków jest sensowna, poziomy nagłówków nie są pomijane? (Nie jest to wymagane, ale zdecydowanie zalecane.)
4.	**Kontrola wzrokowa**: Porównanie konspektu dokumentu z wizualną prezentacją (renderowaniem) strony.
    - Czy wszystkie napisy, które na stronie wyglądają jak nagłówki, znajdują się w konspekcie dokumentu?
    - CCzy w konspekcie dokumentu znajdują się napisy, które na stronie nie są nagłówkami (nie wyglądają jak nagłówki)? 

**Oznakowanie nagłówków**:

1.	Otwórz stronę internetową, którą sprawdzasz.
2.	Rozwiń pasek Web Developer i wybierz opcję *Outline* (Obrysy - Wyróżnianie). Następnie zaznacz opcje *Outline Headings* (Obrysuj nagłówki) oraz *Show Element Tags Names* (Wyświetlaj nazwy znaczników). Nagłówki zostaną obrysowane i oznaczone przed zawartością ikonami `<h1>`, `<h2>`, itp.
3.	Wszystko, co pełni funkcję nagłówka, powinno mieć przed sobą ikonę nagłówka.
4.	Nic, co nie pełni funkcji nagłówka, nie powinno mieć przed sobą ikony nagłówka.

#### Testy w dowolnej przeglądarce  

Aby sprawdzić nagłówki w dowolnej przeglądarce: 

**Konspekt nagłówków:**

1.	Otwórz stronę W3C z [usługą walidatora HTML](https://validator.w3.org/nu/).
2.	Zaznacz pole wyboru *Outline* (Konspekt).
3.	Wybierz opcję *Check by address* (Sprawdź wg adresu).
4.  W polu poniżej wpisz adres URI strony internetowej, którą sprawdzasz (np www.w3.org).

 
5.	Kliknij przycisk *Check* (Sprawdź). Po chwili pojawi się strona wyników.
6.	Przewiń stronę z wynikami w dół, aby przejść do sekcji *Heading-level outline* (Konspekt nagłówków).
 
7.	**Kontrola niewzrokowa**:
	- Czy coś tam jest? Jeżeli nie ma tekstu pomiędzy „Heding-level outline” albo nie wygląda to jak rzeczywisty konspekt strony”, to oznacza, że na stronie nie ma nagłówków.
	- Czy konspekt rozpoczyna się od `H1`] i ułożony jest hierarchicznie z zachowaniem poziomów nagłówków? (To nie jest to wymagane, ale wysoce zalecane).
 
8.	**Kontrola wzrokowa**. Porównanie konspektu dokumentu z wizualną prezentacją (renderowaniem) strony.
	- Czy wszystkie napisy, które na stronie wyglądają jak nagłówki, znajdują się w konspekcie dokumentu?
	- Czy w konspekcie dokumentu znajdują się napisy, które na stronie nie są nagłówkami (nie wyglądają jak nagłówki)? 

**Oznakowanie nagłówków**:

1.	Otwórz stronę internetową [narzędzia oceny dostępności WAVE](http://wave.webaim.org).
2.	W polu *Web page address* ('Adres strony internetowej') wpisz adres strony internetowej, którą chcesz ocenić.
3.	Kliknij przycisk strzałki *WAVE this page!* ('Testuj tę stronę'). Twoja strona internetowa pojawi się w przeglądarce z mnóstwem małych ikon na jej temat. Po lewej stronie w ramce pojawi się panel zarządzania narzędziem WAVE.
4.	Wszystko, co pełni funkcję nagłówka powinno mieć ikonę nagłówka (![h1](/img/03_P_h1.png), ![h2](/img/03_P_h2.png), ![h3](/img/03_P_h3.png),  itd.)
5.	Nic, co nie pełni funkcji nagłówka, nie powinno mieć ikony nagłowka.   



## Przećwicz sprawdzanie nagłówków w demo PrzediPo

1. **Konspekt nagłówków:**
   1. Postępuj zgodnie z jednym scenariuszy określonych powyżej w sekcjach „Konspekt nagłówków” powyżej i zbadaj dostępną stronę NOWINY: https://przedipo.lepszyweb.pl/after/news.html. Zauważ, że istnieje ładna hierarchiczna struktura.

![Wynik testu w Walidatorze HTML - Konspekt nagłówków na dostępnej stronie Nowiny](/img/03_P_naglowki_nu-html-po.png)

   2. Następnie za pomocą niedostępnych stronę NOWINY: https://przedipo.lepszyweb.pl/before/news.html. (W HTML Validator, przycisk „Sprawdź” może teraz powiedzieć: „Ponownie zweryfikuj”). Zauważ, że na stronie nie ma ani jednego nagłówka.

![Wynik testu w Walidatorze HTML - brak konspektu nagłówków na niedostępnej stronie Nowiny](/img/03_P_naglowki_nu-html-przed.png)
 
2. **Oznakowanie nagłówków**:

   1. Zacznij od kontroli wzrokowej, patrząc na naszym demo PrzediPO na niedostępną wersję strony NOWINY: https://przedipo.lepszyweb.pl/before/news.html. Co wygląda na nagłówki? (Nowiny Świateł Miasta, Klimatyzacja źródłem fali upałów, 9 miesięcy za kradzież skrzypiec, Twardy Przewałek, Zwrot do nadawcy, Twój krzyk, Brak mózgów utrudnia badania naukowe,)
   
   ![Napisy na niedostępnej stronie Nowiny wyglądające jak nagłówki](/img/03_P_naglowki_przed.png)  
   2. Następnie sprawdź, jak to powinno wyglądać. Wykonać jedną z instrukcji z sekcji „Znaczniki nagłówków na stronie” powyżej na naszym demo PrzediPo na dostępnej wersji strony NOWINY: https://przedipo.lepszyweb.pl/after/news.html. Na przykłaąd skorzystaj z narzędzia WAVE. Zauważ, że obok nagłówków pojawiają się ikony nagłówków.
   
   ![Wynik testu WAVE - oznakowane nagłówki na dostępnej stronie Nowiny](/img/03_P_naglowki_wave-przed.png)
 
   3. Następnie zobaczyć, jak to wygląda, gdy nagłówki nie są oznakowane. Przetestuj niedostępną wersję strony NOWINY: https://przedipo.lepszyweb.pl/before/news.html Zauważ, że teksty w kilku miejscach wyglądają na nagłówki, ale nie obok nich nie ma ikon symbolizujących nagłówki. (Są żółte ikony z „h?”, ponieważ WAVE uważa, że prawdopodobnie powinny to być nagłówki).
   
   ![Wynik testu WAVE - brak oznakowania nagłówków na niedostępnej stronie Nowiny](/img/03_P_naglowki_wave-po.png)
 
### Dowiedz się więcej o nagłówkach 
-	[Zrozumieć kryterium sukcesu 1.3.1 Informacje i relacje](https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html)  - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 2.4.6 Nagłówki i etykiety](https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html)  - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.
-	[Zrozumieć kryterium sukcesu 2.4.10 Nagłówki sekcji](https://www.w3.org/WAI/WCAG21/Understanding/section-headings.html)  - artykuł w języku angielskim, skorzystaj z tłumaczenia Google.


-------------------------------------
[Teksty alternatywne obrazów &lt; Poprzednia strona](testy/02_P_odpowiedniki-tekstowe-obrazow.md) | [Następna strona &gt; Kontast kolorów](04_P_kontrast-kolorów.md)
