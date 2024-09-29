---
title: Identyfikacja błędów i sugestie korekty

sidebar: testy_sidebar
permalink: H5-02-formularze-bledy
folder: testy/jbt
---


# Identyfikacja błędów i sugestie korekty

### Metoda badania:
Testy ręczne – niewypełnianie pól wymaganych, podawanie danych w formacie niezgodnym z wymaganym, testy z czytnikiem ekranu lub użytkownika z niepełnosprawnością wzrokową  

### Zastosowanie:
Wszystkie komponenty formularzy zbierające dane oznaczone jako wymagane oraz pola z  określonym formatem danych

## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwanie:
Kryteria sukcesu: [3.3.1 Identyfikacja błędu](https://wcag.lepszyweb.pl/#error-identification), [3.3.3 Sugestie korekty błędów](https://wcag.lepszyweb.pl/#error-suggestion), [3.3.4 Zapobieganie błędom (kontekst prawny, finansowy, związany z podawaniem danych)](https://wcag.lepszyweb.pl/#error-prevention-legal-financial-data)
-	Każdy komunikat o błędzie dokładnie opisuje błąd i wskazuje, jak go usunąć.
-	Komunikaty o błędach są łatwo wykrywalne przez wszystkich użytkowników. Możliwe sposoby prezentacji:
    - komunikat o błędzie jest wyświetlany w wyskakującym oknie dialogowym,
    - komunikat o błędzie jest wyświetlany bezpośrednio obok pola błędu ORAZ:
      - Jest powiązany z polem jako część etykiety za pomocą atrybutu `aria-labelledby` lub `aria-describedby` ALBO
      - Jest częścią obszaru z treścią dynamiczną (`aria-live`) i ogłaszaną jako *alert*.
    - Komunikat o błędach prezentowany jest na liście błędów, a fokus klawiatury umieszczany jest tuż przed początkiem listy umieszczonej nad formularzem.
-	Jeśli w polach formularza wprowadzane są dane, które skutkują podjęciem przez użytkownika zobowiązań prawnych lub finansowych albo dotyczą ważnych danych osobowych, wówczas:
    - **Odwracalność**: Wprowadzenie danych jest odwracalne lub
    - **Sprawdzanie**: Dane są sprawdzane pod kątem błędów, a użytkownik ma możliwość poprawienia ewentualnych błędów lub
    - **Potwierdzenie**: Istnieje mechanizm, umożliwiający użytkownikowi sprawdzenie, skorygowanie i potwierdzenie poprawności danych przed ich ostatecznym przesłaniem.

### Procedura testowania:
1.	Wprowadzaj nieprawidłowe wartości w polach zbierających dane, aby uruchomić automatyczne wykrywanie błędów, które powodują powiadomienia o błędach, np.:
    - pomiń wpisywanie danych w polach oznaczonych jako wymagane,
    - w polach daty użyj innego format, niż oczekiwany,
    - w polach e-mail wpisuj adresy bez wymaganego znaku @,
    - w polach przeznaczonych na hasło wpisuj hasła nie spełniające warunków podanych w instrukcji.
2.	Sprawdź, czy wykryte zostały wszystkie przypadki niepoprawnie wprowadzonych danych lub braku danych w polach wymaganych.
3.	Sprawdź, czy:
    - Użytkownik jest informowany o błędzie (albo natychmiast po opuszczeniu błędnie wypełnionego pola, albo przy próbie przesłania formularza) ORAZ
    - błąd jest opisany tekstem, ORAZ
    - pole z błędem jest wyróżnione.
4.	Sprawdź, czy komunikaty o błędach zapewniają dodatkowe wskazówki, jak poprawić błędy, lub przykłady.   

### Zasoby

#### Pomocne narzędzia:

#### Techniki WCAG 2.1

**Identyfikacja błędów**

**Techniki wystarczające** dla kryterium sukcesu 3.3.1**

- **Sytuacja A**: Jeżeli formularz zawiera pola, w których informacje od użytkownika są wymagane.
  - [G83: Zapewnienie opisów tekstowych wskazujących wymagane pola, które nie zostały wypełnione](https://www.w3.org/WAI/WCAG22/Techniques/general/)
  - [ARIA21: Użycie atrybutu aria-invalid do wskazania pola z błędem](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA21)
  - [SCR18: Zapewnienie sprawdzania poprawności i alertu po stronie klienta](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR18)
  - [PDF5: Wskazanie wymaganych kontrolek formularzy w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF5)
- **Sytuacja B**: Jeżeli informacje dostarczone przez użytkownika muszą być w określonym formacie danych lub mieć określone wartości.
  - [ARIA18: Użycie atrybutu aria-alertdialog do identyfikacji błędów](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA18)
  - [ARIA19: Użycie atrybutu role=alert lub role=live do identyfikacji błędów](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA19)
  - [ARIA21: Użycie atrybutu aria-invalid do wskazania pola z błędem](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA21)
  - [G84: Zapewnienie komunikatu tekstowego, gdy użytkownik podaje informacje, które nie znajdują się na liście dozwolonych wartości](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [G85: Zapewnienie komunikatu tekstowego, gdy dane wprowadzane przez użytkownika nie mieszczą się w wymaganym formacie lub zakresie wartości](https://www.w3.org/WAI/WCAG22/Techniques/general/G85)
  - [SCR18: Zapewnienie sprawdzania poprawności i alertu po stronie klienta](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR18)
  - [SCR32: Zapewnienie sprawdzania poprawności po stronie klienta i dodawania tekstu błędu przez DOM](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR32)
  - [PDF22: Wskazywanie, kiedy dane wprowadzone przez użytkownika nie mieszczą się w wymaganym formacie lub wartościach w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF22)

**Techniki pomocnicze** dla kryterium sukcesu 3.3.1
- [G139: Zapewnienie mechanizmu, który umożliwia użytkownikom przechodzenie do błędów](https://www.w3.org/WAI/WCAG22/Techniques/general/G139)
- [G199: Zapewnienie komunikatu o powodzeniu po pomyślnym przesłaniu danych](https://www.w3.org/WAI/WCAG22/Techniques/general/G199)

**Sugestie korekty błędów**

**Techniki wystarczające** dla kryterium sukcesu 3.3.3**

- **Sytuacja A**: Jeżeli obowiązkowe pole nie zawiera żadnych informacji:
  - [G83: Zapewnienie opisów tekstowych wskazujących wymagane pola, które nie zostały wypełnione](https://www.w3.org/WAI/WCAG22/Techniques/general/G83)
  - [ARIA2: Identyfikacja wymaganych pól za pomocą właściwości aria-required](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA2)
  - [PDF5: Wskazanie wymaganych kontrolek formularzy w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF5)
- **Sytuacja B**: Jeżeli informacje w danym polu muszą być w określonym formacie danych:
  - [ARIA18: Użycie atrybutu aria-alertdialog do identyfikacji błędów](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA18)
  - [G85: Zapewnienie komunikatu tekstowego, gdy dane wprowadzane przez użytkownika nie mieszczą się w wymaganym formacie lub zakresie wartości](https://www.w3.org/WAI/WCAG22/Techniques/general/G85)
  - [G177: Zapewnienie tekstu sugerującego korektę](https://www.w3.org/WAI/WCAG22/Techniques/general/G177)
  - [SCR18: Zapewnienie sprawdzania poprawności i alertu po stronie klienta](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR18)
  - [SCR32: Zapewnienie sprawdzania poprawności po stronie klienta i dodawania tekstu błędu przez DOM](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR32)
  - [PDF22: Wskazywanie, kiedy dane wprowadzone przez użytkownika nie mieszczą się w wymaganym formacie lub wartościach w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF22)
- **Sytuacja C**: Informacje dostarczane przez użytkownika muszą być jednym z ograniczonych zestawów wartości:
  - [ARIA18: Użycie atrybutu aria-alertdialog do identyfikacji błędów](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA18)
  - [G84: Zapewnienie komunikatu tekstowego, gdy użytkownik podaje informacje, które nie znajdują się na liście dozwolonych wartości](https://www.w3.org/WAI/WCAG22/Techniques/general/G84)
  - [G177: Zapewnienie tekstu sugerującego korektę](https://www.w3.org/WAI/WCAG22/Techniques/general/G177)
  - [SCR18: Zapewnienie sprawdzania poprawności i alertu po stronie klienta](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR18)
  - [SCR32: Zapewnienie sprawdzania poprawności po stronie klienta i dodawania tekstu błędu przez](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR32)
  - [PDF22: Wskazywanie, kiedy dane wprowadzone przez użytkownika nie mieszczą się w wymaganym formacie lub wartościach w formularzach PDF](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF22)
  
**Techniki pomocnicze** dla kryterium sukcesu 3.3.3

- [G139: Zapewnienie mechanizmu, który umożliwia użytkownikom przechodzenie do błędów](https://www.w3.org/WAI/WCAG22/Techniques/general/G139)
- [G199: Zapewnienie komunikatu o powodzeniu po pomyślnym przesłaniu danych](https://www.w3.org/WAI/WCAG22/Techniques/general/G199)











_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_
