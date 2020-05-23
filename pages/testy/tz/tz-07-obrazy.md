---
title: 7. Obrazy


sidebar: testy_sidebar
permalink: tz-07-obrazy
folder: testy/tz
---
## Cel procedury testowej 

Celem tej procedury testowej jest sprawdzenie, czy obrazy mają równoważne odpowiedniki tekstowe. 

Testy składające się na tę procedurę pomagają ustalić, czy metody zapewniania równoważnych informacji dla obrazów spełniają określone kryteria dostępności:

- Wszystkie znaczące obrazy (treści nietekstowe) muszą mieć równoważny opis tekstowy (aby użytkownicy, którzy nie widzą obrazu, mogli również otrzymywać informacje prezentowane przez obraz).
- Obrazy dekoracyjne nie mogą zawierać alternatywy tekstowej.
- Obrazy tekstu muszą być konfigurowalne lub nie mogą być zastąpione tekstem.

Alternatywy tekstowe dla obrazów można renderować za pomocą różnych modalności sensorycznych, takich jak wizualna, słuchowa lub dotykowa, w zależności od potrzeb użytkownika, co może pomóc zapewnić, że wszyscy użytkownicy mogą otrzymać te same informacje. 

Ta procedura testowa obejmuje również badanie obrazów CAPTCHA, aby sprawdzić, czy zapewniono użytkownikom alternatywne metody weryfikacji, nie polegające wyłącznie na wzroku lub słuchu.

Procedura testowa „Obrazy” obejmuje pięć testów:

1.	Test 7.A: 1.1.1-znaczaca-nazwa-obrazu 
2.	Test 7.B: 1.1.1-obrazy-dekoracyjne
3.	Test 7.C: 1.1.1-dekoracyjne-obrazy-tla
4.	Test 7.D: 1.1.1-alternatywa-captcha
5.	Test 7.E: 1.4.5-obrazy-tekstu


## Obrazy niosące informacje

### Testu 7.A 1.1.1-znaczaca-nazwa-obrazu

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.1.1-znaczaca-nazwa-obrazu | 7.A     | Dostępna nazwa i dostępny opis znaczących obrazów stanowią równoważny opisy obrazów. |

### Cel testu 7.A 1.1.1-znaczaca-nazwa-obrazu
Celem tego testu jest sprawdzenie, czy każdy znaczący obraz ma również równoważny opis. Znaczący obraz to taki, który przekazuje informacje, których usunięcie spowodowałoby utratę treści lub kontekstu. 

Obrazami znaczącymi są między innymi wykresy, schematy, obrazy tekstu, obrazy funkcjonalne (przyciski) użyte do zainicjowania akcji lub obrazy, które wymagają odpowiedzi. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 1.1.1 Treść nietekstowa.

### Metody i narzędzia testowe 

1.	ANDI: grafika/obrazy.
2.	Inspekcja wzrokowa strony.


### Identyfikacja treści
Znajdź wszystkie obrazy na stronie i przejrzyj kontekst każdego obrazu, aby określić jego przeznaczenie. Wybierz obrazy znaczące, to znaczy obrazy, które przekazują informację lub kontekst. Obrazami znaczącymi są obrazy tekstu, obrazy funkcjonalne używane do inicjowania akcji, przekazywania znaczenia lub zachęcania do odpowiedzi; mapy obrazów, wykresy, schematy.

1.	Użyj modułu ANDI: grafika/obrazy, aby znaleźć wszystkie obrazy. Początkowo wokół każdego obrazu pojawia się kropkowana linia.
 
    **Uwaga**: Obraz, których ANDI nie wykrywa, choć są widoczne na stronie, **nie powinny być** uwzględnione w tym teście.

2.	Użyj przycisku „Następny element”, aby przejść do każdego obrazu na stronie. Każdy obraz zostanie obrysowany różowym konturem.

