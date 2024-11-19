## AT-1

### Wyszukiwanie optymalnych tras

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- urządzenie ma dostęp do internetu oraz lokalizacji

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera opcję "Dodaj podróż"
- użytkownik przechodzi do sekcji "Zaplanuj trasę"
- użytkownik wprowadza miejsce początkowe: "Gliwice, Chorzowska 5"
- użytkownik wprowadza miejsce docelowe: "Zabrze, Park Dubiela"
- użytkownik zatwierdza wyszukiwanie przyciskiem "Wyszukaj trasę" 

#### Spodziewane wyniki
- aplikacja wyświetla trasę z "Gliwice, Chorzowska 5" do "Zabrze, Park Dubiela"
- wyświetlana trasa uwzględnia dane o ruchu drogowym i zmianach w organizacji ruchu
- aplikacja poprawnie określa czas i długość trasy oraz potencjalne problemy
- wyświetlana trasa zapisana jest w danych podróży

## AT-2

### Rezerwacja hoteli

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- urządzenie ma dostęp do internetu oraz lokalizacji
- użytkownik zapisał dane karty płatniczej w aplikacji

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera opcję "Dodaj podróż"
- użytkownik przechodzi do sekcji "Rezerwuj nocleg"
- użytkownik wprowadza miejsce: "Zabrze"
- użytkownika ustawia datę zameldowania: "1.11.2024"
- użytkownika ustawia datę wymeldowania: "5.11.2024"
- użytkownik podaje liczbę gości dorosłych: "2"
- użytkownik podaje liczbę gości niepełnoletnich: "0"
- użytkownik zatwierdza wyszukiwanie przyciskiem "Wyszukaj hotel" 
- użytkownik wybiera hotel z listy: "Ibis Hotel Zabrze"
- użytkownik potwierdza rezerwację przyciskiem "Zarezerwuj" 

#### Spodziewane wyniki
- aplikacja wyświetla listę hoteli dostępnych w podanym czasie, z dostępnymi miejscami dla podanej liczby gości
- aplikacja wyświetla szczegóły hotelu po wybraniu go z listy
- zarezerwowany hotel zapisany jest w danych podróży
  
## AT-3

### Rezerwacja restauracji

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- urządzenie ma dostęp do internetu oraz lokalizacji
- użytkownik zapisał dane karty płatniczej w aplikacji

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik przechodzi do sekcji "Rezerwuj restauracje"
- użytkownik wprowadza miejsce: "Gliwice"
- użytkownika ustawia datę i godzinę rezerwacji: "1.11.2024 23:30"
- użytkownik podaje liczbę gości: "2"
- użytkownik zatwierdza wyszukiwanie przyciskiem "Wyszukaj restaurację" 
- użytkownik wybiera restaurację z listy: "Restauracja Bombola"
- użytkownik potwierdza rezerwację przyciskiem "Zarezerwuj" 

#### Spodziewane wyniki
- aplikacja wyświetla listę restauracji dostępnych w podanym czasie
- aplikacja wyświetla szczegóły restauracji po wybraniu jej z listy
- zarezerwowany stolik zapisany jest w danych podróży
  
## AT-4

### Tworzenie harmonogramu podróży

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera opcję "Dodaj podróż"
- użytkownik przechodzi do sekcji "Harmonogram podróży"
- użytkownik wybiera opcję "Nowy punkt"
- użytkownik wprowadza miejsce: "Zabrze, Kopalnia Guido"
- użytkownika ustawia datę i godzinę wizyty: "2.11.2024 11:30"
- użytkownik dodaje notatkę: "Ciepło się ubrać"

#### Spodziewane wyniki
- aplikacja automatycznie dodaje wcześniej dodane informacje (dot. hotelu, restauracji, podróży)
- aplikacja wyświetla pełny harmonogram, z posortowanymi wg. daty kolejnymi punktami podróży
- użytkownik może wyświetlić szczegóły każdego punktu

## AT-5

### Przechowywanie elektronicznych kopii dokumentów podróży

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- aplikacja ma dostęp do pamięci urządzenia

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera opcję "Dodaj podróż"
- użytkownik przechodzi do sekcji "Zapisane dokumenty"
- użytkownik wybiera opcję "Nowy dokument"
- użytkownik wybiera plik zawierający dokument: "bilet_na_pociag.pdf"
- użytkownik nadaje tytuł dokumentowi: "Bilet w obie strony Gliwice-Zabrze"
- użytkownik potwierdza dodanie dokumentu przyciskiem "Zapisz dokument"

#### Spodziewane wyniki
- aplikacja umożliwia zapisanie dokumentu z pliku w różnych formatach (.pdf, .jpg, itd.)
- dokument jest zapisany w danych podróży
  
## AT-6

### Szybki dostęp do zapisanych informacji (dokumentów)

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- użytkownik dodał podróż i zapisał w niej dokument podróży

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera zapisaną podróż: "Romantyczny wypad do Zabrza"
- użytkownik przechodzi do sekcji "Zapisane dokumenty"
- użytkownik wybiera opcję "Nowy dokument"
- użytkownik wybiera zapisany dokument: "Bilet w obie strony Gliwice-Zabrze"
- użytkownik przypina dokument do strony głównej aplikacji

#### Spodziewane wyniki
- aplikacja umożliwia przypięcie dokumentu do strony głównej aplikacji
- aplikacja wyświetla poprawnie wybrany dokument
  
## AT-7

### Dostęp do informacji o miejscu docelowym

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- użytkownik dodał podróż i zaplanował trasę lub dodał punkt do harmonogramu

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik wybiera zapisaną podróż: "Romantyczny wypad do Zabrza"
- użytkownik przechodzi do sekcji "Informacje o miejscu"

#### Spodziewane wyniki
- aplikacja w sekcji "Pogoda" wyświetla informacje o możliwych warunkach pogodowych
- aplikacja w sekcji "Bezpieczeństwo" wyświetla informacje o potencjalnych zagrożeniach
- aplikacja w sekcji "Porady" wyświetla porady dotyczące lokalnych zwyczajów
  
## AT-8

### Funckje społecznościowe

#### Warunki wstępne
- użytkownik jest zalogowany w aplikacji
- aplikacja ma dostęp do pamięci urządzenia
- w systemie istnieje conajmniej 1 dodany post

#### Kroki (dane testowe)
- użytkownik otwiera aplikację Travel
- użytkownik przechodzi do sekcji "Społeczność"
- użytkownik udostępnia plan podróży, klikając przycisk "Udostępnij plan podróży"
- użytkownik klika przycisk "Udostępnij post"
- użytkownik uzupełnia pola: treść, lokalizacja, data
- użytkownik wybiera zdjęcia z pamięci urządzenia
- użytkownik zatwierdza dodanie posta przyciskiem "Opublikuj"
- użytkownik klika przycisk z ikoną serca pod postem innego użytkownika

#### Spodziewane wyniki
- aplikacja wyświetla sekcję "Społeczność" z najnowszymi postami i planami podróży innych użytkowników
- plan podróży użytkownika jest poprawnie udostępniony i widoczny dla innych użytkowników w sekcji „Społeczność”
- opublikowany post zostaje zapisany w zakładce "Moje posty"
- opublikowany post jest widoczny dla w sekcji "Społeczność", z pełną treścią, lokalizacją, datą i zdjęciami
- ilość polubień po naciśnięciu przycisku z ikoną serca, zwiększa się o 1
