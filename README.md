# Dziennik Kosztów i Tankowań Pojazdu

## Opis projektu

Aplikacja mobilna na system Android (Kotlin, Android Studio), która pomoże kierowcom kontrolować wydatki na paliwo i pilnować terminów serwisowych. Użytkownik zapisuje kolejne tankowania, a aplikacja automatycznie liczy średnie spalanie na 100 km, koszt na kilometr oraz miesięczne podsumowanie wydatków. Dodatkowo zapamiętuje lokalizację stacji tankowania oraz przypomina o nadchodzących obowiązkach, takich jak wymiana oleju, przegląd techniczny czy opłacenie OC.

Grupa docelowa: kierowcy samochodów osobowych (w tym aut z instalacją LPG).

Problem: kierowcy wiedzą, ile płacą za jedno tankowanie, ale trudno im śledzić rzeczywiste spalanie, koszt na kilometr i terminy serwisów.

## Wymagania funkcjonalne

1. **Rejestracja tankowania** - dodawanie wpisu z danymi: rodzaj paliwa (PB / LPG / ON), liczba litrów, cena za litr, koszt całkowity, stan licznika, data.
2. **Historia i statystyki** - lista zapisanych tankowań z możliwością edycji i usuwania wpisów oraz automatyczne wyliczanie średniego spalania (l/100 km), kosztu na kilometr i miesięcznego podsumowania wydatków.
3. **Przypomnienia serwisowe** - definiowanie przypomnień (np. wymiana oleju, przegląd, OC) powiązanych z datą lub przebiegiem, z powiadomieniem systemowym.
4. **Eksport danych** - zapis historii tankowań do pliku CSV i udostępnienie go innej aplikacji.
5. **Lokalizacja stacji** - zapis lokalizacji stacji przy wpisie: pobranej automatycznie z GPS lub wybranej ręcznie, dzięki czemu tankowanie można dodać także po fakcie.

## Wymagania niefunkcjonalne

1. **Trwałość i prywatność danych (offline-first)** - wszystkie dane będą przechowywane w lokalnej bazie danych.
2. **Wydajność** - aplikacja dąży do szybkiego uruchamiania i płynnego działania interfejsu, również przy dużej liczbie zapisanych wpisów.
3. **Użyteczność i bezpieczeństwo działania** - interfejs zgodny z wytycznymi Material Design, walidacja pól formularzy oraz poprawna obsługa uprawnień (aplikacja działa także po odmowie zgody na lokalizację).