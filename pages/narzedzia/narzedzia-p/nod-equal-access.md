---
title: IBM Accessibility Checker - podręcznik użytkownika
tags: [rozszerzenia-narzędzi-autorskich,rozszerzenia-przeglądarek]
sidebar: narzedzia_sidebar
permalink: nod-equal-access
folder: narzedzia-p
---

Wersja 3.0.0

IBM Equal Access Accessibility Checker jest rozszerzeniem przeglądarek, które pozwala sprawdzać, &nbsp;oceniać i&nbsp;poprawiać dostępność cyfrową rozwiązań dla Internetu w oparciu o&nbsp;Wytyczne W3C Web Content Accessibilty Guidelines (WCAG) oraz wytyczne IBM z wyjaśnieniami i&nbsp;propozycjami odpowiednich poprawek.

Rozszerzenie prezentuje dwa widoki. Widok panelu **Ocena dostępności** jest kompleksowym narzędziem, które pomaga wykryć problemy z&nbsp;dostępnością i&nbsp;zrozumieć, jak je naprawić. Natomiast karta  **Tester dostępności** w panelu Elementy w Chrome lub panelu Inspektor w&nbsp;Firefoksie jest skanerem kodu dla programistów, którzy chcą szybko znaleźć i naprawić problemy w&nbsp;kodzie i na stronie.

