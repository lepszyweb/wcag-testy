---
title: 4. Dostęp z klawiatury i fokus


sidebar: testy_sidebar
permalink: tz-04-klawiatura
folder: testy/tz
---

## Dostęp z klawiatury

### Identyfikacja treści

1.  Użyj myszy lub innego urządzenia wskazującego, aby określić dostępne funkcje zapewniane przez elementy interaktywne (w tym menu rozwijane, pola formularzy, ujawnianie / ukrywanie treści, podpowiedzi ORAZ wszystkie elementy interfejsu interaktywnego).

2.  Użyj myszy, aby zidentyfikować przypadki, w których elementy interaktywne dostarczają informacji niezbędnych do zrozumienia lub obsługi treści strony.

**Uwaga**:

-   Wymóg WCAG SC 2.1.1 nie dotyczy funkcji, które wymagają danych wejściowych zależnych od ścieżki ruchu użytkownika, a nie tylko punktów końcowych. W przypadku tego procesu testowego, tester nie ma obowiązku identyfikacji i pominięcia tego typu funkcji. Tester powinien uwzględnić wszystkie funkcje, które odpowiadają opisowi Identyfikacja treści Content. W przypadku niektórych funkcji można zastosować wyjątek określony w sekcji 508, jednak jest to poza zakresem procesu testowego.

Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testu **NIE MA ZASTOSOWANIA**: 4.A do 4.H.


Jeśli nie ma takiej treści, wynik dla następujących identyfikatorów testu NIE MA ZASTOSOWANIA : 4.A do 4.H.




### Test 2.1.1-dostep-z-klawiatury 

| Nazwa testu             | ID testu | Warunek testowy |
|----------------|------|-------------------------------------------------------------------|
| 2.1.1-dostep-z-klawiatury | 4.A     | Wszystkie funkcje mogą być dostępne i wykonywane tylko za pomocą klawiatury. |

##### Zastosowanie:

Ten warunek testu **NIE MA ZASTOSOWANIA**, jeśli na stronie nie ma funkcji aktywowanych przez użytkownika.

##### Jak testować:

1.  Użyj myszy, aby zidentyfikować funkcjonalność i niezbędne informacje dostarczane przez elementy interaktywne.

    1.  Funkcja elementy fokusujące: atrybuty title w ANDI: może pomóc zidentyfikować wszelkie istotne informacje zawarte w atrybutach title.

2.  Użyj klawiatury, aby obsługiwać określoną funkcjonalność i / lub uzyskać dostęp do niezbędnych informacji: dostęp do elementu  klawiszem Tab i uruchomienie funkcjonalności (np. naciśnij Enter na element z fokusem).

    1.  W przypadku elementów interaktywnych z atrybutami title umieść fokus klawiatury na elemencie. Jeśli podpowiedź nie pojawi się w ciągu dwóch sekund, fokus klawiatury nie ujawnia informacji o tytule.

3.  Jeśli element interaktywny nie ma dostępu do klawiatury, sprawdź, czy na stronie dostępna jest inna metoda dostępna za pomocą klawiatury, która zapewnia tę samą funkcjonalność, np. Jedna z dwóch podanych metod drukowania jest dostępna za pomocą klawiatury itp. Aby uzyskać szczegółowe informacje, zobacz [Zgodna wersja alternatywna](tz-01-alternatywne.md)

4.  Jeśli element interaktywny nie zapewnia dostępu do istotnych informacji za pomocą interakcji klawiatury, sprawdź, czy informacje są dostępne w innym miejscu strony (np. jako tekst).

**Uwaga:** Nie wszystkie przeglądarki wyświetlają wizualnie atrybut title jako etykietkę narzędzia, gdy element uzyskuje fokus klawiatury.

##### Wyniki oceny:

Jeśli OBA poniższe twierdzenia są **PRAWDZIWE**, treść **ZDAJE**:

1.  Dostęp do wszystkich funkcji można uzyskać za pomocą klawiatury **ORAZ**

2.  Dostęp do wszystkich niezbędnych informacji można uzyskać za pomocą klawiatury **LUB** informacje istnieją w innym miejscu strony.

##### Uwaga: 

