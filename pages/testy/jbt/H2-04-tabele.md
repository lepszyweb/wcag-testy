---
title: Tabele

sidebar: testy_sidebar
permalink: H2-04-tabele
folder: testy/jbt
---

# Tabele

### Metoda badania:
Inspekcja kodu, wykorzystanie narzędzia ujawniającego elementy nagłówka i zakres.

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania:
Kryteria sukcesu: [1.3.1 Informacje i relacje](https://wcag.lepszyweb.pl/#info-and-relationships), [1.3.2 Zrozumiała kolejność](https://wcag.lepszyweb.pl/#meaningful-sequence)
-	Tabele są wykorzystywane wyłącznie do prezentacji danych (najlepsza praktyka).
o	Jeśli tabele są używane do rozmieszczania elementów strony (tabele układu, prezentacyjne), wówczas mają ustawiony atrybut ARIA `role="presentation"` (dobra praktyka)
o	W przypadku tabel układu, poprawna jest kolejność odczytu, gdy tabela jest linearyzowana. (wymagane)
-	Tabele danych posiadają podpis umieszczony w znaczniku `caption`.
-	Dane w tabelach są uporządkowane za pomocą nagłówków kolumn i wierszy utworzonych znacznikiem `<th...>`.
-	Gdy w tabeli występuje więcej niż trzy kolumny albo trzy wiersze z nagłówkami, wówczas komórki z nagłówkami kolumn zawierają atrybut `scope="col"`, a kolumny z nagłówkami wierszy atrybut `scope="row"`.
-	Nagłówki tabel są kodowane przy użyciu elementów nagłówków tabel.
-	W złożonych tabelach danych wszystkie komórki nagłówkowe posiadają atrybut identyfikatora z unikalną wartością.
-	W złożonych tabelach danych komórki danych są powiązane z komórką nagłówka za pomocą atrybutu `headers="identyfikator-komórki-nagłówka"`.
-	Kolejność identyfikatorów w znaczniku headers odpowiada kolejności ich występowania w kolumnach lub wierszach nagłówkowych
-	Jeśli na przekątnej znajdują się nagłówki, to nagłówki są identyfikowane w każdej komórce za pomocą atrybutu nagłówków. Wszystkie komórki nagłówka muszą mieć identyfikatory.
-	Tabele układu wykorzystywane są do rozmieszczania treści i nie sugerują żadnych relacji między komórkami (do znakowania komórek nie zostały użyte znaczniki `th` i związane z nimi atrybuty, ani znaczniki `thead`, `tbody`, `tfoot`  

*Uwaga*: Tabele mogą być utworzone również za pomocą atrybutów WAI ARIA. Przedstawiona tutaj  procedura testowania nie uwzględnia takich przypadków.

### Procedura testowania:
1.	Sprawdź, czy każda tabela ma kod, który poprawnie definiuje cała tabelę i jej elementy – podpis, komórki nagłówkowe, komórki danych.  
2.	Sprawdź, czy w tabeli danych do elementu `<table>` NIE został przypisany atrybut ARIA `role="presentation"`. Gdyby tak było, czytniki ekranu nie otrzymają informacji o strukturze tabeli i nie przekażą ich użytkownikowi.
3.	Sprawdź, czy tabela ma dostępną nazwę – podpis określony znacznikiem `<caption>`. Podpis może być ukryty przed użytkownikami przeglądającymi tabelę na ekranie.
4.	Sprawdź, czy w tabelach zawierających więcej niż 3 kolumny nagłówkowe lub trzy wiersze nagłówkowe dodany został do komórek nagłówkowych atrybut scope.
5.	Sprawdź, czy w złożonych tabelach danych (tabele, w których istnieją połączone komórki danych opisujące więcej niż jedną kolumnę lub jeden wiersz powiązanych z nimi danych), komórki nagłówkowe mają unikalne identyfikatory, a komórki danych atrybuty `headers` z identyfikatorami wymienionymi w poprawnej kolejności.
6.	Sprawdź w tabelach prezentacyjnych, czy NIE zastosowano w nich znaczników i atrybutów wskazujących na relacje (znaczniki i atrybuty  komórek nagłówkowych, znacznik `caption`, atrybuty identyfikatorów i powiązań z identyfikatorami – `headers`)      

### Wykorzystanie skryptozkładki ANDI

{% include image.html file="andi/andi-tabela.png" alt="Wykorzystanie skryptozkładki ANDI" %}

1.	Uruchom skryptozakładkę ANDI.
2.	Wybierz z menu ANDI opcję *tables* i zaznacz w menu poziomym opcję *markup*.
3.	Zobacz szczegółową informację o liczbie i typie wykrytych tabel danych i prezentacyjnych. Użyj łącza *View table list*, aby rozwinąć schowaną informację o tabelach. Zapoznaj się z ta informację. W tabelce podana jest nazwa tabeli i sposób jej oznaczenia, jeśli została zdefiniowana  oraz komunikaty odnoszące się do wykrytych usterek w tabelach.   
4.	Posługując się przełącznikiem między wykrytymi tabelami, wybieraj kolejne tabele do oceny.
5.	Posługując się przełącznikami między wykrytymi elementami struktury strony, zbadaj strukturę każdej tabeli według zaleceń powyżej w sekcji Instrukcje.   
6.	W polu informacji o wybranym elemencie tabeli znajdziesz następujące informacje:
    - *Element*: określenie typu elementu (znacznik html użyty do utworzenia elementu)
    - *Accessibility Components*: liczba wykrytych dostępnych komponentów; liczba większa od 0 wskazuje na liczbę komponentów, które posiadają dostępną nazwę
    - opis: podana jest dostępna nazwa i sposób jej oznaczenia albo ostrzeżenie, że nie wykryto komponentów posiadających dostępną nazwę
    - *ANDI Output*: Treść, która zostanie przekazana użytkownikom czytników ekranu. Często także komunikat informujący o wykrytych usterkach.
7.	Obejrzyj informacje widoczne w obszarze analizowanej tabeli. Jeśli włączona została opcja *markup* (2), w obszarze analizowanej tabeli widoczne będą użyte do jej utworzenia znaczniki i atrybuty.           

### Zasoby

#### Pomocne narzędzia:
-	skryptozakładka [tables](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Wstawia znaczniki i atrybuty tabeli danych na żółtym tle, dzięki czemu można łatwo identyfikować błędy dostępności w tabeli.
-	skryptozakładka [Data Tables](https://jimthatcher.com/favelets/) z kolekcji Jima Tatchera. Wyświetla wszystkie wykryte znaczniki tabel - `th`, `summary`, `scope`, `axis`, `id`, i `headers`. Tester może sprawdzić, czy tabela jest wystarczająco oznakowana.
-	skryptozakładka [Complex Tables Favlet](https://labs.levelaccess.com/index.php/Category:Favlet) z kolekcji Level Access. Pobiera powiązaną zawartość komórki nagłówka z każdej komórki, do której odwołuje się atrybut nagłówka, i umieszcza je na ekranie w komórce danych w taki sam sposób, w jaki czytnik ekranu może prezentować nagłówki użytkownikom czytnika ekranu.
-	skryptozakładka [tables](http://pauljadam.com/bookmarklets/index.html) z kolekcji Paula J. Adama. Wstawia znaczniki i atrybuty tabeli danych na żółtym tle, dzięki czemu można łatwo identyfikować błędy dostępności w tabeli.
-	skryptozakładka [Content Structure](https://accessibility-bookmarklets.org/install.html) z kolekcji Pixo i University of Illinois. z kolekcji Pixo i University of Illinois. Autorzy wykorzystali skrypt Inhalte gegliedert, wzbogacając go o rozpoznawanie struktury list, tabel, linków i elementów formularzy.
-	Opcja *tables* w skryptozakładce [ANDI](https://www.ssa.gov/accessibility/andi/help/install.html)

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
