# Typy testów

typ testu dobieramy w zależności od tego co chcemy oprzetestować

testy potwierdzające (potwierdzenie naprawienia defektó)
testy regresji (testy niezamieżonych zmian)

## Testy funkcjonalne
testy w systemie, sprawdzenie czy wszystkie zmiany są zgodne z naszymi wymaganiami

- na podst. specyfikacji
- historyjkach użytkownika
- przypadkach użycia

## Testy automatyczne
przyśpieszenie cyklu testowania i poprwaienie jakości oprogramowania

- szybsze przeprowadzenie testów
- sprawdzenie czy qaplikacja działa 24h/7
- sprawdza czy naprawione błędy , dalej nie występują

## Testy białoskrzynkowe
testy oparte na strukturze, wykonywane przez programistów (doświadczonego w zakresie technologii użytej w projekcie), analiza kodu

## testy czarnoskrzykowe
nie przez osoby techniczne, pędkość, intuicyjność, testowanie funkcjonalności aplikacji

- czasochłonne i kosztowne
- mogą nie wykryć wszystkich błędów (ograniczenia dla różnych zestawów danych)

## Testy niefunkcjonalne
sprawdzenie własności niefunkcjonalności aplikacji

### Co testujemy?
- wydajność
- niezawodność
- efektywność
- przenaszalność - działanie na różnych urządzeniach
- zdolność do wprowadzania zmian w prazyszłości

### Testy wydajnościowe
praca aplikacji pod obciążeniem
- czas odpowiedzi
- działanie przy różnej liczbie użytkowników
- czas wykonywania działań

#### Planowanie
- cel
- typy testów
- metryki wydajnościowe - na jakim poziomie powinna znajdować się wydajność aplikacji (czas reakcji, przwepustowość, użytkownicy równocześni, liczba błędów)
- scenariusze testowe
- obiążenie
- narzędzie do testów wydajnościowych

#### Przygotowanie
- konfguracja
- zgromadzenie danych
- stworzenie środ. testowego

#### Analiza wyników
interpretacja wyników

### Typy:
- obciążeniowe - realistyczny, rosnący poziom obciążenia, jak aplikacja sobie radzi
- przeciążeniowe - szczytowe obciążenie przy którym aplikacja przestaje działać, jak aplikacja działa w systuacjach awaryjnych
- skalowalności - wydajność aplikacji, jeśli wymagania się zmienią
- skokowe - przy zróżnicowanym obciążeniu aplikacji (raz mało, raz dużo)
- wytrzymałościowe - stabilnoć systemu w przedziale czasowym (wycieki pamięci, połączenia z bazą danych)
- współbieżności - testowanie wykonywania wielu jednoczesnych działa na raz
- przepustowości - określi ilu użytkowników (czynności) system jest w stanie maksymalnie obsłużyć

### Typowe błęy:
- zbyt wolne odpowiedzi, przy każdym poziomie obciążenia
- zbyt wolne odpowiedzi, przy poziomie obciążenia wzrastającym od śrd. do wys.
- pogarszające się czasy odpowiedzi
- nieadekwatna lub nierzetelna ilość ...

### Narzędzia
- JMeter - za darmo
- LoadRunner
- TestComplete

### Testy użyteczności
łatwość użycia i spełnianie potrzeb użytkowników

- zrozumiałość
- użyteczność
- atrakcyjność

#### Typy testów
- z użytkownikami
- z ekspertami
- z prototypami
- z użytkownikami w naturalnym środowisku

### Testy niezawodności
działanie aplikaci przez określony czas w okreslonycg warunkach
- czas działania bez awarii
- odporność - reagowanie na awarie
- odzyskiwanie - czas regeneracji po awarii

#### Typy testów:
- obciążeniowe
- przeciążeniowe
- odporności - reakcja na awarię
- odzyskiwania - regeneracja po awarii

### Testy przenaszalności:

- testy instalowalności:
- zastępowalności
- koegzystencji

### Testy zdolności wporwadzania zmian w przyszłości:
czy aplikacja jest przygotowana do aktualizacji do nowszej wersji

- architektury
- kodu
- dokumentacji
- procesu - czy jest elastyczny (np. podzielony na moduły - małe kawałki)

<!-- wsyzstkie user story z aplikacji gosi  usr story: jako kto, oczekuję, że aplikacja będzie robić coś, po to aby -->