-   W tym teście należy uwzględnić wszelkie zmiany funkcji, które nastąpią automatycznie lub w wyniku interakcji ze stroną.
-   Informacje uważa się za niezbędne lub wymagane, gdy są one niezbędne do wykonania działania lub zrozumienia informacji i relacji.
-   Informacje w atrybucie title lub podpowiedzi, które nie są niezbędne, nie wymagają dostępu do klawiatury.

### Test 2.1.1-bez-czasu-nacisniecia

| Nazwa testu               | ID testu | Warunek testowy  |
|----------------|------|-------------------------------------------------------------------|
| 2.1.1-bez-czasu-nacisniecia | 4.B | Poszczególne naciśnięcia klawiszy nie wymagają określonego czasu aktywacji funkcji. |

#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli strona nie ma funkcji aktywowanej przez użytkownika.

#### Jak testować:

1.  Kontynuuj test 4.A.

2.  Ustal, czy istnieją przypadki, w których określony jest czas naciśnięcia klawiszy, aby aktywować element, np. szybkość, z jaką wpisywane są hasła, jest częścią uwierzytelniania hasła.

3.  Jeśli istnieje funkcja zależna od czasu, sprawdź, czy na stronie istnieje inna metoda wykonania zadania za pomocą klawiatury, która nie wymaga określonego czasu.

#### Wyniki oceny 

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, treść **ZDAJE**:

1.  Istnieje metoda umożliwiająca aktywację funkcji za pomocą klawiatury bez wymagania od użytkowników wykonania określonego czasu aktywacji.

### Test 2.1.2-bez-pulapki-na-klawiature

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.1.2-bez-pulapki-na-klawiature | 4.C     | Nie ma pułapki na klawiaturę. |

#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli strona nie zawiera komponentów, na których można ustawić fokus klawiatury.

#### Jak testować:

1.  Nawiguj tabulatorem między wszystkimi komponentami strony, na których można ustawić fokus klawiatury.
2.  Ustal, czy istnieją przypadki, w których nawigacja klawiaturą jest zablokowana:

<!-- -->

1.  Użytkownicy klawiatury nie mogą wyjść z elementu, np. za pomoca klawisza TAB lub klawiszy strzałek, ESC
2.  Dostęp z klawiatury jest tylko do części interaktywnych komponentów strony, bez możliwości przejścia z „pętli” do innych komponentów interaktywnych.

<!-- -->

1.  Jeśli znaleziono pułapkę na klawiaturę::

    1.  Sprawdź wszelką pomoc (kontekstową, pomoc aplikacji) i dokumentację pod kątem powiadomień o dostępnych alternatywnych poleceniach klawiaturowych (np. niestandardowe sterowanie klawiaturą, klawisze dostępu, klawisze skrótów), które pozwalają wyjść z pułapki na klawiaturę.
    2.  Sprawdź, czy polecenia alternatywne działają.
	
#### Wyniki oceny 
Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, treść **ZDAJE**:

1.  Fokus klawiatury można przenieść z elementu za pomocą:

    1.  Standardowych klawiszy nawigacyjnych
    2.  Niestandardowych naciśnięć klawiszy (które są udokumentowane i dostępne dla użytkowników w aplikacji).

> ORAZ

2.  Fokus klawiatury można przenieść z każdej sekcji strony zawierającej komponenty interaktywne (i nie są one uwięzione w „pętli”, uniemożliwiając dostęp do innych elementów na stronie) za pomocą:

    1.  Standardowych klawiszy nawigacyjnych
    2.  Niestandardowych naciśnięć klawiszy (które są udokumentowane i dostępne dla użytkowników w aplikacji).


##### Uwaga:

- W przypadku, gdy istnieje pułapka na klawiaturę, kontynuuj testowanie interaktywnych elementów poza pułapką, używając myszy do omijania pułapki lub odświeżając stronę i używając klawiatury do nawigowania wstecz po stronie.


## Fokus

### Identyfikacja treści

Użyj klawiatury, aby przejść do komponentów interfejsu dostępnych dla klawiatury (w tym menu rozwijanych, pól formularzy, treści odkrywanej/ukrywanej, podpowiedzi ORAZ wszystkich interaktywnych komponentów interfejsu).

Jeśli nie ma takiej treści, wynikiem dla testów od 4.A do 4.H **NIE MA ZASTOSOWANIA**. 

