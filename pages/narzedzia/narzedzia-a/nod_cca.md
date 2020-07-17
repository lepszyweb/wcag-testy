---
title: CCA - Analizator kontrastu kolorów 
tags: [narzędzia-oceny-dostępności,kontrast kolorów]
sidebar: narzedzia_sidebar
permalink: nod-cca
folder: narzedzia-a
---

## Analizator kontrastu kolorów
Analizator kontrastu kolorów (CCA) pomaga określić czytelność tekstu i kontrast elementów wizualnych, takich jak kontrolki graficzne i wskaźniki wizualne.

Program jest aplikacją komputerową działającą na platformach Windows i Mac OS, stworzoną przez zespół programistów z [https://developer.paciellogroup.com/resources/contrastanalyser/](The Paciello Group), wydaną na Powszechne Licencji Publicznej GNU.

Twórcy programu promują jego 4 główne cechy:

- Wskaźniki zgodności z WCAG 2.1
- Kilka sposobów ustawiania kolorów: wprowadzanie tekstu (akceptuje dowolny prawidłowy format kolorów CSS), suwaki RGB, próbnik kolorów 
- Obsługa przezroczystości alfa w kolorach pierwszego planu
- Symulator ślepoty barw

## Obsługa programu
Jest bardzo prosta. Wystarczy wprowadzić w odpowiednich polach kolor tekstu (pierwszego planu, 'foreground colour') i kolor tła ('background colour'), a CCA wylicza, czy współczynnik kontrastu jest wystarczający, w zależności od rodzaju i rozmiaru treści wizualnej. W ocenie wykorzystane są zalecenia Wytycznych dla dotyczących dostępności treści internetowych (WCAG 2) dla poziomów AA i AAA.

## Instalacja programu
Program w odpowiedniej dla swojego systemu operacyjnego wersji pobieramy z repozytorium umieszczonym na platformie Github pod adresem https://github.com/ThePacielloGroup/CCAe/releases

Sposób instalacji zależy od wybranego formatu. Można rozpakować  archiwum do wybranego katalogu albo zainstalować, korzystając z procedury właściwej dla posiadanego systemu operacyjnego. 

Po instalacji warto w opcjach konfiguracyjnych ustawić opcję Enable Auto Update, co powinno zapewnić automatyczną aktualizację programu (niestety, w wersji 3.1.1 dla systemu Windows próba zapisu ustawienia nie przynosi spodziewanego skutku).

## Okno i funkcje programu
 
W oknie programu możemy wyróżnić kilka sekcji.

W menu (1) znajdziemy takie opcje, jak: *Preferences* (Ustawienia), *Edit -> Copy results* (Edycja – Kopiuj wyniki), *Colour blidness simulation*  (Symulator ślepoty kolorów).

W górnej części okna znajdują się narzędzia do określenia badanych kolorów (2, 3).  Mamy możliwość wyboru jednego z typowych formatów zapisu kolorów (HEX, RGB, HSL, HSV), przy czym w&nbsp;przypadku kolorów pierwszego planu obsługiwane są również formaty z przezroczystością alfa (HEXa, RGBa, HSLa i HSVa). 

![Główne okno programu Colour Contrast Analyser (Windows)](/images/cca/cca-glowny.png)


Kolory można wprowadzić ręcznie, podając w odpowiednich polach ich kody, albo wybrać z&nbsp;badanej strony czy dokumentu, korzystając z&nbsp;próbnika kolorów. Próbnik powiększa obszar, z którego chcemy pobrać próbkę tak, że można wskazać żądany kolor bardzo precyzyjnie. 

![Próbnik (wybierak) kolorów w analizatorze](/images/cca/cca-wybor-koloru.png)

Po wskazaniu kolorów, które chcemy zbadać, w sekcji *Sample preview* (Podgląd przykładu, 4) wyświetlany jest przykładowy tekst na wybranym tle oraz przykładowa grafika (ikona). Za pomocą pierwszej ikony poniżej pola ze wskazanym kolorem pierwszego planu wskazane kolory można przełączyć i podejrzeć efekt inwersji.

![Fragment okna programu z wynikami testu](/images/cca/cca-wynik.png)

Poniżej sekcji z podglądem próbki w trzech rozwijanych panelach wyświetlany jest wyliczony współczynnik kontrastu oraz jego dla kryteriów sukcesu WCAG (5):

- 1.4.3 Kontrast (minimalny) (AA)
- 1.4.6 Kontrast (rozszerzony) AAA
- 1.4.11 Kontrast elementów nietekstowych (AA)

Wynik oznaczony ikoną zielonej fiszki i słowem 'Pass' oznacza spełnienie wymogu WCAG. Wynik oznaczony ikoną z krzyżykiem na czerwonym tle i słowem 'Fail' wskazuje, że wymóg WCAG nie jest spełniony.

Rozwinięcie panelu z oceną odsłania parafrazę tekstu ocenianego kryterium sukcesu WCAG (6).  
Wynik każdego testu można skopiować do schowka, a następnie wkleić do dokumentacji z przeprowadzonego badania.

### Dobór kolorów

![Definiowanie własnych kolorów](/images/cca/cca-dobor-kolorow.png)


### Symulator ślepoty barw
CCA umożliwia również analizę badanych zestawów barw za pomocą symulatora ślepoty barw. Symulator można włączyć, wybierając z menu opcję *Viev -> Colour blidness simulation* albo korzystając ze skrótu klawiaturowego Ctrl+B (w Windows).
 

![Analizator kontrastu kolorów z otwartym oknem symulacji ślepoty kolorów (Windows)](/images/cca/symulacja-slepoty-barw.png)


W starszej wersji CCA istniała pożyteczna funkcja powiększonego podglądu wybranych elementów z równoczesnym zastosowaniem filtrów symulujących zaburzenia widzenia barw. Poniższy zrzut ekranu ilustruje, jak zawodnym sposobem wyróżnienia łączy jest użycie koloru zamiast podkreślenia lub innego niż tylko kolor wyróżnienia. Niepogrubione łącza widziane w skali szarości nie odróżniają się od otaczającego je tekstu.  

![Powiększony podgląd  wybranego fragmentu strony w starszej wersji programu (Windows)](/images/cca/ccs-symulator-zdjecie.png)




