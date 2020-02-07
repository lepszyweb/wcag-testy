---
title: Inspektor dostępności w przeglądarce Firefox

tags: [rozszerzenia_przeglądarek,narzędzia_oceny_dostępności]
sidebar: narzedzia-sidebar
permalink: nod_firefox-inspektor-dostepnosci
folder: narzedzia-p
---

Od wydania w czerwcu 2018 roku wersji 63 Firefox oferuje Inspektora dostępności - potężne narzędzie, które pomaga wykryć i naprawić wiele typowych problemów związanych z dostępnością. Dzięki inspektorowi dostępności można dotrzeć do istotnych znajdujących się na stronie informacji przeznaczonych dla technologii wspomagających i wykryć, czego brakuje lub co wymaga specjalnej uwagi.

## Dostęp do Inspektora dostępności
Inspektor dostępności jest dostępny w przeglądarce domyślnie. Nie trzeba go instalować. Wybierz z menu przeglądarki Narzędzia dla twórców witryn (<kbd>Ctrl + Shift + I</kbd>), a następnie odkryj kartę Dostępność. Możesz również użyć skrótu klawiaturowego <kbd>Shift + F12</kbd>. Możesz też wskazać na stronie myszką dowolny element i wybrać z menu kontekstowego polecenie *Zbadaj własności dostępności*. 

![Karta Dostępność w Narzędziach twórcy witryn](images/narzedzia/firefox_ID_01_widok-ogolny.png)
Początkowo funkcje inspektora dostępności mogą być wyłączone. W takim przypadku użyj przycisku *Włącz funkcje dostępności*. Zwykle za pomocą tego przycisku funkcje analizatora dostępności można również wyłączyć (na przycisku jest wówczas etykieta *Wyłącz funkcje dostępności*). Jeśli nie jest to możliwe, bo np. Firefox rozpoznał, że w systemie zainstalowany jest czytnik ekranu, to przycisk jest nieaktywny (wyszarzony). 

**Uwaga**: Jeśli używasz funkcji dostępności na wielu kartach, wyłączenie ich na jednej karcie, wyłącza je we wszystkich kartach.

## Funkcje inspektora dostępności
Karta inspektora dostępności podzielona jest na dwa panele:
![Po lewej panel z drzewem dostępności, po prawej panel z własnościami wybranego elementu](/images/narzedzia/firefox_ID_02_drzewo-dost.png) 
W lewym panelu wyświetlane jest drzewo dostępności bieżącej strony. Jest to hierarchiczna struktura wszystkich znajdujących się na stronie obiektów. Początkowo drzewo jest zwinięte. Aby je rozwinąć, użyj strzałki przed węzłem. 

Informacje o obiektach uporządkowane są w dwóch kolumnach. Każdy obiekt opisany jest przez dwie właściwości:
-	**Rola** – rola, jaką obiekt pełni na stronie (np. dokument, sekcja, przycisk, stopka). Może to być albo domyślna rola wynikająca z własności elementu HTML, albo rola przypisana elementowi przez twórcę za pomocą nowego w HTML5 atrybutu role przyjętego ze standardu WAI-ARIA. Wszystkie możliwe i poprawne role zostały zdefiniowane w WAI-ARIA. Wszystkie są zdefiniowane słowami z języka angielskiego.
-	**Nazwa** – nazwa elementu, którą technologie wspomagające komunikują użytkownikowi. Nazwa zależy od elementu. Nazwą większości elementów tekstowych jest po prostu ich treść (*textContent*). Nazwami elementów formularza są skojarzone z nimi etykiety (`<label>`). Nazwą przycisku – zwykle tekst na przycisku. Uwaga: słowo „nazwa” rozumiemy zwykle jako zwięzłe określenie identyfikujące nazywany obiekt. W przypadku drzewa dostępności znaczenie słowa nazwa wydaje się być znacznie szersze. Ale w gruncie rzeczy pełni dokładnie taką samą funkcję, jaka pełnią nazwy – niosą esencję informacji przekazywaną przez obiekt. Może to być np. treść długiego akapitu.
 
