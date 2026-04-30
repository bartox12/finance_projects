# Analiza Value at Risk (VaR) dla Kursów Walut

Projekt skupia się na estymacji ryzyka rynkowego dla pary walutowej **USD/GBP** przy wykorzystaniu różnych modeli statystycznych. Celem jest porównanie skuteczności popularnych metod wyznaczania VaR oraz ich walidacja za pomocą backtestingu.

## Wykorzystane Metody VaR:
* **Parametryczna:** przy założeniu rozkładu normalnego oraz rozkładu t-Studenta.
* **Historyczna:** klasyczna symulacja historyczna oraz metoda ważona wykładniczo (WHS).
* **Filtrowana (GARCH-HS):** połączenie modelu zmienności GARCH(1,1) z symulacją historyczną.
* **Monte Carlo:** symulacje oparte na wielowymiarowym rozkładzie t-Studenta.

## Funkcjonalności:
* Pobieranie aktualnych danych finansowych z biblioteki `yfinance`.
* Obliczanie VaR na poziomach ufności 95% i 99% w oknie kroczącym (rolling window).
* **Backtesting:** weryfikacja modeli poprzez statystyczny **Test Kupca (LR)**.
* Wizualizacja wyników: wykresy zwrotów z nałożonymi liniami VaR oraz histogramy przekroczeń.

## Technologie:
Python (pandas, numpy, matplotlib, scipy, arch, yfinance).

# Optymalizacja Portfela Inwestycyjnego (Model Markowitza)

Projekt poświęcony nowoczesnej teorii portfelowej (MPT) oraz analizie ryzyka dla wybranych aktywów finansowych (**XLF** – sektor finansowy, **GLD** – złoto). Aplikacja przeprowadza pełny proces selekcji i oceny portfela w oparciu o historyczne stopy zwrotu.

## Główne Funkcjonalności:
* **Analiza Statystyczna:** Pobieranie danych z `yfinance`, obliczanie rocznych stóp zwrotu, wariancji oraz macierzy korelacji.
* **Granica Efektywna (Efficient Frontier):** Generowanie tysięcy losowych portfeli (metoda Monte Carlo) w celu znalezienia optymalnej relacji zysku do ryzyka.
* **Portfele Specjalne:** Automatyczne wyznaczanie portfela o **minimalnej zmienności** oraz portfela o **maksymalnym wskaźniku Sharpe'a**.
* **Linia Rynku Kapitałowego (CML):** Integracja portfela rynkowego z aktywami wolnymi od ryzyka (rentowność obligacji skarbowych pobierana z bazy FRED).
* **Szacowanie Ryzyka VaR:** Kalkulacja Value at Risk (VaR 95% i 99%) metodą wariancji-kowariancji dla wybranych strategii.

## Wykorzystane Technologie:
Python (Pandas, NumPy, Matplotlib, SciPy, Pandas_datareader).
