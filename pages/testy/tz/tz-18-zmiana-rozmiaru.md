---
title: 18. Zmiana rozmiaru


sidebar: testy_sidebar
permalink: tz-18-zmiana-rozmiaru
folder: testy/tz
---

## Cel procedury testowej

Celem tej procedury jest sprawdzenie, czy cały tekst może zostać powiększony o co najmniej 200% oryginalnego rozmiaru bez utraty treści lub funkcjonalności, aby użytkownicy mogli czytać treść strony bez konieczności korzystania z dodatkowej technologii wspomagającej, takiej jak ekran lupa. 
Pomaga to osobom z ograniczeniami wzroku, pozwalając im zwiększyć rozmiar tekstu w treści, aby mogli łatwiej go czytać.

Procedura testowa Zmiana rozmiaru obejmuje jeden test:
- Test 18.A 1.4.4-zmiana-rozmiaru-tekstu


### Test 18.A 1.4.4-zmiana-rozmiaru-tekstu

| Nazwa testu | ID testu | Wymaganie testowe |
|------------------------|---------|------------------------------------------|
| 1.4.4-zmiana-rozmiaru-tekstu | 18.A    | Istnieje mechanizm zmiany rozmiaru, skali lub powiększania tekstu do co najmniej 200% jego pierwotnego rozmiaru bez utraty treści lub funkcjonalności. |

### Cel testu 
Ten test weryfikuje, czy istnieje mechanizm zmiany rozmiaru, skalowania lub powiększania tekstu do co najmniej 200% jego pierwotnego rozmiaru bez utraty zawartości lub funkcjonalności. Gdy strona zoostanie przzeskalowana do co najmniej 200%, użytkownik musi nadal mieć dostęp do całej treści i funkcjonalności strony, a tekst nie może być obcięty, zasłonięty, lub trudny do odczytania ze względu na efekty wywołane powiększeniem. 

Mechanizm zapewniający skalowalność można zwykle znaleźć w samej przeglądarce, korzystając z wbudowanej funkcji powiększania. 

Gdy ta funkcja nie istnieje lub nie można na niej polegać, aby powiększyć konkretną treść, programista może wdrożyć alternatywną metodę skalowania całego tekstu, na przykład przycisk „Zwiększ rozmiar tekstu”

Wyniki tego testu służą do ustalenia, czy spełnione jest [kryterium sukcesu WCAG 1-4-4 Zmiana rozmiaru tekstu](https://wcag.lepszyweb.pl/#resize-text).

### Metody i narzędzia testowe 
1.	Mechanizm powiększenia (przeglądarka lub inny mechanizm na stronie internetowej).
2.	Ręczna kontrola strony.

### Identyfikacja treści

Cały tekst na stronie, w tym tekst transkrypcji, w modalnych oknch dialogowych lub innych powiązanych dokumentach.

**Z wyłączeniem**: napisów dla mediów zsynchronizowanych oraz obrazów tekstu.

### Zastosowanie

Test 18.A 1.4.4-zmiana-rozmiaru-tekstu **nie ma zastosowania**, jeśli na stronie nie ma tekstu.

### Jak testować:

1.  Użyj wbudowanych funkcji powiększania przeglądarki, aby zmienić rozmiar tekstu do co najmniej 200%.

2.  Jeśli którakolwiek z treści nie powiększyła się przy użyciu wbudowanych funkcji przeglądarki, sprawdź, czy istnieje mechanizm inny niż technologia wspomagająca do zmiany rozmiaru zawartości strony do 200% jej pierwotnego rozmiaru, np. mechanizm systemu operacyjnego, platformy lub inny mechanizm zapewniony bezpośrednio przez stronę internetową / aplikację.

### Ocena wyników

Jeśli wszystkie twierdzenia poniżej są **prawdą**, wówczas strona (treść) **spełnia** wymaganie testowe, jest **zgodna** z&nbsp;KS 1.4.4:

1.  Istnieje mechanizm niezależny od technologii wspomagającej, który pozwala użytkownikowi zmieniać rozmiar tekstu do co najmniej 200% jego oryginalnego rozmiaru **oraz**

2.  Tekst nie jest skracany, obcinany ani zasłaniany, **oraz**

3.  Istnieją wszytskie funkcjonalności, **oraz**

4.  Istnieje cała treść.

**Uwaga**: Ważne jest sprawdzenie, czy cała treść jest czytelna i funkcjonalna po przeskalowaniu do co najmniej 200%.

## Obowiązujące normy

- {% include ks/1-4-4.md %}
- [22. Zmiana rozmiaru tekstu](ICT-22-zmiana-rozmiaru-tekstu.md)                                                                                              
