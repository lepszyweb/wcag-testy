---
title: 2-1-2 Brak pułapki na klawiaturę


sidebar: testy-adept_sidebar
permalink: 2-1-2_Brak-pulapki-na-klawiature
folder: testy-adept
---

## Test
**Czy fokus przemieszczany za pomocą klawiatury można zawsze wyprowadzić z miejsca, do którego został wprowadzony?**

## Wyjaśnienie
Użytkownicy korzystający z serwisu internetowego za pomocą klawiatury mogą przemieszczać fokus klawiatury w różne miejsca. Bywa jednak, że skrypt lub nietypowa konstrukcja elementu interfejsu spowoduje, że fokusa nie da się z któregoś miejsca przenieść. Innymi słowy - fokus może być uwięziony przez pole edycyjne, element menu lub zagnieżdżony obiekt. Jest to poważne naruszenie zasad dostępności, bo użytkownik nie ma możliwości, by kliknąć myszą w innym miejscu i w ten sposób przemieścić fokus. Standardowe kontrolki HTML nie generują tego typu problemów.

## Testowanie
Sprawdzenie polega na korzystaniu z serwisu wyłącznie za pomocą klawiatury i przemieszczaniu fokusa na różne elementy. Szczególnie uważnie trzeba przyjrzeć się formularzom, a jeszcze uważniej - polom edycyjnym. Właśnie w takich elementach najczęściej grzęźnie fokus klawiatury, ponieważ wewnątrz mogą być realizowane skrypty wykonujące zadania w czasie rzeczywistym. Jeżeli odnajdziesz takie miejsca - serwis nie spełnia tego kryterium dostępności.
