---
title: Audyt
sidebar: testy_sidebar
permalink: audyt
folder: ogolne
---

Otrzymujemy coraz więcej pytań o wycenę audytu witryny lub wielu witryn. Z treści mejli można wnioskować, że pytający widzą w zleceniu audytu jedyny sposób na wywiązanie się z ustawowego obowiązku przygotowania i opublikowania deklaracji dostępności.   


## Czy trzeba przeprowadzić badanie i ocenę dostępności witryny?
Tak. Trzeba, chociaż ustawa nie wymienia wprost takiego obowiązku. Ale wynika on z wzoru deklaracji ustanowionego przez Ministra Cyfryzacji na podstawie ustawy oraz Decyzji wykonawczej Komisji (UE) 2018/1523 z&nbsp;11&nbsp;października 2018&nbsp;r. W&nbsp;deklaracji podmiot publiczny musi określić poziom zgodności witryny z przepisami ustawy (zgodna, częściowo zgodna, niezgodna), przedstawić niezgodności, jeśli mają miejsce, oraz wskazać, na jakiej podstawie sporządzono deklarację. Możliwe są dwie &bdquo;podstawy&rdquo; - **samoocena** lub **ocena podmiotu zewnętrznego**. W&nbsp;decyzji wykonawczej znajdujemy bardzo istotne uściślenie tej kwestii. Artykuł 3 zawiera następujace zobowiązanie:  

> &bdquo;Państwa członkowskie zapewniają, aby treść zawarta w oświadczeniu [...] była precyzyjna i opierała się na jednym z następujących elementów:<br />a) rzeczywistej ocenie zgodności strony internetowej lub aplikacji mobilnej z wymogami dyrektywy (UE) 2016/2102 [...]<br />b) wszelkich innych środkach uznanych za właściwe przez państwa członkowskie, dających równorzędną pewność, że treść zawarta w oświadczeniu jest precyzyjna.&rdquo;

Zwróćmy uwagę na kilka słów kluczowych dotyczących treści oświadczenia. Treść ma być **precyzyjna** oraz opierać się na **rzeczywistej ocenie**. Kwestią drugorzędną jest, kto tej oceny dokonuje. 

A skoro ocena musi być **rzeczywista** i **precyzyjna**, to musi się opierać na podstawie, która zapewni **wiarygodne** wyniki. To nie może być ocena **na oko**, **na wyczucie**. 

