1. Wyszukiwanie po nazwie produktu
   - Warunki wstępne: istnieje produkt, którego nazwa zawiera "Laptop"
   - Dane wejściowe: "Laptop"
   - Oczekiwane wyniki: Wyświetlenie wszystkich produktów, które zawierają "Laptop" w nazwie

2. Wyszukiwanie po kategorii produktu
   - Warunki wstępne: istnieje kategoria o nazwie "kable"
   - Dane wejściowe: "kable"
   - Oczekiwane wyniki: Wyświetlenie wszystkich produktów, z kategorii "kable"
     
3. Wyszukiwanie za pomocą błędnej pisowni nazwy
   - Warunki wstępne: istnieje produkt, którego nazwa zawiera "Laptop"
   - Dane wejściowe: "lpatop"
   - Oczekiwane wyniki: Wyświetlenie wszystkich produktów, które zawierają "Laptop" w nazwie
     
4. Wyszukiwanie za pomocą błędnej pisowni kategorii
   - Warunki wstępne: istnieje kategoria o nazwie "kable"
   - Dane wejściowe: "kbale"
   - Oczekiwane wyniki: Wyświetlenie wszystkich produktów, z kategorii "kable"
     
5. Wyszukiwanie nieistniejącego produktu
   - Warunki wstępne: nie istnieje produkt, którego nazwa zawiera "Laptop asdasda"
   - Dane wejściowe: "Laptop asdasda"
   - Oczekiwane wyniki: Wyświetlenie odpowiedniego komunikatu
     
6. Wyszukiwanie nieistniejącej kategorii
   - Warunki wstępne: nie istnieje kategoria o nazwie "kable powyżej 100km"
   - Dane wejściowe: "kable powyżej 100km"
   - Oczekiwane wyniki: Wyświetlenie odpowiedniego komunikatu

7. Sprawdzenie zabezpieczeń przed atakami SQL Injection
   - Warunki wstępne:
   - Dane wejściowe: "OR '1'='1'"
   - Oczekiwane wyniki: Zabezpieczenie przed wykonaniem kodu i wyświetlenie odpowiedniego komunikatu
  
8. Sprawdzenie czasu odpowiedzi przy dużej liczbie wyników
   - Warunki wstępme: istnieje conajmniej 2000 produktów, których nazwa zawiera "a"
   - Dane wejściowe: "a"
   - Oczekiwane wyniki: wyniki wyszukiwania pojawią się maksymalnie po 3 sekundach
  
9. Sprawdzenie działania autouzupełniania w wyszukiwarce
   - Warunki wstępne: istnieje produkt o nazwie "Laptop Lenovo"
   - Dane wejściowe: "Laptop Len"
   - Oczekiwane wyniki: autouzupełnianie wyświetli produkt o nazwie "Laptop Lenovo"
   
