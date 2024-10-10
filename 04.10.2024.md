# 7 zasad testowania oprogramowania

## 1. Testowanie ujawnia usterki, ale nie może dowieść ich braku
  Testowanie nie daje pełnej pewności, że jakiś błąd się nie pojawi. Testowanie zmniejsza ryzyko, że pozostaną jakieś niewykryte defekty.
  
## 2. Testowanie gruntowne jest niemożliwe
  Przetestowanie wszystkiego jest niemożliwe (lub możliwe tylko w prostych przypadkach), ponieważ jest to **kosztowne i czasochłonne**.
  
  Testowanie powinno być ukierunkowane na:
  - analizę ryzyka - wrażliwe obszary
  - odpowiednie techniki testowania - nie wszystkimi technikami trzeba zawsze testować
  - priorytetyzację najważniejszych elementów - wybranie, które elementy można pominąć w procesie testowym

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
  Niemożliwym jest znalezienie (wyeliminowanie) wszystkich błędów, tak więc nie można zakładać ich całkowitego braku.
