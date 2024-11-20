# Testowanie oprogramowania

## Testowanie

### Co to testowanie?
Testowanie oprogramowania to zbiór czynności mających na celu wykrycie defektów i dokonanie oceny
jakości artefaktów (produktów procesu tworzenia oprogramowania) związanych z oprogramowaniem.

### Cele testowania:
- ocena jakości oprogramowania
- zmniejszenie ryzyka awarii
- weryfikacja oprogramowania
- walidacja oprogramowania
- sprawdzanie, czy produkt jest kompletny

### Niezależność zespołu testowego
Testowanie powinno być przeprowadzane przez niezależny (od kadry programistycznej) zespół.

### W każdym etapie procesu rozwoju odbywa się weryfikacja i walidacja

- ### Weryfikacja
  to sprawdzenie zgodności ze specyfikacją -> czy prawidłowo rozwijamy produkt?
  
  #### Cechy weryfikacji:
  - wczesna weryfikacja pomaga zminimalizować błędy i zmniejsza ryzyko
  - regularna weryfikacja pomaga przewidzieć przyszłe problemy oraz przyszły wygląd aplikacji
  - pomaga dostosować produkt do wymagań klienta

  #### Metody:
  - inspekcje
  - przeglądy
  - testy jednostkowe
  - testy integracyjne
  
- ### Walidacja 
  to sprawdzenie zgodności z oczekiwaniami użytkownika -> czy opracowujemy produkt spełniający wymagania klienta? (czy produkt jest prawidłowy?)
  
  #### Cechy walidacji:
  - błędy pominięte w czasie weryfikacji
  - eliminuje błędne założenia w specyfikacji
  - potwierdza zgodność z wymaganiami i oczekiwaniami klienta
  - sprawdza działanie w różnych środowiskach

  #### Metody:
  - testy akceptacyjne
  - testy użytkownika
  - testy badania rynku

### Rodzaje testowania ze względu na stan uruchomienia aplikacji
- testowanie dynamiczne - testowanie uruchomionej aplikacji
- testowanie statyczne - testowanie bez uruchamiania testowanego obiektu (przegląd i analiza statyczna np. samej dokumentacji / kodu)
    
### Koszty naprawy błędów
  Im wcześniej wykryjemy błędy, tym tańsze i łatwiejsze do usunięcia one będą

## Modele rozwoju oprogramowania

- ### Model kaskadowy:
  Sprawdza się najlepiej przy dokładnie sprecyzowanych wymaganiach
  
  Etapy:
  - określenie i analiza wymagań klienta
  - projektowanie / stworzenie specyfikacji aplikacji
  - implementacja
  - testowanie
  - wdrożenie
  - konserwacja

- ### Model przyrostowy:
  Tworzenie aplikacji następuje fragmentami (przyrostami / modułami) wg. modelu kaskadowego
  
  Testowanie przeprowadzamy po przygotowaniu każdego modułu, a następnie integrujemy go z resztą systemu

- ### Model V:
  Równolegle trwają prace testowe i projektowe, prowadzone przez osobne zespoły

  Połączenie etapu rozwoju oprogramowania z odpowiednią fazą testowania

- ### Model W (testowania):
  Rozwinięcie modelu V
  
  Każda etap ma swoje osobne testy
  
  Testowanie trwa przez cały czas pracy

- ### Model programowania odkrywczego:
  Tworzenie kolejnych modyfikacji systemu, które po każdym etapie testowane są przez klienta

- ### Model kontrukcji prototypów:
  Testowanie prototypów przez klienta

  Po akceptacji prototypu, na jego podstawie tworzy się finalny produkt

- ### Model spiralny:
  4 etapy cyklu życia oprogramowania wykonywane są cyklicznie:
  - planowanie
  - analiza ryzyka
  - konstrukcja (wg. modelu kaskadowego)
  - ocena klienta
 
- ### Metoda delficka
  z ekspertami

# 7 zasad testowania oprogramowania

## 1. Testowanie ujawnia usterki, ale nie może dowieść ich braku
  Testowanie nie daje pełnej pewności, że jakiś błąd się nie pojawi. Testowanie zmniejsza ryzyko, że pozostaną jakieś niewykryte defekty.
  
## 2. Testowanie gruntowne jest niemożliwe
  Przetestowanie wszystkiego jest niemożliwe (lub możliwe tylko w prostych przypadkach), ponieważ jest to **kosztowne i czasochłonne**.
  
  Testowanie powinno być ukierunkowane na:
  - analizę ryzyka - identyfikacja wrażliwych obszarów
  - priorytetyzację najważniejszych elementów - wybranie, które elementy można pominąć w procesie testowym
  - odpowiednie techniki testowania - niekonieczne jest wykorzystanie wszystkich technik testowania

