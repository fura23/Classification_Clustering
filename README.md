# Klasyfikacja i analiza skupień w R

## Opis projektu
Projekt stanowi rozwiązanie zadania akademickiego z zakresu klasyfikacji oraz analizy skupień w języku R.

Celem projektu jest porównanie kilku metod klasyfikacyjnych dla zmiennych `X` i `Y` przy klasach wyznaczonych przez zmienną `Z`, a także przeprowadzenie analizy skupień dla zmiennych `A` i `B` z wykorzystaniem różnych metod grupowania.

## Zakres projektu

Projekt obejmuje pięć głównych części:

### 1. Estymator jądrowy gęstości
Dla każdej klasy zmiennej `Z` wyznaczono dwuwymiarowy estymator jądrowy gęstości opisujący rozkład zmiennych `X` i `Y`.

Na podstawie otrzymanych gęstości:
- wyznaczono obszary klasyfikacji,
- przygotowano odpowiedni rysunek,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji `n`-krotnej,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji 10-krotnej.

Kod do wyznaczania procentu poprawnej klasyfikacji w kroswalidacji dla tej części został napisany samodzielnie, bez użycia gotowej funkcji.

### 2. Metoda k najbliższych sąsiadów
Dla różnych wartości parametru `k` zastosowano metodę k najbliższych sąsiadów do klasyfikacji obserwacji na podstawie zmiennych `X` i `Y`.

Dla tej metody:
- wyznaczono obszary klasyfikacji,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji `n`-krotnej,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji 10-krotnej.

### 3. Drzewa klasyfikacyjne i las losowy
W projekcie wykorzystano również:
- drzewa klasyfikacyjne,
- las losowy.

Dla obu metod:
- wyznaczono obszary klasyfikacji,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji `n`-krotnej,
- obliczono procent poprawnej klasyfikacji metodą kroswalidacji 10-krotnej.

Dodatkowo narysowano drzewo klasyfikacyjne dla parametrów dających najwyższy procent poprawnej klasyfikacji.

### 4. Porównanie metod klasyfikacji
Porównano wyniki uzyskane dla:
- estymatora jądrowego gęstości,
- metody k najbliższych sąsiadów,
- drzew klasyfikacyjnych,
- lasu losowego.

Porównanie oparto na procentach poprawnej klasyfikacji otrzymanych w różnych wariantach kroswalidacji.

### 5. Analiza skupień
Dla zmiennych `A` i `B` przeprowadzono analizę skupień trzema metodami:
- k-średnich,
- DBSCAN,
- mieszanin rozkładów normalnych (algorytm EM).

W ramach tej części:
- analizowano liczbę klastrów na podstawie wartości `total withinss`,
- przedstawiono podział obserwacji na klastry na wykresach,
- oceniono jakość grupowania wizualnie oraz za pomocą poznanych miar,
- porównano skuteczność zastosowanych metod.

## Wykorzystane metody i biblioteki

Projekt został przygotowany w języku R z wykorzystaniem wybranych bibliotek, na przykład:
- `MASS`
- `ks`
- `class`
- `rpart`
- `rpart.plot`
- `randomForest`
- `dbscan`
- `mclust`
- `ggplot2`
- `dplyr`
- `caret` lub innych pomocniczych pakietów

Zakres użytych pakietów może się różnić w zależności od ostatecznej implementacji.

## Zawartość repozytorium
- `README.md` — opis projektu,
- `classification_clustering.Rmd` — kod projektu,
- `dane27.csv`,`Anxiety.csv` — dane wejściowe,
- `opis_Anxiety.csv` - opis danych,
- `classification_clustering.html` — raport końcowy z wynikami, wykresami i interpretacją.


## Wyniki
W projekcie analizowano:
- jakość klasyfikacji dla różnych metod,
- wpływ parametrów modeli na skuteczność klasyfikacji,
- zgodność wyników uzyskanych w kroswalidacji `n`-krotnej i 10-krotnej,
- jakość podziału na klastry dla różnych metod grupowania.

## Wnioski
Projekt umożliwia porównanie metod klasyfikacyjnych i metod analizy skupień dla danych dwuwymiarowych.

Szczególny nacisk położono na:
- interpretację obszarów klasyfikacji,
- porównanie procentu poprawnej klasyfikacji,
- ocenę jakości klastrów,
- wskazanie metody dającej najlepsze wyniki.

## Autor
Projekt wykonany w ramach zadania akademickiego w języku R.

## License
This project is provided for viewing, downloading, running, and private modification only.
Redistribution, republication, commercial use, and claiming authorship or ownership are prohibited without prior written permission from the author.
