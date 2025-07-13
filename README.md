# Adult Census Income - Analiza Przewidywania Dochodów

## Opis projektu
Projekt analizy danych Adult Census Income, mający na celu przewidywanie czy osoba zarabia więcej niż $50,000 rocznie na podstawie cech demograficznych i społeczno-ekonomicznych.

## Cel
Stworzenie modelu machine learning do klasyfikacji binarnej dochodów osób na podstawie danych z amerykańskiego spisu powszechnego.

## Dataset
- **Źródło**: Adult Census Income Dataset kaggle: https://www.kaggle.com/datasets/uciml/adult-census-income/data
- **Liczba próbek**: ~32,000+ rekordów
- **Cechy**: 14 zmiennych (wiek, wykształcenie, zawód, status małżeński, itp.)
- **Zmienna docelowa**: Dochód (<=50K lub >50K)

## Technologie
- **Python** - język programowania
- **Pandas** - manipulacja danymi
- **Scikit-learn** - machine learning
- **XGBoost** - zaawansowane modele ensemble
- **Matplotlib/Seaborn** - wizualizacje
- **Jupyter Notebook** - środowisko analizy

## Struktura analizy
1. **Eksploracyjna analiza danych (EDA)**
   - Przegląd danych i statystyki opisowe
   - Analiza rozkładu zmiennej docelowej
   - Macierz korelacji zmiennych numerycznych

2. **Preprocessing danych**
   - Usunięcie brakujących wartości
   - Kodowanie zmiennej docelowej
   - Standaryzacja i one-hot encoding

3. **Analiza wizualna**
   - Rozkład wieku według grup dochodowych
   - Analiza najważniejszych predyktorów
   - Wykrycie wzorców w danych

4. **Modelowanie ML**
   - **Logistic Regression** - model bazowy
   - **Random Forest** - ensemble drzew
   - **Gradient Boosting** - boosting
   - **XGBoost** - zaawansowany gradient boosting

5. **Ewaluacja modeli**
   - Porównanie Accuracy i AUC
   - Confusion Matrix najlepszego modelu
   - Analiza Feature Importance

## Wyniki
- **Najlepszy model**: XGBoost
- **Accuracy**: 87,4%
- **AUC**: 93,4%
- **Najważniejsze cechy**: wiek, wykształcenie, godziny pracy, status małżeński

## Kluczowe wnioski
- Osoby z wyższym wykształceniem mają większe szanse na wysokie dochody
- Wiek jest istotnym predyktorem - szczyt zarobków w wieku 46-55 lat
- Status małżeński znacząco wpływa na poziom dochodów
- Liczba godzin pracy tygodniowo koreluje z wysokością zarobków

## Jak uruchomić
1. Sklonuj repozytorium
2. Zainstaluj wymagane biblioteki: `pip install pandas scikit-learn xgboost matplotlib seaborn`
3. Pobierz dataset `adult.csv`
4. Uruchom notebook `Adult-Census-Income.ipynb`

## Pliki
- `Adult-Census-Income.ipynb` - główny notebook z analizą
- `adult.csv` - dataset (do pobrania)
- `README.md` - ten plik

## Autor 
Franciszek Łasiński
Projekt w ramach nauki machine learning i analizy danych.