### Test 2.4.7-widoczny-fokus 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.7-widoczny-fokus | 4.D     | Graficzny wskaźnik fokusa jest wyświetlany, gdy fokus znajduje się na komponencie interfejsu.|

#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli strona nie zawiera komponentów, na których można ustawić fokus klawiatury.

#### Jak testować:

1.  Kontynuuj test 4.C.

2.  Ustal, czy na elemencie, który ma fokus klawiatury, widoczny jest graficzny wskaźnik fokusa.

    1.  Gdy fokus klawiatury jest ustawiony na ramce, niektóre przeglądarki wyświetlają graficzny wskaźnik fokusa, a inne nie. Jeśli graficzny wskaźnik fokusa nie jest dostępny na ramce, NIE uważaj tego za defekt treści internetowej.	
	
#### Wyniki oceny 

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, treść **ZDAJE**:

1.  Gdy komponent interfejsu otrzymuje fokus klawiatury, widoczny jest graficzny wskaźnik fokusa.


##### Uwaga:

-   Aby potwierdzić, że fokus klawiatury znajduje się na ramce, gdy fokus nie jest widoczny: użyj kombinacji Tab i Shift+Tab, aby wydedukować, że fokus klawiatury jest na ramce. Będąc na ramce, tabulator do przodu powinien przenieść fokus na pierwszy element, który można ustawić za pomocą klawiatury w ramce. Stamtąd, naciśnij klawisz Shift + Tab, aby wrócić do ramki, a kolejne naciśnięcie Tab+Shift powinno przenieść fokus na element, który można ustawić za pomocą klawiatury przed ramką. Tylko ramka może nie mieć widocznego fokusa. Upewnij się, że to ramka nie ma widocznego fokusa, a nie inny element.


### Test 3.2.1-po-oznaczeniu-fokusem 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 3.2.1-po-oznaczeniu-fokusem| 4.E     | Przeniesienie fokusa na element interaktywny nie inicjuje zmiany kontekstu |



#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli strona nie zawiera komponentów, na których można ustawić fokus klawiatury.

#### Jak testować:

1.  Kontynuuj test 4.D.

2.  When the interface component receives focus, evaluate whether an unexpected change of context occurs, e.g., a new window is launched, or focus is moved to another interface component.

Oceń, czy przeniesienie fokusa na każdy z elementów na stronie nie powoduje nieoczekiwanej zmiany kontekstu, np. uruchomienia nowego okna, przeniesienie fokus na inny element, automatycznego wyslania formularza, wykonania akcji z rozwijanej listy opcji.


#### Wyniki oceny

Jeśli poniższe twierdzenie jest **PRAWDZIWE**, treść **ZDAJE**:

1.  Gdy komponent interfejsu otrzymuje fokus, nie jest inicjowana żadna zmiana niespodziewana kontekstu.


### Test 2.4.3-zrozumiala-kolejnosc-fokusa 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-zrozumiala-kolejnosc-fokusa  | 4.F     | Kolejność ustawiania fokusa zachowuje znaczenie i użyteczność strony. |




#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli strona nie zawiera komponentów, na których można ustawić fokus klawiatury.

#### Jak testować:

1.  Ustaw kursor w pasku adresu przeglądarki, a następnie użyj klawisza Tab, aby przemieszczać się do kolejnych interaktywnych elementów strony (łącza, przyciski, przełączniki, pola formularzy, itd.).  Nie używaj myszy.

2.  Oceń, czy kolejność przemieszcznia się fokusa nie wpływa na znaczenie i użyteczność (funkcjonalność)  strony (np. pola przeznaczone na adres otrzymują fokus w logicznej kolejności - zgodnej z budową adresu).

    1.  Najczęściej można zauważyć, że kolejność przemiezczania się fokusa nie jest zgodna z wizualnym porządkiem elementów i logiczną kolejnością działania (zwykle od lewej do prawej, z góry na dół)


    2.  W przypadku modalnych okien dialogowych fokus powinien pozostać w oknie, dopóki nie zostanie ono zamknięte.

    3.  Pomocne może być uruchomienie ANDI: elementy fokusujące i wybranie opcji  porządek tabulacji.


#### Wyniki oceny

