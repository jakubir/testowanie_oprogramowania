# Czynności testowe

<!-- 7 zasad, co to testowanie, po co testowanie, weryfikacja a walidacja, planowanie testów -->

## Błąd, defekt, awaria
**Błąd** popełniony przez programisty skutkuje **defektem**, który może prowadzi do **awarii** systemu

## Planowanie testów

#### Identyfikacja celów testowania
Ustalenie celu (wykrycie defektów, weryfikacja zgodności z wymaganiami)

#### Stworzenie strategii testowania
Opracowanie podejścia do testowania (wybranie rodzaju i szczegółowości testów, dobranie zasobów, ustalenie harmonogramu)

#### Opracowanie planu testowania
Określenie zakresu (i poziomu) testów, kryterii wejścia i wyjścia oraz odpowiedzialności członków zespołu

### Stworzenie planu testów (test planu)
czyli dokumnetu, opisującego zakres i czynności związane z testowaniem

#### Test plan powienien zawierać:
- cel
- zakres testów (typy testów)
- rodzaj głównego przedmiotu testów (wydajność, szybkość, intuicyjność)
- krytyria zaliczenia (kiedy ogólnie kończymy testy) (czas oczekiwania na odwiedź, czas ładowania aplikacji, maksymalny czas odpowiedzi, ilość żądań na sekundę, wykorzystanie pamięci)
- krytyteria wejścia / wyjśćia (warunki rozpoczęcia i zakończenia danej czynności) - konkretne progi
- lista wymagań (funkcjonalności do przetestowania)
- środowisko testowe
- harmonogram (ile czasu na poszczególne zadania)
- raport z testów (co powinno na koniec w raporcie po testach zostać spisane)
  
### Dlaczego warto zaplanować proces testowania?
- wiemy, że nic nie zostanie przeoczone w trakcie testowania
- mamy przewodnik po testach, które należy wykonać
- znamy czas i ilość potrzebnej pracy
- znamy dokładne obowiązki członków
- znamy wymagania dot. zasobów i sprzętu

## Monitorowanie i nadzór nad testami

porównywanie czy to jest w test planie jest zgodne z tym co robią testerzy, czy dostajemy odpowiedzi na postawione pytania

### Metryki testowe:
Metryki służa do ocena poziom jakośći, efektywności testowania, adekwatność obranej metody testowej.

Metryki mogą zawierać:
- pokazują procent wykonanej pracy przygotowywaniu testów
- ilość wykonanych przypadków testowych
- ilość wykrytych defektów
- pokrycie wymagań
- koszty testowania
- zgodność z deadline'ami

### Definicja wykonania 
ma miejsce, gdy wszystkie warunki i krytyteria zostały spełnione

Aby zapenić jakośc musimy spełnić definicję wykonania

### Kryteria akceptacji
warunki, które musi spełnić oprogramowanie, aby zostało zaakceptowane przez użytkownika

## Analiza testów

ustalenie co należy testować

Czynności:
- dokonanie analizy podstawy testów
- ocena testowalności podstawy testów i el. testowych, w celu wykrycia defektów, które przeszkadzają w testowaniu
- identyfikowanie cehc i zbiorów cech, które majaą zostać przetestowane
- definiowanie warumków testowych 

## Projektowanie testów

ustalenie w jaki sposób testować

Czynności:
- wybranie poziomu szczegółowości test casów dla konkretnych obszarów
- wybrać techniki testowania
- stworzyć przypadki testowe

### Warunek testowy

### Przypadek testowy
specyfikacja danych wejściowych, warunków wykonania, procedury testowej oraz oczekiwanych wyników

przypadki testowe muszą być przygotowane dla nie-programistów

Pzypadek testowy powinien składać się z:
 - unikalnego numeru
 - tytuł
 - warunki wstępne
 - kroki (dane testowe)
 - spodziewane wyniki
 - priorytet
 - informacje o środowisku

Zalety:
 - wczesne identyfikacaj ryzyka
 - lepsze zrozumienie błędów
 - poprawa jakości oprogramonia
 - ułatnienie komunikacji między zewspołem programistycznym a testowym

Ważne aspekty testowania  przy przypadkach użcyia:
- interfejs użytkownika (ui intuicyjny i łatwy w użyciu; płynne działanie na róznych urządzeniach)
- wydajność (działa szybko i stabilnie, krótki cas ładowaia)
- błędy i wyjątki (poprawne obsługiwanie błędów (brak poł. int.); odpowiednie komunikaty błędów)
- bezpieczeństwo (dane użytkownika odpowiednio zabezpieczone; spełnianie RODO)

<!--
Aplikacja Travel:
znajdzie najlepsze trasy, hotele, resturacje, a także pomożę w organizacji wyjazdu zaarządzaniu dokumentami

1. Planowanie podróży:
wyszukiwanie optymalnych tras
rezerwacj hoteli i restauracji
tworzenie harmonogramu podróży
2. Zarządzanie dokumentacją
przechowywanie elektrobucznych kopii
dokumentów podróży (bilety, itp.)
szybki dostęp do potrzebnych informacji
3. Wsparcie dla podróżnika:
dostęp do informaci o miejscu docelowym
funkcje społecznościowe (dzielenie się doświadczeniami)
-->

### Tworzenie przypadków testowych
szczegółowe scenariusze testujące różne funckjonalnośći

### Tworzenie danych testowcyh
przygotowanie niezbędnych danych do testowania

### projektowanie środ testowego
odpiedni sprzęt oprogramowanie i dancybg do przeprowadzenia testów

## Implementacja testów

sprawdzamy czy posiadamy wszystko co pozwoli na skuteczne przeprowadzenie testów
 - określenie parametrów testów
 - utworzyć skrypty automatyczne
 - uporządkować zestwawy testów
 - wykonać priorytetyzację

### Automatyzacja testów
automatyzacja powtarzalnych czynności

### Przygotowanie zestawów tesowcyh
grupowanie przypadków testowych w logiczne zestawy

## Wykonywanie testów

wykonanie wszystkich zaplanowanych testów

### Przeprowadzenie testów
wykonanie przypadków testowcyh

### Rejestrowanie błędó
dokumentacja znalezionych defektów

### Śledzenie postępu testów
Monitorowanie realizacji planu testów

<!--## Analiza wyników testów

### Ocena wyników testów
analziza wyników pod kątem zgoności z oczekwianiami

### Weryfikacja defektów
Poprwaność zgłoszoncyh testów

### Raporotwanie
przygotowanie raportów-->

## Zakończenie testów

### ocena krytyteriów zakończenia testów
sprawdzenie czy wspełnione zostąły warunki zakończenia testów

### architetkura artefaktów testowych
archiwizacja wyników i dokumentów etc.
