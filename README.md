# tc-event-tool
Aplikacja do generowania list uczestników i zestawień 1×1 z pliku eventowego The Company. Wrzuć .xlsx → gotowe listy, badge i PDF-y po spotkaniu Grupy.
# the company. · Event Tools

Narzędzie dla koordynatorów Corporate Connections Poland do automatycznego 
generowania list i zestawień ze spotkań Grup.

## Co robi

**Listy uczestników**
Filtruje uczestników wg statusu (wszyscy / potwierdzeni / obecni / nieobecni) 
i wyświetla ich w widoku pełnym lub badge — gotowym do wydruku przed spotkaniem.
Eksport do CSV jednym kliknięciem.

**Zestawienia 1×1 po Grupie**
Dla każdego uczestnika generuje jego osobiste zestawienie spotkań 1×1 
z nazwiskiem partnera, firmą, branżą i godzinami. 
Druk dla jednej osoby lub wszystkich naraz — to co wcześniej zajmowało 
kilka godzin dwóch koordynatorów.

## Jak używać

1. Otwórz aplikację w przeglądarce
2. Przeciągnij plik eventowy `.xlsx` na stronę (lub kliknij i wybierz)
3. Dane wczytują się automatycznie — filtruj, drukuj, eksportuj

Działa w całości lokalnie w przeglądarce. Żadne dane nie są wysyłane 
na zewnętrzny serwer.

## Wymagania dotyczące pliku

Aplikacja odczytuje standardowy plik eventowy CC Poland z zakładkami:
- `PARAMETRY WYDARZENIA` — nazwa, data, miasto, grupa
- `Lista zaproszeń` — dane uczestników od wiersza 5
- `Odbyte 1x1` — pary spotkań od wiersza 3

## Technologie

Czysty HTML + JavaScript, zero backendu, zero instalacji.  
Plik xlsx odczytywany przez [SheetJS](https://sheetjs.com/) bezpośrednio w przeglądarce.
