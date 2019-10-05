## Zasada nr 1: Postrzegalność
Informacje oraz komponenty interfejsu użytkownika muszą być przedstawione użytkownikom w sposób dostępny dla ich zmysłów.

### Wytyczna 1.1 Alternatywa w postaci tekstu
Dla każdej treści nietekstowej należy dostarczyć alternatywną treść w formie tekstu, która może być zamieniona przez użytkownika w inne formy (np. powiększony druk, brajl, mowa syntetyczna, symbole lub język uproszczony).

#### 1.1.1 Treść nietekstowa
Wszelkie <a title="definicja: treść nietekstowa" href="#non-text-contentdef" class="termref">treści nietekstowe</a> przedstawione użytkownikowi posiadają swoją <a title="definicja: tekst alternatywny" href="#text-altdef" class="termref">tekstową alternatywę</a>, która pełni tę samą funkcję, za wyjątkiem sytuacji 
opisanych poniżej (Poziom A):

- **Kontrolki użytkownika i wprowadzanie danych przez użytkownika:** Jeśli treść nietekstowa jest kontrolką użytkownika lub polem wprowadzania danych, wtedy posiada <a title="definicja: nazwa" href="#namedef" class="termref">nazwę</a> opisującą jej przeznaczenie. (<a href="#_Wytyczna_4.1_Kompatybilno%C5%9B%C4%87:">Wytyczna 4.1</a> podaje dodatkowe wymagania dotyczące kontrolek oraz wprowadzania danych przez użytkownika.)
- **Media zmienne w czasie:** Jeśli treść nietekstowa to media zmienne w czasie, wtedy alternatywa w formie tekstu zawiera opis pozwalający zrozumieć przeznaczenie treści nietekstowej. (<a href="http://fdc.org.pl/wcag2/#_Wytyczna_1.2_Media">Wytyczna 1.2</a> podaje dodatkowe wymagania, jeśli chodzi o media.)
- **Media zmienne w czasie:**Jeśli treść nietekstowa to media zmienne w czasie, wtedy alternatywa w formie 
tekstu zawiera opis pozwalający zrozumieć przeznaczenie treści nietekstowej. (<a href="http://fdc.org.pl/wcag2/#_Wytyczna_1.2_Media">Wytyczna 1.2</a> podaje dodatkowe wymagania, jeśli chodzi o media.)
- **Test:**Jeśli treść nietekstowa jest testem 
lub ćwiczeniem, które utraciłoby swój sens ze względu na przedstawienie 
tej samej treści w postaci <a title="definicja: tekst" href="#textdef" class="termref">tekstu</a>, wtedy alternatywa w postaci tekstu podawać powinna przynajmniej opis pozwalający zrozumieć przeznaczenie 
treści nietekstowej.
- **Odczucie zmysłowe:** Jeśli treść nietekstowa 
ma za zadanie przede wszystkim tworzyć <a title="definicja: konkretne odczucie zmysłowe" href="#sensoryexpdef" class="termref">konkretne odczucie zmysłowe</a>,
 wtedy alternatywa w postaci tekstu jest opisem pozwalającym zrozumieć 
przeznaczenie treści nietekstowej.
- **<a title="definicja: CAPTCHA" href="#CAPTCHAdef" class="termref">CAPTCHA</a>:** Jeśli celem treści nietekstowej jest potwierdzenie, że do treści ma dostęp człowiek, a nie komputer, wtedy dostarcza się alternatywę w postaci tekstu, która identyfikuje oraz opisuje cel treści nietekstowej. Dostarcza się również alternatywnych zabezpieczeń typu CAPTCHA, dostosowanych do różnych możliwości percepcji użytkowników, uwzględniając różne rodzaje niepełnosprawności.
- **Cele dekoracyjne, formatowanie, treść niewidoczna:** Jeśli treść nietekstowa pełni [funkcję dekoracyjną](slownik/wylaczniedekoracyjna), używana jest do formatowania wizualnego lub też nie jest przedstawiana użytkownikowi, powinna być wdrożona w sposób umożliwiający [technologiom wspomagającym](slownik/technologiewspomagające) jej zignorowanie.