## Czy istnieje spójny standard dla przeglądów dostępności?
Tak, są to [Wytyczne W3C dotyczące dostępności treści internetowych](https://wcag.lepszyweb.pl) znane jako  WCAG 2.1. Wytyczne zawieraja ogółem 78 wymagań nazwanych kryteriami sukcesu. Zgodnie z ustawą o dostępności cyfrowej strony internetowe instytucji publicznych muszą spełnić 49 spośród kryteriów sukcesu. Są to - z jednym wyjątkiem - wszystkie kryteria sukcesu na poziomie&nbsp;A oraz AA.   

Ponadto ustawa z 19 lipca 2019 r. o zapewnianiu dostępności osobom ze szczególnymi potrzebami dodała wymóg:

> zapewnienie na stronie internetowej danego podmiotu informacji o zakresie jego działalności – w&nbsp;postaci elektronicznego pliku zawierającego tekst odczytywalny maszynowo, nagrania treści w&nbsp;polskim języku migowym oraz informacji w tekście łatwym do czytania

## Czy istnieje jednolita metodologia oceniania dostępności? 
Tak. Istnieje opublikowana przez W3C jako nota [Website Accessibility Conformance Evaluation Methodology (EM-WCAG) 1.0](https://www.w3.org/TR/WCAG-EM/), która opisuje ujętą w 5 kroków szczegółowo procedurę przeprowadzania oceny dostępności. Metodologii towarzyszy specjalnie opracowane narzędzie - [Generator raportów](https://raport.lepszyweb.pl/#!/). 

EM-WCAG **definiuje tylko ogólne zasady oceniania**. Dobór konkretnych metod oceniania należy do oceniających. Oceniający mogą stosować testy automatyczne, analizę poznawczą, testy przypadków użycia i testy użyteczności tak, aby uzyskać wiarygodne wyniki oceny.  

{% include callout.html content="Metodologia ta w żaden sposób nie dodaje ani nie zmienia wymagań określonych w normatywnym standardzie WCAG 2.1, ani też nie dostarcza instrukcji dotyczących oceny zawartości stron internetowych pod względem cech charakterystycznych. " type="success" %}

W polskich zasobach poświęconych dostępności cyfrowej można  znaleźć kilka pozycji, które prezentują dokładniejsze instrukcje i&nbsp;objaśnienia na temat sposobu badania dostępności. Są to: 

- [Metoda oceny dostępności cyfrowej strony internetowej zgodnie z zasadami WCAG 2.1](http://widzialni.org/metoda-oceny-dostepnosci-cyfrowej-strony-internetowej-zgodnie-z-zasadami-wcag-21,new,mg,6,371) - opisuje procedurę audytu i objaśnia wszystkie kryteria sukcesu,  
- [Łatwe testy dostępności](https://testy.lepszyweb.pl/00-P-wprowadzenie) - instruują, jak przeprowadzić wstępny przegląd dostepności we własnym zakresie (zostały opracowane na podstawie dokumentu W3C WAI zatytułowanego [Easy Checks - A First Review of Web Accessibility](https://www.w3.org/WAI/test-evaluate/preliminary/). 
- [Jak zbadać, czy strona www jest dostępna cyfrowo - Lista kontrolna - wersja BETA](https://www.gov.pl/web/dostepnosc-cyfrowa/jak-zbadac-czy-strona-www-jest-dostepna-cyfrowo), która docelowo ma być zalecana przez Ministerstwo Cyfryzacji podmiotom publicznym jako metoda sprawdzania dostepności cyfrowej 
  
- [Jednolita baza testów dostępności cyfrowej](https://testy.lepszyweb.pl/H0-00-wprowadzenie) - projekty testów zgodności z WCAG 2.1 z opisami procedur testowania (baza w trakcie tworzenia)

- [Podstawa testowania TIK](https://testy.lepszyweb.pl/ICT-00-wprowadzenie) - tłumaczenie na język polski podstawowego zestawu testów dostępności cyfrowej stron internetowych stosowanego w agencjach rzadowych Stanów Zjednoczonnych ( [*ICT Testing Baseline*](https://section508coordinators.github.io/ICTTestingBaseline/))

## Czy można zbadać i ocenić dostępność kilkuset stron w dużej witrynie
Oczywiście, można. Skoro można zbadać i ocenić jedną stronę, to można również zbadać 50, 100, 500, a nawet i 5000 czy 10000 stron. Ale byłoby to bardzo czaso- i  pracochłonne. Liczba godzin, jaką trzeba byłoby na audyt poświęcić, byłaby ogromna. A wynagrodzenie audytora-profesjonalisty nie do zaakceptowania nawet dla najbogatszych i uznających dostępność za wartość godną każdej ceny.

Prawidłowa odpowiedź na tytułowe pytanie brzmi więc, że **można, ale nie trzeba**. Aby ocenić dostępność witryny, nie trzeba oceniać wszystkich strona na witrynie, można poddać ocenie odpowiednio dobraną reprezentatywną próbkę.

## Czy wystarczy przeprowadzić ocenę dobrym narzędziem automatycznym?

Absolutnie, nie wystarczy! Oczywiście, trzeba korrzystać z możliwości testów automatycznych. Ale jedyne, co mogą zrobić najdoskonalsze automaty, to wykryć i wskazać niektóre błędy lub braki w kodzie oraz wskazać miejsca, w których mogą się pojawić problemy z dostępnością. Ocenia się, że za pomocą testów automatycznych, zależnie od narzędzia, można wykryć około 20-25% problemów z dostępnością oraz dodatkowo uzyskać wskazanie kolejnych 30-40% miejsc, które wymagają oceny człowieka.

Oznacza to, że warto i trzeba korzystać z testów automatycznych, bo dzięki nim można szybkko i łatwo zbadać nawet wiele tysięcy stron i uzyskać precyzyjne wyniki. Gdyby te testy przeprowadzać ręcznie, trzeba by poświecić niewspółmiernie dużo czasu i wysiłku w stosunku do uzyskanego efektu. Krótko mówiąc, jeśli coś może zrobić maszyna, niech zrobi maszyna, bo będzie i szybciej, i taniej. 

Ale to nie wystarczy. Spełnienie około 75% wymogów dostępności musi zbadać człowiek.

## Jak długo trwa (albo ile kosztuje) ręczny audyt jednej strony?
Audytor musi przejrzeć stronę, ocenić ją pod kątem wymaganych kryteriów sukcesu, odnotować w arkuszu kontrolnym, czy było ocenione i&nbsp;z&nbsp;jakim efektem albo że nie było oceniane, bo nie podlega ocenie albo na stronie nie ma elementów, których dane kryterium dotyczy. W przypadku stwierdzenia, że jakieś kryterium nie jest spełnione, audytor musi ten fakt udokumentować - opisać, wykonać zdjęcie (zrzut ekranu), zacytować fragment kodu, a następnie wskazać, co należy zrobić, aby usunąć problem dostępności.

Nie trzeba dużej wyobraźni, by wyliczyć sobie, ile czasu może zająć przegląd tylko jednej strony, a na tej podstawie, ile czasu zajmie audyt na przykład 30 stron.

Na audyt pojedynczej prostej strony potrzeba zwykle 1-2 godziny (przegląd pod kątem 49 wymagań, odnotowanie zgodności, dokumentacja niezgodności). Natomiast audyt jednej, złożonej interaktywnej i unikalnej strony zajmuje specjaliście kilka godzin - 3, 5, a bywa że nawet 8-10. Wszystko zależy od złożoności strony i ilości wystepujących na niej problemów.

Oznacza to, że wykonanie audytu obejmującego próbkę 30 stron (badanie i sporządzenie raportu) zajmuje audytorowi w granicach 100-120 godzin pracy. 

Nie trzeba dużej wyobraźni, by wyliczyć sobie orientacyjną cenę takiej usługi, a także ocenić szczególnie &bdquo;atrakcyjne&rdquo; oferty wykonania audytu. 

## Co to znaczy &bdquo;solidny&rdquo;, &bdquo;pełny&rdquo; audyt?
Wszystko zależy od celu i zakresu audytu. Rozważmy trzy sytuacje: prosta witryna licząca do kilkunastu stron, większa witryna licząca do 100 stron i złożona witryna, zawierająca formularze lub tzw. bogate aplikacje internetowe (galerie zdjęć, slajdery, multimedia) albo licząca więcej niż 100 stron. Celem audytu jest stwierdzenie zgodności z WCAG 2.1 na poziomie AA.

### Audyt małej prostej witryny
Solidny audyt prostej witryny powinien objąć co najmniej automatyczne testy wszystkich stron, audyt ręczny strony głównej oraz audyt 1-2 innych stron szczególnie ważnych dla witryny, np. strony kontaktowej, strony z wynikami wyszukiwania, jeśli taka jest na witrynie. Po pobieżnym przeglądzie wszystkich stron, co zajmie 10-15 minut, audytor może wybrać stronę, czy strony, które powinny być zbadane, aby wynik audytu był wiarygodny. 

Oczywiście, może się zdarzyć, że audytowi ręcznemu trzeba poddać więcej niż 2-3 strony. Kluczowe jest tutaj założenie, że mamy do czynienia z &bdquo;prostą witryną&rdquo;, czyli witryną, na której są tylko strony informacyjne, bez formularzy, zbudowane na jednym szablonie.

### Audyt większej witryny - do 100 stron
Liczba stron jest tutaj tylko orientacyjnym wyznacznikiem rodzaju witryny. Wciąż myślimmy o niewielkich, raczej prostych witrynach.   
W przypadku takiej witryny na solidny audyt złoży się prawdopodobnie co najmniej audyt automatyczny 10-20 lub więcej stron oraz audyt ręczny próbki 4-5 stron, w tym strony głównej. 
Jeśli strony witryny są oparte na szablonie i&nbsp;2-3 różnych układach treści oraz jeśli na witrynie nie ma specyficznych usług, badanie przyniesie wiarygodny wynik w&nbsp;odniesieniu do całej witryny. 

Ale jeśli na witrynie są jakieś usługi wymagająca złożonych interakcji użytkownika z witryną albo wykorzystuje się na witrynie bogate aplikacje internetowe, to ich badanie z natury rzeczy zwiększy liczbę stron, które trzeba przebadać. 

Oczywiście, może się zdarzyć, że nie zostaną wykryte jakieś usterki, których nie było na badanych stronach, a objawią się na innych, niebadanych. W takim przypadku trzeba je będzie po prostu naprawić, jeśli się da, a jeśli - odnotować w deklaracji dostępności i naprawić w późniejszym czasie. 
           
### Audyt złożonej witryny
W tym przypadku solidny audyt musi obejmować tzw. reprezentatywną próbkę stron i stanów, wybraną zgodnie z&nbsp;metodologią określoną przez W3C.    
Reprezentatywna probka stron powinna obejmować różne typy stron (także stanów stron). Liczba stron, które powinny być poddane audytowi, aby przynieść wiarygodne dla całej witryny wyniki, wynosi zwykle od 30 do 50 stron. I, oczywiście, zależy od złożoności witryny. 

## Czy konieczne są badania z użytkownikami?
Badania z użyytkownikami sa bardzo skutecznym, ale też najkosztowniejszym sposobem oceny dostępności cyfrowej witryny. Testy z użytkownikami są wyśmienitym uzupełnieniem testów automatycznych i ręcznych i wydają się logicznie najlepszym wyborem do sprawdzania dostępności. Aby zbadać zgodność z WCAG oraz zebrać wiarygodne dane o dostępności, badanie z użytkownikami nie jest konieczne.

O ewentualnym przeprowadzeniu testów z użytkownikami i ich zakresie powinien zdecydować audytor w porozumieniu ze zlecającym audyt.

Warto przy tym pamiętać, że wiedzę o problemach, jakie napotykają osoby ze specjalnymi potrzebami można również pozyskać od rzeczywistych użytkowników. Angażowanie użytkowników z niepełnosprawnościami do oceny dostepności cyfrowej witryny niekoniecznie musi polegać tylko na formalnych testach.    

## Czy można uzyskać certyfikat dostępności cyfrowej witryny?
Nie istnieją powszechnie przyjęte i akceptowane procedury certyfikacji witryn internetowych i aplikacji mobilnych. Tym samym nie ma testerów czy audytorów, którzy są upoważnieni do takiej certyfikacji. Można się wszkaże spotkać z firmami, które twierdzą, że &bdquo;certyfikują&rdquo; witryny, zwłaszcza wykonane w swoich pracowniach. Takie &bdquo;certyfikaty&rdquo; oznaczają co najwyżej, że w wyniku przeprowadzonego audytu nie stwierdzono żadnych problemów z dostępnością. Mogą więc być świadectwem zaangażowania wydawcy w dostępność, ale nie stanowią żadnego dowodu, że witryna jest w pełni dostępna. Chociażby dlatego, że jeszcze tego samego dnia na wittrynie mogą być umieszczone nowe niedostępne treści - zeskanowany dokument PDF, wideo bez transkrypcji i audiodeskrypcji, galeria zdjęć bez opisów alternatywnych, artykuł z niepoprawną strukturą nagłówków, itd. 

Oczekiwanie, że audytor wyda jakiś &bdquo;certyfikat dostępności&rdquo; jest bezprzedmiotowe. Od audytora ttrzeba oczekiwać rzeczowego raportu z badania, w którym wskaże, które kryteria dostępności są spełnione, których wymagań witryna nie spełnia oraz co należy zrobić, aby naprawić wykryte defekty.  
 
## Jak najlepiej przygotować i zamówić audyt?

**Po pierwsze** i przede wszystkim należy rozważyć, czy 


**Po pierwsze** i przede wszystkim należy rozważyć, czy i czym uzsadanione jest zlecanie audytu podmiotowi zewnętrznemu. Audyt zewnętrzny ma swoje niewątpliwe zalety. Należą do nich profesjonalność i doświadczenie ekspertów, obiektywność oceny, niezależność, bezstronny punkt widzenia, status raportu wzmocniony zewnętrznym, eksperckim punktem widzenia. Ale decydując się na zlecennie audytu, należy uwzględnić, nie tylko, że jest kosztowny, ale przede wszystkim realne możliwości &bdquo;skonsumowania&rdquo; wyników audytu. 
Jeżeli nasze środki na zapewnienie dostępności cyfrowej są ograniczone, sensowniej jest zainwestować je np. w konsultacje eksperckie i podjęcie możliwych działań naprawczych, w szkolenie i przygotowanie własnej kadry do przeprowadzania okresowych badań dostępności czy nawet zbudowanie nowej dostępnej witryny. 

**Po drugie**, zanim zlecimy wykonanie profesjonalnego audytu, należy przeprowadzić wstępny przegląd dostępności witryny i doprowadzić do wyeliminowania typowych błędów. Przegląd wstępny można wykonać we włąsnym zakresie lub zlecić podmiotowi zewnętrznemu. Instrukcję przeprowadzenia przegladu wstępnego można znaleźć na stronie [Łatwe testy dostępności](https://testy.lepszyweb.pl/00-P-wprowadzenie).

**Uwaga**: wykonanie przeglądu wstępnego i naprawa błędów wykrytych w wyniku przeglądu wstępnego nie jest **obowiązkowa**, ale może przyczynić się do obniżenia kosztów pełnego audytu nawet o 20-40%. 


**Po trzecie**, w zamówieniu audytu należy sprecyzować oczekiwania zamawiającego dotyczące zakresu audytu oraz czasu wykonania. W tym celu należy się zapoznać z cennikiem audytora lub firmy oferującej audyty, jeśli jest dostępny, lub zapytać o cennik, jeśli nie jest dostępny. Kierowanie pytań o wycenę audytu bez sprecyzowania oczekiwań mija się z celem.  

    






Zważywszy, że urzędy i instytucje wydają w Polsce ponad 280 tysięcy witryn, a specjalistów, którym można zlecić wykonanie audytu, jest niewielu, prawie wszystkie urzędy i instytucje są zmuszone wykonać tę pracę własnymi siłami.




## Czy coś może być certyfikowane jako dostępne i / lub być zatwierdzone przez certyfikowanych testerów?

Nie ma powszechnie przyjętej i akceptowanej zewnętrznej certyfikacji witryn / aplikacji ani  testerów. Niemniej jednak w niektórych częściach rządu federalnego USA istnieje program zaufanych testerów DHS, ale to nie znaczy wiele poza stronami rządu federalnego. Istnieje kilka organizacji zewnętrznych, które wymyśliły określoną wiedzę i test, ale nie oznacza to zbyt wiele poza wskazaniem, że ktoś ma wiedzę na temat WCAG.
Jest też kilka organizacji zajmujących się dostępnością, które twierdzą, że " certyfikują " witrynę jako dostępną po zapoznaniu się z nią, choć tak naprawdę nie oznacza to niczego poza faktem, że dokonali jej przeglądu i potwierdzili, że problemy zostały naprawione.
VPAT jest czasem niezbędny w kontaktach z rządem federalnym USA. Jest to samocertyfikacja, w której organizacja informuje użytkowników / nabywców rządowych, że uważają swoją stronę za w pełni dostępną.
Rada: Skoncentruj się na znalezieniu kompetentnych osób, które dokonają przeglądu jakości, a nie jakiejkolwiek certyfikacji testerów lub wyników.



## Czy można przejrzeć tysiące stron pod kątem dostępności?
Cóż, jest to  możliwe,  ale byłoby to bardzo czasochłonne, a godziny pracy byłyby ostatecznie znaczące, a zatem przy wynajmie, drogie.
Kluczową kwestią jest to, że dokonując przeglądu pod kątem dostępności, mimo że istnieje wiele wspaniałych zautomatyzowanych narzędzi dostępności, najlepsze, co mogą zrobić te narzędzia, to wyraźnie zidentyfikować pewne problemy. W przypadku wielu potencjalnych problemów związanych z dostępnością większość z tych narzędzi może oznaczyć potencjalne obszary do późniejszego ręcznego przeglądu. A w przypadku niektórych problemów narzędzia nie mogą tego zrobić.
Porada: Zdecydowanie rozważ uruchomienie automatycznego narzędzia, które pozwoli Ci oznaczyć potencjalne problemy i wątpliwości, ale pamiętaj, że nie zastępuje to ręcznego przeglądu.

Aplikacje i elementy interaktywne nie mogą być przeglądane za pomocą narzędzi automatycznych.
W wielu przypadkach trzeba przejrzeć elementy interaktywne, np. gdy użytkownik musi dokonać wyboru lub wprowadzić jakąś informację, a następnie system wysyła je lub dalej kieruje użytkownika do następnego kroku. W innych przypadkach konieczne jest sprawdzenie aplikacji. W takich przypadkach zautomatyzowane narzędzia na ogół nie będą działać w ogóle, więc ponownie wrócimy do ręcznej oceny.
Porada: W przypadku aplikacji i elementów interaktywnych ręczna recenzja jest nie tylko ważna, ale jest jedynym sposobem na przeprowadzenie dowolnego przeglądu.

## Jak długo trwa pełny przegląd ręczny?
Chociaż możliwe jest ręczne sprawdzenie aplikacji lub witryny z ograniczoną i skończoną liczbą ekranów (lub wybranej nowej części, jeśli oryginalny produkt był już dostępny), w przypadku witryn i aplikacji z bardzo dużą liczbą ekranów, przegląd prawdopodobnie potrzebuje być próbkowaniem.
Zasadniczo zakładam, że jedna złożona, interaktywna i unikalna strona może zająć kilka godzin na sprawdzenie, zgłoszenie i omówienie z zespołem programistów. Kolejne podobne strony zwykle zajmują znacznie mniej czasu, w dużej mierze zależnie od tego, jak wiele jest unikalnych w przypadku tych podobnych stron oraz od oczekiwanej dokładności przeglądu i raportowania na stronie.
Rada: Określ, jakie unikalne szablony, style i elementy interaktywne są do sprawdzenia i oceny, a następnie przejrzyj próbkę każdego rodzaju unikalnych elementów z całej witryny.


## Co ze stronami lub ekranami, które nie zostały sprawdzone?
Chociaż sam nie jestem programistą, uważam, że recenzje unikalnych elementów często identyfikują wady kodowania, które można następnie zidentyfikować gdzie indziej i wszędzie poprawić. Czasami problemy nie są związane z kodem, ale z wprowadzaniem informacji. Na przykład obrazy są umieszczane w systemie zarządzania treścią, a ci, którzy ułatwiają wprowadzanie obrazu, są instruowani, aby oznaczyć obrazy jako „czysto dekoracyjne”, aby ominąć alternatywny wymóg dotyczący tekstu, lub alternatywny tekst jest dostarczany przez system jako nazwa obrazu . Następnie zespół wie, aby wrócić i poszukać tych spójnych problemów w całej witrynie.
Porada: Jeśli dokładny przegląd każdej strony nie jest realny, rozważ przynajmniej zerknięcie na inne strony, które są poza zakresem, aby pomóc w sprawdzeniu, jakie mogą być powtarzające się tematy.


## Czy istnieje spójny standard dla przeglądów dostępności?
Tak, są to Wytyczne W3C dotyczące dostępności treści internetowych znane jako  WCAG 2.0 (wkrótce 2.1) . W Stanach Zjednoczonych najczęstszym innym zestawem wytycznych jest Sekcja 508, która jest przeznaczona wyłącznie dla witryn rządowych. Prawda jest taka, że sekcja 508 i WCAG 2.0 były w harmonii od kilku lat, więc są mniej więcej tym samym zbiorem wytycznych.
Porada: Bez względu na to, czy zatrudniasz do oceny dostępności, czy robisz to we własnym zakresie, zapoznaj się z ramami zgodności dostępności, zapoznając się przynajmniej z WCAG.




## Czy celem jest perfekcja?
Prawdopodobieństwo, że duża witryna będzie w większości dostępna, ale nie absolutnie idealne. Napraw każdy element, który możesz, upewniając się, że wszystkie zamierzone funkcje mogą być używane w różnych technologiach wspomagających, ale wiedz, że absolutna doskonałość jest trudna do osiągnięcia.
Porada: Zawsze będą pojawiać się problemy z dostępnością, które po prostu się zdarzają, więc staraj się na bieżąco śledzić dostepność i być na bieżąco z opiniami użytkowników o tych drobnych usterkach..

## Od czego zacząć
Najlepszą możliwą rzeczą, którą możesz zrobić, zanim jeszcze rozpocznie się rozwój, jest przeszkolenie zespołu programistów w zakresie zasad dostępności. Spraw, by produkowali witryny i aplikacje, które są w większości dostępne od samego początku i będą dostępne na bieżąco w miarę zmian.
Rada: Niezależnie od tego, czy jesteś w domu, czy przez opcję zewnętrzną, rozpocznij ten trening dostępności i zaoszczędź sobie bólu głowy w przyszłości!




Oczywiste jest, pomimo braku wytycznych w WCAG, że poprzez zastosowanie różnych poziomów potwierdzają, że nie wszystkie problemy z dostępnością są sobie równe. Niektóre elementy mają większy wpływ na użytkowników niż inne. Niektóre przedmioty są technicznie trudne lub niemożliwe do osiągnięcia. Niektóre elementy nie mają dobrego wsparcia wśród programów użytkownika lub technologii asystujących. W wyniku wszystkich tych i wielu innych czynników lekkomyślność traktowałaby wszystko tak, jakby wszystkie były równe. W niektórych przypadkach może to zaryzykować budżety, nie pomagając użytkownikowi końcowemu. Zamiast tego należy ukierunkować środki zaradcze, aby zapewnić najlepsze korzyści szybko i tanio.



Jeśli witryna będzie generalnie dostępna, wydawcy mogą liczyć na informacje zwrotne od rzeczywistych użytkowników, jeśli   


wydawca witryny może się dowiedzieć o problemach z dostepnoscią 


Nie, nie są konieczne. Chociaż testy z użytkownikami są skutecznym sposobem badania dostępności, to nie są konieczne w audytach dostępności, których celem jest zbadanie zgodności z WCAG. Doświadczony audytor bada  

Testy z użytkownikami są niewątpliwie skutecznym sposobem badania dostępności, 

to nie są konieczne w audytach dostępności, których celem jest zbadanie zgodności z WCAG. 


To oczywiście prawda, że &bdquo;Dopóki Twoja witryna nie została przetestowana przez prawdziwą osobę z prawdziwymi niepełnosprawnościami, tak naprawdę nie została przetestowana&rdquo; (Keith Bundy, konsultant Siteimprove). Inaczej, dopóki witryna nie zostanie przetestowana przez użytkowników z niepełnosprawnościami, **nie można być pewnym** jej dostępności. 


W metodologii zalecanej przez W3C również znajdziemy stwierdzenie, że &bdquo;Najbardziej efektywne i wiarygodne wyniki badania strony internetowej uzyskuje się łącząc ekspercką analizę w oparciu o listę kontrolną WCAG z badaniem z&nbsp;użytkownikami. Opinie użytkowników uzupełniają wyniki analizy.&rdquo;.

{% include callout.html content="Najbardziej efektywne i wiarygodne wyniki badania strony internetowej uzyskuje się łącząc ekspercką analizę w oparciu o listę kontrolną WCAG z badaniem z&nbsp;użytkownikami. Opinie użytkowników uzupełniają wyniki analizy." type="success" %}  


, w tym:
- strony kluczowe, takie jak strona główna, strony poczatkowe głównych obszarów (działów) witryny,
- strony wspólne, takie jak  strona kontaktowa, strony prawne (regulamin, polityka prywatności, deklaracja dostępności), mapa witryny
- strony reprezentatywne dla głównych zastosowań witryny,
- strony reprezentatywne dla istotnych (niezbędnych) funkcjonalności witryny, np. formularze rejestracyjne,procedury wypełniania i przesyłania kwestionariuszy  
- strony reprezentatywne dla różnych typów stron, np. różnych typów i układów treści, strony o odmiennym wyglądzie i stylu, 
- strony reprezentatywne dla różnych technologii internetowych, takich jak strony zawierajace ramki, tabele danych, formularze, bogate aplikacje internetowe oparte na skryptach (karty, harmonijki, suwaki, galerie, itp.).

Niektóre strony mogą reprezentować równocześnie kilka wymienionych powyżej kategorii stron.
Reprezentatywna próbka będzie liczyć zwykle około 30-40 stron.
   


W mejlach ani słowa o oczekiwaniach albo niezbyt spójne wymagania przepisane z jakichś opracowanych przed kilku laty &bdquo;wkładów&rdquo; do zapytań oferowych. 




Przy czym pytający albo w ogóle nie określa swoich oczekiwań, albo przeciwnie - przytacza jakieś opracowane przed kilku laty &bdquo;wkłady&rdquo; do zapytań oferowych, w których wyszczególnia 

Z pytań wynika, że  audyt ma posłużyć przygotowaniu deklaracji dostępności. Bywa, że 


Bywa, że nawet wycenę audytu 10 witryn z dwutygodniowym terminem realizacji.


W pytaniach 
W prośbach albo ani słowa o oczekiwaniach albo przeciwnie - przepisane z jakichś opracowań niezbyt spójne wymagania, świadczące jedynie o tym, że pytający nie bardzo wiedzą, czego chcą. Z treści zapytań wynika jedynie oczekiwanie, że witryna bądź wiele witryn zostaną dokładnie przebadane, a wynikiem będzie przede wszystkim jakieś świadectwo, które da się wykorzystać w deklaracji dostępności jako potwierdzenie zgodności z ustawą.  
   

  








