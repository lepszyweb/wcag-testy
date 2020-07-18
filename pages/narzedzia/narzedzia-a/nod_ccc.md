---
title: WCAG Color Contrast Checker 
tags: [narzędzia-oceny-dostępności,kontrast kolorów]
sidebar: narzedzia_sidebar
permalink: nod-ccc
folder: narzedzia-a
---

## Do czego służy?
Jednym z najbardziej poręcznych narzędzi oceny kontrastu między tekstem i tłem jest rozszerzenie przeglądarek Chrome i Firefox autorstwa Jorge Rumosoro. 

Dodatek analizuje kontrast między barwą tekstu i barwą tła wszystkich elementów tekstowych na stronie internetowej. 

Z dokumentacji dodatku wynika, że może również analizować kontrast w dokumentach osadzonych na stronie za pomocą ramek łączonych (iframe). Do przełączania się między dokumentami miałby służyć specjalny przycisk, którego do chwili napisania tego poradnika nie udało nam się zlokalizować.

Niestety, rozszerzenie nie analizuje kontrastu między obiektami nietekstowymi i ich tłem. Autor objaśnia, że „Jeśli element jest obrazem, to wykrytym kolorem pierwszego planu jest ten, którego używałby tekst alternatywny obrazu, a jeśli element zawiera obraz jako tło, to kolor tła jest tym, który został określony bez uwzględnienia obrazu.” Trochę to skomplikowane, ale w praktyce raczej bez znaczenia. Nie spotkaliśmy się z przypadkiem, by dodatek „pomylił” tekst z nie-tekstem. Ale możliwe jest, że w przypadkach, gdy tłem dla tekstu jest obraz osadzony lub obraz tła, uzyskamy błędny wynik. Na przykład, gdy na jednolicie czarnym obrazie zostanie umieszczony biały tekst dodatek zgłosi błąd współczynnika kontrastu, gdy kolorem tła strony będzie kolor biały lub niewystarczająco ciemny. 

## Instalacja
Rozszerzenie instalujemy jak każdy inny dodatek do przeglądarki. Przejdź do internetowego sklepu Chrome lub Mozilla Add-ons, wyszukaj WCAG Color Contrast Checker i zainstaluj w przeglądarce, naciskając przycisk Dodaj do… (Chrome, Firefoxa).

## Stosowanie 
Korzystanie z dodatku nie wymaga specjalnych umiejętności. Po prostu przejdź na stronę, którą chcesz zbadać i uruchom dodatek. Niemal natychmiast w bocznym oknie wyświetlą się wyniki testu.


## Okno i funkcje programu
Okno dodatku podzielone jest na trzy sekcje. W nagłówku znajduje się logo, menu z dostępem do opcji Pomoc, Powtórz test i Uwagi o wydaniu, przycisk wyłączania dodatku oraz trzy rozwijane listy opcji z możliwością ustawienia wymaganego poziomu WCAG – AA lub AAA, filtra symulatora ślepoty barw oraz autoodświeżania.

![Główne okno programu Colour Contrast Analyser (Windows)](/images/cca/ccc-wcag.png)

Główna część okna podzielona jest na dwie sekcje. W pierwszej, górnej wyświetlana jest tabela z wynikami testów, w dolnej dynamicznie wyświetlane są szczegółowe dane każdego z wykrytych przypadków pary kolorów.
 
## Wyniki testów

![Tabela wyników testów](/images/cca/ccc-tabela.png)

Wyniki w tabeli uporządkowane są w trzech kolumnach. W kolumnie *Contrast* wyświetlana jest ikona informująca, czy spełnione zostały wymagania WCAG, a obok niej podany jest wyliczony współczynnik kontrastu. W kolumnie *Size* podany jest rozmiar tekstu – small (mały) lub large (duży), w kolumnie *Elements* znajdują się kolejno: próbka koloru pierwszego planu na tle, liczba wykrytych elementów, nazwa elementu html oraz ikona sygnalizująca, czy element jest widoczny (oko), czy ukryty (przekreślone oko).

## Elementy widoczne i ukryte
Ikonę sygnalizującą, czy element jest widoczny czy ukryty narzędzie dodaje w wierszu wyników, gdy wykryje, że w badanym elemencie strony zastosowano techniki ukrywania treści (dla elementów składanych, wysuwanych, menu, itp.).

Zaznaczenie wiersza z danymi powoduje otoczenie czerwonym obramowaniem wykrytych i ocenionych instancji zestawienia barw i równocześnie  wyświetlenie w dolnej części okna dodatku szczegółowych danych analitycznych:

-	Kodu koloru pierwszego planu (tekstu)
-	Kodu koloru tła
-	Próbek tekstu: małego, małego pogrubionego i dużego
-	Tabelki zgodności z kryteriami sukcesu 1.4.3 i 1.4.6.  

 
## Selektor ślepoty barw
Narzędzie pozwala także ocenić dostępność zastosowanego schematu kolorystycznego dla osób z różnymi rodzajami ślepoty barw. Wystarczy wybrać dowolną z opcji z listy rozwijanej w nagłówku okna, a kolor na stronie będą naśladować widzenie w sposób dostosowany do wybranego rodzaju schorzenia, a kontrast kolorów zostanie ponownie oszacowany zgodnie ze zmienionym stanem wizualnym.

![Tabela wyników testów](/images/cca/ccc-protanopia.png)


## Analiza własnych kolorów
Rozszerzenie zawiera analizator kolorów, który pozwala wprowadzić kombinację kolorów w celu oceny różnicy kontrastu między nimi.  W polach tekstowych można wpisać kody szesnastkowe kolorów do zbadania albo wybrać kolory z palety próbnika.   
Analizator posiada również funkcję wybierania kolorów bezpośrednio z dokumentu. Można ją aktywować za pomocą kroplomierza umieszczonego obok pól na kody kolorów.

![Tabela wyników testów](/images/cca/ccc-analizator-kolorow.png)

 
## Aktualizacja DOM i odświeżanie wyników testu
Ciekawą funkcjonalnością jest możliwość  przetestowania zmian w drzewie DOM lub zmiany wartości klas stylów CSS za pomocą narzędzi programisty w przeglądarce. Można np. zmodyfikować dowolny kolor wybranego elementu, a następnie użyć przycisku check contrast (sprawdź kontrast), aby ocenić efekt modyfikacji. 



