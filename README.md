# Snake w C# 🐍

## Opis projektu
Prosta gra zręcznościowa **Snake** zaimplementowana w języku C# (Aplikacja Konsolowa). Projekt został stworzony w celach edukacyjnych, aby przećwiczyć współpracę w systemie kontroli wersji Git oraz dokumentowanie poprawek w kodzie (Code Review).

## Funkcje gry
* Sterowanie za pomocą strzałek na klawiaturze.
* Zbieranie jedzenia (`*`) zwiększające wynik.
* Dynamicznie rosnący ogon węża.
* Wykrywanie kolizji ze ścianami oraz własnym ogonem.
* System punktacji wyświetlany w czasie rzeczywistym.

## Naprawione błędy )
W ramach projektu przeprowadzono szereg poprawek błędów składniowych i logicznych:
1. **Obstakel.cs**: Dodano brakującą współrzędną `Ypos` niezbędną do pozycjonowania przeszkód.
2. **Snake.cs**: 
   - Usunięto zduplikowane deklaracje obiektów i naprawiono literówki w nazwach właściwości.
   - Poprawiono logikę ruchu (dodanie instrukcji `break` w pętli switch).
   - Naprawiono warunek detekcji kolizji z jedzeniem (zastosowanie operatora logicznego `&&`).
   - Ujednolicono zarządzanie listami pozycji ogona (`teljePositie`).
   - Rozwiązano problem z indeksowaniem pętli rysującej ogon (`i += 2`).

## Technologie i Narzędzia
* **Język:** C# (.NET Core / Framework)
* **IDE:** Visual Studio 2022
* **System kontroli wersji:** Git / GitHub

## Dokumentacja współpracy
Zgodnie z wymaganiami zadania, każda poprawka błędu była realizowana jako osobny krok:
* Identyfikacja błędu.
* Naprawa w lokalnej gałęzi.
* Dokumentacja zmiany poprzez czytelny komunikat **commit**.
* Wypchnięcie zmian do repozytorium zdalnego (**push**).