### Wytyczna 1.2 Media zmienne w czasie
Należy dostarczyć alternatywę dla mediów zmiennych w czasie.

#### 1.2.1 Tylko audio lub tylko wideo (nagranie)
Dla <a title="definicja: nagranie" href="#prerecordeddef" class="termref">mediów nagranych</a> w systemie <a title="definicja: materiał dźwiękowy" href="#audio-onlydef" class="termref">tylko audio</a> lub <a title="definicja: tylko wideo" href="#video-onlydef" class="termref">tylko wideo</a> stosuje się następujące zasady, za wyjątkiem sytuacji, kiedy nagranie audio lub wideo jest <a title="definicja: multimedia alternatywne dla tekstu" href="#multimedia-alt-textdef" class="termref">alternatywą dla tekstu</a> i w taki sposób jest oznaczone: (Poziom A)
- **Nagranie tylko audio:** Zapewniona jest <a title="definicja: alternatywa dla mediów zmiennych w czasie" href="#alt-time-based-mediadef" class="termref">alternatywa dla mediów zmiennych w czasie</a>, przedstawiająca tę samą treść, co w nagraniu audio.
- **Nagranie tylko wideo:** Zapewniona jest alternatywa dla mediów zmiennych w czasie, albo nagranie audio, przedstawiające te same informacje, jak w nagraniu wideo.

#### 1.2.2 Napisy rozszerzone (nagranie)
<a title="definicja: napisy rozszerzone" href="#captionsdef" class="termref">Napisy rozszerzone</a> dołączone są do wszystkich <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań</a> <a title="definicja: audio" href="#audiodef" class="termref">audio</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz), za wyjątkiem sytuacji, kiedy są one <a title="definicja: multimedia alternatywne dla tekstu" href="#multimedia-alt-textdef" class="termref">alternatywami dla tekstu</a> i w taki sposób są oznaczone. (Poziom A)
#### 1.2.3 Audiodeskrypcja lub alternatywa dla mediów (nagranie)
Zapewnia się <a title="definicja: alternatywa dla mediów zmiennych w czasie" href="#alt-time-based-mediadef" class="termref">alternatywę dla mediów zmiennych w czasie</a> lub <a title="definicja: audiodeskrypcja" href="#audiodescdef" class="termref">audiodeskrypcję</a> dla <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań wideo</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> 
(dźwięk i obraz), za wyjątkiem sytuacji, kiedy są one alternatywami dla tekstu i w taki sposób są oznaczone. (Poziom A)
#### 1.2.4 Napisy rozszerzone (na żywo)
<a title="definicja: napisy rozszerzone" href="#captionsdef" class="termref">Napisy rozszerzone</a> dołączone są do wszystkich treści <a title="definicja: audio" href="#audiodef" class="termref">audio</a> przekazywanych <a title="definicja: na żywo" href="#livedef" class="termref">na żywo</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz). (Poziom AA)
#### 1.2.5 Audiodeskrypcja (nagranie):
Zapewniona jest <a title="definicja: audiodeskrypcja" href="#audiodescdef" class="termref">audiodeskrypcja</a> dla wszystkich <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań</a> <a title="definicja: wideo" href="#videodef" class="termref">wideo</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz). (Poziom AA)
#### 1.2.6 Język migowy (nagranie):
Zapewnione jest 
<a title="definicja: tłumaczenie języka migowego" href="#sign-languageinterpdef" class="termref">tłumaczenie w języku migowym</a> wszystkich <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań</a>  <a title="definicja: audio" href="#audiodef" class="termref">audio</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz). (Poziom AAA)
#### 1.2.7 Rozszerzona audiodeskrypcja (nagranie)
Zapewniona jest <a title="definicja: rozszerzona audiodeskrypcja" href="#extended-addef" class="termref">rozszerzona audiodeskrypcja</a> dla wszystkich <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań</a> <a title="definicja: wideo" href="#videodef" class="termref">wideo</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz), jeśli przerwy w ścieżce dźwiękowej danego nagrania nie pozwalają na zamieszczenie <a title="definicja: audiodeskrypcja" href="#audiodescdef" class="termref">audiodeskrypcji</a>, przekazującej sens treści w wystarczającym stopniu. (Poziom AAA)
#### 1.2.8 Alternatywa dla mediów (nagranie)
Zapewnia
 się <a title="definicja: alternatywa dla mediów zmiennych w czasie" href="#alt-time-based-mediadef" class="termref">alternatywę dla wszystkich mediów zmiennych w czasie</a> — <a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagrań</a> w <a title="definicja: zsynchronizowane multimedia" href="#synchronizedmediadef" class="termref">multimediach zsynchronizowanych</a> (dźwięk i obraz) oraz dla wszystkich nagrań <a title="definicja: tylko wideo" href="#video-onlydef" class="termref">tylko wideo</a> (sam obraz). (Poziom AAA)
