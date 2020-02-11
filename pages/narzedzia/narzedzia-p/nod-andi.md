---
title: ANDI - inspektor dostępnych nazw i opisów
tags: [rozszerzenia_przeglądarek,narzędzia_oceny_dostępności]

sidebar: narzedzia_sidebar
permalink: nod-andi
folder: narzedzia-p
---

Skrót ANDI pochodzi od angielskiego <span lang="en">Accessible Name and Description Inspector</span>, co po polsku oznacza &bdquo;inspektor dostępnych nazw i opisów&rdquo;. Wbrew nazwie, ANDI pomaga przeprowadzić o wiele bogatsze badanie niż tylko sprawdzenie, czy wszystkie obiekty strony mają dostępne nazwy lub opisy.

ANDI jest skryptozakładką, czyli niewielkim skryptem JS, który dodajemy w przeglądarce do zakładek, aby móc swobodnie korzystać z jego funkcjonalności. A są niemałe!

![logo](images/narzedzia/skryptozakladka_andi.png)

ANDI z powodzeniem zastąpi Ci, przynajmniej na pewien czas, eksperta ds. dostępności. Oczywiście, będzie to ekspert z ograniczonymi, ale niemałymi kompetencjami. Na pewno pomoże w dużym stopniu poprawić dostępność Twoich stron. Niezależnie od tego, czy Twoja wiedza na temat dostępności jest duża, czy dopiero stawiasz w dostępności pierwsze kroki, wskazówki, jakich udzieli Ci ANDI spowodują większą dostępność Twojej witryny dla użytkowników.

ANDI jest stosowany z powodzeniem w testach dostępności prowadzonych przez amerykańskie agencje federalne, dla których jest zalecanym narzędziem badania dostępności.  

## Dane zakładki
- **Autor**: Accessible Solutions Branch w Social Security Administration
- **Źródło**: [ANDI - help](https://www.ssa.gov/accessibility/andi/help/install.html)

## Stosowanie
Opis funkcjonalności ANDI znajdziesz w polskiej adaptacji tego narzędzia wykonanej przez naszą Pracownię Dostępności Cyfrowej LepszyWeb.pl: [ANDI po polsku](https://lepszyweb.pl/andi/). Możesz również zapoznać się z oryginalnym podręcznikiem ppod adresem [ANDI - podrecznik oficjalny](https://www.ssa.gov/accessibility/andi/help/howtouse.html). Albo zapoznać się z nią w oryginale.

ANDI dzieli testy na moduły. Przy pierwszym ładowaniu uruchamiany jest moduł domyślny, który analizuje elementy interaktywne, kolejność tabulacji i występowanie klawiszy dostępu. Kolejne moduły umożliwiają analizę elementów graficznych, linków i przycisków, tabel, struktury (nagłówki, listy, punkty orientacyjne, atrybuty ARIA, atrybuty języka), kontrast i elementy ukryte.

Wybierając „moduł” z listy rozwijanej wyboru modułu (2), możesz metodycznie przetestować różne obszary dostępności.

Po wybraniu modułu ANDI ponownie zeskanuje stronę i przedstawi wyniki w zależności od wybranego modułu. Za pomocą selektora elementów (1) możesz odsłaniać szczegółowe wyniki analizy kolejnych elementów. W obszarze analizy elementu (3) znajdziesz m.in. nazwę elementu, rolę, różne komponenty dostępności, przewidywany komunikat czytnika ekranu.

Wyniki testów ANDI przedstawia w sekcji Analiza strony (4). Znajdziesz tu liczbę wykrytych elementów danego typu oraz, jeśli zostaną wykryte jakieś problemy, komunikaty wskazujące wagę problemu (krytyczny, umiarkowany i możliwy). Podkreślmy wyraźnie, nawet w przypadku wskazania błędu krytycznego ostateczna decyzja, czy istnieje problem z dostępnością, zawsze należy do człowieka. ANDI jest jedynie narzędziem kontrolnym sygnalizującym możliwość wystąpienia błędu i jego wagę.
