# Streszczenie

## Podsumowanie ustaleń


## 1.	 Funkcje na wielu stronach

Są to funkcje, które występują na każdej stronie i w większości przypadków będą szczegółowo testowane na pierwszej stronie oraz potwierdzane pod względem spójności na podzbiorze stron.

### Identyfikacja języka
**Metoda badania**: Sprawdzenie elementu html w kodzie strony. W górnej części strony kliknij prawym przyciskiem myszy i wybierz element kontroli (IE lub Chrome). Zeskanuj stronę pod kątem zawartości w innym języku.  Sprawdzenie elementu zawierającego element w poszukiwaniu odpowiedniego atrybutu językowego.

#### Oczekiwanie: 
- Element html zawiera atrybut języka, a określony język pasuje do głównego języka strony. [3.1.1 Język strony](https://wcag.lepszyweb.pl/#language-of-page)
- Zawartość w innych językach ma odpowiednio zdefiniowany atrybut językowy na elemencie zawierającym. [3.1.2 Język części](https://wcag.lepszyweb.pl/#language-of-parts)

#### Ustalenia:

#### Limity czasu
**Metoda badania**: Poczekaj, aż strona się skończy, jest to zazwyczaj odkrywane podczas szczegółowych testów.

#### Oczekiwanie: 
[2.2.1 Możliwość dostosowania czasu](https://wcag.lepszyweb.pl/#timing-adjustable)
- Ostrzeżenie jest przedstawiane - i ukierunkowane
- Obecna jest metoda klawiaturowa umożliwiająca wydłużenie limitu czasu pracy.

#### CAPTCHA

**Metoda badania**: Zidentyfikować wszystkie dostępne metody ukończenia CAPTCHA.

#### Oczekiwanie:
Istnieją metody uzupełnienia CAPTCHA przy użyciu różnych sensów i metod. [1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content)

#### Ustalenia:

#### Nagłówek
##### Logo

**Metoda badania**: Kontrola kodu, użycie narzędzia ujawniającego tekst zmiany.

**Oczekiwania**: ([1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content)
-Alternatywny tekst będzie zawierał tekst w logo i wskazywał podmiot będący właścicielem strony.

#### Ustalenia:

##### Wyszukiwarka

#### Oczekiwanie:
- Oznaczone jako "Szukaj" lub równorzędne.
- Etykieta jest trwała.
- Brak pułapki na klawiaturę
- Aktywuje się tylko na czynnościach użytkownika.

#### Nawigacja
##### Linki pomijające
**Metoda badania**: Kontrola i test ręczny
Określić liczbę aktywnych elementów przed rozpoczęciem zawartości głównej.
Przejdź na górę strony i naciśnij raz przycisk zakładki, aby ustawić ostrość na łączu.
- Użyj narzędzia kontrolnego lub aktywuj łącze, aby określić miejsce przeznaczenia łącza "skip".

#### Oczekiwanie:
Oczekiwania [2.4.1 Możliwość pominiecia bloków](https://wcag.lepszyweb.pl/#bypass-blocks)
Jeśli pomiędzy górną krawędzią strony a jej zawartością główną znajduje się więcej niż pięć aktywnych elementów, znajduje się link do pomijania.
- Link "skip" jest linkiem tekstowym (patrz wymagania dotyczące kontrastu).
- łącze przeskoku jest zawsze widoczne lub staje się widoczne na ostrości.
- Uruchomienie linku powoduje, że na początku głównego obszaru treści skupiają się miejsca, w których znajduje się link.

#### Punkty orientacyjne lub oznaczenia sekcji
**Metoda badania**: Inspekcja
- Użyj narzędzia kontrolnego, aby określić obszary orientacyjne.

#### Oczekiwanie:
Oczekiwania (jeśli stosowane są regiony przełomowe): [3.2.3 Konsekwentna nawigacja](https://wcag.lepszyweb.pl/#consistent-navigation), [3.2.4 Konsekwentna identyfikacja](https://wcag.lepszyweb.pl/#consistent-identification)

- Każdy obszar na stronie ma charakterystyczny region, który odpowiada jego celowi.
  - Header/Banner (nagłówek, tylko jeden)
  - Search (yyszukiwanie)
  - Footer/ContentInfo (stopka, tylko jedna)
  - Nav/Navigation (nawigacja, jeżeli więcej niż jedna, każda jest wyraźnie zidentyfikowana)
  - Main/Main  (główna zawartość, tylko jeden)
  - Aside (jeśli więcej niż jeden, każda jest wyraźnie zidentyfikowany)
- Gdy używana jest więcej niż jedna instancja typu regionu, identyfikuje się ją za pomocą
  - atrybutu aria-labelledby wskazującego widoczny nagłówka
  - atrybutu aria-label, jeżeli sekcja nie rozpoczyna się od nagłówka
- Liczba sekcji została zminimalizowana.


#### Ustalenia:

##### Menu nawigacyjne

**Metoda badania**: Inspekcja/Manualna
- Użyj narzędzia kontrolnego, aby określić rolę i stan pozycji menu z podmenu
- Testuj ręcznie za pomocą klawiatury i czytnika ekranu, aby ustalić, czy podmenu otwiera się tylko po akcji użytkownika
- Testuj ręcznie za pomocą czytnika ekranu, aby ustalić, czy stan jest przekazywany poprawnie
#### Oczekiwanie:
- Podmenu można pominąć.
- Stan podmenu jest przekazywany za pomocą rozszerzenia atrybutu aria-expanded.

### Footer (Stopka)
(Dodaj funkcje z testów na poziomie strony, które są obecne w stopce.)




## 2. Cechy na każdej stronie

## Tytuł strony
**Metoda badania**: Sprawdzenie elementu tytułowego w nagłówku dokumentu. Kliknij prawym przyciskiem myszy i wybierz element kontrolny (IE lub Chrome).
#### Oczekiwanie:
 Tytuł strony jest unikalny dla strony w interfejsie i dokładnie opisuje cel strony. [2.4.2 Tytuły stron](https://wcag.lepszyweb.pl/#page-titled)

#### Ustalenia:

### Kolory i kształty
Kolor nie jest jedynym środkiem przekazu znaczenia.
**Metoda badania**: Obejrzyj stronę wizualnie.
#### Oczekiwanie:
 Jeśli kolor jest używany do identyfikacji, ta sama identyfikacja jest dostępna w tekście. [1.4.1 użycie koloru](https://wcag.lepszyweb.pl/#use-of-color)


### Kształt, rozmiar lub położenie nie są jedynymi środkami przekazu znaczenia.
**Metoda badania**: Obejrzyj stronę wizualnie.
#### Oczekiwanie:
 Jeśli elementy sterujące lub inne elementy różnią się kształtem lub położeniem, wówczas tekst jest również używany w celu zapewnienia tej samej identyfikacji. [1.3.3. Właściwości zmysłowe](https://wcag.lepszyweb.pl/#sensory-characteristics)


### Wymogi dotyczące powiększenia
### 200% Powiększenie ogólne
**Metoda badania**: Zwiększenie powiększenia przeglądarki do 200%.
#### Oczekiwanie:
 Za pomocą powiększenia przeglądarki ekran można powiększyć do 200% bez utraty informacji lub funkcjonalnie. [1.4.4 Zmiana rozmiaru tekstu](https://wcag.lepszyweb.pl/#resize-text)
#### Ustalenia:

### 200% Powiększenie tekstu
**Metoda badania**: Zwiększenie rozmiaru tekstu do 200% (Firefox działa najlepiej)
#### Oczekiwanie:
 Korzystając z funkcji przeglądarek w celu zwiększenia rozmiaru tekstu, tekst można powiększyć do 200% bez utraty informacji i funkcjonalności. [1.4.4 Zmiana rozmiaru tekstu](https://wcag.lepszyweb.pl/#resize-text)

### Porządek czytania/treści
**Metoda badania**: 
1.	Wyłączyć CSS, Jest to treść prezentowana w sposób logiczny. (Zwróć uwagę, że niektóre treści przeznaczone do ukrycia mogą być wyświetlane).
2.	Czytnik ekranu, Czytaj od początku do końca strony.
#### Oczekiwanie:
- Kolejność czytania jest logiczna i zrozumiała. Zazwyczaj będzie to od lewej do prawej i od góry do dołu. [1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence)
- Wszystkie widoczne teksty są odczytywane przez czytnik ekranu. 
- Tekst, który ma być ukryty, jest ukryty przed czytnikiem ekranu.
#### Ustalenia:

## Tekst
### Prezentacja
**Metoda badania**: Wyłączanie obrazów i określanie, czy tekst informacyjny znika.
#### Oczekiwanie:
 Rzeczywisty tekst jest używany, chyba że nie ma innego sposobu przedstawienia potrzebnej stylizacji niż użycie obrazu tekstu. [1.4.5 Obrazy tekstu](https://wcag.lepszyweb.pl/#images-of-text)
#### Ustalenia:

### Współczynnik kontrastu tekstu na pierwszym planie w stosunku do tła
**Metoda badania**: Użyj narzędzia do testowania kontrastu, aby określić współczynniki kontrastu.
#### Oczekiwanie:
 [1.4.3 Kontrast (minimalny)](https://wcag.lepszyweb.pl/#contrast-minimum)
- Współczynnik kontrastu dla wszystkich standardowych tekstów na stronie jest równy lub większy niż 4,5:1.
- Współczynnik kontrastu dla dużych tekstów (Nagłówki i inne duże pozycje) przekracza 3,0:1.
- Współczynnik kontrastu dla obrazów tekstu, innych niż logotypy i wizerunki marki, które są wykorzystywane do przekazywania informacji przekracza 3,0:1.
- Współczynnik kontrastu dla wszystkich tekstów w aktywnych kontrolach przekracza 4,5:1.
  - Wyłączone elementy sterujące nie wymagają kontrastu.

#### Ustalenia:

### Nagłówki
**Metoda badania**: Kod i kontrola wzrokowa
#### Oczekiwanie:
- Nagłówki służą do identyfikacji części strony. [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
- Tekst nagłówka poprawnie identyfikuje zawartość sekcji lub strony [2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels)
- Nagłówek gniazda odzwierciedla hierarchię treści strony [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
- Główne tematy są identyfikowane przy użyciu <h1> (preferowane).
- Poziomy nagłówków nie są pomijane (preferowane).

#### Ustalenia:

### Listy
**Metoda badania**: Kod i kontrola wzrokowa
#### Oczekiwanie:
 [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships)
- Listy ciągłe znajdują się w obrębie jednego elementu listy (ol lub ul).
- Pozycje w wykazie używają elementu li
- Lista gniazdowania jest poprawna (podlisty są zawarte w li)

#### Ustalenia:


### Obrazy
Niebezpieczeństwo 
**Metoda badania**: Wyłączanie obrazów
#### Oczekiwanie:
 Przy wyłączonych obrazach (na pierwszym planie lub w tle) nie występuje utrata informacji lub funkcjonalności.
Opisy: przy wyłączonym obrazie (pierwszy plan lub tło) nie występuje utrata informacji lub funkcjonalności.
**Metoda badania**: Kontrola kodu, użycie narzędzia ujawniającego tekst zmiany.
#### Oczekiwanie:
 [1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content)
- Jeśli obraz jest używany do podania kontekstu, informacji lub znaczenia, wówczas alternatywny tekst obrazu dostarcza tego samego kontekstu, informacji lub znaczenia. W przeciwnym razie obraz znajduje się w tle lub ma pusty tekst alternatywny.
- Jeśli obraz jest łączem lub elementem kontrolnym, tekst alternatywny podaje cel istnienia łącza lub funkcji elementu kontrolnego.
- Obrazy nie są wykorzystywane do przekazywania informacji tekstowych, chyba że prezentacja tekstu w formacie obrazu jest niezbędna.
- Obrazy używane do przekazywania tekstu muszą spełniać wymagania dotyczące kontrastu tekstu, chyba że są one logo.
#### Ustalenia:

### Tabele
**Metoda badania**: Kontrola kodu, wykorzystanie narzędzia ujawniającego elementy nagłówka i zakres.
#### Oczekiwanie:
 [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships), [1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence)
- Tabele są wykorzystywane wyłącznie do prezentacji danych (najlepsza praktyka).
  - Jeśli tabele są używane do układania, mają aria-role=" prezentacja" (najlepsza praktyka)
  - Jeśli tabele są używane do układu, kolejność odczytu jest poprawna, gdy tabela jest linearyzowana. (wymagane)
- Nagłówki tabel są kodowane przy użyciu elementów nagłówków tabel.
- Jeśli nagłówków kolumn jest więcej niż jeden rząd, wówczas wszystkie komórki nagłówka kolumny zawierają atrybut zakresu ustawiony na col scope=" col".
- Jeśli nagłówków wierszy jest więcej niż jedna kolumna, to wszystkie komórki nagłówków wierszy zawierają atrybut zakresu ustawiony na wiersz scope=" wiersz".
- Jeśli na przekątnej znajdują się nagłówki, to nagłówki są identyfikowane w każdej komórce za pomocą atrybutu nagłówków. Wszystkie komórki nagłówka muszą mieć identyfikatory.
- Jeśli dla całej tabeli istnieje nagłówek lub napis rozpiętości, nie ma go w wierszu tabeli ani nie jest zakodowany jako komórka nagłówka.

#### Ustalenia:



### Podstawy obiektów aktywnych 
Porządek tabulacji
**Metoda badania**: Inspekcja, użyj narzędzia ujawniającego sekwencję zakładek i/lub zakładek ręcznych na stronie. [2.4.3 Kolejność fokusa](https://wcag.lepszyweb.pl/#focus-order)
#### Oczekiwanie:
 
- Wszystkie aktywne obiekty są ustawiane ostrością podczas nawigacji za pomocą klawisza tabulatora.
- Brak aktywnych obiektów nie otrzymuje ostrości (pola formularza tylko do odczytu są uważane za aktywne)
- Kolejność, w jakiej obiekty otrzymują ostrość jest logiczna i odpowiada oczekiwanej kolejności wizualnej/wybranej przez mysz.

### Widoczny wskaźnik fokusa
**Metoda badania**: Ręczna taulacja poprzez aktywne obiekty, w razie potrzeby sprawdź poziom kontrastu.
#### Oczekiwanie:
  [2.4.7 Widoczny fokus](https://wcag.lepszyweb.pl/#focus-visible)
- Wizualne wskazanie miejsca ustawienia ostrości jest wyraźne.
  - Kontur lub podkreślenie ma współczynnik kontrastu 4,5:1 w stosunku do tła.
  - Przesunięcie koloru obiektu ma współczynnik kontrastu pomiędzy dwoma kolorami 3,0:1.

### Zachowanie
**Metoda badania**: Ręczna zakładka poprzez aktywne obiekty
#### Oczekiwanie:
  [2.1.2 Brak pułapki na klawiaturę](https://wcag.lepszyweb.pl/#no-keyboard-trap), [3.2.1 3.2.1
Po oznaczeniu fokusem](https://wcag.lepszyweb.pl/#on-focus)
- Wszystko, co można wprowadzić za pomocą klawisza zakładki, można pozostawić za pomocą klawisza zakładki.
- Wejście lub wyjście i obiekt nie powoduje zmiany położenia ostrości.


### Linki
**Metoda badania**: Inspekcja 
- Przeczytaj tekst linku i otaczający go tekst, 
- Określić, że połączenia zostały utworzone przy użyciu elementu kotwiącego z href, jeśli nie, 
  -  tab do łącza i naciśnij klawisz Enter, aby aktywować łącza utworzone przy użyciu innej metody.
#### Oczekiwanie:
  [2.4.4. Cel linku w kontekście](https://wcag.lepszyweb.pl/#link-purpose-in-context)
● Tekst linku opisuje miejsce przeznaczenia linku (preferowany).
● Tekst linku opisuje miejsce przeznaczenia linku w kontekście (wymagane).
● Połączenie można aktywować za pomocą klawisza Enter.

#### Ustalenia:


### Informacje o przemieszczaniu, mruganiu, miganiu, miganiu lub automatycznej aktualizacji
**Metoda badania**: Kontrola, testowanie ręczne, testowanie przy użyciu specjalistycznych narzędzi.
#### Oczekiwanie:
  [2.2.2. Wstrzymywanie (pauza), zatrzymywanie, ukrywanie](https://wcag.lepszyweb.pl/#pause-stop-hide), [2.3.1 Trzy błyski lub wartości poniżej progu](https://wcag.lepszyweb.pl/#three-flashes-or-below-threshold)
- Nic nie miga częściej niż trzy razy na sekundę (preferowane) lub
  -  Obszar lampy błyskowej jest wystarczająco mały lub
  -  Próg jest testowany za pomocą narzędzia.
     -  [Harding FPA](https://www.hardingfpa.com/)
     -  [Narzędzie do analizy padaczki światłoczułej](https://trace.umd.edu/peat)
- Istnieje mechanizm pauzowania lub restartu autoodtwarzania, aktualizacji lub przenoszenia treści.

#### Ustalenia:



### Pola i kontrolki formularza
Etykietowanie i instrukcje
**Metoda badania**: Inspekcja/Ręczna
- Przeczytaj etykiety i instrukcje.
- Umieść ostrość w polu i dokonaj wpisu.
- Użyj narzędzia kontrolnego, aby ustalić, czy etykieta jest związana z polem.
- Należy użyć narzędzia kontrolnego, aby ustalić, czy legendy są stosowane prawidłowo i odpowiednio.
- Użyj narzędzia kontrolnego, aby określić, czy atrybuty arii używane do znakowania formularzy są używane prawidłowo.
  - atrybut aria-labelledby wskazuje na etykiety
  - atrybut aria-describedby wskazuje dodatkowe informacji instruktażowe, takich jak formatowanie lub wymagania dotyczące hasła.
  - atrybut aria-label jest używany tylko wtedy, gdy etykieta tekstowa nie byłaby odpowiednia dla osoby korzystającej z czytnika ekranu (preferowany tytuł)

#### Oczekiwanie:
  [1.1.1. Treść nietekstowa](https://wcag.lepszyweb.pl/#non-text-content), [2.4.6 Nagłówki i etykiety](https://wcag.lepszyweb.pl/#headings-and-labels), [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships), [3.3.2 Etykiety lub instrukcje](https://wcag.lepszyweb.pl/#labels-or-instructions), )
  
- Instrukcje i etykiety zawierają dostatecznie szczegółowe informacje, w tym wszelkie wymagania dotyczące formatowania (w tym zasady dotyczące hasła) oraz to, czy pole jest wymagane.
- Wszystkie pola formularza i kontroli posiadają etykietę tekstową.
  - Wiele pól formularza może współdzielić etykietę tekstową.
- Etykieta tekstowa wyraźnie określa cel lub funkcję pola formularza lub kontroli.
- Etykieta tekstowa pozostaje widoczna, gdy pole jest zaznaczone i gdy pole jest wypełnione.
- Wszystkie etykiety związane z polem formularza muszą być programowo powiązane z polem formularza lub alternatywna etykieta musi być dostarczona poprzez atrybut tytułu lub atrybut etykiety aria.
- Pola formularza, które mają jedną niepowtarzalną etykietę tekstową, muszą wykorzystywać element etykiety z prawidłowymi atrybutami i atrybutami id. (Ostrzeżenie)
- Gdy pola formularza mają wiele etykiet, pola formularza są etykietowane przy użyciu legend zestawów pól lub etykietowanych przez arię.
- Formatowanie opisów lub innych krytycznych informacji w celu prawidłowego wypełnienia pola formularza jest dodawane przy użyciu aria-opisanej lub zawartej w etykiecie pola formularza.
- Używane są odpowiednie typy wejściowe HTML 5 (preferowane).
- Stosuje się odpowiednie atrybuty autokompletności (preferowane, wymagane dla 2.1).
  - Patrz Cele wejściowe

#### Ustalenia:

### Komunikaty o błędach
**Metoda badania**: Pozostawić informacje poza wymaganymi polami lub wprowadzić informacje nieprawidłowo i sprawdzić komunikaty o błędach. Uzyskaj dostęp do komunikatów o błędach wizualnie i za pomocą czytnika ekranu.
#### Oczekiwanie:
  [3.3.1 Identyfikacja błędu](https://wcag.lepszyweb.pl/#error-identification), [3.3.3 Sugestie korekty błędów](https://wcag.lepszyweb.pl/#error-suggestion), [.3.4
Zapobieganie błędom (kontekst prawny, finansowy, związany z podawaniem danych)](https://wcag.lepszyweb.pl/#error-prevention-legal-financial-data)
- Komunikat o błędzie dokładnie opisuje błąd i wskazuje, jak go usunąć.
- Komunikat o błędzie jest łatwo rozpoznawalny dla wszystkich użytkowników. Możliwe prezentacje są:
  - Komunikat o błędzie jest wyświetlany w oknie dialogowym.
  - Komunikat o błędzie jest prezentowany bezpośrednio obok pola błędu oraz
    - Jest związany z obszarem jako część etykiety, poprzez oznakowanie aria-etykietą lub poprzez opisaną aria-opisaną przez lub
    - Jest częścią żywego regionu i ogłaszana jako alarm.
  - Komunikat o błędzie prezentowany jest na liście błędów, a ostrość klawiatury umieszczana jest tuż przed rozpoczęciem listy.
- Jeśli wprowadzenie jest częścią formularza, który zobowiązuje użytkownika do wypełnienia zobowiązania prawnego lub finansowego, wówczas:
  - Zgłoszenie jest odwracalne lub
  - Informacje mogą być sprawdzone pod kątem błędów, a zgłaszający ma możliwość poprawienia ewentualnych błędów lub
  - Użytkownik może przeglądać, potwierdzać i korygować informacje przed ich ostatecznym przesłaniem.

#### Ustalenia:

#### Funkcjonalność pola tekstowego
**Metoda badania**:  Wprowadź dane do pola i wyjdź z pola. (Klawiatura i czytnik ekranu)
#### Oczekiwanie:
 
- Wprowadzony tekst ma wystarczający kontrast.
- Jeżeli podczas wprowadzania pola pojawią się instrukcje lub dodatkowe informacje, które można odczytać za pomocą czytnika ekranu, są one widoczne w powiększeniu.
- Wprowadzenie danych lub opuszczenie pola nie powoduje nieoczekiwanej akcji.

#### Funkcjonalność Przycisk radiowy
**Metoda badania**: Wybieranie przycisków radiowych za pomocą klawiatury i czytnika ekranu
#### Oczekiwanie:
 
- W przypadku zakładania tylko wybrany przycisk radiowy lub pierwszy przycisk radiowy znajduje się w pierścieniu zakładki.
- Po wybraniu przycisku radiowego wybór można zmienić za pomocą klawiszy strzałek.
- Wybranie przycisku radiowego lub dokonanie wyboru nie powoduje nieoczekiwanej zmiany miejsca ustawienia ostrości lub interfejsu.

#### Funkcjonalność pola rozwijanego
**Metoda badania**: Dokonaj wyboru w rozwijanym menu za pomocą klawiatury i czytnika ekranu.
#### Oczekiwanie:
- Zmiana wyboru bez otwierania pola nie powoduje zmiany lokalizacji ostrości lub zmiany w interfejsie.
- Wyboru można dokonać za pomocą strzałki w górę i w dół.
- Sterowanie można otworzyć za pomocą strzałki alt+down.

#### Przycisk Funkcjonalność
**Metoda badania**: Obsługa przycisku z klawiaturą i czytnikiem ekranu.
#### Oczekiwanie:
 
- Przyciski mogą być aktywowane za pomocą spacji.
- Przyciski można aktywować za pomocą klawisza Enter.

### Kontrolki sterowane skryptami
Kryteria skryptowych kontroli muszą być zweryfikowane dla każdego projektu. W większości przypadków wymagania można wyprowadzić z wzorców projektowych i przykładów zawartych w Praktykach Autorskich WAI-ARIA 1.1.




