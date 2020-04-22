# dw_competition_6

Konkurs | 6 edycja kursu "Praktyczne uczenie maszynowe" - Dlaczego tak ważna jest walidacja?
Cel:
Prognozowanie wartości zwrotu dla danego zamówienia.

Na czym polega konkurs?
Jest sklep online, który sprzedaje różne produkty dla ludzi z różnych krajów. Jedno zamówienie (faktura) może zawierać więcej niż jeden produkt. Trend, który jest dość popularny w szczególności w krajach zachodnich, to możliwość zwrotów i klienci chętnie z tego korzystają. Zwroty generują koszty i warto umieć przewidzieć to i jakoś z tym podziałać (pomijając skrajne przypadki takie jak "nie sprzedawać" klientowi X, bo to pewnie jest zakazane prawem). Natomiast pewnie dałoby się coś zrobić, jeśli wiedzielibyśmy, które zamówienia mogą być z dużym prawdopodobieństwem zwrócone.

To zadanie można podzielić na 2 części: z jednej strony jest to klasyfikacja, ponieważ ostatecznie trzeba stwierdzić, czy ten produkt będzie zwrócony czy nie. Z drugiej strony (i to jest docelowe zadanie) przez to, że zamówienie może zawierać więcej niż jeden produkt, to ostatecznie chcemy obliczyć sumaryczny koszt zwrotów. Możesz założyć, że jeśli w danym złożonym i opłaconym zamówieniu jest zwrot nawet jednego produktu, to zwracana jest całość zamówienia (czyli wszystkie produkty zawarte w tym zamówieniu). Suma cen tych produktów daje całkowitą wartość zwrotu, właśnie to będziemy przewidydwać.

Metryką sukcesu
będzie mean squared error.

Dane
W danych jest 1 067 371 wierszy, które zostały podzielone prawie na równe części:

train_online_retail (520 142 wierszy)
test_online_retail (547 229 wierszy)
Walidacja
lokalna na zbiorze testowym
na 30% danych testowych czyli "Public Leader Board" na Kaggle
na 70% danych testowych czyli "Private Leader Board"
na całym zbiorze testowym
