Zadanie polega na przewidywaniu liczby wypożyczonych rowerów/hulajnóg w danym mieście. Do dyspozycji mamy informacje historyczne na temat tego, ile pojazdów zostało wypożyczonych o danej godzinie danego dnia, jakie były wtedy warunki atmosferyczne, czy był to zwykły dzień pracy czy wolny itp. Interesuje mnie wartość ostatniej kolumny ze zbioru data.csv czyli cnt - to jest sumaryczna liczba wypożyczeń. Dodatkowo ta suma jest rozbita na liczbę wypożyczeń użytkowników zarejestrowanych (registered) i niezarejestrowanych (casual). Jeżeli ktoś chce to może stworzyć osobny model per grupa użytkowników co może poprawić wyniki. Na koniec proszę zwrócić sumaryczną liczbę wypożyczeń, czyli przewidywane registered + przewidywane casual lub przewidywane cnt.


Omówienie plików:
- data.csv - dane treningowe
- evaluation_data.csv - dane do testowania
- wynik.csv - predykcja dla evaluation_data.csv
