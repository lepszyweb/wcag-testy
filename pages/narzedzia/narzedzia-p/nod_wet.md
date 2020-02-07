---
title: WET - Web Evaluation Tools
summary:
tags: [rozszerzenia_przeglądarek, skryptozakładka,narzędzia_oceny_dostępności]
sidebar: narzedzia-sidebar
permalink: nod_wet
folder: narzedzia-p
---

Web Evaluation Tools bookmarklet to zestaw 10 narzędzi pomagających zbadać i ocenić dostępność strony internetowej. Narzędzie przeznaczone jest dla osób, które dysponują podstawową wiedzą o dostępności.

## Dane źródłowe
- **Autor:** IT Accessibility z [NC State University](https://accessibility.oit.ncsu.edu/)
- **Źródło**: [Web Evaluation Tools Bookmarklet](https://accessibility.oit.ncsu.edu/tools/web-evaluation-tools/)

## Stosowanie
Aby korzystać z narzędzia, dodaj do zakładek w swojej przeglądarce następujący link: [Web Evaluation Tools](javascript:%20(function()%7Bvar%20yourURL=(window.location.protocol=='http:'?'http://webapps.ncsu.edu/web-evaluation-tools/web-evaluation-tools.php':'https://webapps.ncsu.edu/web-evaluation-tools/web-evaluation-tools.php');function%20getScript(url,success)%7Bvar%20script=document.createElement('script');script.src=url;var%20head=document.getElementsByTagName('head')%5B0%5D,done=false;script.onload=script.onreadystatechange=function()%7Bif(!done&&(!this.readyState%7C%7Cthis.readyState=='loaded'%7C%7Cthis.readyState=='complete'))%7Bdone=true;success();script.onload=script.onreadystatechange=null;head.removeChild(script);%7D%7D;head.appendChild(script);%7D%20getScript(yourURL,function()%7B%7D);%7D)();)

**Uwaga:** Aby narzędzie działało w Twojej przeglądarrce, nie wystarczy kliknięcie powyższego łącza. Musisz dodać link do zakładek, przeciągając go do menu zakładek lub używając menu kontekstowego przeglądarki.

Aby uaktywnić skryptozakładkę na przeglądanej stronie, klikamy w menu zakładek jej łącze, co spowoduje, że przy górnej krawędzi okna przeglądarki zostanie wyświetlony pasek narzędziowy z 10 polami wyboru i etykietami. Obok etykiety wyświetlana jest liczba wystąpień danego obiektu na stronie. Zaznaczenie pola spowoduje wyróżnienie zaznaczonych elementów. Odznaczenie pola wyboru spowoduje usunięcie wskazówek wizualnych ze strony. Równocześnie można zaznaczyć wiele elementów.

![Pasek narzędzi skryptozakładki WET](/images/narzedzia/wet.png)

Za pomocą narzędzi na badanej stronie możemy zobaczyć właściwości niewidoczne bez dokładniejszej analizy albo wręcz niewidoczne.

- **Headings** - wyróżnia nagłówki, w tym tekst ukrytych etykiet,
- **ARIA Landmarks** - wyróżnia punkty orientacyjne wraz z etykietami, jeśli istnieją (nie wyróżnia obszarów oznaczonych atrybutem role="region"),
- **Aria Roles** - wyróżnia obiekty z jawnie określonymi atrybutami role, innymi niż punkty orientacyjne, a także obszary z atrybutem role="region",
- **ARIA Attributies** - wyróżnia obiekty z oznaczonymi atrybutami ARIA i wartości tych atrybutów,
- **Tabindex** - wyróżnia obiekty z oznaczonym atrybutem tabindex, podaje wartość atrybutu,
- **Internal Link** - wyróżnia łącza wewnętrzne, prowadzące do miejsc na stronie, zarówno ich źródło, jak i cel. Jeśli określono dla łącza atrybut *tabindex*, podaje jego wartość, jeśli nie określono, komunikuje brak atrybutu (*missing tabindex*), ale nie jest to bład.
- **Cross Site Content** - wyróżnia obszary zawartości pochodzące z innych witryn (np. reklamy),
- **Force Show Visual Focus** - wymusza widoczność fokusa (punktów uwagi),
- **High Contrast CSS** - przełącza widok w tryb wysokiego kontrastu,
- **Language Attributes** - wyróżnia części strony z oznaczonym atrybutem języka i wartość atrybutu.

**Uwaga**: za każdym razem, gdy aktywujesz ten bookmarklet, zostanie załadowana najnowsza wersja kodu, więc nie musisz aktualizować tego bookmarkletu w przyszłości.