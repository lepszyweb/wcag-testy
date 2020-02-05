---
title: Obsługiwane funkcje
tags:
  - getting_started
keywords: "features, capabilities, scalability, multichannel output, dita, hats, comparison, benefits"
last_updated: "July 16, 2016"
summary: "Jeśli nie masz pewności, czy Jekyll i ten motyw będą obsługiwać Twoje wymagania, ta lista zawiera pół kompleksowy przegląd dostępnych funkcji."
published: true
sidebar: mydoc_sidebar
permalink: mydoc_supported_features.html
folder: mydoc
---

Zanim zaczniesz eksplorować Jekyll jako potencjalną platformę dla treści pomocy, możesz zastanawiać się, czy obsługuje on niektóre podstawowe funkcje potrzebne do spełnienia wymagań twojego dokumentu technicznego. Poniższa tabela pokazuje, co jest obsługiwane w Jekyll i tym temacie.



## Obsługiwane funkcje

Funkcje | Obsługa | Uwagi
--------|-----------|-----------
Ponowne wykorzystanie treści | Tak | Obsługuje ponowne użycie za pośrednictwem Liquid. Możesz ponownie używać zmiennych, fragmentów kodu, całych stron i innych. W DITA speak obejmuje to conref i keyref. Aby uzyskać więcej informacji, zobacz[Ponowne wykorzystanie treści][mydoc_content_reuse] for more details.|
Markdown | Tak | Możesz tworzyć treści przy użyciu składni Markdown, w szczególności [kramdown](https://kramdown.gettalong.org/). Jest to podobna do wiki składnia HTML, którą prawdopodobnie można pobrać w ciągu 10 minut. Tam, gdzie nie ma Markdown, możesz użyć HTML. Tam, gdzie brakuje HTML, używasz Liquid, czyli skryptu, który pozwala na zastosowanie bardziej zaawansowanej logiki.|
Elastyczny układ | Tak | Wykorzystuje [framework Bootstrap](http://getbootstrap.com/)  do responsywnego projektowania.
Tłumaczenie | Tak | Aby przetłumaczyć treść, wyślij wygenerowany kod HTML do grupy tłumaczącej. Możesz przetłumaczyć źródło Markdown, jeśli twój tłumacz akceptuje format, ale zwykle Markdown jest problematyczny. Pamiętaj, że ten motyw nie jest dobrze skonstruowany, aby pomieścić projekty tłumaczeniowe.|
Współpraca | Tak | Współpracujesz z projektami Jekyll w taki sam sposób, jak programiści współpracują z projektami oprogramowania. (Nie potrzebujesz CMS.) Ponieważ pracujesz z formatami plików tekstowych, możesz używać dowolnego oprogramowania do kontroli wersji (Git, Mercurial, Perforce, Bitbucket itp.) Jako CMS dla swoich plików.|
Skalowalność | Tak | Twoja strona może być skalowana do dowolnego rozmiaru. Od Ciebie zależy, jak zaprojektujesz architekturę informacji dla swoich stron. Możesz wybrać, co wyświetlasz na pierwszym, drugim, trzecim, czwartym i więcej poziomach itd. Pamiętaj, że gdy twój projekt ma tysiące stron, czas kompilacji będzie dłuższy (może 1 minuta na tysiąc stron?). To zależy od tego, ile masz pętli iterujących po stronach. Zalecam stosowanie mniejszych repozytoriów. [mniejszych repozytoriów](http://idratherbewriting.com/2017/05/26/big-repos-versus-small-repos/)  w architekturze treści. |
Lekka architektura | Tak | Nie potrzebujesz architektury stosu LAMP (Linux, Apache, MySQL, PHP), aby uruchomić witrynę. Cały proces budowy odbywa się na własnym komputerze, a następnie wypychasz statyczne pliki HTML na serwer.|
Skinnability | Tak | Możesz skorygować swoją witrynę Jekyll, aby wyglądała identycznie jak każda inna strona internetowa. Jeśli masz zespół UX, mogą naprawdę skórować i projektować witrynę przy użyciu wszystkich narzędzi znanych współczesnemu projektantowi - JavaScript, HTML5, CSS, jQuery i innych. Jekyll jest oparty na nowoczesnym stosie do tworzenia stron internetowych, a nie na stosie XML (XSLT, XPath, XQuery). Zobacz [ten samouczek](http://jekyllrb.com/tutorials/convert-site-to-jekyll/) , aby uzyskać szczegółowe informacje na temat tworzenia własnego motywu Jekyll. |
Support | Tak | Społeczność Twojej witryny Jekyll to nie tyle inni pisarze technologii (jak w przypadku DITA), ale raczej szersza społeczność programistów. [Jekyll Talk](http://talk.jekyllrb.com) to świetny zasób. Podobnie [Stack Overflow](https://stackoverflow.com/questions/tagged/jekyll). Zobacz sekcję [Uzyskiwanie pomocy](http://jekyllrb.com/help/)  w Jekyll. |
Blogowanie | Tak | Istnieje prosta funkcja blogowania. To pojawia się jako [news](news.html) i ma na celu promowanie wiadomości, które dotyczą różnych produktów.|
Wersjonowanie| Tak | Jekyll nie zmienia wersji twoich plików. Przesyłasz swoje pliki do systemu kontroli wersji, takiego jak Github. Twoje pliki są tam wersjonowane.|

PC platform | Tak | Jekyll działa na systemie Windows. Chociaż doświadczenie w pracy z wierszem poleceń jest lepsze na komputerze Mac, system Windows również działa, zwłaszcza teraz, gdy Jekyll 3.0 porzucił zależności w Pythonie, które domyślnie nie były dostępne w systemie Windows.|
Wtyczki jQuery | Tak | Możesz używać dowolnych wtyczek jQuery i innych narzędzi JavaScript, CMS lub szablonów. Pamiętaj jednak, że jeśli używasz wtyczek Ruby, nie możesz bezpośrednio hostować plików źródłowych na stronach Github, ponieważ strony Github nie zezwalają na wtyczki Ruby. Zamiast tego możesz po prostu wypchnąć dane wyjściowe na dowolny serwer WWW. Jeśli nie planujesz korzystać ze stron Github, nie ma żadnych ograniczeń dla jakichkolwiek wtyczek jakiegokolwiek rodzaju. Jekyll sprawia, że ​​bardzo łatwo jest zintegrować każdy rodzaj wtyczki, jaki można sobie wyobrazić. Ten motyw nie używa żadnych wtyczek, więc możesz publikować w Github, jeśli chcesz.|
Integracja z Bootstrapem | Tak | Ten motyw jest oparty na [Bootstrap](http://getbootstrap.com/). Jeśli nie wiesz, czym jest Bootstrap, w zasadzie oznacza to, że istnieją setki gotowych komponentów, stylów i innych elementów, które możesz po prostu wrzucić na swoją stronę. Na przykład responsywna jakość strony pochodzi z bazy kodu Bootstrap.|

Szybkie ładowanie stron| Tak | To jedna z mocnych stron Jekylla. Ponieważ pliki są statyczne, ładują się niezwykle szybko, około 0,5 sekundy na stronę. Nie da się tego pokonać pod względem wydajności. (Witryna zwykle oparta na bazie danych, taka jak WordPress, ma średnio około 2,5 + sekund ładowania na stronę.) Ponieważ wszystkie strony są statyczne, oznacza to, że są również wyjątkowo bezpieczne. Nie zostaniesz zhakowany jak na stronie WordPress.
Themes | Tak | Możesz mieć różne motywy dla różnych wyników. Jeśli znasz CSS, tworzenie zarówno stron internetowych, jak i wydruków jest dość łatwe.
Open source | Tak | Ten motyw jest całkowicie otwarty. Każdy fragment kodu jest otwarty, widoczny i można go edytować. Pamiętaj, że ta otwartość ma swoją cenę - łatwo wprowadzić zmiany, które łamią motyw lub w inny sposób powodują błędy.
Oglądanie offline | Tak | W tym motywie zastosowano łączenie względne, dzięki czemu można przeglądać zawartość offline i na dowolnym serwerze internetowym bez konfigurowania adresów URL i baseurls w pliku konfiguracyjnym.


## Funkcje niedostępne

Następujące funkcje nie są dostępne..

Funkcja | Obsługa | Uwagi
--------|-----------|-----------
Interfejs CMS | No | W przeciwieństwie do WordPressa nie logujesz się do interfejsu i nie przechodzisz do swoich plików. Pracujesz z plikami tekstowymi i dynamicznie przeglądasz witrynę w przeglądarce. Nie martw się - to część uproszczenia, która sprawia, że ​​Jekyll jest niesamowity. Polecam używanie WebStorm jako edytora tekstu.
Interfejs WYSIWYG | No | Używam WebStorm do tworzenia treści, ponieważ lubię pracować w formatach plików tekstowych. Możesz jednak użyć dowolnego edytora Markdown (np. Lightpaper dla komputerów Mac, Marked) do tworzenia treści.
Różne wyjścia | No | Ten motyw zapewnia pojedyncze wyniki witryny zawierające dokumentację dotyczącą wielu produktów. W przeciwieństwie do poprzednich iteracji motywu nie jest przeznaczony do obsługi różnych wyników z tej samej treści. Możesz jednak z łatwością to skonfigurować, tworząc po prostu wiele plików konfiguracyjnych i uruchamiając różne kompilacje dla każdego pliku konfiguracyjnego.
Solidne wyszukiwanie | No | Funkcja wyszukiwania to uproszczone wyszukiwanie JSON. Aby uzyskać bardziej niezawodne wyszukiwanie, należy zintegrować Swiftype lub Algolię. Jednak usługi te nie są obecnie zintegrowane z kompozycją.
Standardowe szablony | No | Możesz tworzyć strony o dowolnej strukturze. Motyw nie wymusza typów tematów, takich jak zadanie lub koncepcja, jak specyfikacja DITA.
Integracja z | No | Możesz połączyć się z wyjściem SwaggerUI, ale nie ma wbudowanej integracji SwaggerUI z tym motywem dokumentacji.
Szablony dla punktów końcowych | No | Chociaż statyczne generatory witryn działają dobrze z dokumentacją API, nie ma żadnych wbudowanych szablonów specyficznych dla punktów końcowych w tym motywie. Możesz jednak zbudować własny.
Wyjście eBooka | No | Brak treści eBook dla treści.

{% include links.html %}