#### 1.2.9 Tylko audio (na żywo)
Zapewniona jest 
<a title="definicja: alternatywa dla mediów zmiennych w czasie" href="#alt-time-based-mediadef" class="termref">alternatywa dla mediów zmiennych w czasie</a>, przedstawiająca informacje takie same, jak w przekazie <a title="definicja: materiał dźwiękowy" href="#audio-onlydef" class="termref">tylko audio</a> <a title="definicja: na żywo" href="#livedef" class="termref">na żywo</a>. (Poziom AAA)


### Wytyczna Wytyczna 1.3 Możliwość adaptacji
Należy tworzyć treści, które mogą być prezentowane na różne sposoby (np. uproszczony układ wizualny), bez utraty informacji czy struktury.

#### 1.3.1 Informacje i relacje
Informacje, <a title="definicja: struktura" href="#structuredef" class="termref">struktura</a> oraz <a title="definicja: relacja" href="#relationshipsdef" class="termref">relacje</a> pomiędzy treściami <a title="definicja: przedstawianie" href="#presentationdef" class="termref">przedstawiane w treści</a> <a title="definition:definicja: możliwy do odczytania przez program komputerowy" href="#programmaticallydetermineddef" class="termref">mogą być odczytane przez program komputerowy</a> lub są dostępne w postaci tekstu. (Poziom A).

#### 1.3.2 Zrozumiała kolejność
Jeśli kolejność, w 
jakiej przedstawiona jest treść, ma znaczenie dla zrozumienia treści — 
<a title="definicja: prawidłowa kolejność odczytu" href="#correct-reading-sequencedef" class="termref">kolejność</a> taka musi być możliwa do <a title="definicja: możliwy do odczytania przez program komputerowy" href="#programmaticallydetermineddef" class="termref">odczytania przez program komputerowy</a>. (Poziom A)

#### 1.3.3 Właściwości zmysłowe
Instrukcje co do zrozumienia i operowania treścią nie opierają się wyłącznie na właściwościach zmysłowych, takich, jak kształt, rozmiar, wzrokowa lokalizacja, orientacja w przestrzeni lub dźwięk. (Poziom A)

*Uwaga* Wymogi dotyczące koloru opisane są w <a href="#visual-audio-contrast">Wytycznej 1.4</a>.

### Wytyczna Wytyczna 1.4 Możliwość rozróżnienia
Użytkownik powinien móc dobrze widzieć bądź słyszeć treści — mieć możliwość oddzielenia informacji od tła.

#### 1.4.1 Użycie koloru
Kolor nie jest wykorzystywany jako jedyny wizualny sposób przekazywania informacji, wskazywania czynności do wykonania lub oczekiwania na odpowiedź, czy też wyróżniania elementów wizualnych. (Poziom A)

*Uwaga* To kryterium sukcesu dotyczy szczególnie percepcji koloru. Inne formy percepcji zostały omówione w <a href="#content-structure-separation">Wytycznej 1.3</a>, w tym programistyczny dostęp do koloru oraz inne rodzaje zaprogramowania 
prezentacji wizualnej.

#### 1.4.2 Kontrola odtwarzania dźwięku
Jeśli jakieś nagranie audio włącza się automatycznie na danej stronie i jest odtwarzane przez okres dłuższy niż 3 sekundy, dostępny jest albo <a title="definicja: mechanizm" href="#mechanismdef" class="termref">mechanizm</a> umożliwiający przerwanie lub wyłączenie nagrania, albo mechanizm kontrolujący poziom głośności niezależnie od poziomu głośności całego systemu. (Poziom A)