W prawym panelu wyświetlane są szczegółowe informacje na temat aktualnie wybranego (zaznaczonego) elementu. Pewnym utrudnieniem są niewątpliwie angielskie nazwy właściwości, ale ich tłumaczenie na język użytkownika mogłoby spowodować spore zamieszanie i o wiele większe problemy z komunikacją, niż nazwy oryginalne. 

Każdy obiekt charakteryzowany jest przez następujący zestaw właściwości: 
-	*name* – nazwa elementu, jak opisano powyżej.
-	*role* - rola elementu, jak opisano powyżej.
-	*actions* (akcje) - lista akcji, które można wykonać na elemencie, na przykład akcją dla przycisku będzie „Naciśnij”, a dla łącza „Skocz”; zauważ, że akcje są zdefiniowane w języku użytkownika
-	*value* – wartość elementu. Może to oznaczać różne rzeczy w zależności od typu elementu; na przykład pola danych w formularzu (role: *entry*) będą miały wartość tego, co zostanie wprowadzone w polu, a wartością łącza będzie adres URL podany w atrybucie `<href>` elementu `<a>`.
-	*DOMNode* – rodzaj węzła w Obiektowym Modelu Dokumentu (DOM). 
   ![Ikona celu obok określenia węzła DOM](/images/narzedzia/firefox_ID_03_DOMnode.png) 
   
   Najechanie kursorem na ikonę „cel” podświetla węzeł DOM w treści strony.
   
   ![Oznaczenie obiektu na stronie](/images/narzedzia/firefox_ID_04_DOMnode-oznaczenie.png) 
   
   Właściwość *DOMNode* jest szczególnym przypadkiem. Umożliwia bezpośrednie przejście do inspektora kodu HTML, do elementu generującego dostępny obiekt. Należy pamiętać, że drzewo dostępności jest zawsze podzbiorem drzewa DOM, nie wszystkie elementy DOM mają dostępny obiekt
