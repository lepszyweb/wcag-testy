---
title: 2-4-7 Widoczny fokus


sidebar: testy-adept_sidebar
permalink: 2-4-7_Widoczny-fokus
folder: testy-adept
---

## Test
**Czy fokus przemieszczany za pomocą klawiatury jest zawsze widoczny?**

## Wyjaśnienie
Fokus jest miejscem na stronie internetowej, z którym użytkownik może wchodzić w danym momencie w interakcje, na przykład nacisnąć przycisk, kliknąć link, zaznaczyć pole wyboru, czy wpisać tekst. Fokus może być umieszczany na obiekcie za pomocą myszki lub klawiatury, a zazwyczaj jest oznaczany cienką ramką. Taki fokus przemieszczany za pomocą klawiatury musi być zawsze widoczny dla użytkowników, aby wiedzieli, w którym miejscu strony się znajduje. Ukrywanie fokusa czyni go zupełnie bezużytecznym dla osób posługujących się klawiaturą.

## Testowanie
Sprawdź, czy fokus jest zawsze widoczny, gdy przesuwasz go za pomocą klawiatury. Po otwarciu strony naciskaj klawisz Tab i obserwuj przesuwanie się fokusa. Fokus nie może znikać ani też jego widoczność nie może być sztucznie obniżana. Najlepiej, gdy jego widoczność zostanie wzmocniona za pomocą stylów CSS. Po przejściu klawiaturą całej strony kliknij na jakiś link i sprawdź, czy na kolejnej podstronie fokus jest nadal widoczny.