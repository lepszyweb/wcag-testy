---
title: 3-1-2 Język części


sidebar: testy-adept_sidebar
permalink: 3-1-2_Jezyk-czesci
folder: testy-adept
---

## Test
**Czy fragmenty tekstu w języku innym niż podstawowy na stronie są prawidłowo zadeklarowane?**

## Wyjaśnienie
W serwisie internetowym tekst pisany jest w konkretnym języku, na przykład po polsku. Jednak mogą się w nim znaleźć fragmenty w innych językach, na przykład po angielsku lub niemiecku. Takie fragmenty powinny mieć deklarację języka, podobnie jak cała strona. Dzięki temu syntezatory mowy będą w stanie samoczynnie przełączyć się na właściwy język.

## Testowanie
Przejrzyj serwis internetowy pod kątem pojawiania się w nim fragmentów w języku innym, niż podstawowy. Możesz sprawdzić w kodzie źródłowym strony, czy taki fragment ma przypisaną deklarację w rodzaju lang="en" (angielski) lub lang="de" (niemiecki). Możesz też użyć bezpłatnego czytnika ekranu NVDA, który w domyślnej konfiguracji przełącza się na inny język syntezy mowy, gdy napotka odpowiednią deklarację.

