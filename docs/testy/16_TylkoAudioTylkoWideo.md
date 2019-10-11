# 16. Tylko audio i tylko wideo

## Wymagania dostępności
------------------------
-   [KS WCAG: 1.2.1 Tylko audio lub tylko wideo (nagranie)](https://wcag.lepszyweb.pl/#audio-only-and-video-only-prerecorded) -- Dla mediów nagranych w systemie tylko audio lub tylko wideo stosuje się następujące zasady, za wyjątkiem sytuacji, kiedy nagranie audio lub wideo jest alternatywą dla tekstu i w taki sposób jest oznaczone:
    -   **Nagranie tylko audio:** Zapewniona jest alternatywa dla mediów zmiennych w czasie, przedstawiająca tę samą treść, co w nagraniu audio.
    -   **Nagranie tylko wideo:** Zapewniona jest alternatywa dla mediów zmiennych w czasie, albo nagranie audio, przedstawiające te same informacje, jak w nagraniu wideo.

## Uzasadnienie metody badania
------------------------------
Ocena treści alternatywnej w celu oceny jej równoważności z treściami tylko audio lub tylko wideo obejmuje zazwyczaj ręczne, poznawcze porównanie oryginalnej treści z jej alternatywą (lub alternatywami).

## Ograniczenia, założenia lub wyjątki
--------------------------------------
### Tylko audio
-   Jeśli audio jest zsynchronizowane z wideo, slajdami, animacjami lub innymi mediami wizualnymi opartymi na czasie, zamiast tego testu, wykonaj test [17. Media zsynchronizowane.md](17_MediaZsynchronizowane.md)
-   Dźwięk będący alternatywą dla tekstu nie wymaga dodatkowego opisu, jeśli jest wyraźnie oznaczony jako taki.
-   Krótkie dźwięki używane do powiadamiania użytkownika, takie jak sygnały potwierdzające i powiadomienia o błędach, nie są objęte tym wymogiem.
-   Informacje i/lub instrukcje przekazywane wyłącznie w formie treści audio muszą zawierać równoważne wskazówki programowe i/lub tekstowe; sprawdzenie tego wymogu odbywa się zgodnie z [17. Media zsynchronizowane.md](17_MediaZsynchronizowane.md).


### Tylko wideo
-   W prezentacji wyłącznie wideo informacje są przedstawiane na różne sposoby, w tym animację, tekst lub grafikę, otoczenie i tło, działania i ekspresję ludzi, zwierząt itp.
-   Wideo będące alternatywą dla tekstu nie wymaga dodatkowego opisu, jeśli jest wyraźnie oznaczone jako takie.
-   Jeżeli prezentacji wideo towarzyszą dźwięki o określonym czasie trwania lub znaczące dialogi, nie jest to tylko wideo. Odpowiednimi w takim przypadku są testy [17. Media zsynchronizowane.md](17_MediaZsynchronizowane.md) 
-   Treści tylko wideo mogą przedstawiać informacje ruchome, migające, przewijane lub automatycznie aktualizowane. Jednak do pezentacji podobnych treści można zastosować inne metody. W obu przypadkach, niezależnie od tego, czy treść jest prezentowana wyłącznie w formie wideo, czy też w inny sposób, musi istnieć możliwość wstrzymania, zatrzymania lub ukrycia treści. Sprawdzenia tego wymogu dokonuje się zgodnie z [21. Limity czasu.md](21_LimityCzasu.md).

## Procedura testu dla KS Tylko audio (nagranie)
------------------------------------------------
### Identyfikacja treści
Nagrane treści tylko audio.

### Instrukcja testowania
1.  Sprawdź, czy treść zawiera transkrypcję dla treści tylko audio.
2.  Sprawdź, czy transkrypcja jest tekstem (tzn. obraz transkrypcji nie wystarczyłby do zaliczenia tego testu).
3.  Odtwarzaj wyłącznie treści audio.
4.  Sprawdź, czy informacje w transkrypcji są dokładnym i kompletnym przedstawieniem treści tylko audio i zawierają odpowiednie dźwięki oprócz dialogu, takie jak trzaskanie drzwiami, wycie syren, identyfikacja osób wypowiadających kwestie w dialogu itp.

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.2.1  oraz wymaganie podstawowe nr 16 kończy się niepowodzeniem.

## Procedura testu dla KS 1.2.1 Tylko wideo (nagranie)
------------------------------------------------------
### Identyfikacja treści
Nagrane treści tylko wideo.

### Instrukcja testowania
1.  Sprawdź, czy wszystkie informacje o treści tylko do wideo są dostępne za pośrednictwem tekstu alternatywnego (np. tekstu zawierającego opis treści wideo i działań) lub ścieżki dźwiękowej opisującej treść wideo.
2.  Wyświetl tylko treść wideo, odnosząc je jednocześnie do alternatywy.
3.  Sprawdź, czy informacje zawarte w alternatywie zawierają te same informacje, które są wyświetlane w prezentacji tylko wideo (np. jeżeli film wideo zawiera wiele znaków, alternatywna musi określać, który znak jest powiązany z każdą przedstawioną czynnością).

### Wynik testów
Jeżeli którakolwiek z powyższych prób zakończy się niepowodzeniem, wówczas test KS 1.2.1  oraz wymaganie podstawowe nr 16 kończy się niepowodzeniem.

##  Wskazówki dotyczące usprawniania procesu testowego
----------------------------------------------------------
Brak.
### Techniki WCAG 2.1
---------------------
Opracowując tę procedurę testową, wzięto pod uwagę następujące wystarczające techniki i typowe defekty:
-   [G158: Zapewnienie alternatywy dla treści audio w mediach zmiennych w czasie](https://www.w3.org/TR/WCAG20-TECHS/G158.html)
-   [G159: Zapewnienie alternatywy dla treści tylko wideo w mediach zmiennych w czasie](https://www.w3.org/TR/WCAG20-TECHS/G159.html)

----------------------------------------
[Początek/Spis treści](index.md) | [Poprzedni](15_Jezyk.md) | [[Następny]](17_MediaZsynchronizowane.md)
