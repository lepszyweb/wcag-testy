---
title: Metody oceniania dostępności
summary: "Na całym świecie specjaliści stosują różne podejścia do oceniania dostępności i wciąż podejmują nowe próby zdefiniowania skutecznych i efektywnych procedur testowania."

sidebar: metoda_sidebar
permalink: met-wprowadzenie
folder: metoda
toc: false
---

## Dostępna nazwa
### Wymaganie
Wszystkie interaktywne elementy muszą mieć dostępną nazwę

### Kogo może to dotyczyć

- Użytkownicy czytników ekranu
- Użytkownicy sterujący głosem

### Opis

Technologie wspomagające, takie jak czytniki ekranu i sterowanie głosowe, odczytują lub wyświetlają użytkownikowi etykietę elementu, aby mógł zrozumieć przeznaczenie elementu i przewidzieć wynik interakcji z nim.
Dlatego każdy interaktywny element interfejsu użytkownika (np. etykieta, przycisk, łącze, dane wejściowe itp.) musi mieć zdefiniowaną dostępną nazwę. Oprócz elementów interaktywnych elementy nietekstowe (np. obrazy i elementy graficzne), które są częścią treści lub są niezbędne do jej zrozumienia, wymagają również dostępnych etykiet. Dostępna nazwa powinna być na tyle znacząca i opisowa, aby w pełni spełniała swoje zadanie, a także unikalna, by użytkownik wiedział, z jakim elementem wchodzi w interakcję.

### Co zrobić
Ustaw etykietę dostępności dla każdego interaktywnego elementu
#### iOS (SwiftUI):
```
Button{
// Akcja przycisku
}:{
Image("checkmark")
}
.accessibilityLabel("Potwierdź")
Button{
// Akcja przycisku
}:{
Image("checkmark")
}
```

#### Android (.xml):
```
<Button
      android:id="@+id/btnBuy"
      android:text="Kup teraz"
      android:contentDescription="Kup teraz"
      .../>
<Button
      android:id="@+id/btnBuy"
      android:text="Kup teraz"
    .../>
```

#### Android (Kotlin):
```
.=getString(R..)
```

#### Android (Java):
```
.setContentDescription(getString(R..))
```

#### React Native:
```
<Button
      title="Kup teraz"
      color="#841584"
      accessibilityLabel="Kup teraz"
    />
<Button
      title="Kup teraz"
      color="#841584"
    />
```

**Uwaga**: Na niektórych platformach (np. iOS) widok musi być zarejestrowany w drzewie dostępności, aby można było przypisać mu dostępną etykietę, w przeciwnym razie zostanie zignorowana przez technologie wspomagające.
**Uwaga**: Unikaj używania w etykiecie widoku zwrotów takich jak „przycisk”, „pole edycji” lub link – tego typu informacje powinny być zdefiniowane w semantyce elementu.

### Jak to wpływa na użytkowników
Dostępna nazwa jest używana przez technologie wspomagające do oznaczania, ogłaszania i wywoływania działań interaktywnych elementów interfejsu użytkownika (np. przycisków, łączy, pól wejściowych itp.). Gdy elementy interaktywne nie mają prawidłowej dostępnej nazwy, technologiom wspomagającym brakuje zaczepu, którego mają używać.
#### Użytkownicy czytników ekranu
Jeśli interaktywny element UI nie ma dostępnej etykiety, VoiceOver ogłosi go ogólnie według jego typu (np. przycisk, łącze itp.); ten brak kontekstu może utrudnić, a nawet uniemożliwić użytkownikom czytników ekranu zrozumienie i korzystanie z niego. 
#### Użytkownicy sterujący głosem
VoiceControl wykorzystuje dostępne etykiety jako „zaczepy głosowe”, z którymi użytkownik może wchodzić w interakcje. Na poniższej ilustracji szare etykiety narzędzi to dostępne nazwy, które zostały wykryte przez VoiceControl. Widać, że przycisk, który nie ma dostępnej nazwy, jest oznaczony znakiem zapytania i nie ma wyraźnego zaczepu do interakcji głosowej.
 
Rysunek 1. przykład tego, jak sterowanie głosowe oznacza przyciski z dostępną nazwą i bez niej
### Kryteria sukcesu WCAG
Ten problem może spowodować, że elementy nie spełnią jednego lub więcej z następujących kryteriów sukcesu:
- KS 1.3.1. Informacje i relacje (A): Informacje, struktura oraz relacje między treściami przekazywane poprzez prezentację mogą być odczytane przez program komputerowy lub istnieją w postaci tekstu.
- KS 2.4.6 Nagłówki i etykiety (AA): Nagłówki i etykiety opisują temat lub cel treści.
- KS 4.1.2 Nazwa, rola, wartość (A): Dla wszystkich komponentów interfejsu użytkownika nazwa oraz rola (przeznaczenie) mogą być odczytane przez program komputerowy, a stan, właściwości oraz wartości, które mogą być ustawione przez użytkownika, mogą również być ustawione przez program komputerowy; powiadomienie o zmianach w tych elementach dostępne jest dla programów użytkownika, w tym technologii wspomagających.

### Zalecane lektury
- Dostępne nazwy. Baza wiedz Evinced
- Accessible Name and Description Computation 1.1. Rekomendacja W3C




## Cel i struktura repozytorium
Celem tej części repozytorium jest zbudowanie bazy podejść do oceny dostępności i dobrych praktyk postulowanych w różnych metodologiach, poradnikach, przewodnikach. Znaleźć je można zarówno w kompletnych opracowaniach, jak i różnych przyczynkach.

Materiały w tej części repozytorium będą się koncentrować wobec trzech głównych kwestii:
- koncepcje oceniania dostępności,
- procedury oceniania dostępności,
- metodyki oceniania dostępności.

## Jak możesz pomóc?
- Opisz znaną Ci koncepcję oceniania dostępności
- Przetłumacz wybrany fragment [WCAG-EM 1.0](https://www.w3.org/TR/WCAG-EM/)
- Podziel się własnym opracowaniem wybranego problemu oceniania dostępności
- Zgłoś sugestie, uwagi, poprawki do opublikowanych materiałów

Zobacz artykuł [Zaangażuj się](zaangazuj-sie), aby dowiedzieć się więcej.

## Licencja
- Wszystkie materiały autorskie publikowane są na warunkach licencji CC BY-NC-SA 4.0
[Uznanie autorstwa-Użycie niekomercyjne-Na tych samych warunkach 4.0 Międzynarodowe](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pl)
- w przypadku materiałów tłumaczonych obowiązują licencje, na jakich zostały udostępnione oryginały.
