---
title: 3-2-2 Podczas wprowadzania danych


sidebar: testy-adept_sidebar
permalink: 3-2-2_Podczas-wprowadzania-danych
folder: testy-adept
---

## Test

**Czy serwis zachowuje się w sposób przewidywalny dla niepełnosprawnego użytkownika w momencie wprowadzania danych?**

## Wyjaśnienie
Niepełnosprawny użytkownik może mieć ograniczony dostęp do całości informacji. Na przykład osoba słabowidząca widzi tylko powiększony fragment strony i może nie zauważyć zmiany dokonującej się w innej części. Podobny problem mają osoby niewidome oraz mające problemy z rozumieniem działania serwisu. Dlatego serwis nie powinien zaskakiwać użytkownika zmianą kontekstu informacji w momencie, gdy użytkownik wprowadza w nim dane. Wprowadzanie danych oznacza zaznaczanie pól wyboru (checkbox), wybieranie z opcji lub list wyboru, wpisywanie tekstu oraz w każdy inny sposób, na przykład głosem. Zmianą kontekstu są na przykład następujące sytuacje:
-	przejście na inną stronę,
-	otwarcie zewnętrznej aplikacji, na przykład odtwarzacza,
-	istotna zmiana treści wyświetlanej na stronie,
-	przeniesienie fokusa w inne miejsce.

## Testowanie
Najbardziej podatnymi na tego typu błędy są formularze do wprowadzania danych. Przyjrzyj się im korzystając z klawiatury i sprawdź, jak się zachowują. Możesz zaznaczać pola wyboru, pola opcji, wpisywać tekst i wykonywać inne czynności, najlepiej naprzemiennie za pomocą klawiatury i myszki. Błędy mogą się objawiać wyskakującymi oknami, przeładowywaniem strony, zmianami w treści bez przeładowywania (Ajax), uruchamianiem odtwarzacza i w podobny sposób. Natomiast działania takie mogą być realizowane po naciśnięciu przycisku. Za tego typu zachowania odpowiadają akcje typu onChange, które możesz znaleźć w kodzie strony internetowej.
