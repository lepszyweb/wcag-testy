---
title: UWEM 1.2


sidebar: metoda_sidebar
permalink: met_uwem
folder: metoda
---

## Unified Web Evaluation Methodology (UWEM) 1.2

Pierwsza wersja jednolitej metodologii oceny dostępności internetowej została opublikowana w listopadzie 2006 roku. 

Metodologia powstała w wyniku prac prowadzonych w ramach trzech europejskich projektów badawczych 6.&nbsp;Ramowego programu badań w&nbsp;zakresie technologii społeczeństwa informacyjnego (Sixth Framework Programme Information Society Technologies) zgrupowanych w&nbsp;ramach klastra Web Accessibility Benchmarking (wzorcowe testy dostępności Sieci). 

Celem projektów było wypracowanie metodologii, która byłaby podstawą oceny i certyfikacji dostępności Sieci w&nbsp;Europie. 

Dyskusje i dalsze prace nad UWEM 1.0 doprowadziły do opublikowania we wrześniu 2007 roku finalnej wersji [Unified Web Evaluation Methodology (UWEM) 1.2](http://www.wabcluster.org/uwem1_2/).

UWEM jest metodologią oceny zgodności stron internetowych z [WCAG 1.0](https://www.w3.org/TR/WAI-WEBCONTENT/) opublikowanymi przez World Wide Web Consortium (W3C) w&nbsp;1999 roku.

Metodologia UWEM obejmowała:
- określenie podstawowych założeń,
- opis procedur oceniania,
- zalecenia dotyczące zakresu oceny i pobierania próbek zasobów do oceny, 
- testy dla punktów kontrolnych WCAG 1.0 na poziomie priorytetu 1 i 2,
- zalecenia dotyczące raportowania wyników oceny,
- szablony i definicje danych.
- słownik terminów.

## Definicja metodologii
UWEM definiuje metodologię oceniania dostępności jako _system zasad i praktyk dla ekspertów i&nbsp;automatycznej oceny dostępności stron internetowych przez ludzi i interfejsy maszyn_.

## Założenia metodologii 
UWEM została zaprojektowana tak, aby była zgodna z priorytetami 1 i&nbsp;2 punktów kontrolnych WCAG 1.0 w&nbsp;odniesieniu do kryteriów technicznych. Celem UWEM było _zwiększenie wartości ocen poprzez oparcie ich na wspólnej interpretacji WCAG 1.0 i&nbsp;zestawie testów, które są wystarczająco solidne, aby dać zainteresowanym stronom zaufanie do wyników_.

UWEM została opracowana w taki sposób, aby spełniała następujące wymagania:
- zgodność techniczna z istniejącymi dokumentami Web Accessibility Initiative (WAI),
- niezależność narzędzi i przeglądarek.
- jednoznaczność (unikalna interpretacja): opisy powinny być interpretowane tylko w&nbsp;jeden sposób
- replikacyjność: te same testy na tej samej stronie wykonane przez różnych oceniających powinny przynosić te same wyniki.
- zgodność z rozporządzeniem (WE) nr 808/2004 Parlamentu Europejskiego i&nbsp;Rady dotyczącym statystyk Wspólnoty w sprawie społeczeństwa informacyjnego.

## Proces oceny
UWEM zdefiniowała trzy główne scenariusze zastosowania, zależne od celów oceny:
- zastosowanie w celu potwierdzenia zgodności z WCAG,
- zastosowanie w celu oceny, jak strona lub witryna spełnia wymagania WCAG (ale nie w&nbsp;celu stwierdzenia zgodności),
- zastosowanie w celu monitorowania dostępności dużej liczby stron internetowych.

## Procedury 
UWEM wskazuje na trzy zasadnicze procedury testowania dostepności:
- testowanie automatyczne,
- badanie eksperckie,
- testy użyteczności z udziałem użytkowników z niepełnosprawnościami.   

Każda z tych procedur ma swoje mocne i słabe strony. Żadna nie jest kompletna i wyczerpująca. 

Najlepszym sposobem zapewnienia rzetelnej i warygodnej oceny dostępności i&nbsp;zgodności z&nbsp;normami jest zastosowanie podejścia łączonego, obejmującego wszystkie metody oceny: ocenę automatyczną, ocenę ekspercką i testowanie z udziałem użytkowników z niepełnosprawnościami.


## Zakres i pobieranie próbek zasobów
W metodologii UWEM stwierdzenia dotyczące zgodności i inne raporty oceniające muszą odnosić się do listy zasobów ocenianych w&nbsp;ramach strony internetowej (stron internetowych). 

## Procedura wyznaczania zakresu ocenianych zasobów
Dla celów UWEM witrynę internetową definiuje się jako dowolny zbiór połączonych hiperłaczami zasobów internetowych, z których każdy jest określany zgodnie z procedurą opisaną w sekcji definiującej.  

Do celów UWEM witrynę internetową definiuje się jako dowolny zbiór hiperłączonych zasobów internetowych, z których każdy jest identyfikowany zgodnie z procedurą opisaną w sekcji 4.1.
Celem UWEM jest wspieranie powtarzalności wyników. Z tego powodu jednoznaczna identyfikacja ocenianych zasobów ma zasadnicze znaczenie dla agregacji i porównywania wyników. Stwierdzenia ogólne, takie jak: "http://przyklad.org/ jest zgodna z normą UWEM 1.2 Poziom 1" są nie do przyjęcia w stwierdzeniach o zgodności z normą UWEM 1.2. Takie stwierdzenie sugerowałoby, że zestaw zasobów „zalążkowych / nasiennych / ?????” został przeszukany do końca zgodnie z pewnymi wcześniej ustalonymi limitami lub ograniczeniami. Biorąc jednak pod uwagę szeroką gamę istniejących przeszukiwaczy i różne stosowane przez nich technologie, nie można zweryfikować wiarygodności tych stwierdzeń. Ponadto różne RFC związane z nazwami domen pozostawiają otwarte pole do interpretacji w odniesieniu do koncepcji poddomeny i jej rozdzielczości.
Dlatego w przypadku deklaracji zgodności UWEM 1.2 zakres witryny MUSI być wyrażony w formie listy zasobów (patrz Załącznik C).

### Procedury wyboru próbek do oceny
Testowanie wszystkich zasobow witryny pod kątm wszystkich kryteriów oceny nie jest praktyczne. W zwiazku z tym, po ustaleniu listy zasobów do oceny oraz celów oceny, można wybrać podzbiór lub „próbkę” zasobów do oceny.    

UWEM określa dwie procedury doboru ocenianych próbek:
- **próbka losowa**, wygenerowana automatycznie przez narzędzie; jeżeli ocena musi być powtarzalna i umożliwiać porównania synchroniczne lub asynchroniczne (np. monitorowanie), próbka do oceny musi być wygenerowana w drodze jednolitej procedury losowej.
- **próbka nielosowa**, wybierana przez eksperta.




### 

Lista zasobów podstawowych powinna składać się z jak największej liczby następujących zasobów, które mają zastosowanie:


jest zbiorem zasobów ogólnych, które mogą być obecne na większości stron internetowych i które są kluczowe dla oceny użytkowania i dostępności strony. Lista zasobów podstawowych stanowi zatem zbiór zasobów, które powinny być zawarte w każdej ocenie dostępności witryny dokonywanej przez ekspertów. Lista zasobów podstawowych nie może, ogólnie rzecz biorąc, być automatycznie identyfikowana, ale wymaga wybrania ludzkich osądów.

-	Zasoby "Home". Jest ona definiowana jako zasób identyfikowany przez adres URL składający się wyłącznie ze składnika protokołu HTTP, po którym następuje nazwa hosta. Mapowanie z tego adresu URL do zasobów domowych może polegać na przekierowaniu po stronie serwera. Ten zasób musi być obecny na stronie (choć może mieć inną nazwę).
-	Zasoby "Informacje kontaktowe" (jeśli istnieją).
-	Ogólny zasób "Pomocy" (jeśli istnieje).
-	Zasób "Mapa witryny" (jeśli istnieje).
-	Zasoby składające się na usługę "Podstawowe wyszukiwanie stron internetowych" (jeśli dotyczy). Obejmuje to co najmniej jeden zasób, w którym można rozpocząć wyszukiwanie i co najmniej jeden zasób pokazujący wyniki przykładowego wyszukiwania.
-	Zasoby opisujące funkcje dostępności i/lub politykę dostępności strony (jeśli takie istnieją).
-	Przykłady zasobów reprezentatywnych dla głównych zamierzonych zastosowań witryny (jeśli są możliwe do zidentyfikowania).
-	Jeśli witryna świadczy usługi, które obejmują użytkownika systematycznie przeszukującego sekwencję zasobów (np. wielostronicowy formularz lub transakcja), wówczas należy uwzględnić reprezentatywne zasoby dostępne na każdym etapie każdego z takich kluczowych scenariuszy (jeśli ma to zastosowanie i tylko wtedy, gdy są one objęte zakresem).
-	Zasoby reprezentatywne dla każdej kategorii zasobów o zasadniczo odmiennym &bdquo;wyglądzie i odczuciu&rdquo; (zazwyczaj reprezentatywne dla różnych podstawowych &bdquo;szablonów&rdquo; witryny) (jeśli są możliwe do zidentyfikowania).
-	Zasoby reprezentatywne dla każdej z następujących odrębnych technologii internetowych (gdzie są one wykorzystywane):
	-	formularze,
	-	ramki,
	-	tabele danych,
	-	skrypty po stronie klienta,
	-	kaskadowe arkusze stylów,
	-	aplety, wtyczki, multimedia itp.



Jeśli próbka ewaluacyjna jest tworzona ręcznie, musi zawierać listę zasobów podstawowych. Jeśli lista zasobów podstawowych zawiera mniej stron niż wymagana wielkość próbki, należy dodać dodatkowe zasoby z następujących kategorii:

-	Zasoby reprezentatywne dla głównych zamierzonych zastosowań witryny (jeśli są możliwe do zidentyfikowania).
-	Jeżeli witryna świadczy usługi, w które użytkownik systematycznie przeszukuje sekwencję zasobów (np. wielostronicowy formularz lub transakcja), należy uwzględnić reprezentatywne zasoby dostępne na każdym etapie każdego z takich kluczowych scenariuszy (jeżeli ma to zastosowanie i tylko wtedy, gdy są one objęte zakresem).
-	Zasoby reprezentatywne dla każdej kategorii zasobów o zasadniczo odmiennym &bdquo;wyglądzie i odczuciu&rdquo; (zazwyczaj reprezentatywne dla różnych podstawowych &bdquo;szablonów&rdquo; witryny) (jeśli są możliwe do zidentyfikowania).
-	Zasoby reprezentatywne dla każdej z następujących odrębnych technologii internetowych (gdzie są one wykorzystywane):
	-	formularze,
	-	ramki,
	-	tabele danych,
	-	skryptów po stronie klienta,
	-	Kaskadowe arkusze stylów,
	-	aplety, wtyczki, multimedia itp.

Oczywiście, każdy pojedynczy zasób może należeć do więcej niż jednej z powyższych kategorii: wymogiem jest po prostu to, że lista zasobów podstawowych jako całość powinna, w miarę możliwości, wspólnie zająć się wszystkimi stosownymi celami próbkowania. 

Każdy konkretny zasób powinien pojawić się tylko raz w próbie ewaluacyjnej.




