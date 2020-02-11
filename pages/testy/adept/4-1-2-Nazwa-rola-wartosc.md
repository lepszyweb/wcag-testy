---
title: 4-1-2 Nazwa, rola, wartość


sidebar: testy_sidebar
permalink: 4-1-2-Nazwa-rola-wartosc
folder: testy/adept
---

## Test
**Czy wszystkie elementy interfejsu mają określoną nazwę i rolę, a wartość jest dostępna dla technologii asystujących?**

## Wyjaśnienie
To kryterium sukcesu ma charakter bardzo techniczny i odnosi się do semantyki interfejsu użytkownika.
Nazwa - każdy element interfejsu powinien mieć indywidualną, unikalną nazwę (identyfikator), po którym można odróżnić poszczególne elementy. W ten sposób technologie asystujące mogą lepiej komunikować użytkownika z interfejsem.
Rola - każdy element interfejsu powinien mieć zdefiniowaną rolę, jaką pełni w interfejsie. Takimi rolami mogą być przycisk, link, tabela, menu, pole edycyjne itd. Język HTML i pochodne mają zestaw gotowych kontrolek, które zastosowane zgodnie z ich przeznaczeniem przyjmują automatycznie odpowiednią rolę. Jeżeli jednak elementy są stosowane niezgodnie z ich przeznaczeniem lub programista tworzy własne rozwiązania, to takie role należy przypisać, stosując role ARIA.
Wartość - każdy element interfejsu powinien być zaprojektowany w sposób, który będzie umożliwiał odczytanie jego wartości oraz zmianę. Odczyt i zmiana mogą być dokonywane przez użytkownika lub program. Wartością dla pola wyboru (checkbox) jest stan „zaznaczone” lub „niezaznaczone”. Wartością pola tekstowego jest tekst doń wpisany.

## Testowanie
Najprostszym sposobem na sprawdzenie spełnienia tego kryterium sukcesu jest użycie bezpłatnego programu odczytu ekranu NVDA. Za jego pomocą możesz przeglądać stronę, wypełniać formularze, nawigować. Jednoczesna obserwacja interfejsu i odsłuchiwanie komunikatów generowanych mową syntetyczną pozwoli na wychwycenie niezgodności. Na przykład gdy na stronie wyświetlany jest przycisk, a NVDA informuje, że jest to link, to oznacza niezgodność roli. Gdy za pomocą NVDA nie da się odczytać zawartości pola edycyjnego lub niczego do niego wpisać - oznacza to problemy z odczytem i zapisem wartości.
CZAS