*Uwaga* Ponieważ każda treść, która nie spełnia tego kryterium sukcesu może utrudnić użytkownikowi odczytanie całej strony, 
wszelkie treści na stronie (bez względu na to, czy spełniają inne kryteria sukcesu, czy nie) muszą spełnić niniejsze kryterium. Więcej 
informacji: <a href="http://www.w3.org/TR/WCAG/#cc5">Spełnienie wymagań: brak zakłóceń: Non-Interference</a>.

#### 1.4.3 Kontrast (minimalny):
Wizualne przedstawienie <a title="definicja: tekst" href="#textdef" class="termref">tekstu</a>, lub <a title="definicja: obraz tekstu" href="#images-of-textdef" class="termref">obrazu tekstu</a> posiada <a title="definicja: współczynnik kontrastu" href="#contrast-ratiodef" class="termref">kontrast</a> wynoszący przynajmniej 4,5:1, poza następującymi wyjątkami: (Poziom AA)

- **Duży tekst:** <a title="definicja: duża wielkość tekstu" href="#larger-scaledef" class="termref">Duży tekst</a> oraz grafiki takiego tekstu posiadają kontrast przynajmniej 3:1. 
- **Przypadkowość:** Nie stosuje się wymogów 
minimalnego kontrastu dla tekstów lub obrazu tekstu, będących elementem 
nieużywanych <a title="definicja: komponent interefejsu użytkownika" href="#user-interface-componentdef" class="termref">części interfejsu użytkownika</a>, mających cel <a title="definicja: wyłącznie dekoracyjny" href="#puredecdef" class="termref">czysto dekoracyjny</a>, nie są widoczne lub też są częścią obrazu zawierającego 
inne istotne treści wizualne.
- **Logo:** Nie wymaga się minimalnego kontrastu dla tekstu, który jest częścią logo lub nazwy własnej produktu (marki).

#### 1.4.4 Zmiana rozmiaru tekstu
Oprócz <a title="definicja: napisy rozszerzone" href="#captionsdef" class="termref">napisów rozszerzonych</a> oraz <a title="definicja: obraz tekstu" href="#images-of-textdef" class="termref">tekstu w postaci grafiki</a>, rozmiar <a title="definicja: tekst" href="#textdef" class="termref">tekstu</a> może zostać powiekszony do 200% bez użycia <a title="definicja: technologie wspomagające (w rozumieniu tego dokumentu)" href="#atdef" class="termref">technologii wspomagających</a> oraz bez utraty treści lub funkcjonalności. (Poziom AA)

#### 1.4.5 Obrazy tekstu
Jeśli wykorzystywane technologie mogą przedstawiać treść wizualnie, do przekazywania informacji wykorzystuje się <a title="definicja: tekst" href="#textdef" class="termref">tekst</a>, a nie <a title="definicja: obraz tekstu" href="#images-of-textdef" class="termref">tekst w postaci grafiki</a>, za wyjątkiem następujących sytuacji: (Poziom AA)

- **Możliwy do dostosowania:** Obraz tekstu może być <a title="definicja: dostosowany wygląd" href="#visually-customizeddef" class="termref">dostosowany wizualnie</a> do wymagań użytkownika.
- **Istotny:** Prezentacja tekstu w postaci graficznej jest <a title="definicja: istotny" href="#essentialdef" class="termref">istotna</a> dla zrozumienia przekazywanej informacji.

*Uwaga* Tekst, który jest częścią logo lub nazwy własnej produktu, jest w tym przypadku uznawany za istotny.

#### 1.4.6 wzmocniony kontrast
Wizualne przedstawienie <a title="definicja: tekst" href="#textdef" class="termref">tekstu</a>, lub <a title="definicja: obraz tekstu" href="#images-of-textdef" class="termref">obrazu tekstu</a>, posiada <a title="definicja: współczynnik kontrastu" href="#contrast-ratiodef" class="termref">kontrast</a> wynoszący przynajmniej 7:1, poza następującymi wyjątkami: (Poziom AAA) </p>

