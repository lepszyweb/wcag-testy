---
title: 2-4-3 Kolejność fokusa


sidebar: testy_sidebar
permalink: 2-4-3_Kolejnosc-fokusa
folder: testy/adept
---

## Test
**Czy fokus przemieszczany za pomocą klawiatury przemieszcza się w zaplanowanej i logicznej kolejności?**

## Wyjaśnienie
Użytkownicy korzystający z klawiatury do obsługi serwisu internetowego przesuwają fokus za pomocą klawisza Tab. Często kolejność elementów, na których umieszczany jest fokus, jest ważna lub wręcz kluczowa. Bywa przy tym, że projektant przygotował serwis tylko pod kątem wyglądu, a nie semantyki. Jeżeli wyświetlane jest okno dialogowe do logowania, to oczekujemy odpowiedniej kolejności fokusa: pole tekstowe nazwy użytkownika, pole tekstowe hasła, pole wyboru do zapamiętania hasła i wreszcie przycisk do zalogowania. Oczekujemy także, że kursor będzie przemieszczany po kolei po elementach menu nawigacyjnego, a nie w losowej kolejności.

## Testowanie
Sprawdzenie tego warunku wymaga posługiwania się serwisem internetowym za pomocą klawiatury (bez użycia myszy) z jednoczesną obserwacją miejsca, w którym znajduje się fokus. Jeżeli zauważysz, że fokus pojawia się w innym miejscu, niż byś się spodziewał, to znaczy że warunek dostępności nie jest spełniony. Ze szczególną starannością sprawdź formularze służące do wprowadzania danych oraz system nawigacji serwisu internetowego.