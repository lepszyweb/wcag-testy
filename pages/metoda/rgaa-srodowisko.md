---
title: "Środowisko testowe - RGAA 4.1"
keywords: "RGAA, RGAA 4.1, francuskie wytyczne dostępności, tłumaczenie polskie, środowisko testowe"
lang: pl
permalink: rgaa-srodowisko

sidebar: metoda_sidebar
---

### Środowisko testowe dla RGAA 4.0

Wiele kryteriów RGAA, zwłaszcza związanych z JavaScript, odnosi się do testów, które należy przeprowadzić z&nbsp;użyciem zestawu rożnych technologii wspomagających, przeglądarek i&nbsp;systemów operacyjnych. Ten dokument opisuje i wyjaśnia kombinacje wybrane jako podstawowe.

Testy przeprowadzone przy użyciu tych kombinacji (technologia wspomagająca, system operacyjny, przeglądarka) pozwalają stwierdzić, że ​​oprogramowanie oparte na HTML/ARIA [„obsługuje dostępność", jak zdefiniowano w&nbsp;WCAG](https://testy.lepszyweb.pl/slownik#o).

Lista kombinacji została sporządzona w drodze wyboru na podstawie listy technologii wspomagających, które są wystarczająco rozpowszechnione, lub w niektórych przypadkach, gdy są dostarczane natywnie i&nbsp;stanowią preferowany przez użytkowników sposób dostępu do informacji i&nbsp;funkcjonalności.


### Środowisko testowe - komputer stacjonarny

Stosowane systemy operacyjne to Windows i Mac OS X oraz przeglądarki, Internet Explorer, Firefox i Safari. Do audytora należy określenie, w&nbsp;porozumieniu z&nbsp;kierownictwem audytowanej witryny, wersji systemu operacyjnego i&nbsp;przeglądarki, zgodnie z&nbsp;kontekstem użytkowania witryny i&nbsp;środowiskiem testowym używanym podczas tworzenia witryny. Wersje technologii wspomagających, które zostaną zastosowane, powinny być albo najnowszą wersją dostępną w języku polskim dla wybranego systemu operacyjnego albo wersją poprzednią.

Gdy witryna lub aplikacja jest przeznaczona dla użytkowników, których sprzęt jest kontrolowany (np. w&nbsp;firmowym intranecie), testy należy przeprowadzić w&nbsp;środowisku testowym dostosowanym do kontekstu środowiska kontrolowanego.

Aby narzędzie HTML5/ARIA lub jego alternatywa mogło być uznane za zgodne z wymogami dostępności, musi być w&nbsp;pełni funkcjonalne w&nbsp;zakresie odtwarzania i&nbsp;funkcjonalności, w&nbsp;co&nbsp;najmniej jednej z&nbsp;następujących kombinacji:


#### Środowisko testowe -  komputer stacjonarny  - kombinacja 1

| Technologia wspomagająca | Przeglądarka |
|:--------|:-------:|
| NVDA (najnowsza wersja) | Firefox |
| JAWS (poprzednia wersja) | Firefox lub Internet Explorer |
| VoiceOver (najnowsza wersja) | Safari |

#### Środowisko testowe - komputer stacjonarny - kombinacja 2

| Technologia wspomagająca | Przeglądarka |
|:--------|:-------:|
| JAWS (poprzednia wersja) | Firefox |
| NVDA (najnowsza wersja)  | Firefox lub Internet Explorer |
| VoiceOver (najnowsza wersja) | Safari |


### Środowisko testowe terminali przenośnych

Wybrane systemy operacyjne to Android i iOS oraz przeglądarki Chrome i Safari. Do audytora należy określenie, w&nbsp;porozumieniu z kierownictwem audytowanej witryny, wersji systemu operacyjnego i&nbsp;przeglądarki, zgodnie z&nbsp;kontekstem użytkowania witryny i&nbsp;środowiskiem testowym używanym podczas tworzenia witryny. Wersje technologii wspomagających, które zostaną zastosowane, powinny być albo najnowszą wersją dostępną w&nbsp;języku polskim dla wybranego systemu operacyjnego albo wersją poprzednią. Aby przetestować stronę internetową na terminalu mobilnym, środowisko testowe będzie musiało zawierać jedną z&nbsp;dwóch następujących uzupełniających się kombinacji:

#### Środowisko testowania terminali przenośnych - kombinacja 1

| System operacyjny | Technologia wspomagająca | Przeglądarka |
|:--------|:--------|:-------:|
| iOS | VoiceOver (najnowsza wersja) | Safari |

#### Środowisko testowania terminali przenośnych - kombinacja 2

| System operacyjny | Technologia wspomagająca | Przeglądarka |
|:--------|:--------|:-------:|
| Android | TalkBack (najnowsza wersja) | Chrome |

Należy pamiętać, że w przypadku strony internetowej przeznaczonej dla urządzeń przenośnych do powszechnego użytku zdecydowanie zaleca się testowanie w&nbsp;obu środowiskach.

Inne środowiska {#inne}

Ponadto, zależnie od kontekstu sprawdzanej strony, przydatne mogą być inne uzupełniające technologie wspomagajace, takie jak:

-   ZoomText w systemie Windows lub Mac OSX.
-   Dragon Naturally Speaking w systemie Windows lub Mac OSX.

### Środowisko kontrolowane

Jeśli witryna internetowa jest przeznaczona do rozpowszechniania i użytkowania w środowisku kontrolowanym, środowisko testowe (podstawowe) musi się składać z&nbsp;konfiguracji (technologie wspomagające, system operacyjny, przeglądarka) rzeczywiście używanych w środowisku kontrolowanym.

Na przykład, gdy witryna jest używana wyłącznie w środowisku GNU/Linux, testy muszą być wykonane tylko w&nbsp;przeglądarkach i&nbsp;technologiach wsspomagających używanych na tej platformie. To środowisko testowe zastępuje środowisko testowe używane w&nbsp;środowiskach niekontrolowanych.