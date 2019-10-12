## Limity czasu

### Metoda badania: 
Obserwacja, test ręczny 

## Zastosowanie
_do opracowania_
## Założenia, zastrzeżenia lub wyjątki
_do opracowania_

## Obsługa dostępności
_do opracowania_

### Oczekiwania: 
Kryterium sukcesu: [2.2.1 Możliwość dostosowania czasu](https://wcag.lepszyweb.pl/#timing-adjustable)
-	Użytkownik jest informowany, jak długo trwa czas sesji.
-	Użytkownik jest monitowany przed upływem czasu trwania sesji.
-	Fokus jest przenoszony do okna lub obszaru strony z monitem.
-	Użytkownik może wyłączyć lub dostosować limit czasu za pomocą prostej czynności.
-	Gdy użytkownik potwierdzi zapoznanie się z monitem, fokus powraca do miejsca, w którym był przed monitem
-	Użytkownik jest powiadamiany że sesja wygasła i otrzymuje instrukcje, jak powrócić do sesji. 

*Uwaga*. W WCAG zdefiniowano 3 wyjątki, których nie obejmują wymagania kryterium sukcesu 2.2.1:  
-	Wyjątek dotyczący czasu rzeczywistego: sytuacje, gdy nie można zmienić limitu czasu, który wynika z organizacji pewnych procesów w czasie rzeczywistym, np. wyznaczonego czasu trwania aukcji, promocji, terminu składania ofert, lub:
-	Wyjątek dotyczący istoty czynności: sytuacje, gdy wydłużenie limitu czasu powodowałoby zaburzenie sensu czynności, przekroczenie istotnych warunków (np. w przypadku testów, w których istotnym kryterium jest czas reakcji.   
-	Wyjątek 20 godzin: sytuacje, w których limit czasowy jest dłuższy niż 20 godzin.   

### Procedura testowania:
1.	Sprawdź przed upływem limitu czasu, czy:
-	Użytkownik jest ostrzegany o ograniczonym limicie czasu
-	Użytkownik ma możliwość wyłączenia albo przedłużenia limitu czasu co najmniej dziesięciokrotnie
-	Użytkownik otrzymuje monit o zbliżającym się wygaśnięciu sesji i ma przynajmniej 20 sekund na wydłużenie jej czasu za pomocą prostej czynności.
2.	Sprawdź, czy alert ostrzegający o upływającym limicie czasu jest przekazywany w sposób wymuszający uwagę użytkownika, np. jest wyświetlany w oknie modalnym.
3.	Sprawdź, czy użytkownik jest powiadamiany, że sesja wygasła oraz czy w powiadomieniu znajduje się prosta instrukcja, jak powrócić do sesji (np. „Zaloguj się ponownie”).


### Zasoby
-	Przeczytaj: [SSA Accessibility Best Practices Library](https://www.ssa.gov/accessibility/bpl/bps/forms/timeout/default.htm)
-	Przeczytaj: [Accessible timeout notifications](https://tink.uk/accessible-timeout-notifications/)

#### Pomocne narzędzia:

#### Techniki WCAG 2.1
_do opracowania_

### Przypadki testowe

#### Zaliczone
_do opracowania_

#### Niezaliczone
_do opracowania_ 