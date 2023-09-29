## 10-delegations-calculator

Należy zaimplementować kalkulator kwoty przysługującej za delegację pracowniczą: klasa `Calc`, metoda `calculate`.

Dane testowe znajdują się w pliku `src/test/resources/delegations.csv`

Parametry:
* start: początek delegacji, w formacie `yyyy-mm-dd HH:MM timezone`
* end: koniec delegacji, w formacie `yyyy-mm-dd HH:MM timezone`
* dailyRate: stawka dzienna za delegację.

Dane testowe zawierają dodatkowo kolumnę expected, w której znajduje się oczekiwany wynik obliczeń.


Zasady obliczania delegacji:
* za pełną dobę - przysługuje pełna stawka dzienna,
* do 8 godzin - przysługuje 1/3 stawki dziennej,
* ponad 8 do 12 godzin - przysługuje 1/2 stawki dziennej,
* ponad 12 godzin - przysługuje pełna stawka dzienna,
* jeśli czas rozpoczęcia jest późniejszy lub taki sam jak czas końcowy, przysługuje 0.