3.	Dla każdego obrazu znalezionego przez ANDI określ, czy obraz ma znaczenie.

    - Znaczący obraz to taki, w którym przekazywana jest informacja, a jeśli zostanie usunięty, nastąpi utrata treści lub kontekstu.
    - **Uwaga**: Tekst w sąsiedztwie obrazu lub inna treść strony może w pełni objaśnić obraz, czyniąc go dekoracyjnym, ponieważ usunięcie obrazu nie powodowałoby utraty treści ani kontekstu
    - **Wskazówka**: Dobrą metodą oceny jest zadanie sobie pytania, czy jeśli obraz zostałby usunięty, to użytkownik nadal otrzymywałby te same informacje?

       - Jeśli **nie**, jest to znaczący obraz.
       - Jeśli **tak**, jest to obraz dekoracyjny i jest testowany w 7.B.

    **Uwaga**: ANDI może zidentyfikować obrazy, które są częścią złożonego elementu strony, na którym można ustawić fokus klawiatur. W takich przypadkach przetestuj obraz za pomocą modułu ANDI: interaktywne (elementy).

Ten test dotyczy **tylko** obrazów znaczących.

### Zastosowanie

Test 7.A: 1.1.1-znaczaca-nazwa-obrazu **nie ma zastosowania**, jeśli na stronie nie ma znaczących obrazów. W takim przypadku oznacz wynik testu jako **ND**. Przypomnienie: Wszelkie istniejące na stronie obrazy, których ANDI nie wykrywa, nie są uwzględnione w tym teście.

### Jak testować

1. Przejrzyj Wyjście ANDI w poszukiwaniu znaczących obrazów.
   1. Jeśli obraz jest używany jako CAPTCHA, wyjście ANDI opisuje przeznaczenie CAPTCHA.
   2. Jeśli obraz zawiera znaczący tekst, wyjście ANDI zawiera ten sam tekst.
   3. Jeśli wyjście ANDI wskazuje w opisie obrazu na treść strony, należy ustalić, czy ten opis istnieje.
   4. Jeśli obraz jest elementem składowym lub dzieckiem elementu otrzymującego fokus (np. przycisku lub łącza), należy ocenić dostępną nazwę dla całego fokusowanego elementu, a nie tylko dla obrazu. Użyj ANDI: interaktywne (elementy) lub ANDI: łącza/przyciski), aby określić dostępną nazwę dla złożonego elementu.
	
	
### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 1.1.1:

1.	Dane wyjściowe ANDI zawierają równoważny opis znaczącego obrazu lub przywołują opis istniejący w treści strony.

Jeśli ANDI wykryje, że tekst alternatywny nie ma charakteru opisowego, wyświetli ostrzeżenie. W razie potrzeby możesz zweryfikować treść alt w Komponentach dostępności.

### Uwaga

-   Wszelkie zmiany znaczących obrazów, które pojawiają się automatycznie lub w wyniku interakcji ze stroną, należy uwzględnić w tym teście. 

    -   Powiadomienia o automatycznych zmianach są testowane w teście 2.D, 4.1.2-powiadamianie-o-automatycznej-zmianie.

    -   Powiadomienia o zmianach wynikające z interakcji z innymi treściami są testowane albo w teście 5.E albo 6.B.

-   Obraz, który znajduje się na stronie, ale nie został wykryty przez ANDI zgodnie z opisem w części Identyfikacja treści, nie powinien być uwzględniany w tym teście.

-   Wyjście ANDI jest puste dla obrazu, który ma `role="presentation"`, `role="none"` lub `aria-hidden="true"`. Nie można ich ustawić dla znaczących obrazów, które muszą mieć równoważny opis w wyjściu ANDI.


## Obrazy dekoracyjne