Jeśli WSZYSTKIE poniższe twierdzenia są **PRAWDZIWE**, treść **ZDAJE**:

1.  Kolejnośc ustawiania fokusa zachowuje znaczenie treści, ORAZ

2.  Kolejność ustawienia fokusa zachowuje funkcjonalności strony.

##### Uwaga:

-   Znaczniki kolejności tabulatorów ANDI mogą się nieznacznie różnić od rzeczywistej kolejności tabulatorów klawiatury w niektórych przeglądarkach. Zawsze używaj wyników z kolejności tabulatorów klawiatury.

### Test 2.4.3-fokus-do-tresci-odkrytej 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-fokus-do-tresci-odkrytej | 4.G     | Fokus jest przenoszony na odkryte treści. |

#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli podczas nawigacji lub interakcji z treścią strony (np. opcje podmenu, wybór z rozwijanego menu) nie zostanie ujawniona lub wywołana przez inne elementy trec wczesniej ukryta. 

#### Jak testować:

1. Użyj klawiatury, aby aktywować elementy sterujące, które ujawniają ukrytą zawartość (np. menu, okna dialogowe, modalne okna dialogowe, rozwijana lista drzew).

2. Przemieszczaj fokus poprzez ujawnioną treść za pomocą klawisza TAB.


<!-- -->

1.  Visible focus may not move to revealed content that does not contain focusable elements or if the revealed content is not itself focusable.

Widoczny fokus może nie przechodzić na ujawnioną treść, jesli nie zawiera ona elementów, które mogą otrzymać fokus lub jeśli na całą ujawnioną treść nie można ustawić fokusa.

#### Wyniki oceny

Jeśli którekolwiek z poniższych twierdzen jest **PRAWDZIWE**, treść **ZDAŁA**

1.  Fokus klawiatury przenosi się bezpośrednio na ujawnioną treść **ALBO**

2.  Jedno dodatkowe naciśnięcie klawisza przenosi fokus na ujawnioną treść


##### Uwaga:

-   W przypadku modalnych okien dialogowych, widoczny fokus powinien pozostać w oknie do momentu jego zamknięcia. (Jest to uwzględnione w teście 4.F.)

-   Ujawniona treśc nie zawiera informacji, które pojawiają sie jak część atrybutu title podpowiedzi (tooltipa).


### Test 2.4.3-fokus-powraca-do-porządku 

| Nazwa testu              | ID testu | Warunek testowy             |
|--------------------------|----------|-----------------------------|
| 2.4.3-fokus-powraca-do-porządku | 4.H     | Fokus powraca do logicznej sekwencji |

#### Zastosowanie:

Ten warunek testowy **NIE MA ZASTOSOWANIA**, jeśli nie ma elementów interaktywnych,  kóre ujawiniają treśc ukrytą.

#### Jak testować:

1.  Kontynuuj test 4.G

2.  Jeśli to możliwe, aby zamknąć/ukryć lub odrzucić ujawnianą treść, użyj klawiatury, aby zamknąć / ukryć i / lub przenieść fokus z ujawnionej treści.

3.  Zidentyfikuj element, który ma fokus klawiatury.

    1.  Konieczne może być naciśnięcie klawiszy SHIFT + TAB lub klawisza strzałki, aby przesunąć fokus do tyłu.


##### Oceń wyniki:

Jeśli którekolwiek z poniższych stwierdzeń jest  **PRAWDZIWE**, treść **ZDAJE**:

1.  Fokus klawiatury automatycznie powraca do logicznej sekwencji kolejności fokusa sprzed ujawnienia treści, **ALBO**

2.  Jedna dodatkowe naciśnięcie klawisza lub kombinacji klawiszy przywraca fokus do logicznej sekwencji kolejności fokusa sprzed ujawnienia treści.

### Zastosowane standardy


{% include ks/2-1-1.md %}

{% include ks/2-1-2.md %} 

[1. Dostęp z klawiatury](ICT-01-klawiatura) 

{% include ks/2-4-7.md %}

[2. Widoczny fokus](ICT-02-widoczny-fokus)

| {% include ks/2-4-3.md %}

{% include ks/3-2-1.md %}

[3. Kolejność fokusa](ICT-03-kolejnosc-fokusa)