- **Duży tekst:** <a title="definicja: duża wielkość tekstu" href="#larger-scaledef" class="termref">Duży tekst</a> oraz grafiki takiego tekstu posiadają kontrast przynajmniej 4,5:1.&nbsp;
- **Przypadkowość:** Nie stosuje się wymogów minimalnego kontrastu dla tekstu lub obrazu tekstu, będących elementem nieużywanych <a title="definicja: komponent interefejsu użytkownika" href="#user-interface-componentdef" class="termref">części interfejsu użytkownika</a>, mających cel <a title="definicja: wyłącznie dekoracyjny" href="#puredecdef" class="termref">czysto dekoracyjny</a>, nie są widoczne lub też są częścią obrazu zawierającego 
inne istotne treści wizualne.
- **Logo:** Nie wymaga się minimalnego kontrastu dla tekstu, który jest częścią logo lub nazwy własnej produktu (marki).

#### 1.4.7 Niska głośność lub brak tła dźwiękowego
Dla 
<a title="definicja: nagranie" href="#prerecordeddef" class="termref">nagranej</a> treści <a title="definicja: materiał dźwiękowy" href="#audio-onlydef" class="termref">tylko audio</a>, która (1) na pierwszym planie zawiera głównie mowę, (2) nie jest dźwiękową CAPTCHA lub logo w postaci dźwiękowej, oraz (3) nie jest wokalizacją mającą na celu głównie ekspresję muzyczną, np. w przypadku śpiewu lub rapu, przynajmniej jedno z poniższych założeń jest spełnione: (Poziom AAA) </p>

- **Brak treści w tle:** Nagranie audio nie zawiera dźwięków tła.&nbsp;
- **Możliwość wyłączenia:** Dźwięki tła mogą zostać wyłączone.&nbsp;
- **20 dB:** Głośność dźwięków tła jest przynajmniej o 20 decybeli mniejsza, niż głośność mowy, która stanowi 
główną treść nagrania, za wyjątkiem okazyjnych, jedno– lub dwusekundowych dźwięków tła. </p>

*Uwaga* Z definicji terminu „decybel” wynika, iż 
dźwięki tła spełniające powyższy wymóg, będą 4 razy cichsze od głównej 
treści nagrania.

#### 1.4.8 Prezentacja wizualna
Dla wizualnego przedstawienia <a title="definicja: blok tekstu" href="#blockstextdef" class="termref">bloków tekstu</a>, dostępny jest <a title="definicja: mechanizm" href="#mechanismdef" class="termref">mechanizm</a>, za pomocą którego można osiągnąć, co następuje: (Poziom AAA) </p>

1. Kolory na pierwszym planie oraz kolory tła mogą być zmienione przez użytkownika.&nbsp;
2. Szerokość nie przekracza 80 znaków (40 w przypadku alfabetów: chińskiego, japońskiego i koreańskiego).&nbsp;
3. Tekst nie jest wyjustowany (tzn. wyrównany do prawego i lewego marginesu).&nbsp;
4. Odstępy między wierszami w akapitach wynoszą przynajmniej 1,5 wysokości linii, a odległość między akapitami jest przynajmniej 1,5 razy
 większa niż ta pomiędzy wierszami.&nbsp;
5. Rozmiar tekstu może zostać powiększony do 200% bez użycia technologii wspomagających, nie wymagając od użytkownika, chcącego 
odczytać cały wiersz, przesuwania tekstu w poziomie przy <a title="definicja: okno pełnego ekranu" href="#fullscreenwindowdef" class="termref">zmaksymalizowanym  oknie ekranu</a>.&nbsp;

#### 1.4.9 Obrazy tekstu (bez wyjątków)
<a title="definicja: obraz tekstu" href="#images-of-textdef" class="termref">Teksty w postaci grafiki</a> są wykorzystywane jedynie w celach <a title="definicja: wyłącznie dekoracyjny" href="#puredecdef" class="termref">czysto dekoracyjnych</a> lub też w przypadkach, gdy takie przedstawienie <a title="definicja: tekst" href="#textdef" class="termref">tekstu</a> jest <a title="definicja: istotny" href="#essentialdef" class="termref">istotne</a> dla przekazywanej informacji. (Poziom AAA)

*Uwaga* ekst, który jest częścią logo lub nazwy własnej produktu, jest w tym przypadku uznawany za istotny.
