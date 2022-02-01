## 1.1.1 Treść nietekstowa

**Wszystkie treści nietekstowe prezentowane użytkownikowi mają alternatywę tekstową, która służy równoważnemu celowi.**

### Dlaczego to jest ważne
Wszelkie informacje przekazywane w inny sposób niż tekst muszą być również podane w tekście. Tekst powinien zapewniać równoważne informacje. Przykładami treści nietekstowych są obrazy, wykresy, multimedia, animacje, CAPTCHA i powiadomienia dźwiękowe.

W razie potrzeby można użyć krótkich i długich alternatyw tekstu, aby przekazać odpowiednik treści nietekstowej. Najczęstszą alternatywą w postaci krótkiego tekstu jest użycie atrybutów tekstu ALT dla obrazów. Przykłady długich alternatyw obejmują opisy wykresów, schematów lub złożonych obrazów.

Wyjątki: 

Istnieją sytuacje, w których podanie odpowiednika tekstu nie jest możliwe lub jest  niepożądane. Wyjątki obejmują kontrolki, dane wejściowe, testy i CAPTCHA. 

Treść nietekstowa, która ma przede wszystkim wywołać określone wrażenia zmysłowe, wówczas alternatywy tekstowe powinny co najmniej zawierać opisową identyfikację treści nietekstowej. 

Treści dekoracyjne, służące do formatowania lub wizualnie ukryte nie wymagają alternatywnego tekstu.

Więcej informacji na temat wyjątków, intencji, korzyści i technik można znaleźć w opisie [Objaśnienia 1.1.1 Treści nietekstowe](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html).

## Projektowanie

Poziom 1
- Zidentyfikuj i opisz dekoracyjne obrazy
- Jeśli znaczący obraz można łatwo opisać, podaj tekst alternatywny
- Jeśli obraz jest kontrolką, upewnij się, że alternatywa opisuje cel, a nie obraz
- Podaj zwięzły opis złożonych wizualizacji, a następnie podaj bardziej szczegółowe informacje

Poziom 2

- Podaj krótką nazwę dla ikon bez etykiet tekstowych
- Nadaj filmom tytuł lub krótkie opisy

Poziom 3
- Użyj podpisów rycin (figcaption), aby ulepszyć tekst alternatywny

## Programowanie
- Nadaj dekoracyjnym obrazom atrybut ALT z pustym ciągiem znaków (alt = "")
- Użyj HTML, ARIA lub technik specyficznych dla technologii, aby dodać krótkie alternatywy tekstowe
- Jeśli w interfejsie użytkownika znajduje się odpowiedni tekst, użyj jako odniesienia aria-labelledby i aria-describedby
- Zapewnij dostępną metodę ujawniania alternatywnych długich tekstów
- Test jednostkowy: programiści powinni używać narzędzi weryfikacyjnych

## Testowanie

### Zautomatyzowane
Przetestuj za pomocą rozszerzenia przeglądarki IBM Equal Access Accessibility Checker lub modułu testowania integracji, aby zidentyfikować problemy wykryte dla tego wymagania

### Ręczne
Sprawdź dźwięk, wideo, flashowanie i automatyczne odtwarzanie

### Czytnik ekranu
Sprawdź ALT, etykiety i obce frazy

