## 3-3-4 Zapobieganie błędom 
(kontekst prawny, finansowy, związany z podawaniem danych)
**Czy serwis posiada odpowiednie zabezpieczenia przed popełnieniem błędów o konsekwencjach prawnych, finansowych lub związanych z wprowadzaniem i modyfikowaniem danych?**

### Wyjaśnienie
Jeżeli w serwisie internetowym użytkownik dokonuje transakcji finansowych, pojawiają się zobowiązania prawne (zawieranie umów) lub można wprowadzać i modyfikować dane, to powinny zostać zaprojektowane odpowiednie zabezpieczenia przed popełnieniem błędów.
Zabezpieczenia są trojakiego rodzaju:
-	Wprowadzone dane można odwołać i przywrócić stare po stwierdzeniu błędu.
-	Dane są sprawdzane pod kątem błędów, a użytkownik ma możliwość ich poprawienia.
-	Dane można sprawdzić i potwierdzić przed ostatecznym wysłaniem na serwer.
Mechanizmy takie są stosowane w bankowości elektronicznej i w większości sklepów internetowych. Zazwyczaj w systemie istnieje mechanizm wstępnego sprawdzenia błędów, a następnie wyświetlany jest ekran z podsumowaniem, które użytkownik może przejrzeć i ostatecznie zaakceptować. Niezbyt często implementowane jest przywracanie starych danych po popełnieniu błędu.

### Testowanie
W pierwszej kolejności musisz sprawdzić, czy w serwisie internetowym użytkownik wprowadza dane mające kontekst prawny, finansowy lub związany z wprowadzaniem i modyfikowaniem danych. Z całą pewnością są to serwisy bankowości elektronicznej, sklepy internetowe, ale także wszystkie, w których zawierane są umowy i podawane dane osobowe, choćby nawet tylko składające się z adresu e-mail. Jeżeli serwis spełnia te warunki, to trzeba sprawdzić, czy przy wprowadzaniu danych zastosowano przynajmniej jeden z poniższych mechanizmów:
-	Wprowadzone dane można odwołać i przywrócić stare po stwierdzeniu błędu.
-	Dane są sprawdzane pod kątem błędów, a użytkownik ma możliwość ich poprawienia.
-	Dane można sprawdzić i potwierdzić przed ostatecznym wysłaniem na serwer.