IBM Equal Access Accessibility Checker jest częścią otwartego pakietu narzędzi automatyzujących pracę nad dostępnością. Dla zespołów poszukujących rozwiązań zintegrowanego testowania dostępności, IBM oferuje [wtyczki i moduły](https://github.com/IBMa/equal-access/blob/master/README.md) dla NodeJS i&nbsp;Karma, które wykonują międzyplatformowe testy dostępności w procesie budowania i rozwoju. Narzędzia te wykorzystują ten sam silnik testowy, co Accessibility Checker.


## 1. Wymagania wstępne

Obsługiwane przeglądarki:
- Google Chrome w wersji 81.x lub nowszej
- Mozilla Firefox wersji 8.x lub nowszej

## 2. Instalacja

Wykonaj poniższe kroki, aby zainstalować rozszerzenie przeglądarki dla Google Chrome:

1. Otwórz przeglądarkę Google Chrome.
2. Przejdź na IBM [Equal Access Accessibility Checker](https://chrome.google.com/webstore/detail/ibm-equal-access-accessib/lkcagbfjnkomcinoddgooolagloogehp) w Chrome Web Store.
3. Naciśnij przycisk **Dodaj do Chrome**.

Wykonaj poniższe kroki, aby zainstalować rozszerzenie przeglądarki dla Mozilla Firefox:

1. Otwórz przeglądarkę Firefox.
2. Przejdź na [IBM Equal Access Accessibility Checker](https://addons.mozilla.org/en-US/firefox/addon/accessibility-checker/) na stronie Dodatki do przeglądarki.
3. Naciśnij przycisk **Dodaj do Firefoksa**.

## 3. Kategorie problemów dostępności

Narzędzie zgłasza trzy rodzaje problemów z dostępnością:

- <img src="" alt="Ikona naruszeń " style="vertical-align: middle;"> **Naruszenia** - błędy dostępności, które wymagają naprawy.
- <img src="" alt="ikona Do przeglądu " style="vertical-align: middle;"> **Do przeglądu** - przypadki, które mogą nie być naruszeniem. Wymagają one ręcznego przeglądu w celu określenia, czy istnieje problem z dostępnością.
- <img src="" alt="ikona Ulepszenia" style="vertical-align: middle;"> **Ulepszenia** - możliwości zastosowania najlepszych praktyk w celu dalszej poprawy dostępności.

Jak w przypadku każdego narzędzia do automatycznego testowania dostępności, testy te nie wychwytują wszystkich problemów. Dopełnij swoją ocenę dostępności [szybkim testem jednostkowym](https://ibm.com/able/toolkit/develop/considerations/unit-testing) lub przejdź do [pełnego procesu testowania dostępności](https://ibm.com/able/toolkit/verify).

## 4. Sposoby przeglądania problemów

Istnieją trzy sposoby przeglądania i badania problemów wykrytych przez narzędzie. Wszystkie widoki pokazują ten sam zestaw problemów:

- **Wymagania** - problemy są uporządkowane według wymagań IBM, co odpowiada standardom WCAG 2.1. Każdy problem jest zmapowany do konkretnego wymagania WCAG 2.1. Ten  widok sprawia, że łatwo jest zobaczyć, jak klasyfikować i raportować problemy wykryte przez narzędzie.
- **Role elementów** - problemy są zorganizowane w hierarchicznej strukturze określonej przez role WAI-ARIA dla elementów DOM. Widok ten pokazuje zarówno role ukryte, jak i role jawne. Nie pokazuje on nazw elementów. Ten widok jest idealny do eksploracji problemów w obrębie konkretnego elementu i&nbsp;jego dzieci.
= **Reguły** - problemy są uporządkowane według reguł w zestawie wymagań. Są podzielone na naruszenia, kwestie wymagające przeglądu i ulepszenia. Ten widok jest najlepszym sposobem na równoczesny przegląd wszystkich problemów różnego typu.

## 5. Opcje

Użyj strony opcji, aby zmienić domyślny zestaw reguł dla obsługiwanego standardu lub datę wdrożenia zestawu reguł.

Domyślnie, IBM Equal Access Accessibility Checker używa najnowszego wdrożenia zestawu reguł, które odpowiadają najnowszym standardom WCAG oraz kilku dodatkowym wymaganiom uzupełniającym IBM. W&nbsp;razie potrzeby do wyboru są również dostępne zestawy reguł z regułami, które odpowiadają konkretnym wersjom WCAG. Te zestawy reguł są regularnie aktualizowane, a każda aktualizacja ma datę wdrożenia. W przypadku konieczności powtórzenia wcześniejszego testu należy wybrać datę wdrożenia oryginalnego testu.

Po zmianie opcji zamknij i otwórz ponownie narzędzia programistyczne, aby zmiany zaczęły obowiązywać.

Wykonaj poniższe kroki, aby otworzyć stronę z opcjami programu Tester dostępności:

1. W pasku narzędzi przeglądarki, wybierz ikonę IBM Equal Access Accessibility Checker, widoczną jako fioletowa pszczoła 
<img src="" alt="ikona aplikacji Tester dostępności">. Zazwyczaj znajduje się on w&nbsp;prawym górnym rogu okna okna przeglądarki. Pojawi się nakładka.

2. Wybierz w nakładce **Opcje**. Opcje zostaną otwarte na nowej karcie przeglądarki. **Uwaga:** W przeglądarce Firefox, gdy w opcjach *Wzmocniona ochrona przed śledzeniem* wybrano ustawienie **Ścisła**, zdarza się, że niektóre witryny lub treści mogą zostać uszkodzone i może to uniemożliwić otwarcie strony Opcje. Zmień ustawienia prywatności przeglądarki na Standard, aby uniknąć tej sytuacji.<br />
![Zrzut ekranu strony opcji - strona, na której można wybrać wdrożenie zestawu reguł oraz zestaw reguł, z jakiego ma korzystać kontroler.](/images/equal-access/5_Options.png)

### 5.1 Data wdrożenia zestawu reguł

1. Z listy rozwijanej **Wybierz datę wdrożenia zestawu reguł** wybierz jedną z opcji:

   - **Najnowsze wdrożenie** - użyj najnowszej wersji  wybranego zestawu reguł. Jest to opcja domyślna.
   - **Wdrożenie &lt;data&gt;** - użyj zestawu reguł z określonej daty w celu spójnego testowania w całym projekcie albo żeby powtórzyć wcześniejsze testy.
   - **Podglądowe reguły** - wypróbuj eksperymentalny zestaw przyszłych reguł.
2. Wybierz przycisk **Zapisz**, aby zachować zmiany, lub przycisk **Przywróć domyślne**, aby odrzucić zmiany. Zamknij i otwórz ponownie narzędzia programistyczne, aby zmiany zaczęły obowiązywać.

### 5.2 Wybierz wytyczne dla dostępności

1. Z listy rozwijanej **Wybierz wytyczne dla dostępności** wybierz jedną z opcji:
   - **IBM Accessibility** - Reguły obejmujące Wytyczne dla dostępności WCAG 2.1 zgodnie z poziomami A i AA oraz dodatkowe wymagania IBM. Jest to opcja domyślna.
   - **WCAG 2.1 (A,AA)** - Aktualne zalecenie W3C. Treści zgodne z WCAG 2.1 są również zgodne z 2.0. Zasady te są zgodne z europejską normą EN 301 549.
   - **WCAG 2.0 (A,AA)** - Te reguły są zgodne z obowiązującym w USA poprawionym standardem Sekcja 508, ale nie z najnowszą rekomendacją W3C.
   - **IBM Accessibility BETA** - Reguły dla WCAG 2.1 AA i dodatkowe wymagania IBM oraz reguły eksperymentalne.
2. Po wprowadzeniu zmiany należy wybrać przycisk **Zapisz**, a następnie zamknąć i&nbsp;ponownie otworzyć narzędzia programistyczne, aby zmiana zaczęła obowiązywać.

## 6. Stosowanie

IBM Equal Access Accessibility Checker oferuje dwa widoki. Widok Tester dostępności (Accessibility Checker) jest skanerem kodu dla programistów, którzy chcą szybko znaleźć i&nbsp;naprawić błędy podczas budowania komponentu. Natomiast widok Ocena dostępności (Accessibility Assessment) zapewnia wyjaśnienie i&nbsp;sugerowane rozwiązania dla każdego wykrytego problemu. 

**Uwaga**: W rzadkich przypadkach rozszerzenie Accessibility Checker nie pojawia się w&nbsp;narzędziach programistycznych na niektórych stronach z powodu błędu w tych narzędziach. Obejściem jest przejście do witryny, o&nbsp;której wiesz, że sprawdzanie zostanie na niej uruchomione, i&nbsp;uruchomienie sprawdzania. Następnie załaduj na tej samej karcie przeglądarki stronę, która nie została uruchomiona.

### 6.1 Tester dostępności

1. Otwórz panel narzędzi programisty:
   - W Chrome: z menu przeglądarki wybierz „Więcej narzędzi”, a następnie „Narzędzia dla deweloperów” albo 
   - W Firefox: w menu przeglądarki „Narzędzia” wybierz „Narzędzia przeglądarki”, a następnie wybierz „Narzędzia dla twórców witryn”, lub
   - Naciśnij **Command+Option+I** w systemie  MacOS® albo **Control+Shift+I** w&nbsp;systemie Microsoft Windows®, lub
   - Kliknij prawym przyciskiem myszy element strony i&nbsp;wybierz z menu kontekstowego „Zbadaj”.
2. Otwórz panel „Elementy” (Chrome) lub „Inspektor” (Firefox).
3. Wybierz **Tester dostępności** z&nbsp;kart w&nbsp;prawym okienku: <br />
![Zrzut ekranu Accessibility Checker - skaner kodu dla programistów](/images/equal-access/Chrome_Checker.png)
4. Kliknij przycisk **Skanuj**, aby zeskanować stronę internetową.
5. Wynik skanowania wyświetla łączną liczbę wykrytych problemów oraz liczbę naruszeń, kwestii wymagających przeglądu i zaleceń. Domyślnie lista problemów jest wyświetlana w&nbsp;widoku „Role elementów” (patrz poprzednia definicja), dostępne są również karty „Wymagania” i&nbsp;„Reguły”. Wszystkie widoki pokazują ten sam zestaw problemów.<br />
![Wyniki oceniania dostępności](/images/equal-access/6_1_AccessibilityChecker5.png)
6. Aby **filtrować** problemy i skupić się tylko na naruszeniach, kwestiach, które wymagają sprawdzenia lub na ulepszeniach, usuń zaznaczenie pola wyboru obok typu problemu w obszarze liczby problemów poniżej przycisku **Skanuj**, aby wykluczyć typ problemu z wyników. Zaznacz pole wyboru obok typu problemów, aby uwzględnić typ problemu w wynikach. Na tym zrzucie ekranu elementy „Do przeglądu” zostały odfiltrowane.<br />
![Wyniki sprawdzania dostępności z odfiltrowanymi problemami Do przeglądu](/images/equal-access/6_1_AccessibilityChecker6.png)
7. Wybierz ikonę rozwijania (^) obok roli elementu, wymagania lub reguły w tabeli, aby wyświetlić odpowiednie znalezione problemy.
8. Wybierz link „Dowiedz się więcej” w definicji problemu, aby wyświetlić bardziej szczegółowe informacje pomocy opisujące problem i&nbsp;sposoby jego rozwiązania. Pomoc zawiera łącza do bardziej szczegółowych wyjaśnień i&nbsp;podsumowuje, dlaczego ten problem jest ważny i&nbsp;kogo dotyczy.
9. Karta Role elementu:
   - Wybierz instancję problemu lub element w obiektowym modelu dokumentu (DOM) lub użyj polecenia „Zbadaj” na stronie internetowej, aby:
     - Podświetlić wybrany element lub element zawierający wybrane zagadnienie w DOM pod panelem Elementy przeglądarki i zaznacz jego lokalizację na stronie internetowej.
     - Zobaczyć liczniki podsumowujące pokazujące liczbę problemów każdego typu w wybranym elemencie i jego dzieciach.
     - Otwórzyć i zaznaczyć wszystkie problemy w elemencie, jeśli występują (fioletowe podświetlenie)
     - Otwórzyć i zaznaczyć wszystkie problemy w elementach potomnych elementu, jeśli występują (jasnofioletowe podświetlenie).
10. Karta Wymagania:
    - Wybierz kartę **Wymagania**, aby wyświetlić wyniki skanowania <a href="https://www.ibm.com/able/requirements/requirements/">według wymagań dostępności IBM
    - Wybierz element lub wystąpienie problemu, aby wyróżnić ten sam zestaw problemów i&nbsp;problemów podrzędnych, co na karcie „Role elementów”. W&nbsp;tym widoku problemy zostaną pokazane w&nbsp;ramach odpowiednich wymagań.
11. Karta Reguły:
    - Wybierz kartę **Reguły**, aby wyświetlić wyniki skanowania według reguł sprawdzania dostępności.
    - Wybierz element lub wystąpienie problemu, aby wyróżnić ten sam zestaw problemów i&nbsp;problemów podrzędnych, co na karcie „Role elementów”. Z&nbsp;tego punktu widzenia problemy zostaną pokazane w ramach odpowiednich zasad.
    - Przełączaj się między kartami, aby zobaczyć ten sam zestaw wyróżnionych problemów w&nbsp;różnych widokach.
    - Użyj przycisku menu **Raporty**, aby pobrać raporty oraz przechowywać i&nbsp;zarządzać skanami w celu połączenia ich w raporty. Aby uzyskać szczegółowe informacje, zobacz sekcje [6.4 Tworzenie raportu ze skanowania](), [6.5 Tworzenie raportu z wielu skanów]() oraz [7 Raporty sprawdzania dostępności]
    - Opcjonalnie możesz zaktualizować kod w panelu Elementy przeglądarki i&nbsp;ponownie uruchomić **Skanuj**, aby potwierdzić, że zmiany w kodzie rozwiązują problem.

### 6.2 Widok skoncentrowany

Przełącznik **Widok skoncentrowany** umożliwia przełączanie między wyświetlaniem wszystkich problemów na stronie lub tylko problemów z wybranym elementem lub komponentem w DOM. Aby skupić się na dowolnym pojedynczym elemencie lub komponencie:

1. Wybierz element lub komponent w DOM **albo**
2. Kliknij prawym przyciskiem myszy na elemencie strony i&nbsp;wybierz z&nbsp;menu kontekstowego „Zbadaj”.
3. Wybierz nazwę elementu w przełączniku **Widok skoncentrowany**, aby wyświetlić tylko problemy dotyczące tego elementu i&nbsp;jego dzieci.
4. Wybierz opcję **Wszystko** w przełączniku **Widok skoncentrowany**, aby wyświetlić wszystkie problemy na stronie.
5. Domyślnie, po pierwszym skanowaniu strony, wyświetlane są wszystkie zagadnienia, a&nbsp;element &lt;html&gt; jest zaznaczony, jak pokazano na tym zrzucie ekranu:<br />
![Zrzut ekranu narzędzia Accessibility Checker - widok główny z wszystkimi problemami](/images/equal-access/6_2_FocusView1.png)<br />
Na tym zrzucie ekranu wybrano element wyszukiwania &lt;input&gt; w DOM, a przełącznik  **Widok skoncentrowany** został ustawiony tak, aby wyświetlał wszystkie problemy na całej stronie:<br />
![Zrzut ekranu narzędzia sprawdzania dostępności. Opcje przełączania widoku ostrości to 'input' i 'Wszystko' (wybrane) i wszystkie problemy na stronie są pokazane](/images/equal-access/6_2_FocusView2.png)<br />
Na tym zrzucie ekranu wybrano pole wyszukiwania &lt;input&gt; w DOM, a przełącznik **Widok skoncentrowany**  został ustawiony tak, aby wyświetlał tylko problemy dla tego elementu wyszukiwania &lt;input&gt;:<br />
![Zrzut ekranu narzędzia sprawdzania dostępności. Opcje przełączania widoku ostrości to 'input' (zaznaczone) i 'Wszystko', pokazane są tylko dwa problemy w obrębie elementu wejściowego wyszukiwania](/images/equal-access/6_2_FocusView3.png)

### 6.3 Ocena dostępności

1. Otwórz Narzędzia dla programistów:
   - W przeglądarce Chrome: z menu przeglądarki wybierz „Więcej narzędzi”, a&nbsp;następnie „Narzędzia dla deweloperów” lub 
   - W przeglądarce Firefox: z menu „Narzędzia” przeglądarki wybierz „Narzędzia przeglądarki”, a następnie wybierz „Narzędzia dla twórców witryn” lub
   - Naciśnij **Command+Option+I** w systemie MacOS® lub **Control+Shift+I** w&nbsp;systemie Microsoft Windows®, lub
   - Kliknij prawym przyciskiem myszy element strony i&nbsp;wybierz z&nbsp;menu kontekstowego „Zbadaj”
2. Wybierz panel  **Ocena dostępności** panel: 

<img src="chrome-extension://agkmeejjncicmdgdmbcecphplicjmjbd/assets/img/6_3_AccessibilityAssessment2.png" alt="Zrzut ekranu oceny dostępności - Kompleksowe narzędzie do oceny dostępności" width="100%" height="100%">

3. Kliknij przycisk **Skanuj**, aby zeskanować stronę internetową.
4. Domyślnie wyniki są wyświetlane według  **Wymagań** z podziałem całkowitej liczby wykrytych problemów według kategorii.
5. Prawy panel wyświetla podsumowanie raportu Testera dostępności, a lewy panel pokazuje wynik skanowania z łączną liczbą wykrytych problemów, z liczbami naruszeń, kwestii, które wymagają sprawdzenia oraz ulepszeniami: 

<img src="chrome-extension://agkmeejjncicmdgdmbcecphplicjmjbd/assets/img/6_3_AccessibilityAssessment5.png" alt="Zrzut ekranu raportu Oceny dostępności - przykładowy raport Oceny dostępności" width="100%" height="100%">

6. Domyślnie problemy są wyświetlane w widoku „Wymagania”, ale dostępne są również karty „Role elementów” i&nbsp;„Reguły”. Wszystkie widoki pokazują ten sam zestaw problemów.
7. Karta Wymagania:
   - Wybierz ikonę rozwijania obok wymagania w tabeli, aby wyświetlić listę problemów znalezionych w ramach tego wymagania.
   - Wybierz wystąpienie problemu, a podsumowanie raportu zostanie zastąpione szczegółowym opisem, który zawiera poziom błędu, dlaczego treść nie działa dostępnie, jakie są wymagania, jakich zasobów użyć, co zrobić, aby naprawić problem, kogo dotyczy i&nbsp; dlaczego jest to ważne: 

<img src="6_3_AccessibilityAssessment7.png" alt="Zrzut ekranu panelu pomocy Oceny dostępności - przykładowy panel pomocy Oceny dostępności " width="100%" height="100%">

8. Karta Rola elementu:
   - Wybierz kartę **Role elementów**, aby wyświetlić wyniki skanowania uporządkowane według ról elementów na stronie internetowej.
   - Rozwiń rolę elementu, aby wyświetlić problemy dla tej roli elementu.
   - Wybierz problem, aby:
     - Podświetlić problem.
     - Wyświetlić szczegółowy opis tego problemu w okienku podsumowania (po lewej stronie).
9. Karta Reguły:
   - Wybierz kartę **Reguły**, aby wyświetlić wyniki skanowania według reguły sprawdzania dostępności.
   - Rozwiń regułę, aby wyświetlić problemy dla tej reguły.
   - Wybierz problem, aby:
     - Poświetlić problem.
     - Wyświetlić szczegółowy opis tego problemu w okienku podsumowania (po lewej stronie).
10. Opcjonalnie możesz wybrać panel Elementy w przeglądarce Chrome lub Inspektor w Firefox, aby wyświetlić wyniki sprawdzania dostępności wraz z&nbsp;poprawkami kodu i&nbsp;testów.

### 6.4 Tworzenie raportu ze skanowania

Aby wygenerować raport dla pojedynczego skanu w widoku **Tester dostępności**:

1. Postępuj zgodnie z instrukcjami w [6.1 Tester dostępności](), aby zeskanować stronę internetową.
2. Otwórz menu rozwijane **Raporty**, które znajduje się za przyciskiem skanowania.<br />
![Zrzut ekranu menu 'Raporty'](/images/equal-access/6_4_CreatingSingleScanReport2.png)
3. Wybierz **Pobierz aktualny skan**.
4. Raport z ostatniego skanowania zostanie pobrany w formacie arkusza kalkulacyjnego HTML i MS Excel.

Aby wygenerować raport dla pojedynczego skanowania w widoku **Ocena dostępności**:

1. Postępuj zgodnie z instrukcjami w [6.3 Ocena dostępności](), aby zeskanować stronę internetową.
2. Wybierz przycisk **Raporty**.
3. Raport z ostatniego skanowania zostanie pobrany w formacie arkusza kalkulacyjnego HTML i&nbsp;MS Excel.

### 6.5 Tworzenie raportu z wielu skanów

Wykonaj poniższe czynności, aby połączyć kilka skanów w jeden raport. Można połączyć do 50 skanów. Raporty zawierające więcej niż 50 skanów mogą nie otwierać się poprawnie w&nbsp;MS Excel ze względu na ograniczenia bibliotek używanych do pisania raportów.

1. Otwórz widok **Tester dostępności** (opisany w [6.1 Tester dostępności]()).
2. Otwórz menu rozwijane **Raporty**.
3. Wybierz pozycję menu **Rozpocznij przechowywanie skanów**.
4. Wskaźnik stanu poniżej przycisku skanowania pokaże, że teraz przechowujesz skany w&nbsp;celu utworzenia raportu i&nbsp;że żadne skany nie są przechowywane.<br />
![Status: przechowywanie, brak zapisanych skanów](/images/equal-access/6_5_CreatingMulti-scanReport4.png)
5. Zeskanuj strony, które chcesz uwzględnić w raporcie. Może to obejmować skany tej samej strony w różnych stanach. Wskaźnik stanu zaktualizuje się, pokazując, ile skanów jest przechowywanych.<br />
![Status: zapisywanie, 3 skany zapisane](/images/equal-access/6_5_CreatingMulti-scanReport5.png)
6. Podczas zapisywania skanów możesz przestać zapisywać skany, wybierając opcję **Zatrzymaj przechowywanie skanów** w&nbsp;menu rozwijanym **Raporty**, a&nbsp;zapisane skany nie zostaną utracone. W&nbsp;dowolnym momencie możesz ponownie zapisywać skany.
7. Aby usunąć wszystkie zapisane skany, otwórz menu rozwijane **Raporty** i&nbsp;wybierz opcję **Wyczyść przechowywane skany**.
8. Po zapisaniu skanów do raportu otwórz menu rozwijane **Raporty** i&nbsp;wybierz opcję **Pokaż przechowywane skany**. Spowoduje to otwarcie widoku menedżera skanowania, zawierającego tabelę zawierającą wszystkie zapisane skany.<br />
![Zrzut ekranu panelu przechowywanych skanów - tabela zawierająca listę zapisanych skanów](/images/equal-access/6_5_CreatingMulti-scanReport8.png)

Tworzenie raportu w widoku menedżera skanowania:

1. Przejrzyj wymienione skany i wybierz te, które chcesz umieścić w&nbsp;raporcie. Zaznacz lub usuń zaznaczenie wszystkich zapisanych skanów za pomocą pola wyboru w&nbsp;pierwszej kolumnie wiersza nagłówka tabeli.
2. Użyj linku **Wyświetl** w kolumnie „Szczegóły” po prawej stronie tabeli, aby zobaczyć zrzut ekranu każdego skanu.<br />
![Wyskakujące okno dialogowe zawierające zrzut ekranu i szczegóły dotyczące skanowania](/images/equal-access/6_5_CreatingMulti-scanReport10.png)

3. Usuń zaznaczenie dowolnego skanowania, którego nie chcesz umieścić w&nbsp;raporcie, odznaczając jego pole wyboru w tabeli.<br />
![Zrzut ekranu panelu przechowywanych skanów - jeden skan jest niezaznaczony](/images/equal-access/6_5_CreatingMulti-scanReport11.png)
4. [Opcjonalnie] Aby ułatwić rozróżnienie skanów w raporcie końcowym, wpisz odpowiednie etykiety skanowania w kolumnie „Etykieta skanowania” w&nbsp;tabeli. Etykiety te pojawią się w&nbsp;raporcie końcowym.<br />
![Zrzut ekranu panelu przechowywanych skanów - trzy skany są oznaczone jako 'oryginalny skan', 'z formularzem' i 'z linkiem'](/images/equal-access/6_5_CreatingMulti-scanReport12.png)
5. Pobierz arkusz z raportem z wielu skanów, wybierając przycisk  **Pobierz** u&nbsp;góry tabeli. Arkusz kalkulacyjny zostanie pobrany automatycznie.
6. Usuń wybrane zapisane skany za pomocą przycisku  **Usuń** Pozwala to zachować pamięć do przechowywania nowych skanów.
7. Wróć do głównego widoku sprawdzania, wybierając **Powrót do widoku listy**.

### 6.6 Skanowanie ukrytych treści

Domyślnie narzędzie pomija ukrytą zawartość (strony internetowe, które używają elementów <var>visibility:hidden
</var> lub <var>display:none</var>, jeśli ta zawartość jest wyświetlana użytkownikowi w&nbsp;dowolnym momencie, należy przetestować treśc strony internetowej, w pełni wykorzystując interfejs użytkownika zgodnie ze scenariuszem użycia w&nbsp;planie testów testów. Upewnij się, że testy uruchamiają wyświetlanie ukrytej treści, aby narzędzie sprawdzania ułatwień dostępu mogło sprawdzić poprawność wyświetlanej treści.

### 6.7 Skanuj pliki lokalne

Narzędzie sprawdzania ułatwień dostępu domyślnie skanuje lokalne pliki .html lub .htm uruchamiane w przeglądarce Firefox. Wykonaj poniższe czynności, aby zezwolić na skanowanie lokalnych plików .html lub .htm w&nbsp;przeglądarce Chrome:

1. Otwórz przeglądarkę Chrome.
2. Otwórz menu **Okno**.
3. Wybierz opcję menu **Rozszerzenia**, aby zobaczyć wszystkie zainstalowane rozszerzenia.
4. Wybierz przycisk **Szczegóły** rozszerzenia IBM Equal Accessibility Checker.
5. Przewiń w dół do **Zezwól na dostęp do adresów URL plików** i&nbsp;włącz tę opcję.

### 6.8 Rozważania dotyczące dostępności

Poniżej wyróżniono kilka funkcji dostępności umożliwiających dostosowanie i&nbsp;zapewniających łatwy dostęp do funkcji Checker, w&nbsp;tym za pomocą klawiatury lub czytnika ekranu:

1. Narzędzie Tester dostępności reaguje na preferowany rozmiar i&nbsp;kolory czcionki użytkownika.
2. Zarówno widok Ocena dostępności, jak i widok Tester dostępności są w&nbsp;pełni dostępne za pomocą klawiatury, nawiguj w następujący sposób:
   - Użyj klawisza **Tab**, aby przejść do dowolnego elementu sprawdzania, który można ustawić, zaczynając od przycisku **Skanuj** po uruchomieniu sprawdzania.
   - Po uruchomieniu skanowania ponownie naciśnij klawisz **Tab**, aby przejść do przycisku menu rozwijanego **Raporty**.
   - W widoku Tester dostępności ponownie naciśnij klawisz **Tab**, aby przejść do przycisku przełączania „Widok skoncentrowany”. Użyj klawiszy strzałek, aby wybrać, czy lista spraw zawiera wszystkie sprawy (domyślnie), czy tylko sprawy dla aktualnie wybranego elementu i&nbsp;jego elementów podrzędnych. Ta funkcja nie jest dostępna w widoku Ocena dostępności.
   - Naciśnij klawisz **Tab**, aby przejść do pola wyboru według każdego typu problemu i naciśnij klawisz **Enter**, aby przefiltrować listę problemów według **Naruszeń**, **Do przeglądu** lub według **Rekomendacji**.
   - Naciśnij klawisz **Tab**, aby przejść do kart z **listą problemów** i użyj klawiszy **strzałka w&nbsp;prawo** lub **strzałka w&nbsp;lewo**, aby przechodzić między widokami **Role elementów**, **Wymagania** i&nbsp;widokiem **Reguły**.
   - Naciśnij klawisz **Tab**, aby poruszać się po **grupach problemów** związanych z każdym wymaganiem, rolą elementu lub regułą. Użyj klawisza **Enter**, aby otworzyć lub zamknąć grupowanie spraw. W ramach otwartej grupy naciśnij klawisz **Tab**, aby przejść do każdego problemu, i&nbsp;naciśnij klawisz **Enter**, aby wybrać bieżący problem.
   - Naciśnij klawisz **Tab**, aby przejść do linku **Więcej informacji** lub przejść do następnego problemu.
3. Użyj **hierarchii nagłówków** lub zaimplementowanych **punktów orientacyjnych**, aby szybko przechodzić z&nbsp;jednej sekcji do drugiej. <br>Lista wdrożonych punktów orientacyjnych jest następująca:
   - Główny punkt orientacyjny w widokach **Ocena dostępności** lub **Tester dostępności** zawiera główną funkcjonalność narzędzia i&nbsp;obejmuje,
     - Obszar **Liczba problemów**: zawiera liczbę problemów według typu oraz łączną liczbę wykrytych problemów.
     - Obszar **Lista problemów**: zawiera listę problemów pogrupowanych według ról elementów, wymagań lub reguł.
     - W widoku Tester dostępności główny punkt orientacyjny zawiera również pomoc dotyczącą problemów oraz przegląd zapisanych skanów, jeśli użytkownik o&nbsp;nie poprosi.
   - Obszar uzupełniający **Podsumowanie skanowania** w widoku Ocena dostępności zawiera podsumowanie skanowania po zakończeniu skanowania lub pokazuje pomoc dotycząca problemu, gdy zostanie wybrany.
   - Obszar uzupełniający **Problem Pomoc** w widoku Ocena dostępności zawiera pomoc dotyczącą problemu po wybraniu dowolnego problemu.

## 7. Raporty sprawdzania dostępności

Narzędzie sprawdzania dostępności może tworzyć raporty dla pojedynczego skanowania lub dla wielu skanów połączonych (raporty z wielu skanów). Raporty pojedynczego skanowania są dostarczane zarówno w formacie arkuszy kalkulacyjnych HTML, jak i&nbsp;MS Excel. Raporty z&nbsp;wielu skanów są dostępne tylko w formacie arkusza kalkulacyjnego MS Excel. Rozdziały [6.4 Tworzenie raportu ze skanowania]() oraz [6.5 Tworzenie raportu z wielu skanów]() opisują sposób generowania raportów.

### 7.1 Raport HTML

Jest to interaktywny raport zapisany jako plik HTML do wykorzystania w przyszłości. Zawiera datę i godzinę skanowania raportu, adres URL oraz podsumowanie wyników testów, a następnie szczegóły problemu uporządkowane według wymagań, ról elementów i reguł. Każde wystąpienie problemu zawiera również łącze **Dowiedz się więcej**, które otwiera nakładkę zawierającą bardziej szczegółowy opis problemu.

Bieżący stan dostępności treści internetowych jest wyświetlany jako procent elementów bez wykrytych naruszeń lub elementów do przejrzenia. 

**Ważna uwaga:** ten odsetek jest oparty wyłącznie na testach automatycznych. Pamiętaj, aby wykonać dodatkowe przeglądy i testy ręczne, aby ukończyć oceny dostępności. Użyj zestawu <[IBM Equal Access Toolkit](https://www.ibm.com/able/toolkit) jako przewodnika. <br />
![Zrzut ekranu raportu z narzędzia sprawdzania dostępności](/images/equal-access/7_1_Report.png)


### 7.2 Raport w arkuszu kalkulacyjnym MS Excel

Raport zkłada się z 5 arkuszy kalkulacyjnych. Może opisywać pojedynczy skan lub wiele skanów.

1. **Przegląd** zawiera nazwę narzędzia i jego wersję, datę skanowania, zestaw reguł, wytyczne i platformę używaną do skanowania oraz podsumowanie ogólnych wyników wszystkich uwzględnionych skanów.
2. **Zestawienie skanowań** zawiera przegląd zestawu skanów w raporcie.
3. **Zestawienie problemów** zawiera przegląd problemów znalezionych we wszystkich skanach. Zagadnienia są podsumowywane według priorytetów, zaczynając od pozycji Poziomu 1, zgodnie z&nbsp;definicją w IBM Equal Access Toolkit, a następnie Poziomu 2 oraz Poziomów 3 i 4. Poziomy 1-3 są niezbędne do spełnienia wymagań IBM. Na każdym poziomie zestawienie zawiera listę problemów, które stanowią naruszenia, kwestie wymagające przeglądu oraz ulepszenia. Liczby są podane dla każdego rodzaju problemu.
4. **Problemy** zawiera szczegóły poszczególnych spraw. Obejmuje to etykietę skanu, identyfikator każdego problemu, odpowiednie wymagania dla dostępności i poziomy zestawu narzędzi.
5. **Definicja pól** definiuje kolumny w pozostałych arkuszach.

W raporcie z wielu skanów, w którym ta sama strona jest skanowana kilka razy, problemy mogą się powtarzać w różnych skanach tej samej strony. Te zduplikowane problemy można zidentyfikować, mając ten sam identyfikator problemu. W przypadku wystąpienia problemów z&nbsp;szablonem witryny lub ponownie użytym komponentem, zostaną one również powtórzone w&nbsp;raporcie, ale mogą mieć różne identyfikatory problemów.

## 8. Informacje zwrotne

Odwiedź [repozytorium git Equal Access](https://github.com/IBMa/equal-access/issues), aby:

1. Zgłosić problem z narzędziem do sprawdzania.
2. Zgłosić problem z regułami sprawdzania lub dokładnością błędów zgłoszonych przez sprawdzarkę.
3. Znaleźć informacje o istniejących problemach.
