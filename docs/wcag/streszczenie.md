## Streszczenie

„Wytyczne dla dostępności treści internetowych 2.0 (WCAG 2.0)” to szeroki wachlarz rekomendacji dotyczących tworzenia treści internetowych bardziej dostępnymi. Wdrożenie niniejszych wytycznych sprawi, iż treść stron WWW stanie się dostępna dla szerszego grona użytkowników niepełnosprawnych, w tym dla osób niewidomych i słabowidzących, głuchych i niedosłyszących, osób mających trudności w uczeniu się, osób z ograniczeniami kognitywnymi, niepełnosprawnych ruchowo, z zaburzeniami mowy, nadwrażliwością na światło, oraz osób z niepełnosprawnościami złożonymi. Wprowadzenie wytycznych w życie, sprawi również, że treści internetowe będą bardziej przyjazne dla każdego innego użytkownika.

Kryteria sukcesu WCAG 2.0 są twierdzeniami możliwymi do zweryfikowania i nie są powiązane z konkretną technologią. Wytyczne dotyczące spełnienia kryteriów sukcesu dla konkretnych technologii, jak również ogólne informacje dotyczące interpretacji kryteriów sukcesu zawarte są w osobnych dokumentach. Więcej na ten temat przeczytać można w [Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/intro/wcag.php), gdzie znajduje się wstęp i odnośniki do materiałów edukacyjnych oraz informacji technicznych dotyczących WCAG.

