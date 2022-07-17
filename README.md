# CoProT
## Moja strona: [adam.szczecin.pl](https://www.adam.szczecin.pl)
### CoProT -> Competitive Programming Tool
Narzędzie do competitive programming (budowanie, uruchamianie na testach przykładowych, tworzenie projektów, etc.) napisane w Pythonie

w pliku conf.txt znajduje się konfiguracja według schematu:
* linia 1 -> CoProT uruchamia się w tej ścieżce
* ścieżka do pliku wykonywalnego Sublime Text
* coś co będzie wyświetlane jako autor kodu

objaśnienie komend:
* q / quit -> wychodzi z programu
* cd -> wyświetla aktualną ścieżkę; cd [path] -> zmienia aktualną ścieżkę na [path]
* ls / dir -> wyświetla zawartość folderu
* cls / clear -> czyści ekran terminala
* create (py/python)/(cpp/c++) [name] tworzy nowy projekt o strukturze:  
```
name
 |-samples
 |   |_
 |-o.sh
 |-wzor.py/cpp
 |-brut.py/cpp
 |-generator.py/cpp
 |_
```  
* cat -> wyświetla zawartość pliku
* open [dic=aktualna ścieżka] -> otwiera wy Sublime Text lub innym edytorze [dic] (plik lub ścieżkę)
* set [spec] [val] -> ustawia (do końca sesji) na [val]:
  * [spec] = subl/sublime -> ścieżkę do Sublime Text
  * [spec] = title -> tytuł okna
  * [spec] = author/autor -> autora kodów
* exec [com] -> wykonuje w bashu/batchu komendę [com]
* time [com] -> wykonuje w bashu/batchu komendę [com] i mierzy czas jej wykonania
* make [file] -> uruchamia (w c++ uruchamia i kompiluje) plik, dostępne rozszerzenia to cpp i py
* samples [file] -> instrukcja:  
```
- w katalogu "samples" umieścić wejścia do testów z rozszerzeniem ".in" (np.: "test1.in")
- w katalogu "samples" umieścić wyjścia do testów z rozszerzeniem ".out" (np.: "test1.out")

Nazwa wejścia musi zgadzać się z nazwą wyjścia do tego testu np.:
"test1.in" <- wejście do testu test1
"test1.out" <- wyjście do testu test1

uruchom komendę "smamples [file]", gdzie [file] to program, na którym zostaną wykonane testy i czekaj na wynik

samples uruchamia i w przypadku c++ kompiluje
```
* about/help -> wyświetla krótką informacje
* mkdir [dir] -> tworzy folder [dir]
* mkfile [file] -> tworzy nowy plik [file]
