## Zgodność
Ta sekcja pełni funkcję <a title="definicja: normatywny" href="#normativedef" class="termref">normatywną</a>.

W tej sekcji znajdują się wymagania dotyczące <a title="definicja: zgodność" href="#conformancedef" class="termref">zgodności</a> z wytycznymi WCAG 2.0, jak również informacje, w jaki sposób można ogłosić zgodność strony (opcjonalnie). Na końcu wyjaśnione zostało pojęcie <a title="definicja: wspierający dostępność" href="#accessibility-supporteddef" class="termref">wsparcia dla 
dostępności</a>, gdyż tylko technologie wspierające dostępność mogą stanowić <a title="definicja: (technologie) stanowiące podstawę zgodności" href="#reliedupondef" class="termref">wiarygodną podstawę zgodności</a>. Dokument o nazwie „[Understanding Conformance](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html)” zawiera dalsze wyjaśnienie pojęcia wsparcia dla dostępności.

### Wymogi zgodności
Aby strona internetowa była zgodna z wytycznymi WCAG 2.0, wszystkie poniższe wymogi zgodności muszą zostać spełnione:

   1. **Poziom zgodności:** Jeden z poniższych poziomów zgodności jest w pełni osiągnięty:
      - **Poziom A:** Aby osiągnąć poziom zgodności A (poziom minimalny), <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strona internetowa</a> <a title="definicja: spełnienie kryterium sukcesu" href="#satisfiesdef" class="termref">spełnia</a> wszystkie kryteria sukcesu na poziomie A, lub też dostępna jest <a title="definicja: wersja alternatywna zapewniająca zgodność" href="#conforming-alternate-versiondef" class="termref">wersja alternatywna spełniająca kryteria</a> sukcesu na poziomie A.
	  - **Poziom AA:** Aby osiągnąć poziom zgodności AA, strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A oraz na poziomie AA, lub też dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie AA.
	  - **Poziom AAA:** Aby osiągnąć poziom zgodności AAA, strona internetowa spełnia wszystkie kryteria sukcesu na poziomie A, na poziomie AA oraz na poziomie AAA, lub też dostępna jest wersja alternatywna spełniająca kryteria sukcesu na poziomie AAA.

      *Uwaga 1:* Chociaż zgodność może zostać osiągnięta tylko na oznaczonych poziomach, zachęca się autorów, aby podawali (w oświadczeniu zgodności) jakikolwiek postęp na drodze do spełnienia kryteriów sukcesu na poziomach wyższych niż osiągnięty.
	  
	  *Uwaga 2:* Odradza się wyznaczania poziomu AAA jako wymaganego dla całych serwisów, gdyż w przypadku niektórych treści, spełnienie wszystkich kryteriów sukcesu na poziomie AAA nie jest możliwe.
	  
   2. **Całe strony:** <a title="definicja: zgodność" href="#conformancedef" class="termref">Zgodność</a> (oraz poziomy zgodności) dotyczy całej <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strony</a> i nie można jej osiągnąć, jeśli jakaś część strony zostanie wyłączona z oceny.
   
   *Uwaga 1:* W celu ustalenia zgodności, przyjmuje się, iż wersje alternatywne części treści strony są częścią strony, jeśli wersje alternatywne są dostępne bezpośrednio z danej strony, np. długi opis lub alternatywna prezentacja nagrania wideo.
   
   *Uwaga 2:* Autorzy stron internetowych, którzy nie mogą osiągnąć zgodności ze względu na treść pozostającą poza ich kontrolą, mogą rozważyć [Stwierdzenie częściowej zgodności](http://www.w3.org/TR/2008/REC-WCAG20-20081211/#conformance-partial).
   
   3. **Zakończona procedura:** Jeśli dana <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strona</a> jest jedną z wielu stron prezentujących jakąś <a title="definicja: procdura" href="#processdef" class="termref">procedurę</a> (tzn. sekwencję kroków, które należy wykonać, aby dokończyć jakąś czynność), to wszystkie te strony osiągają co najmniej ten sam lub wyższy poziom zgodności. (Zgodność na wybranym poziomie nie jest możliwa, jeśli którakolwiek ze stron nie spełnia wybranego poziomu.)
   
   *Przykład:* Sklep internetowy prezentuje na kilku stronach procedurę wybierania i zakupu produktów. Wszystkie strony w tej procedurze, od początku do końca (do wykonania płatności) są zgodne na tym samym poziomie.

   4. **Użycie technologii wspierających dostępność:**  Tylko <a title="definicja: technologie tworzenia treści internetowych" href="#technologydef" class="termref">technologie</a> <a title="definicja: wspierający dostępność" href="#accessibility-supporteddef" class="termref">wspierające dostępność</a> są uwzględniane jako podstawa spełnienia kryteriów sukcesu. Każda informacja czy funkcjonalność, która nie jest dostarczona w postaci wspierającej dostępność, ma swoją alternatywną wersję wspierającą dostępność. (Więcej informacji: [Understanding accessibility suport](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-accessibility-support-head))

   5. **Brak zakłóceń:** Jeśli na stronie wykorzystywane są <a title="definicja: technologie tworzenia treści internetowych" href="#technologydef" class="termref">technologie</a>, które nie <a title="definicja: wspierający dostępność" href="#accessibility-supporteddef" class="termref">wspierają dostępności</a> lub są użyte tak, że nie wspierają dostępności, użytkownicy powinni mieć swobodny dostęp do pozostałej części strony. Dodatkowo, <a title="definicja: strona internetowa" href="#webpagedef" class="termref">strona</a> nadal spełnia wymogi zgodności pod każdym z następujących warunków:

     1. kiedy technologia, która nie jest <a title="definicja: (technologie) stanowiące podstawę zgodności" href="#reliedupondef" class="termref">uwzględniana</a>, jest włączona w programie użytkownika,

     2. kiedy technologia, która nie jest uwzględniana, jest wyłączona w programie użytkownika, oraz

     3. kiedy technologia, która nie jest uwzględniana, nie jest wspierana przez program użytkownika.

     Dodatkowo, następujące kryteria sukcesu dotyczą całej treści na stronie, włącznie z treścią, która w innych przypadkach nie jest podstawą spełnienia wymogów zgodności, gdyż niezastosowanie poniższych kryteriów mogłoby uniemożliwić jakiekolwiek skorzystanie ze strony:

     - **1.4.2 Kontrola odtwarzania dźwięku**
     - **2.1.2 Brak pułapki na klawiaturę**
     - **2.3.1 Trzy błyski lub wartości poniżej progu**
     - **2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie**

      *Uwaga:* Jeśli strona nie jest zgodna (na przykład testowa strona zgodności lub strona przykładowa), nie może być włączona w zakres zgodności lub dołączona do oświadczenia zgodności.

      Więcej informacji, w tym przykłady, w [Understanding Conformance Requirements](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conformance-requirements-head).

### Stwierdzanie zgodności (opcjonalne)

Zgodność zdefiniowana została tylko dla (pojedynczych)  <a title="definicja: strona internetowa" href="#webpagedef" class="termref">stron internetowych</a>. Jednak oświadczenie zgodności może dotyczyć pojedynczej strony, kilku stron lub całych serwisów internetowych.

#### Wymagane części składowe oświadczenia zgodności
Oświadczenie zgodności **nie jest wymagane**. Autorzy mogą wdrożyć wytyczne WCAG 2.0 bez oświadczania zgodności. Jednak jeśli takie oświadczenie zostanie wykonane, wtedy **musi** zawierać następujące informacje:

1. **Data** stwierdzenia.</p>
2. **Tytuł wytycznych, wersja oraz adres URI** („Wytyczne dla dostępności treści internetowych 2.0” pod adresem <a href="http://www.w3.org/TR/2008/REC-WCAG20-20081211/">http://www.w3.org/TR/2008/REC-WCAG20-20081211/</a> (wersja anglojęzyczna).</p>
3. Osiągnięty **poziom zgodności** (Poziom A, AA lub AAA).
4. **Zwięzły opis stron internetowych**, taki jak lista adresów URI objętych oświadczeniem, wraz z adnotacją czy włączone są również poddomeny.

*Uwaga 1:* Strony mogą być opisane oddzielnie, ale również może być użyty jeden opis dla wszystkich adresów URI.

*Uwaga 2:* Produkty internetowe nie posiadające adresów URI przed instalacją na stronie klienta, mogą zostać opatrzone informacją, 
że po instalacji będą spełniać wymogi.

5. Lista **<a title="definition: relied upon (technologies that are)" href="#reliedupondef" class="termref">uwzględnionych</a> <a title="definicja: technologie tworzenia treści internetowych" href="#technologydef" class="termref">technologii tworzenia treści internetowych</a>**.

*Uwaga:* Jeśli wykorzystywane jest logo zgodności, oznacza to de facto oświadczenie zgodności i musi wystąpić razem z wymaganymi, wyżej wymienionymi składowymi oświadczenia zgodności.


#### Opcjonalne części składowe oświadczenia zgodności
Poza wymaganymi składowymi oświadczenia zgodności, które zostały wymienione powyżej, warto rozważyć umieszczenie dodatkowych informacji, przydatnych dla użytkowników. Polecane dodatkowe informacje to, na przykład:

- Lista spełnionych kryteriów sukcesu, wyższych niż zawarty w oświadczeniu poziom zgodności. Taką informację należy podać w formie, którą użytkownik mógłby wykorzystać, najlepiej jako metadane odczytywalne maszynowo.
- Lista poszczególnych technologii, które „są wykorzystywane, ale nie są <a title="definicja: (technologie) stanowiące podstawę zgodności" href="#reliedupondef" class="termref">uwzględniane w ocenie zgodności</a>”.
- Lista programów użytkownika, w tym technologii wspomagających, wykorzystywanych do testowania treści.
- Informacja na temat wszelkich podjętych kroków w celu zwiększenia dostępności, a które wykraczają poza kryteria sukcesu.
- Lista poszczególnych technologii, które są <a title="definicja: (technologie)stanowiące podstawę zgodności" href="#reliedupondef" class="termref">uwzględnione</a> w ocenie, w formie metadanych odczytywalnych maszynowo.
- Wersja oświadczenia zgodności, w formie metadanych odczytywalnych maszynowo.


*Uwaga 1:* Więcej informacji oraz przykładowe oświadczenia zgodności można znaleźć w dokumencie „[Understanding Conformance Claims](http://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html#uc-conformance-claims-head)”.

*Uwaga 2:* Więcej informacji na temat wykorzystania metadanych w oświadczeniach zgodności znajduje się w dokumencie [Understanding Metadata](http://www.w3.org/TR/UNDERSTANDING-WCAG20/appendixC.html#understanding-metadata)”.

### Oświadczenie częściowej zgodności – treść umieszczana przez dostawców zewnętrznych

Czasem strony internetowe tworzone są w taki sposób, aby móc je później uzupełnić dodatkową treścią. Na przykład jest to program do 
poczty elektronicznej, blog, artykuł, który pozwala użytkownikom na dodanie swoich komentarzy, lub też aplikacja pozwalająca na tworzenie 
treści przez użytkowników. Kolejny przykład, to strona, taka jak portal lub serwis informacyjny, składający się z treści agregowanych od wielu współautorów, lub też strony, które automatycznie umieszczają treść pobraną z innych źródeł w danym okresie czasu, np. dynamicznie 
umieszczane reklamy.

W takich przypadkach nie można przewidzieć, w momencie opublikowania strony, jaka dodatkowa, niekontrolowana przez autora treść
 pojawi się w przyszłości. Ważna jest świadomość, iż niekontrolowana treść może negatywnie wpłynąć także na dostępność treści zaplanowanej przez autora. Istnieją dwa rozwiązania:

1. Ustalenie zgodności można oprzeć na zasadzie pełnej posiadanej wiedzy na dany moment. Oznacza to, iż strona jest zgodna, jeśli jest 
monitorowana i skorygowana (treść niezgodna jest usuwana lub zmieniona tak, aby spełniała wymogi zgodności) w ciągu dwóch dni roboczych; od tego momentu można ustalać zgodność strony, wykluczając błędy w treści dodanej zewnętrznie, które są poprawiane lub usuwane, kiedy się je napotka. Nie można złożyć oświadczenia zgodności, jeśli monitorowanie lub korekta niezgodnej treści nie jest możliwa.

**LUB:**

2. Można złożyć „Oświadczenie częściowej zgodności”, jeśli strona nie jest zgodna, lecz spełniałaby wymogi zgodności, gdyby pewne jej 
części zostały usunięte. Brzmienie takiego oświadczenia jest następujące: „Niniejsza strona nie jest zgodna, lecz spełniałaby wymogi 
WCAG 2.0 na poziomie X, gdyby następujące, niekontrolowane przez autora treści zostały usunięte”. Dodatkowo, treść niekontrolowana musi spełnić poniższe kryteria:
   
   1. Nie jest to treść, która jest pod kontrolą autora.
   2. Jest opisana w sposób identyfikowalny dla użytkowników (np. nie można stwierdzić jedynie „wszystkie części, których nie kontrolujemy”, muszą być one odpowiednio oznaczone).
   
### Oświadczenie częściowej zgodności – język
„Oświadczenie częściowej zgodności ze względu na język” umieszczane jest w przypadkach, kiedy dana strona nie jest zgodna, 
jednak mogłaby spełnić wymogi zgodności, jeśli istniałoby <a title="definicja: wspierający dostępność" href="#accessibility-supporteddef" class="termref">wsparcie dla dostępności</a> wszystkich języków użytych na tej stronie. Brzmienie takiego oświadczenia jest następujące: „Niniejsza strona nie jest zgodna, lecz spełniałaby wymogi WCAG 2.0 na poziomie X, gdyby istniało wsparcie dla dostępności następujących języków”.
