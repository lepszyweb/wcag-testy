---
title: 3-1-1 Język strony


sidebar: testy_sidebar
permalink: 3-1-1-Jezyk-strony
folder: testy/adept
---

## Test
**Czy każda strona serwisu internetowego ma prawidłowo zadeklarowany język, w którym jest napisana treść?**

## Wyjaśnienie
Każdy tekst na stronach internetowych jest zapisany w jakimś konkretnym języku, na przykład po polsku, angielsku lub chińsku. Nie chodzi tu o języki w rodzaju HTML, XHTML, PHP, czy JavaScript, ale języki ludzkie. Prawidłowa deklaracja jest istotna dla osób niewidomych, których programy odczytu ekranu automatycznie przełączają się pomiędzy językami syntezatorów. Jest ważna także dla programów agregujących treści i automatów tłumaczących, bo mają wtedy precyzyjnie podany język źródłowy.

## Testowanie
Sprawdzenia tego warunku można dokonać na kilka sposobów.
Możesz podejrzeć kod strony i spróbować znaleźć tam następującą deklarację lang="pl", która znajduje się przy znaczniku HTML. W cudzysłowach znajduje się kod języka, w tym wypadku polskiego.
Możesz spróbować przeczytać stronę za pomocą bezpłatnego programu NVDA, który w podstawowej konfiguracji przełącza się pomiędzy językami. To rozwiązanie ma tę wadę, że wymaga wsłuchiwania się w niezrozumiałą dla nie przyzwyczajonej osoby syntezę mowy. Poza tym NVDA pozwala na wykrycie źle zadeklarowanego języka, ale nie pozwala na wykrycie braku deklaracji.
