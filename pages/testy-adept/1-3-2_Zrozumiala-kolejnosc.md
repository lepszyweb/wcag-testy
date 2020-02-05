---
title: 1-3-2 Zrozumiała kolejność


sidebar: testy-adept_sidebar
permalink: 1-3-2_Zrozumiala-kolejnosc
folder: testy-adept
---

## Test
**Czy treści publikowane w serwisie oraz system nawigacji mają prawidłowo zaprogramowaną kolejność odczytu?**

## Wyjaśnienie
Projektowanie serwisów internetowych odbywa się często przez układanie elementów interfejsu na siatce układu strony, bez brania pod uwagę struktury informacji. Powoduje to czasem, że informacja może być odczytywana w nieprawidłowej kolejności, innej niż sobie to zaplanował projektant. Kolejność odczytu informacji jest szczególnie istotna dla osób posługujących się klawiaturą, w tym osób niewidomych. Baczną uwagę należy zwrócić też na skomplikowane układy graficzne, na przykład kilkukolumnowe, zawierające ramki i podobne rozwiązania. Zaprogramowana kolejność odczytu, wynikająca z drzewa dokumentu (DOM) powinna być zgodna z prezentacją wizualną.

## Testowanie
Kolejność odczytu możesz sprawdzić na dwa sposoby:
Za pomocą bezpłatnego czytnika ekranu NVDA. Tworzy on na podstawie DOM strony specjalny bufor z informacjami, które prezentuje użytkownikowi za pomocą mowy syntetycznej. Przejrzyj za pomocą NVDA serwis internetowy i sprawdź, czy kolejność odczytu tą metodą zgadza się z tym, czego byś oczekiwał widząc serwis.
Możesz też wykorzystać narzędzie wspomagające WAVE Toolbar, w którym wybierz narzędzie Structure/Order. Przy każdym elemencie pojawi się teraz liczba określająca kolejność odczytu, dzięki czemu możesz się upewnić, czy kolejność ta jest prawidłowa.
WAVE - narzędzie do walidacji i prezentacji