### Test 7.B 1.1.1-obrazy-dekoracyjne

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| Test 7.B: 1.1.1-obrazy-dekoracyjne | 7.B     | Obrazy dekoracyjne nie mają alternatywy tekstowej (dostepnej nazwy lub opisu. |


### Cel testu 7.B 1.1.1-obrazy-dekoracyjne
Celem tego testu jest sprawdzenie, czy żaden obraz dekoracyjny nie ma dostępnej nazwy ani opisu. Brak dostępnej nazwy lub opisu, a także inne atrybuty, takie jak `role="presentation"`, `role="none"`, lub  `aria-hidden="true"` informują technologie wspomagające, aby ignorowały obraz i unikały głośnego odczytywania niepotrzebnych treści. 

Obraz jest dekoracyjny, jeśli nie dodaje ważnych lub istotnych informacji do treści strony. Obrazy mogą być ozdobą, jeśli są czysto dekoracyjne, służyć wyłącznie do formatowania wizualnego lub nie są prezentowane użytkownikom (niewidoczne):

-	ozdobniki graficzne, takie jak ramki, przekładki i narożniki.
-	uzupełnienia tekstu łączy, aby poprawić ich wygląd lub zwiększyć obszar klikalny.
-	ilustracje sąsiadującego tekst, które nie wnoszą do treści dodatkowych informacji („cukierki do oczu” lub upiększacze graficzne).
-	obrazy opisane w sąsiadującym tekście.
-	niewidoczna treść nie prezentowana użytkownikom.

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 1.1.1 Treść nietekstowa.


### Metody i narzędzia testowe 

1.	ANDI: grafika/obrazy.
2.	Inspekcja wzrokowa strony.

### Identyfikacja treści
Znajdź wszystkie obrazy na stronie i przejrzyj kontekst każdego obrazu, aby określić jego przeznaczenie. Wybierz obrazy dekoracyjne, to znaczy obrazy, które  nie przekazują żadnych istotnych informacji lub są opisane w treści.

1.	Użyj modułu ANDI: grafika/obrazy, aby znaleźć wszystkie obrazy. Początkowo wokół każdego obrazu pojawia się kropkowana zielona linia. 
    **Uwaga**: Obrazy, których ANDI nie wykrywa, choć są widoczne na stronie, **nie powinny być** uwzględnione w tym teście.
	
	Niektóre obrazy dekoracyjne są obrazami tła i powinny być testowane w teście nr 7.C: 1.1.1-dekoracyjne-obrazy-tla
	
2.	Użyj przycisku „Następny element”, aby przejść do każdego obrazu na stronie. Każdy obraz zostanie obrysowany różowym konturem.

3.	Dla każdego obrazu znalezionego przez ANDI określ, czy  jest to obraz dekoracyjny.
 
    -   Obraz dekoracyjny to obraz, który służy jedynie celowi estetycznemu (np. obramowania, przekładki i narożniki), obraz niewidoczny/nieprzedstawiony użytkownikom, obraz będący częścią łącza w celu poprawy wyglądu lub zwiększenia obszaru  klikalnego, obraz używany wyłącznie w celach wizualnych lub opisane w otaczającym tekście.

    - **Wskazówka**: Dobrą metodą oceny jest zadanie sobie pytania, czy jeśli obraz zostałby usunięty, to użytkownik nadal otrzymywałby te same informacje?
       - Jeśli **nie**, jest to znaczący obraz i jest testowany w teście 7.A.
       - Jeśli **tak**, jest to obraz dekoracyjny.

    **Uwaga**: ANDI może zidentyfikować obrazy, które są częścią złożonego elementu strony, na którym można ustawić fokus klawiatur. W takich przypadkach przetestuj obraz za pomocą modułu ANDI: interaktywne (elementy). 


Ten test dotyczy **tylko** obrazów dekoracyjnych.

### Zastosowanie

Test 7.B: 1.1.1-obrazy-dekoracyjne  **nie ma zastosowania**, jeśli na stronie nie ma obrazów dekoracyjnych. W takim przypadku oznacz wynik testu jako **ND**. Przypomnienie: Wszelkie istniejące na stronie obrazy, których ANDI nie wykrywa, nie są uwzględnione w tym teście.

### Jak testować

1.  Przejrzyj wyjście ANDI dla każdego obrazu dekoracyjnego.


### Ocena wyników

Jeśli poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 1.1.1:

1.  Wyjście ANDI dla obrazów dekoracyjnych jest puste.

#### Uwaga:

-   Obrazy, których ANDI nie wykrywa, choć są widoczne na stronie, **nie powinny być** uwzględnione w tym teście, jak podkreślono w sekcji Identyfikacja treści. Niektóre obrazy dekoracyjne są obrazami tła i powinny być testowane i raportowane w teście 7.C: 1.1.1-dekoracyjne-obrazy-tla

-   W teście należy uwzględnić wszelkie zmiany obrazów dekoracyjnych, które pojawiają się automatycznie lub w wyniku interakcji ze stroną.

-   Wyjście ANDI jest puste dla obrazów, które mają `role="presentation"`, `role="none"` lub `aria-hidden="true"`. Są to trzy techniki ukrywania obrazu przed technologiami wspomagającymi i są odpowiednie dla treści dekoracyjnych.


W przypadku obrazów, które mają atrybuty `role="presentation"` lub `role="none"` może pojawić się następujący alert: „Obraz jest prezentacyjny; jego [alt] nie zostanie przekazany.”, tzn. że czytnik ekranu nie odczyta tekstu alt, ponieważ widzi obraz jako prezentacyjny lub dekoracyjny. Jeśli obraz jest naprawdę dekoracyjny (nieistotny), upewnij się, że czytnik ogłasza informacje związane z tym obrazem zgodnie z oczekiwaniami. 

### Test 7.C: 1.1.1-dekoracyjne-obrazy-tla

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.1.1-dekoracyjne-obrazy-tla | 7.C     | Obraz w tle nie jest jedynym środkiem wykorzystywanym do przekazywania ważnych informacji. |

### Cel testu 7.C: 1.1.1-dekoracyjne-obrazy-tla 
Celem tego testu jest sprawdzenie, czy w przypadku wyświetlania każdego znaczącego obrazu tła za pomocą kaskadowych arkuszy stylów (CSS), informacje o treści obrazu znajdują się na stronie także wtedy, gdy obraz jest ukryty.  

Zasadniczo programiści nie dysponują sposobem przekazywania alternatywy tekstowej (dostępnej nazwy lub opisu) dla obrazów tła umieszczonych za pomocą CSS w taki sposób, jak w przypadku obrazów wbudowanych (osadzonych) w treści strony. W rezultacie technologie wspomagające nie są w stanie podać opisu znaczących obrazów tła CSS. Dlatego obrazy tła CSS powinny być albo wyłącznie dekoracyjne, albo znaczenie przekazane przez obrazy tła musi być dostępne gdzie indziej na stronie.  

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 1.1.1 Treść nietekstowa.

### Metody i narzędzia testowe 

1.	ANDI: grafika/obrazy > ukryj obrazy tła.
2.	Inspekcja wzrokowa strony.

### Identyfikacja treści

1. Użyj modułu ANDI: grafiki/obrazy, aby znaleźć obrazy tła CSS. Jeśli istnieją przyciski „znajdź obrazy tła” i „ukryj obrazy tła”, to znaczy, że obrazy tła znajdują się na stronie.

### Zastosowanie

Test 7.C: 1.1.1-dekoracyjne-obrazy-tla  **nie ma zastosowania**, jeśli na stronie nie ma obrazów tła. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Wybierz przycisk „znajdź obrazy tła” w ANDI: grafika/obrazy, aby obrysować wszystkie obrazy tła (na zielono).

2.  Znajdź obrysowane obrazy tła na stronie. (ANDI nie wyświetla informacji dla obrazów tła).

3.	Ustal, czy ważne informacje zawarte w obrazie tła są dostępne bez obrazu tła.

    1.  Wybierz w ANDI funkcję „Ukryj obrazy tło”, aby ukryć obrazy tła i określić, czy informacje zawarte w obrazie są dostępne również na stronie bez obrazu tła.

    2.  Przyjrzyj się sekwencji treści, w jakiej pojawia się obraz tła i jego pozycji na stronie, aby ustalić czy równoważne informacje są prezentowane w tej samej kolejności logicznej.
	
**Uwaga**:  W teście należy uwzględnić wszelkie zmiany obrazów tła, które pojawiają się automatycznie lub w wyniku interakcji ze stroną. W takim przypadku może być konieczne odświeżenie ANDI.


### Ocena wyników

Jeśli którekolwiek poniższe twierdzenie jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 1.1.1:

1.  Obraz tła jest obrazem dekoracyjnym, **lub**

2.  Znaczenie obrazu tła jest również dostępne bez obrazu tła.

#### Uwaga:

**Uwaga**:  W teście należy uwzględnić wszelkie zmiany obrazów tła, które pojawiają się automatycznie lub w wyniku interakcji ze stroną. W takim przypadku może być konieczne odświeżenie ANDI.



## Obrazy CAPTCHA

#### Test 7.D: 1.1.1-alternatywa-captcha

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.1.1-alternatywa-captcha | 7.D     | Na stronie istnieją alternatywne formy CAPTCHA. |

### Cel testu 7.D: 1.1.1-alternatywa-captcha

Celem testu jest sprawdzenie, czy każdy obraz użyty jako CAPTCHA ma alternatywną metodę weryfikacji, która nie opiera się wyłącznie na wzroku lub słuchu, aby użytkownicy z niepełnosprawnością wzroku lub słuchu mogli również wykonać test CAPTCHA. CAPTCHA to program używany na stronach internetowych, aby się utwierdzić, że dane wprowadza człowiek, a nie maszyna (robot) i ochronić strony internetowe przed spamem. Istnieje kilka różnych form CAPTCHA, które mogą być zastosowane na stronach i w aplikacjach. 

Wszystkie formy CAPTCHA i alternatywne formy CAPTCHA powinny zostać przetestowane. 

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG 1.1.1 Treść nietekstowa.

### Metody i narzędzia testowe 

1. Inspekcja wzrokowa strony
2. Test ręczny

### Identyfikacja treści

Znajdź wszystkie obrazy CAPTCHA.

**Uwaga**: Na niektórych stronach internetowych stosowane jest obecnie rozwiązanie reCAPTCHA, która prosi tylko o zaznaczenie pola wyboru lub kliknięcie przycisku, aby udowodnić, że nie jesteś robotem. Takie rozwiązanie nie powinno to być traktowane jako obraz CAPTCHA do przetestowania, ale jako kontrolka formularza, ponieważ takie pole CAPTCHA jest powiązane z formularzem, a nie z obrazem. Dopiero wtedy, gdy  po interakcji pojawi się wyskakujące okno z obrazem lub obrazami CAPTCHA, to ten obraz powinien zostać przetestowany w tym teście.

### Zastosowanie

Test 7.C: 1.1.1-alternatywa-captcha  **nie ma zastosowania**, jeśli na stronie nie ma obrazów CAPTCHA. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.	Ustal, czy zapewnione są alternatywne formy CAPTCHA, które opierają się na innych możliwościach percepcji (postrzegania), niż tylko wzrok i słuch.

### Ocena wyników

Jeśli wszystkie poniższe twierdzenia są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 1.1.1:

1.	CAPTCHA ma format dla użytkowników niewidomych i słabowidzących, **oraz**

2.	CAPTCHA ma format dla użytkowników Głuchych lub słabosłyszących.


## Obrazy tekstu

### Test 7.E: 1.4.5-obrazy-tekstu

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.5-obrazy-tekstu | 7.E     | Obrazu tekstu nie można zastąpić tekstem lub można go dostosować. |

### Cel testu 7.E: 1.4.5-obrazy-tekstu

Celem tego testu jest sprawdzenie, czy zawsze używany jest rzeczywisty tekst, a nie obrazy tekstu, chyba że określona prezentacja tekstu jest niezbędna do przekazywanych informacji (np. część logo, próbka czcionki, konkretna czcionka nie jest powszechnie obsługiwana, nazwa marki) albo sposób prezentacji obrazu tekstu można dostosować. 

Używanie rzeczywistego tekstu zamiast obrazu tekstu lub obrazów tekstu, które użytkownicy mogą dostosować do swoich możliwości postrzegania (np. zmienić krój czcionki, tło, rozmiaru tekstu, kolor) jest szczególnie ważne dla użytkowników niewidomych, słabowidzących, nierozróżniających kolorów, użytkowników z ograniczonymi umiejętnościami językowymi, poznawczymi i trudnościami w uczeniu się.    

Wyniki tego testu służą do ustalenia, czy spełnione jest kryterium sukcesu WCAG  1.4.5 Obrazy tekstu.

### Metody i narzędzia testowe 

1. ANDI: grafika/obrazy
2. Inspekcja wzrokowa strony

### Identyfikacja treści
Znajdź wszystkie obrazy tekstu.

**WYKLUCZ** teksty, które są częścią obrazów zawierających inne istotne treści wizualne, takie jak wykresy, zrzuty ekranowe i schematy, które przekazują ważne informacje oprócz tekstu.

Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testów **NIE MA ZASTOSOWANIA**: 7.E.


### Zastosowanie

Test 7.E 1.4.5-obrazy-tekstu  **nie ma zastosowania**, jeśli na stronie nie ma obrazów tekstu. W takim przypadku oznacz wynik testu jako **ND**.

### Jak testować

1.  Ustal, czy zamiast obrazu tekstu można użyć rzeczywistego tekstu, aby przedstawić ten sam efekt i informacje.

    1.  Logotypy (tekst będący częścią logo lub nazwy marki) nie mogą być zastępowane tekstem.

    2.  Przykłady typów, marki, obrazy konkretnych czcionek, które nie są powszechnie obsługiwane, są dodatkowymi przykładami obrazów tekstu, które nie mogą być zastępowane tekstem.

2.	Określ, czy obraz tekstu może być dostosowany wizualnie: dostosuj czcionkę, rozmiar, kolor i tło za pomocą elementów sterujących dostępnych na stronie internetowej.

    1.  Dostosowanie rozmiaru czcionki dla obrazu tekstu oznacza również możliwość dostosowania rozmiaru bez pikselizacji (co jest zwykle widoczne podczas korzystania z funkcji zmiany rozmiaru okna przeglądarki internetowej w celu zmiany rozmiaru obrazów).

### Ocena wyników

Jeśli którekolwiek z poniższych stwierdzeń jest **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z KS 1.4.5:

1.  Obraz tekstu nie może być zastąpiony tekstem, **lub**

2.  Obraz tekstu można dostosować wizualnie.

**Uwaga**

Pamiętaj, że sama strona internetowa musi oferować opcje dostosowywania, aby zmienić czcionkę, rozmiar, kolor i tło (WCAG definiuje wizualne dostosowanie jako możliwość ustawienia czcionki, rozmiaru, koloru i tła; dlatego wszystkie cztery opcje dostosowywania muszą istnieć na stronie, aby wystarczająco umożliwić wizualne dostosowanie wymagane do spełnienia tego warunku testowego).

### Zastosowane standardy
- {% include ks/1-1-1.md %}
- {% include ks/1-4-5.md %}
- {% include ks/4-1-2.md %}

- [4. Obrazy](ICT-06-obrazy)
- [5. Treść zmienna](ICT-05-tresc-zmienna)

