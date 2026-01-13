# Schemat działania aplikacji

```mermaid
graph TD;
    Start[Uruchomienie aplikacji] --> Wybor{Co chcesz zrobić?};
    Wybor -- Dodaj wydatek --> Formularz[Wpisanie kwoty i kategorii];
    Formularz --> Baza[Zapisanie do bazy danych];
    Baza --> Aktualizacja[Aktualizacja salda];
    Aktualizacja --> Koniec[Koniec];
    Wybor -- Sprawdz saldo --> Wykres[Wyswietlenie wykresu];
    Wykres --> Koniec;