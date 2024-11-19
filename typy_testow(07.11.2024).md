# Typy testów
Typ testu dobieramy w zależności od tego, co chcemy przetestować.

## Testy potwierdzające:
Potwierdzenie naprawienia defektów.

## Testy regresji:
Testowanie niezamierzonych zmian.

## Testy automatyczne:
Przyspieszają cykl przeprowadzania testowania i poprawiają jakość oprogramowania.

### Zastosowanie
- Sprawdzenie, czy aplikacja działa 24/7.
- Sprawdzenie, czy naprawione błędy nie występują.

## Technika testowania białoskrzynkowego (strukturalnego):
Wykonywane przez programistów (osoby techniczne), oparte na analizie kodu (wewnętrznej struktury) i doświadczeniu w technologii użytej w projekcie.

## Technika testowania czarnoskrzynkowego:
Wykonywane przez osoby nietechniczne, skupiają się na prędkości, intuicyjności i funkcjonalności aplikacji.

## Testy funkcjonalne:
Sprawdzenie, czy wszystkie zmiany są zgodne z wymaganiami - czy system robi to co powinien.

#### Oparte na:
- specyfikacji
- historyjkach użytkownika
- i przypadkach użycia.

## Testy niefunkcjonalne:
Sprawdzenie własności niefunkcjonalnych aplikacji - jak aplikacja coś robi.

### Co testujemy?
- Wydajność.
- Niezawodność.
- Efektywność.
- Przenaszalność - działanie na różnych urządzeniach.
- Zdolność do wprowadzania zmian w przyszłości.

### Testy wydajnościowe:

#### Zakres:
- Praca aplikacji pod obciążeniem.
- Czas odpowiedzi.
- Działanie przy różnej liczbie użytkowników.
- Czas wykonywania działań.

#### Planowanie:
- Cel.
- Typy testów.
- Metryki wydajnościowe - określenie poziomu wydajności aplikacji (czas reakcji, przwepustowość, użytkownicy równocześni, liczba błędów).
- Scenariusze testowe.
- Obciążenie.
- Narzędzie do testów wydajnościowych.

#### Przygotowanie:
- Konfiguracja.
- Zgromadzenie danych.
- Stworzenie środowiska testowego.

#### Analiza wyników:
- Interpretacja wyników.

### Typy testów wydajnościowych:
- Obciążeniowe.
- Przeciążeniowe.
- Skalowalności.
- Skokowe.
- Wytrzymałościowe.
- Współbieżności.
- Przepustowości.

##### Typowe błędy:
- Zbyt wolne odpowiedzi przy każdym poziomie obciążenia.
- Pogarszające się czasy odpowiedzi.
- Nieadekwatna lub nierzetelna ilość...

##### Narzędzia:
- JMeter.
- LoadRunner.
- TestComplete.

### Testy użyteczności:
- Łatwość użycia i spełnianie potrzeb użytkowników.
- Zrozumiałość.
- Użyteczność.
- Atrakcyjność.

#### Typy testów:
- Z użytkownikami.
- Z ekspertami.
- Z prototypami.
- Z użytkownikami w naturalnym środowisku.

### Testy niezawodności:
- Działanie aplikacji przez określony czas w określonych warunkach.
- Czas działania bez awarii.
- Odporność na awarie.
- Odzyskiwanie po awarii.

#### Typy testów:
- Obciążeniowe.
- Przeciążeniowe.
- Odporności.
- Odzyskiwania.

### Testy przenaszalności:
- Testy instalowalności.
- Testy zastępowalności.
- Testy koegzystencji.

### Testy zdolności wprowadzania zmian w przyszłości:
Sprawdzenie, czy aplikacja jest przygotowana do aktualizacji do nowszej wersji.
- Architektura.
- Kod.
- Dokumentacja.
- Proces.

<!-- Wszystkie user story z aplikacji Gosi:
- Jako kto, oczekuję, że aplikacja będzie robić coś, po to aby... -->