-	*description* (opis) - każdy dodatkowy opis elementu, np. dodany w treści atrybutu title.
-	*keyboardShortcut* - skrót klawiaturowy, którym można uaktywnić element, określony w atrybucie accessKey.
-	*childCount* - liczba elementów potomnych, które bieżący element ma w hierarchii drzewa dostępności.
-	*indexInParent* - wartość indeksu elementu wewnątrz elementu nadrzędnego. Jeżeli element jest pierwszym w elemencie nadrzędnym, to ma wartość 0, jeśli jest drugi, ma wartość 1, i tak dalej.
-	*states* (stany) - lista stanów elementu istotnych z punktu widzenia dostępności. W zależności od elementu na liście mogą znajdować się różne stany. Na przykład na liście stanów łącza znajdą się: *focusable* (fokusowane), *linked* (połączone), *selectable text* (tekst możliwy do wyboru), *opaque* (nieprzezroczyste), *enabled* (włączone) i *sensitive* (wrażliwe). Pełną listę stanów silnika Gecko można znaleźć na stronie [Gecko states](https://developer.mozilla.org/en-US/docs/Mozilla/Tech/Accessibility/AT-APIs/Gecko/States).
   
   ![Stany obiektu łącze](/images/narzedzia/firefox_ID_05_stany.png) 
   
-	*relations* (relacje) - lista związanych z dostępnością relacji między tym a innymi elementami. Na przykład w formularzu pola danych może mieć relację "labelled by" („oznaczone przez”) z elementem etykiety, która z kolei może mieć relację "label for" („etykieta dla”) z elementem pola danych.
-	*attributes* (atrybuty) – lista wszystkich istotnych z punktu widzenia dostępności atrybutów elementu. Może to obejmować atrybuty związane ze stylem, takie jak *margin-left* (lewy margines) i *text-indent* (wcięcie tekstu) oraz inne atrybuty istotne z punktu widzenia informacji o dostępności, takie jak *draggable* (przeciągalne)czy *level* (poziom, np. jaki jest to poziom nagłówka, w przypadku nagłówków).). Pełna lista możliwych atrybutów znajduje się na stronie [Gecko object attributes](https://developer.mozilla.org/en-US/docs/Web/Accessibility/AT-APIs/Gecko/Attrs).

 **Uwaga**: Wyeksponowane informacje są takie same na wszystkich platformach - inspektor odsłania drzewo dostępności Gecko, a nie informacje z warstwy dostępności platformy.

### Obsługa za pomocą klawiatury
Karta Dostępność jest w pełni dostępna z klawiatury:
-	Klawiszem <kbd>Tab</kbd> możesz się poruszać między przyciskami *Wyłącz funkcje dostępności* i *Wyszukaj problemy* oraz między lewym i prawym panelem karty.
-	Gdy punkt uwagi znajduje się w panelu, możesz przesuwać fokus w górę i w dół za pomocą klawiszy strzałek w górę i w dół oraz używać klawiszy strzałek w lewo i w prawo do rozwijania i zwijania rozwijanych wierszy (np. różnych poziomów hierarchii drzewa dostępności).

### Wyświetlanie drzewa dostępności w formacie JSON
Zawartość drzewa dostępności można wyświetlić w przeglądarce JSON. W tym celu wystarczy prawym przyciskiem myszy kliknąć dowolny wpis na karcie Dostępność i wybrać polecenie *Wyświetl jako JSON*.

![Opcja Wyświetl jako JSON](/images/narzedzia/firefox_ID_07_JSON.png) 
 
## Znajdowanie problemów z dostępnością
Domyślnie drzewo dostępności zawiera wszystkie obiekty decydujące o dostępności strony. Aby poddać analizie tylko obiekty, które mogą stwarzać problemy z dostępnością, można posłużyć się filtrem *Wyszukaj problemy*. Filtr oferuje kilka opcji:

![Filtr Wyszukaj problemy](/images/narzedzia/firefox_ID_06_filtry.png) 
 
-	**Brak** (filtra) – wyświetlane są wszystkie obiekty drzewa dostępności
-	**Wszystkie problemy** – wyświetlane są wszystkie, które mogą powodować problemy
-	**Kontrast** – wyświetlane są obiekty, które mogą powodować problemy z kontrastem wizualnym
-	**Klawiatura** - wyświetlane są obiekty, które mogą powodować problemy z nawigacją za pomocą klawiatury
-	**Etykiety tekstowe** - wyświetlane są obiekty, które nie mają etykiet tekstowych

Gdy wybierzesz jeden lub kilka niewykluczających się elementów filtra, Firefox przeskanuje dokument i zredukuje lewy panel do problemów w wybranej kategorii lub kategoriach. Może to potrwać kilka sekund.
 
![Lista obiektów z możliwymi błędami](/images/narzedzia/firefox_ID_08_oznaczone-problemy.png) 

Obok nazwy każdego obiektu, który może powodować problemy, pojawi się etykieta określająca kategorię problemu. Po wybraniu elementu z listy problemów, w prawym panelu wyświetlane są bardziej szczegółowe informacje, w tym oznaczenia i zwięzłe opisy problemów wraz z łączem do dodatkowych objaśnień na stronie [Zasobów dla programistów (MDN Web Docs)](https://developer.mozilla.org/pl/) (niestety, łącza nie zawsze działają), gdzie można znaleźć sugestie dotyczące rozwiązania problemu.
 
![Komunikat w panelu Testy](/images/narzedzia/firefox_ID_09_problem-info.png)  
 
Po wykryciu problemu, korzystając z właściwości DOMNode można przejść do inspektora HTML i wprowadzić zmiany naprawiające tymczasowo wykrytą usterkę, aby natychmiast zobaczyć wyniki zarówno na stronie, jak i w inspektorze dostępności. Firefox będzie dynamicznie aktualizować informacje dotyczące dostępności w miarę wprowadzania zmian w inspektorze strony. Uzyskujesz więc natychmiastową informację zwrotną na temat tego, czy Twoje podejście rozwiąże problem.

### Obiekty bez nazw – brak etykiet tekstowych
Drzewo dostępności można filtrować, aby wyświetlać tylko obiekty, które nie są odpowiednio oznakowane, to znaczy nie mają nazw. Nazwa jest podstawowym źródłem informacji dla technologii wspomagających. Informuje użytkownika, co dany element robi. Na przykład etykieta przycisku *Wyślij* informuje technologię, a za jej pośrednictwem użytkownika, że po aktywacji przycisku nastąpi przesłanie formularza.

Inspektor testuje wszystkie obiekty i sprawdza, czy posiadają nazwę określoną programowo. Analizuje przy tym różne zależne od rodzaju obiektu możliwość programowego określania nazwy. Na przykład, sprawdza, czy dokument ma tytuł (znacznik `<title>` w sekcji `<head>`), bo to treść znacznika `<title>` jest nazwą dokumentu. Sprawdza, czy obrazy i mapy obrazów posiadają opis alternatywny (atrybut `alt`). Sprawdza, czy okna dialogowe, elementy osadzone, elementy iframes posiadają tytuł, np. określony atrybutem `title`. Sprawdza, czy kontrolki formularzy posiadają skojarzone z nimi etykiety, a grupy pól legendę (określoną w znaczniku `<legend>`). I tak dalej. Listę wszystkich znanych sposobów określania nazwy znajdziesz w artykule [Text labels and names](https://developer.mozilla.org/en-US/docs/Web/Accessibility/Understanding_WCAG/Text_labels_and_names) na stronie MDN Web Docs.
 
### Problemy z klawiaturą
Inspektor dostępności potrafi wykryć wszystkie znane potencjalne problemy z obsługą tylko za pomocą klawiatury, takie jak:
-	Czy do każdego elementu, którym można spowodować zmianę, można dotrzeć tylko za pomocą klawiatury?
-	Czy atrybut `tabindex` posiada tylko zalecane wartości (-1, 0 i 1)?
-	Czy elementy, które można kliknąć, można osiągnąć także za pomocą klawiatury?
-	Czy elementy interaktywne można uaktywnić tylko za pomocą klawiatury?
-	Czy każdy element interaktywny otrzymuje fokus podczas tabulacji?
-	Czy do elementów uzyskujących fokus została zastosowana odpowiednia stylistyka? 
Pamiętać należy, że istnieje wiele sposobów stylizacji wskaźnika fokusa, stąd mogą się przytrafić inspektorowi dostępności fałszywe alarmy. Ale trochę doświadczony audytor łatwo zweryfikuje takie przypadki. 
 
### Kontrast
Kolejną zdolność Inspektora dostępności zapewnia moduł testowania kontrastu kolorów na całej stronie. Inspektor sprawdza wszystkie trzy typy problemów z kontrastem wskazywane przez WCAG 2.1:
-	Czy zwykły tekst na tle spełnia minimalne wymagania dotyczące współczynnika kontrastu 4,5: 1?
-	Czy duży tekst na tle (zwykle) nagłówki spełnia wymóg współczynnika kontrastu 3:1?
-	Czy elementy interaktywne i graficzne spełniają minimalny współczynnik 3: 1 (dodany w WCAG 2.1)?

![Wyświetlanie błędów kontrastu](/images/narzedzia/firefox_ID_10_kontrast.png)

Oprócz tego, że inspektor filtruje listę obiektów niespełniających wymogów kontrastu, oznacza je także na stronie, umożliwiając bardzo dokładną lokalizację błędu. 
 
![Wyświetlanie błędów kontrastu na różnobarwnym tle](/images/narzedzia/firefox_ID_10_kontrast.png)

Gdy tekst znajduje się na różnobarwnym tle, np. gradientowym, inspektor dostępności potrafi wskazać, czy poszczególne części tekstu spełniają wymagania dotyczące współczynnika kontrastu. 
Ponadto moduł sprawdzania kontrastu kolorów zapewnia informacje o współczynniku kontrastu na poziomie AAA. Możesz więc od razu zobaczyć, czy Twoja strona spełnia ten zaawansowany standard.

### Symulator niedoboru widzenia kolorów
Od wersji Firefox 70 inspektor dostępności oferuje możliwość symulacji niedostatków widzenia kolorów, znanych szerzej jako ślepota barw, oraz utratą wrażliwości na kontrast. O ile problemy z widzeniem kolorów dotyczą około 8% mężczyzn i 0,5% kobiet na całym świecie, co już stanowi spory odsetek populacji, to problemy z utratą wrażliwości na kontrast, są znacznie częstsze, bo mogą być powodowane przez inne schorzenia siatkówki oka, na przykład zwyrodnienie plamki związane z wiekiem.
 
Symulator niedowidzenia kolorów domyślnie jest wyłączony. Aby go włączyć, należy w about:config przełączyć właściwość *gfx.webrender.all* na *true* (Wpisz w pasku adresu przeglądarki *about:config*, a następnie – po potwierdzeniu, że rozumiesz skutki zmian w ustawieniach, wyszukaj właściwość *gfx.webrender.all* i kliknij dwukrotnie w wierszu z tą właściwością. Wartość *false* powinna się zmienić na *true*.) 
 
Po włączeniu symulatora pojawi się dodatkowe menu inspektora *Włącz symulację*. Wybór dowolnej pozycji menu spowoduje zmianę widoku strony symulującą jej widzenie przez osobę z wybranym rodzajem niewrażliwości.

![Opcje symulatora niedowidzenia kolorów](/images/narzedzia/firefox_ID_12_symulator-opcje.png)
 
## Inne użyteczne funkcje Inspektora dostępności

### Selektor elementów interfejsu użytkownika
Podobnie jak w Inspektorze DOM, w inspektorze dostępności również mamy do dyspozycji selektor elementów dostępności. Korzystając z selektora, można wybrać i wyróżnić na stronie wybrany z drzewa dostępności obiekt oraz wyświetlić jego właściwości. 

![Lokalizacja symulatora elementów interfejsu](/images/narzedzia/firefox_ID_13_selektor-elementow.png)
 
Dodatkowo, gdy selektor elementów interfejsu jest uaktywniony, możesz najeżdżać myszką na elementy strony, a Firefox wyświetli dla każdego wskazanego elementu pasek informacyjny, który pokazuje jego nazwę, rolę i stany, a także współczynnik kontrastu. Jeśli chcesz wyświetlać właściwości elementu po kliknięciu, uaktywnij selektor elementów z wciśniętym równocześnie klawiszem <kbd>Shift</kbd>.
 
### Opcje menu kontekstowego
Zarówno na stronie internetowej, jak i w widoku inspektora HTML, a nawet w widoku kodu źródłowego strony zostały dodane opcje menu kontekstowego. Z poziomu strony własności elementu związane z dostępnością można wyświetlić, wybierając z menu kontekstowego opcję *Zbadaj własności dostępności*. 

![Opcja Zbadaj własności dostępności w menu kontekstowym na stronie](/images/narzedzia/firefox_ID_14_menu-kontekstowe-strona.png) 

Natomiast w inspektorze DOM ta opcja ma nazwę *Wyświetl własności dostępności*. 

![Opcja Wyświetl własności dostępności w menu kontekstowym Inspektora DOM](/images/narzedzia/firefox_ID_15_menu-kontekstowe-DOM.png)
 
Po wybraniu z menu kontekstowego opcji *Zbadaj własności dostępności* oraz *Wyświetl własności dostępności* natychmiast otwiera się karta Dostępność i wyświetla odpowiedni element drzewa dostępności i jego właściwości.

**Uwaga**: Niektóre elementy DOM nie mają właściwości dostępności - w takim przypadku elementy menu kontekstowego *Wyświetl własności dostępności* jest wyszarzona.

![Nieaktywna opcja menu](/images/narzedzia/firefox_ID_16_nieaktywne-menu-kontekstowe.png)
