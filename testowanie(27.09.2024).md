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

  <!-- Testy weryfikacyjne są stosowane przed i podczas cyklu tworzenia aplikacji -->
  
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

  <!-- 
  Proces walidacji następuje po zakończeniu każdego kroku w cyklu programistycznym:
  - wykorzystanie testów jednostkowych -> po każdej jednostce kodu
  - testy integracyjne -> po ukończeniu kilku modułów gotowych do połączenia w podsystem / system
  -->

### Rodzaje testowania ze względu na stan uruchomienia aplikacji
- testowanie dynamiczne - testowanie uruchomionej aplikacji
- testowanie statyczne - testowanie bez uruchamiania testowanego obiektu (przegląd i analiza statyczna np. samej dokumentacji / kodu)

### Poziomy testów (Pięć etapów procesu testowania)
  - testowanie jednostek - niezależne testowanie komponentów, tak by sprawdzić, czy każdy z nich działa poprawnie osobnie
  - testowanie modułów - testowanie powiązanych komponentów
  - testowanie podsystemów - wykrycie błędów interfejsów, testowanie współdziałania kolekcji modułów
  - testowanie systemu - wykrycie nieprzewidzianych interakcji między podsystemami, sprawdzenie zgodności z wymaganiami funkcjonalnymi (co robi?) i niefunkcjonalnymi (jak robi?) aplikacji
  - testowanie odbiorcze - korzystając z zestawu danych od klienta; **przed przekazaniem**; błędy i niedopatrzenia w definicji wymagań
    
### Koszty naprawy błędów
  Im wcześniej wykryjemy błędy, tym tańsze i łatwiejsze do usunięcia one będą

### Czynności (etapy) testowe:
  - planowanie
  - monitorowanie i nadzór (aż do ukończenia danego procesu testowego)
  - analiza (co testować?)
  - projektowanie (jak testować?)
  - implementacja (przygotowanie testów)
  - wykonywanie (właściwe testowanie)
  - ukończenie
    
### Przydatne linki
- https://sjsi.org/slownik-terminow-testowych-istqb/
- https://sjsi.org/ist-qb/do-pobrania/
- https://academybugs.com

<!-- ### Testowanie czarnoskrzynkowe
  Testowanie zgodności ze specyfikacją (wymaganiami funkcjonalnymi i niefunkcjonalnymi oraz na podstawie diagramów UML: klas, stanów itp.) -->

## Modele rozwoju oprogramowania

- ### Model kaskadowy:
  Sprawdza się najlepiej przy dokładnie sprecyzowanych wymaganiach
  
  Etapy:
  - (planowanie) - weryfikacja umów, analiza ryzyka, listy kontrolne
  - określenie i analiza wymagań klienta - ocena wymagań, testowanie systemu
  - projektowanie / stworzenie specyfikacji aplikacji - ocena projektu
  - implementacja - ocena kodu źródłowego, przypadki testowe
  - testowanie - 
  - wdrożenie - test instalacji  
  - (ekploatacja) - ocena nowych ograniczeń (pod obciążeniem)
  - konserwacja - ocena anomalii i proponowanie zmian

- ### Model przyrostowy:
  Tworzenie aplikacji następuje fragmentami (przyrostami / modułami) wg. modelu kaskadowego
  
  Testowanie przeprowadzamy po przygotowaniu każdego modułu, a następnie integrujemy go z resztą systemu

- ### Model V:
  Równolegle trwają prace testowe i projektowe, prowadzone przez osobne zespoły

  Połączenie etapu rozwoju oprogramowania z odpowiednią fazą testowania (

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

#### Prezentacja o modelach rozwoju oprogramowania:
  http://mariusz.makuchowski.staff.iiar.pwr.wroc.pl/download/courses/komputerowe.wspomaganie.zarzadzania/wyk.slajdy/wyk09.cykl.zycia.pdf
