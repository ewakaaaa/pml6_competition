# Konkurs 6 edycja kursu "Praktyczne uczenie maszynowe" - Walidacja

#### Cel to prognozowanie wartości zwrotu dla danego zamówienia.

#### Metryką sukcesu jest mean squared error.

#### Dane
W danych jest 1 067 371 wierszy, które zostały podzielone prawie na równe części:

train_online_retail (520 142 wierszy)
test_online_retail (547 229 wierszy)

#### Porównuje walidacje na:
- lokalnym na zbiorze testowym
- 30% danych testowych czyli "Public Leader Board" na Kaggle
- 70% danych testowych czyli "Private Leader Board"
- całym zbiorze testowym
