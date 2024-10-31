# Poziomy testów

## Testy modułowe
Dotyczą poszczególnych elementów, które można przetestować oddzielnie

### Obszary testowania:
- przedmiot: moduły, jednostki i komponenty aplikacji
- cel: wykrycie defektów w module, tak by nie wpływały na inne powiązane moduły
- podstawa: kod, projekt, specyfikacja techniczna
- typowe defekty: niepoprawna logika, martwy kod, niepoprawna funckjonalność
- środ. testowe: programistyczne

## Testy integracyjne
Dotyczą głównie miejsc połączeń modułów

### Obszary testowania
- przedmiot: podsystemy, infrastruktura, API
- cel: defekty, które powodują błędy w wielu modułach na raz
- podstawa: porjekt oprgrmamowania, przepłuw pracy, przyopadki użycia
- typowe defekty: błędy w komuniiacji, niezgodność interfejsów, nieporawne dane
- środ. test: programistyczne

### Zasady integracji
- moduły integrtowane tylko raz
- koklejnoć i terminy integtrracji, powinny być dokumentiowane
- jak najmniej modułów integrowanych na raz
- nie integrować 2 systemów na raz
- minimalizacja ilości zaślepek i sterowników

## Testy systemowe
skupiają się na całości działania systemu

### Obszary testowania
- przedmiot: aplikacje, OS, inne systemy
- cel: działanie całego systemu, zgodność wymagania funckjonanlne i niefunkcjonalne i specyfikacją
- podstawa: specyfikacja, przyoadkui użcyia, user story
- nietypowe zachowania sytemu
- środ. test.: testowe

## Testy akceptacyjne
Całość działania systemu

### Rodzaje:
- ALFA (gotowy system)
- BETA (w środ. produkcyjnym)

### Obszary testowe
- przedmiot: aplikacje, OS, inne systemy
- cel: walidacja i weryfikacja
- podstawa: specyfikacja, procesy biznesowe, przyoadkui użcyia, user story, wymogi prawne
- typowe defekty: niepoprawnie zaimplementowane reguły biznesowe, nieoczekiwane zachowania funkcjonalne, niezgodność z opisanmi w intrukcji, niedostateczna wydajność, słabe zabezpieczenia
- środ. test.: testowe