## 3. Wczesne testowanie oszczędza czas i pieniądze
  Należy testować od samego początku. Wcześniej wykryte błędy są tańsze do naprawienia.

## 4. Kumulowanie się defektów
  Większość błędów znajduje się w tej samej (małej) ilości modułów (zasada 80/20 -> 20% modulów powoduje 80% błędów) - po znalezieniu jednego błędu należy dalej ich szukać w tym module.

## 5. Paradoks pestycydów
  Ciągłe powtarzanie tych identycznych testów prowadzi do sytuacji, że przestają wykrywać defekty.
  Ważne, aby zmieniać dane testowe, aktualizować bazę testów i przypadki testowe.

## 6. Testowanie zależy od kontekstu
  Różne testowania (dla różnych aplikacji, o różnych warunkach) przeprowadza się w różny sposób, wybierając różne typy testów.
  Podczas planowania testów kluczowa jest wiedza o produkcie.

## 7. Przekonanie o braku błędów jest błędem
  Zbudowanie systemu bez błędów nie zapewnia, że potrzeby klienta zostały zaspokojone

# Czynności testowe

## Planowanie testów

### Test plan powienien zawierać:
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
Porównywanie czy to co jest w test planie jest zgodne z tym co robią testerzy (czy dostajemy odpowiedzi na postawione pytania)

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

Ustalenie co należy testować

### Czynności:
- Przeanalizowanie materiałów potrzebnych do testów.
- Sprawdzenie, czy elementy do testowania są łatwe do przetestowania i wykrycie problemów, które mogą utrudniać testowanie.
- Określenie, jakie cechy systemu będą testowane.
- Ustalenie, elementów do przetestowania

## Projektowanie testów

ustalenie w jaki sposób testować

### Czynności:
- wybrać techniki testowania
- stworzyć przypadki testowe, z uwzględnieniem ich szczegółowości dla poszcególnych obszarów
- przygotowanie danych testowych i środowiska testowego

### Warunek testowy
element lub zdarzenie modułu lub sysytemu, który może być zweryfikowny przez jeden lub więcej przypadków testowych

## Implementacja testów
Sprawdzamy czy posiadamy wszystko co pozwoli na skuteczne przeprowadzenie testów

### Czynności:
 - określenie parametrów testów
 - utworzyć skrypty automatyczne
 - uporządkować przypadki testowe w logiczne zestawy
 - wykonać priorytetyzację

## Wykonywanie testów

### Czynności
- wykonanie wszystkich zaplanowanych testów (przypadków testowych)
- dokumentacja znalezionych defektów
- Monitorowanie realizacji planu testów

## Zakończenie testów

Sprawdzenie czy spełnione zostały warunki zakończenia testów oraz archiwizacja wyników i dokumentów, podsumowanie

# Poziomy testów

## Testy modułowe
Dotyczą poszczególnych elementów, które można przetestować oddzielnie

### Obszary testowania:
- przedmiot: poszczególne moduły
- cel: wykrycie defektów w module, tak by nie wpływały na inne powiązane moduły
- podstawa: kod, projekt, specyfikacja techniczna
- typowe defekty: niepoprawna logika, martwy kod, niepoprawna funckjonalność
- środ. testowe: programistyczne

## Testy integracyjne
Dotyczą głównie miejsc połączeń modułów

### Obszary testowania
- przedmiot: podsystemy, infrastruktura, API
- cel: defekty, które powodują błędy w wielu modułach na raz
- podstawa: projekt oprogramowania, przepływ pracy, przyppadki użycia
- typowe defekty: błędy w komuniiacji, niezgodność interfejsów
- środ. test: programistyczne

### Zasady integracji
- moduły integrowane tylko raz
- jak najmniej modułów integrowanych na raz
- minimalizacja ilości zaślepek i adapterów

## Testy systemowe
skupiają się na całości działania systemu

### Obszary testowania
- przedmiot: aplikacje, OS, inne systemy
- cel: działanie całego systemu, zgodność z wymaganianiami i specyfikacją
- podstawa: specyfikacja, przypadki użycia, user story
- typowe defekty: nietypowe zachowania sytemu
- środ. test.: testowe

## Testy akceptacyjne
Całość działania systemu

### Obszary testowe
- przedmiot: aplikacje, OS, inne systemy
- cel: walidacja i weryfikacja
- podstawa: specyfikacja, procesy biznesowe, przyoadkui użcyia, user story, wymogi prawne
- typowe defekty: niepoprawnie zaimplementowane reguły biznesowe, nieoczekiwane zachowania funkcjonalne, niezgodność z opisanmi w intrukcji, niedostateczna wydajność, słabe zabezpieczenia
- środ. test.: 
  - ALFA (w środ. produkcyjnym / testowe)
  - BETA (w środ. konsumenta)

# Typy testów
Typ testu dobieramy w zależności od tego, co chcemy przetestować.

