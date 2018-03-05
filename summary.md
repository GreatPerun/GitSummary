# Git

### Podstawowe komendy

`git config --list` - wylistowuje aktualną konfiguracje

`git help funkcjonalność` lub `git funkcjonalność --help` - wyswietlenie helpa dotyczącego danej funkcjonalności


### Zarządzanie repo

Inicjacja repozytorium gita

    git init

Dodanie pliku/katalogu do śledzenia

    git add nazwa_pliku/ów

Usunięcie pliku/katalogu z śledzenia

    git rm nazwa_pliku

**Pro Tip:** Dodając na końcu flagę -A doda wszystkie pliki i katalogi znajdujące się w danej lokalizacji

Dodanie Commita

    git commit -m "wiadomość commita"

**Pro Tip:** Dodając flagę -a możemy pominąć poczekalnię gdyż wszystkie pliki zostaną zatwierdzone

Klonowanie repozytorium

    git clone URL/ścieżka_dostępu - klonuje repozytorium

**Pro Tip:** Po URLu można podać w jakim miejscu ma być zapisane repo, wstawiając kropkę zapiszę tam gdzie aktualnie się znajduje

Sprawdzanie stanu swoich plików

    git status

Rodzaje statusów plików
- Nieśledzony - plik nieznajdujący się w repo
- Niemodyfikowany - plik który znajduje się w repo ale nie został zmieniony
- Modyfikowany - plik znajdujący się w repo, zmieniony ale nie zacommitowany
- Zatwierdzone - pliki które zostały zatwierdzone i czekają w poczekalni na commita

`.gitignore` - plik definiujący pliki i katalogi które mają być pomijane przez repo

### Porównywanie plików

`git diff` - zwróci różnicę między plikami średzonym ale niezatwierdzonym (które nie zostały dodane do poczekalni)
`git diff --cached` - pokaże wszystkie zmiany które zostaną dodane do repo
`git diff --staged` - j.w.

### Podgląd historii

`git log` - wyświetla wszystkie commity

`git log -p` - wyświetli commity wraz z różnicami

`git log -2` - wyświetli dwa ostatnie commity

`git log --stat` - pokaże skróconą wersję historii

|Opcja   |Opis   |
|-----------|-----------|
|-p | Pokaż pod każdą zmianą powiązaną łatkę|
|--stat|Pokaż pod każdą zmianą statystyki zmodyfikowanych plików|
|--shortstat |Pokaż wyłącznie zmienione/wstawione/usunięte linie z polecenia --stat|
|--name-only|Pokaż pod każdą zmianą listę zmodyfikowanych plików|
|--name-status|Pokaż listę plików o dodanych/zmodyfikowanych/usuniętych informacjach.|
|--abbrev-commit|Pokaż tylko pierwsze kilka znaków (zamiast 40-tu) sumy kontrolnej SHA-1.|
|--relative-date|Pokaż datę w formacie względnym (np. 2 tygodnie temu)|
|--graph|Pokaż graf ASCII gałęzi oraz historię scaleń obok wyniku|
|--pretty|Pokaż zatwierdzone zmiany w poprawionym formacie. Dostępne opcje obejmują oneline, short, full, fuller oraz format (gdzie określa własny format)|



