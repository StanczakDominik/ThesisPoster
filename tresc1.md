
Dominik Stańczak, Politechnika Warszawska (stanczakdominik@gmail.com)
Dr Sławomir Jabłoński, Instytut Fizyki Plazmy i Laserowej Mikrosyntezy

# Intro

Jednym z najpowszechniejszych rodzajów prowadzenia symulacji w fizyce plazmy
są symulacje **Particle-in-Cell** (dalej zwane PIC), łączące rozwiązywanie równań
Maxwella na dyskretnych siatkach z ewolucją czasową gęstości ładunku i prądu
w układzie prowadzoną poprzez iterowanie równań **makrocząstek** odpowiadających
grupom rzeczywistym.

Tradycyjnie symulacje tego typu wykonywane są w językach niskopoziomowych,
jak C i Fortran. Te zaś są jednak trudne w obsłudze, utrzymaniu i ponownym
wykorzystaniu. Alternatywnym podejściem jest wykorzystanie
języków wysokopoziomowych, jak **Python**, zdolnych do zbliżenia się do poziomów
wydajności reprezentowanych przez poprzednio wymienione języki  poprzez
odwołania do bibliotek implementujących zoptymalizowane operacje na wektorach
bądź tablicach wielowymiarowych (*Numpy*) bądź kompilację Just-In-Time (*Numba*).

Bieżąca praca polega na implementacji w Pythonie przykładowego programu Particle-in-Cell
realizującego jednowymiarową symulację interakcji wiązki laserowej z tarczą wodorową, wraz
z pomniejszymi symulacjami elektrostatycznymi pełniącymi rolę przypadków testowych
poszczególnych elementów algorytmu.

## Wykresy

* Niefizyczna niestabilność siatki wynikająca ze zbyt małej dokładności numerycznej przyjętych parametrów
* Niestabilność dwóch strumieni zimnej plazmy, silnie powiązana z niestabilnością Kelvina-Helmholtza.
* Symulacja interakcji tarczy wodorowej z wiązką lasera
    * Spłaszczenie
    * Rozbicie
