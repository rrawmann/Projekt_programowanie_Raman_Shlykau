# Projekt_programowanie_Raman_Shlykau
Projekt zaliczeniowy 

# Teen Mental Health Analysis using Machine Learning

## Opis projektu

Projekt został wykonany w języku Python w środowisku Google Colab.
Celem projektu była analiza danych dotyczących zdrowia psychicznego nastolatków oraz przewidywanie występowania depresji przy użyciu modeli uczenia maszynowego.

W projekcie przeanalizowano zależności pomiędzy:

* poziomem stresu,
* poziomem lęku,
* długością snu,
* korzystaniem z platform społecznościowych,
  a występowaniem depresji.

Do budowy modeli wykorzystano:

* Logistic Regression,
* Random Forest Classifier.

---

## Wykorzystany zbiór danych

Dataset zawiera informacje dotyczące zdrowia psychicznego nastolatków, między innymi:

* poziomu stresu,
* poziomu lęku,
* liczby godzin snu,
* czasu spędzanego w mediach społecznościowych,
* poziomu uzależnienia od social media,
* używanych platform społecznościowych.

Zmiennej docelowej użytej do klasyfikacji nadano nazwę:

`depression_label`

gdzie:

* `0` oznacza brak depresji,
* `1` oznacza występowanie depresji.

---

## Wykorzystane biblioteki

W projekcie wykorzystano biblioteki:

* pandas,
* numpy,
* matplotlib,
* seaborn,
* scikit-learn.

---

## Etapy projektu

### 1. Wstępna analiza danych

Sprawdzono:

* strukturę danych,
* typy kolumn,
* statystyki opisowe,
* brakujące wartości.

---

### 2. Wizualizacja danych

W projekcie wykonano kilka wykresów:

* rozkład zmiennej docelowej,
* zależność poziomu stresu od depresji,
* zależność długości snu od depresji,
* zależność poziomu lęku od depresji,
* analiza korzystania z platform społecznościowych,
* mapa korelacji zmiennych numerycznych.

---

### 3. Przygotowanie danych

Dane zostały podzielone na:

* dane numeryczne,
* dane kategoryczne.

W preprocessingu wykorzystano:

* `StandardScaler`,
* `OneHotEncoder`,
* `Pipeline`,
* `ColumnTransformer`.

---

### 4. Trenowanie modeli

W projekcie zaimplementowano dwa modele:

* Logistic Regression,
* Random Forest Classifier.

---

### 5. Ocena modeli

Modele zostały ocenione przy użyciu:

* `classification_report`,
* accuracy,
* F1-score,
* recall,
* confusion matrix.

---

### 6. Optymalizacja hiperparametrów

Dla modelu Random Forest wykorzystano:

* `GridSearchCV`.

---

## Wyniki

Zbiór danych był mocno niezbalansowany, dlatego najważniejszymi metrykami były:

* recall,
* F1-score.

Lepsze wyniki osiągnął model Logistic Regression, który skuteczniej wykrywał przypadki depresji.

Random Forest osiągnął wysoką accuracy, jednak wykrywał mniej przypadków pozytywnych.

---

## Najważniejsze wnioski z analizy danych

Analiza danych pokazała, że:

* osoby z depresją osiągały wyższe poziomy stresu,
* osoby z depresją osiągały wyższe poziomy lęku,
* osoby z depresją spały średnio mniej godzin,
* większa aktywność w mediach społecznościowych może być związana z częstszym występowaniem depresji.

---

## Uruchomienie projektu

Projekt został przygotowany w Google Colab.

Notebook automatycznie pobiera dane przy użyciu komendy:

`wget`

Dzięki temu projekt można uruchomić bez ręcznego dodawania pliku CSV.

---

## Autor

Raman Shlykau

