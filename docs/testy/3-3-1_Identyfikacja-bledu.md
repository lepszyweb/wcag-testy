## 3-3-1 Identyfikacja błędu

**Czy błędy popełnione przez użytkownika, a wykryte przez serwis internetowy, są prezentowane użytkownikowi w postaci komunikatu tekstowego?**

### Wyjaśnienie
Użytkownicy dosyć często wprowadzają w serwisach internetowych dane. Są to okna logowania, formularze danych teleadresowych i wiele innych. W takich systemach błędy popełniane przez użytkowników są często wykrywane automatycznie, a użytkownik jest o nich informowany. Najpopularniejszym sposobem jest oznaczanie błędnych danych kolorem, co nie jest wystarczające. Użytkownik powinien otrzymać informację o tym gdzie i jaki błąd popełnił, a informacja taka powinna być zaprezentowana w postaci tekstowej. Może to być na przykład komunikat "Nie wpisałeś numeru telefonu", "login lub hasło są nieprawidłowe", czy "Musisz zaznaczyć przynajmniej jeden produkt".

### Testowanie
Przyjrzyj się formularzom służącym do wprowadzania danych przez użytkowników. Wprowadź w różnych miejscach błędne dane (zły format daty, opuszczenie pola obowiązkowego, spacje w haśle itp.) Jeżeli o wszystkich błędach otrzymujesz informację w postaci tekstowej, to formularz spełnia to kryterium.
