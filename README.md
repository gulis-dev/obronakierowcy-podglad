# Podgląd serwisu ObronaKierowcy.pl

Zrzut statyczny do obejrzenia treści i wyglądu przed kupnem domeny.

**Tego katalogu się nie edytuje.** Powstaje w całości z repozytorium
`obronakierowcy-pl` poleceniem `php narzedzia/eksport-podgladu.php`,
a każdy kolejny eksport nadpisuje zawartość.

Czego tu nie ma i nie będzie:

- **formularz zapytania** - to są pliki statyczne, nie ma PHP. W jego miejscu
  stoi informacja, że to podgląd, żeby nikt nie wysłał opisu sprawy w próżnię,
- **statystyka odwiedzin**,
- **nagłówki bezpieczeństwa** (CSP, HSTS) - wysyła je PHP i `.htaccess`
  na docelowym serwerze.

Każda podstrona ma `noindex, nofollow`, a `robots.txt` zabrania wszystkiego.
Powód: zaindeksowany podgląd pod adresem `github.io` konkurowałby z docelową
domeną o te same frazy.

Zrzut z dnia: 2026-09-06.