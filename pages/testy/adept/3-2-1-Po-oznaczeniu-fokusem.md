---
title: 3-1-2 Język części


sidebar: testy_sidebar
permalink: 3-2-1-Po-oznaczeniu-fokusem
folder: testy/adept
---
## 3-2-1 Po oznaczeniu fokusem
1. Czy serwis zachowuje się w sposób przewidywalny dla niepełnosprawnego użytkownika w momencie oznaczenia każdego elementu fokusem?

## Wyjaśnienie
Niepełnosprawny użytkownik może mieć ograniczony dostęp do całości informacji. Na przykład osoba słabowidząca widzi tylko powiększony fragment strony i może nie zauważyć zmiany dokonującej się w innej części. Podobny problem mają osoby niewidome oraz mające problemy z rozumieniem działania serwisu. Dlatego serwis nie powinien zaskakiwać użytkownika zmianą kontekstu informacji w momencie, gdy na element zostanie przeniesiony fokus. Fokus, czyli punkt zainteresowania obwiedziony ramką, może być przenoszony za pomocą klawiatury lub w inny sposób (myszką, dotykiem). Użytkownik zaś nie wykonał jeszcze żadnej akcji (zaznaczenia pola, kliknięcia, wpisania tekstu). Zmianą kontekstu są na przykład następujące sytuacje:
-	przejście na inną stronę,
-	otwarcie zewnętrznej aplikacji, na przykład odtwarzacza,
-	istotna zmiana treści wyświetlanej na stronie,
-	przeniesienie fokusa w inne miejsce.
## Testowanie
Najbardziej podatnymi na tego typu błędy są formularze do wprowadzania danych i system nawigacyjny. Przyjrzyj się im korzystając z klawiatury i sprawdź, jak się zachowują. Jednym z częściej popełnianych błędów są rozwijane listy, w których użytkownik ma za zadanie kliknąć konkretny element, czyli umieścić na nim fokus. Już w momencie umieszczenia fokusa strona się przeładowuje i zmienia język wyświetlanego tekstu lub opis produktu. Tymczasem użytkownik posługujący się klawiaturą musi przesuwać fokus po kolei przez poszczególne elementy listy i strona zmienia treść wielokrotnie, bez jego woli. Innym tego typu błędem jest uruchamianie odtwarzania lub pobierania pliku w momencie, gdy znajdzie się na nim fokus. Za tego typu zachowania odpowiadają akcje typu onFocus i onBlur, które możesz znaleźć w kodzie strony internetowej.
