---
title: Poziom 6


sidebar: testy_sidebar
datatable: true
permalink: MSU_01_poziom_6
folder: testy/msu
---


## Poziom 6 

| Test        | Protokoły                    |OK|Źle|ND| Uwagi  |KS WCAG|
|-------------|------------------------------|--|---|--|--------|--------|
|1. Walidacja kodu|Uruchom każdą stronę poprzez walidatory HTML (https://validator.w3.org/nu/) i CSS (https://jigsaw.w3.org/css-validator/) i upewnij się, że nie znaleziono żadnych błędów. | | | | |[4.1.1](https://wcag.lepszyweb.pl/#parsing)|
|2. Język strony|Upewnij się, że HTML wskazuje naturalny (ludzki) język (np. angielski lub polski) każdej strony (np. `"lang="en"` w znaczniku `html`). | | | | |[3.1.1](https://wcag.lepszyweb.pl/#language-of-page)|
|3. Zmiany w języku|Upewnij się, że wszelkie zmiany języka w stosunku do całej strony (np. strona polska z kilkoma angielskimi słowami lub wyrażeniami) są wskazane w kodzie obejmującym te fragmenty.| | | | |[3.1.2](https://wcag.lepszyweb.pl/#language-of-parts)|
|4. Spójność UI|Upewnij się, że stylizacja elementów równoważnych funkcjonalnie (np. linków, przycisków) jest konsekwentna, spójna.| | | | |[3.2.4](https://wcag.lepszyweb.pl/#consistent-identification)|
|5. Obrazy tekstu|Upewnij się, że na stronie nie są używane obrazy tekstu, chyba że określony styl wizualny jest niezbędny i nie może być osiągnięty poprzez tekst w stylu (np. tekst logo). Dodaj w arkuszu stylów w przeglądarce regułę `* {color:#CC0AAA !important; text-shadow:3px 2px #CC0AAA ! !important;}`, aby znaleźć obrazy tekstu (prawdziwy tekst powinien zmienić kolor na różowy/uzyskać różowy cień).| | | | |[1.4.5](https://wcag.lepszyweb.pl/#images-of-text)|
|6. Nazwa, rola, wartość|Upewnij się, że wszystkie niestandardowe elementy interfejsu użytkownika są zakodowane tak, aby działały poprawnie z czytnikami ekranu. Upewnij się, że czytniki ekranu podają prawidłowe nazwy elementów (tj. to, jak się nazywają), role (tj. co robią) i wartości (tj. ich aktualny stan). Na przykład, rolą pola wyboru jest „pole wyboru”, jego wartość jest albo „zaznaczone” albo „odznaczona”, a jego nazwa jest jego etykietą; zawartość, która się odsłania/zasłania, potrzebuje roli, która wskazuje, że jest ukrywana, a wartość, która wskazuje, czy jest rozwijana czy zwinięta.| | | | |[4.1.2](https://wcag.lepszyweb.pl/#name-role-value)|