## Testy potwierdzające:
Potwierdzenie naprawienia defektów.

## Testy regresji:
Testowanie niezamierzonych zmian.

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
- Użyteczność.
- Efektywność - optymalne wykorzystanie zasobów.
- Przenaszalność - działanie na różnych urządzeniach.
- Zdolność do wprowadzania zmian w przyszłości.

### Testy wydajnościowe:

#### Metryki wydajnościowe
Określenie poziomu wydajności aplikacji, wg. miar:
- czas reakcji
- przepustowość
- użytkownicy równocześni
- liczba błędów.

### Typy testów wydajnościowych:
- obciążeniowe - realistyczny, rosnący poziom obciążenia, jak aplikacja sobie radzi
- przeciążeniowe - jak aplikacja działa w systuacjach awaryjnych, ponadprzeciętnego obciążenia
- skalowalności - wydajność aplikacji, jeśli wymagania się zmienią
- skokowe - przy zróżnicowanym obciążeniu aplikacji (raz mało, raz dużo)
- wytrzymałościowe - stabilnoć systemu w przedziale czasowym (wycieki pamięci, połączenia z bazą danych)
- współbieżności - testowanie wykonywania wielu jednoczesnych działa na raz
- przepustowości - określi ilu użytkowników (czynności) system jest w stanie maksymalnie obsłużyć

##### Typowe błędy:
- Zbyt wolne odpowiedzi przy każdym poziomie obciążenia.
- Pogarszające się czasy odpowiedzi przy rosnącej liczbie użytkowników.
- Nieadekwatna lub nierzetelna obsługa błędów przy dużym lub nadmienym poziomie obciążenia

### Testy użyteczności:
- Łatwość użycia i spełnianie potrzeb użytkowników.
- Zrozumiałość.
- Użyteczność.
- Atrakcyjność.

#### Metody:
- Z użytkownikami.
- Z ekspertami.
- Z prototypami.
- Z użytkownikami w naturalnym środowisku.

### Testy niezawodności:
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
Sprawdzenie, czy aplikacja jest przygotowana do aktualizacji do nowszej wersji, pod względem kompatybilności
- Architektura.
- Kod.
- Dokumentacja.
- Proces.

# Testowanie czarnoskrzynkowe

## Testowanie oparte na składni
słownik (gramatyka) danych, które wprowadzamy do aplikacji - określenie jak mają wyglądać

### Notacja Backusa-Naura (BNF) 
sposób definiowania danych

## Tablice decyzyjne
rozpisanie konkretnego przypadku i co w tym momencie może się stać 

### Co zawiera?
- warunki
- działanie
- zasada - połączenie warunków z działaniem (tabela)
  
### Dlaczego?
- łatwe w zrozumieniu
- indetyfikacja błędów logicznych
- automatyzacja
- kompleksowe pokrycie

## Przypadki użycia
szkic interakcji użytkownika z systemem

### Przypadek użycia:
- aktor - osoba / system, który wykonuje interakcję
- cel - co aktor chce osiągnąc
- warunki wstępne
- kroki
- stan po ukończeniu testów

# Słownik:

## Błąd, defekt, awaria
**Błąd** popełniony przez programisty skutkuje **defektem**, który może prowadzi do **awarii** systemu

## Testy automatyczne:
Przyspieszają cykl przeprowadzania testowania i poprawiają jakość oprogramowania.

### Zastosowanie
- Sprawdzenie, czy aplikacja działa 24/7.
- Sprawdzenie, czy naprawione błędy nie występują.

## Przypadek testowy
specyfikacja danych wejściowych, warunków wykonania, procedury testowej oraz oczekiwanych wyników

### Pzypadek testowy powinien składać się z:
 - unikalnego numeru
 - tytuł
 - warunki wstępne
 - kroki (dane testowe)
 - spodziewane wyniki
 - priorytet
 - informacje o środowisku

### Rodzaje przypadków testowych:
- pozytywny - prawidłowe warunki
- negatywny - nieprawidłowe warunki
- graniczny - dopuszczalne wartości
- wyjątkowy - nieoczekiwane zdarzenia

### Zalety:
 - wczesne identyfikacaj ryzyka
 - lepsze zrozumienie błędów
 - poprawa jakości oprogramonia
 - ułatnienie komunikacji między zewspołem programistycznym a testowym

### Ważne aspekty testowania przy przypadkach użycia:
- interfejs użytkownika (ui intuicyjny i łatwy w użyciu; płynne działanie na róznych urządzeniach)
- wydajność (działa szybko i stabilnie, krótki cas ładowaia)
- błędy i wyjątki (poprawne obsługiwanie błędów (brak poł. int.); odpowiednie komunikaty błędów)
- bezpieczeństwo (dane użytkownika odpowiednio zabezpieczone; spełnianie RODO)