WCAG 2.0 zastępuje [Web Content Accessibility Guidelines 1.0 (WCAG10)](http://www.w3.org/TR/WCAG10/), dokument, który został oficjalnie opublikowany w maju 1999 roku, jako rekomendacja Konsorcjum W3C. Chociaż można stosować się do wytycznych WCAG 1.0 lub WCAG 2.0 (lub też do obu), Konsorcjum W3C sugeruje, aby dla nowych i aktualizowanych treści stosować kryteria WCAG 2.0. Rekomenduje się również odnoszenie się do wytycznych WCAG 2.0 w kwestii polityki dostępności.</p>

## Status dokumentu
    
<em>Poniższa część opisuje status dokumentu w momencie jego publikacji. Inne dokumenty mogą w przyszłości zastąpić niniejszy. Lista 
bieżących publikacji Konsorcjum W3C oraz zaktualizowany raport techniczny znajdują się na stronie [W3C technical reports index](http://www.w3.org/TR/) pod adresem http://www.w3.org/TR/.</em>
    
Ten dokument to „Wytyczne dla dostępności treści internetowych 2.0 (WCAG 2.0)”, [rekomendacja Konsorcjum W3C](http://www.w3.org/2004/02/Process-20040205/tr.html#RecsW3C), sporządzona przez [Grupę Roboczą ds. wytycznych dostępności treści internetowych](http://www.w3.org/WAI/GL/) (Web Content Accessibility Guidelines Working Group).

Niniejszy dokument został zrecenzowany przez członków Konsorcjum W3C, programistów, inne grupy W3C oraz inne zainteresowane strony, a 
następnie zaakceptowany przez Dyrektora Konsorcjum W3C, jako Rekomendacja Konsorcjum W3C. Jest to wersja finalna dokumentu, która może zostać wykorzystana jako materiał źródłowy lub być cytowana w innych dokumentach W3C. Rolą Konsorcjum W3C jest zwrócenie uwagi na tę specyfikację i wspieranie jej rozpowszechniania. Stosowanie zaleceń zawartych w tej specyfikacji, zwiększa funkcjonalność oraz interoperacyjność sieci.

Wytyczne WCAG 2.0 są powiązane z innymi, nienormatywnymi dokumentami, a mianowicie <a href="">[Understanding WCAG 2.0](http://www.w3.org/TR/UNDERSTANDING-WCAG20/) (Zrozumieć WCAG 2.0) oraz [Techniques for WCAG 2.0](http://www.w3.org/TR/WCAG20-TECHS/)  (Techniki WCAG 2.0). Chociaż wymienione dokumenty nie posiadają formalnego statusu, jaki ma WCAG 2.0, zawierają informacje ważne dla 
zrozumienia i wdrożenia wytycznych WCAG 2.0.

Grupa Robocza pracująca nad dokumentem prosi o składanie wszelakich komentarzy za pomocą [formularza internetowego](http://www.w3.org/WAI/WCAG20/comments/). Jeśli z jakichś przyczyn, nie jest to możliwe, komentarze można też przesyłać na adres [public-comments-wcag20@w3.org](http://mailto:public-comments-wcag20@w3.org). Dostępne jest również [archiwum publicznych komentarzy](http://lists.w3.org/Archives/Public/public-comments-wcag20). Komentarze na temat rekomendacji WCAG 2.0 nie będą skutkować zmianami 
niniejszej wersji. Mogą jednak zostać uwzględnione w erracie lub przyszłych wersjach WCAG. Nie przewiduje się przesyłania formalnych 
odpowiedzi na komentarze. Archiwum dyskusji na [listach mailingowych WCAG WG](http://lists.w3.org/Archives/Public/w3c-wai-gl/) są publicznie dostępne, a Grupa Robocza może wziąć pod uwagę komentarze dotyczące niniejszego dokumentu w przyszłości.

Dokument powstał w ramach [Web Accessibility Initiative](http://www.w3.org/WAI/WCAG20/comments/) (WAI) Konsorcjum W3C. Cele Grupy Roboczej WCAG 2.0 zostały sprecyzowane w [Karcie Grupy Roboczej WCAG](http://www.w3.org/2004/04/wcag-charter). Grupa Robocza WCAG 2.0 jest częścią [działań technicznych WAI](http://www.w3.org/WAI/Technical/Activity) (WAI Technical Activity).

Niniejszy dokument został stworzony zgodnie z [Polityką Patentową Konsorcjum W3C z 5 lutego 2004 roku](http://www.w3.org/Consortium/Patent-Policy-20040205/). Konsorcjum W3C [przechowuje pełną listę zgłoszonych publicznie patentów](http://www.w3.org/2004/01/pp-impl/35422/status) odnośnie tego dokumentu. Powyższa strona zawiera również instrukcje zgłaszania patentu. Osoby, które twierdzą, iż posiadają wiedzę na temat patentów zawierających [istotne roszczenia](http://www.w3.org/Consortium/Patent-Policy-20040205/#def-essential) (Essential Claim(s)) powinny zgłosić takie informacje, zgodnie z [Rozdziałem 6 Polityki Patentowej Konsorcjum W3C](http://www.w3.org/Consortium/Patent-Policy-20040205/#sec-Disclosure).


## Spis treści
- Wprowadzenie 
  - Poziomy wytycznych WCAG 2.0
  - Dokumenty uzupełniające WCAG 2.0
  - Ważne pojęcia zastosowane w WCAG 2.0
- Wytyczne WCAG 2.0
  - 1 Postrzegalność
    - 1.1 Alternatywa w postaci tekstu: Dla każdej treści nietekstowej należy dostarczyć alternatywną treść w formie tekstu, która może być zamieniona przez użytkownika w inne formy (np. powiększony druk, brajl, mowa syntetyczna, symbole lub język uproszczony).
	- 1.2 Media zmienne w czasie: Należy dostarczyć alternatywę dla mediów zmiennych w czasie.
	- 1.3 Możliwość adaptacji: Należy tworzyć treści, które mogą być prezentowane na różne sposoby (np. uproszczony układ wizualny), bez utraty informacji czy struktury.
	- 1.4 Mozliwość rozróżnienia: Użytkownik powinien móc dobrze widzieć bądź słyszeć treści — mieć możliwość oddzielenia informacji od tła.
  - 2 Funkcjonalność
    - 2.1 Dostępność z klawiatury: Zapewnij dostępność wszystkich funkcjonalności za pomocą klawiatury. 
	- 2.2 Wystarczająca ilość czasu: Zapewnij użytkownikom wystarczająco dużo czasu na przeczytanie i skorzystanie z treści.
	- 2.3 Ataki padaczki: Nie należy projektować treści w taki sposób, aby prowokować ataki padaczki.
	- 2.4 Możliwość nawigacji: Dostarczenie narzędzi ułatwiających użytkownikowi nawigowanie, znajdowanie treści i ustalanie, gdzie się w danym momencie znajduje.
  - 3 Zrozumiałość
    - 3.1 Możliwość odczytania: Treść powinna być zrozumiała i możliwa do odczytania.
	- 3.2 Przewidywalność: Strony internetowe powinny otwierać się i działać w przewidywalny sposób.
	- 3.3 Pomoc przy wprowadzaniu informacji: Istnieje wsparcie dla użytkownika, by mógł uniknąć błędów lub je skorygować.
  - 4 Solidność
    - 4.1 Kompatybilność: Zmaksymalizowanie kompatybilności z obecnymi oraz przyszłymi programami użytkowników, w tym z technologiami wspomagającymi.
  - Zgodność
    - Wymogi zgodności
	- Stwierdzanie zgodności (opcjonalne)
	- Oświadczenie częściowej zgodności – treść umieszczana przez dostawców zewnętrznych
	- Oświadczenie częściowej zgodności – język

### Załączniki

- Załącznik A: <a href="#glossary">Słownik terminów</a> (Normatywny)
- Załącznik B: <a href="#acknowledgments">Podziękowania</a>
- Załącznik C: <a href="#references">Literatura</a>
