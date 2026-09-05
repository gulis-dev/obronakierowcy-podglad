# Podgląd serwisu ObronaKierowcy.pl

Zrzut statyczny do obejrzenia treści i wyglądu przed kupnem domeny.
Generowany z repozytorium `obronakierowcy-pl` poleceniem
`php narzedzia/eksport-podgladu.php`, więc **nie edytuje się go tutaj** —
każdy kolejny eksport nadpisuje całą zawartość.

Czego tu nie ma i nie będzie:

- **formularz zapytania** — to są pliki statyczne, nie ma PHP. W miejscu
  formularza stoi informacja, że to podgląd, żeby nikt nie wysłał opisu
  sprawy w próżnię,
- **statystyka odwiedzin**,
- **nagłówki bezpieczeństwa** (CSP, HSTS) — wysyła je PHP i `.htaccess`
  na docelowym serwerze.

Każda podstrona ma `noindex, nofollow`, a `robots.txt` zabrania wszystkiego.
Powód: zaindeksowany podgląd pod adresem `github.io` konkurowałby
z docelową domeną o te same frazy.
