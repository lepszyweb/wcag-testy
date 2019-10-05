# Zasada nr 4: Rzetelność
Treść musi być solidnie opublikowana, tak, by mogła być skutecznie interpretowana przez różnego rodzaju oprogramowania użytkownika, w tym technologie wspomagające.

## Wytyczna 4.1 Kompatybilność 
Zmaksymalizowanie kompatybilności z obecnymi oraz przyszłymi programami użytkowników, w tym z technologiami wspomagającymi.

### 4.1.1 Parsowanie:
W treści wprowadzonej przy użyciu języka znaczników, elementy posiadają pełne znaczniki początkowe i końcowe, elementy są zagnieżdżane według swoich specyfikacji, elementy nie posiadają zduplikowanych atrybutów oraz wszystkie ID są unikalne, z wyjątkiem przypadków, kiedy specyfikacja zezwala na wyżej wymienione cechy. (Poziom A)

*Uwaga:* Początkowe i końcowe znaczniki, w których brak kluczowych znaków, takich, jak zamykający nawias ostry lub pytajnik 
błędnie dopasowany do atrybutu wartości, nie są uznawane za znaczniki pełne.

### 4.1.2 Nazwa, rola, wartość
Dla wszystkich <a title="definicja: komponent interefejsu użytkownika" href="#user-interface-componentdef" class="termref">komponentów interfejsu użytkownika</a> (włączając w to, ale nie ograniczając jedynie do elementów formularzy, linków oraz komponentów 
wygenerowanych przez skrypty) <a title="definicja: nazwa" href="#namedef" class="termref">nazwa</a> oraz <a title="definicja: rola" href="#roledef" class="termref">rola</a> (przeznaczenie) <a title="definicja: możliwy do odczytania przez program komputerowy" href="#programmaticallydetermineddef" class="termref">mogą być odczytane przez program komputerowy</a>, a stan, właściwości oraz wartości, 
które mogą być ustawione przez użytkownika, mogą również być <a title="definicja: programowo ustawione" href="#programmaticallysetdef" class="termref">ustawione przez program komputerowy</a>; zawiadomienie o zmianach w tych elementach dostępne jest dla <a title="definicja: program użytkownika" href="#useragentdef" class="termref">programów użytkownika</a>, w tym <a title="definicja: technologie wspomagające (w rozumieniu tego dokumentu)" href="#atdef" class="termref">technologii 
wspomagających</a>. (Poziom A)

*Uwaga:* Powyższe kryterium sukcesu stosuje się głównie do autorów stron, którzy budują lub piszą swoje własne komponenty 
interfejsu użytkownika. Przykładowo, standardowe kontrolki HTML już spełniają to kryterium, jeśli użyte są zgodnie ze specyfikacją.

### 4.1.3 Komunikaty o stanie
W treści zaimplementowanej przy użyciu języków znaczników komunikaty o stanie mogą być programowo określane poprzez role lub właściwości, dzięki czemu mogą być prezentowane użytkownikowi za pomocą technologii wspomagających bez uzyskiwania fokusa.