# :computer: TASK 1 :computer:
## Subtask 1
9/10
## Subtask 3
Dlaczego zdecydował_ś się na udział w challenge portfolio?
* Jestem mamą powracającą do zawodowej aktywności po okresie towarzyszenia dzieciom w edukacji domowej. Chcę się przebranżowić i aktywnie działam w tym kierunku. Uczestniczę w programie mentoringowym firmy Roche, szkolę się także we własnym zakresie. W związku z tym chcę prezentować efekty swojej aktywności w portfolio. Dlatego też postanowiłam wziąć udział w wyzwaniu. Chcę dowiedzieć się jak takie profesjonalne portfolio powinno wyglądać, poznać dobre praktyki w tym zakresie. Poza tym wyzwanie wymaga systematyczności i pozwala uzyskać feedback, co skłoniło mnie do skorzystania właśnie z tej formy nauki.
## Subtask 4 _Testy eksploracyjne_
### Opis aplikacji 'Scout Panel'
Aplikacja ('Scouts Panel')[https://scouts-test.futbolkolektyw.pl/pl] gromadzi dane o zawodnikach, rozegranych przez nich meczach oraz pozwala na generowanie raportów na temat konkretnego zawodnika (m.in. zdobyte, stracone gole, przeprowadzone przez zawodnika akcje, jego punktową ocenę w skali 1-5). Aplikacja pozwala dodać informacje na temat udziału zawodnika w meczu (m.in. strzały, podania, dośrodkowania, faule). 
### Funkcjonalności aplikacji 'Scout Panel'
\1 logowanie/wylogowanie
  * logowanie do aplikacji
  * wylogowanie z aplikacji

\2 menu główne/main page
* zawodnik
  * dodawanie zawodnika
  * czyszczenie formularza dodawania zawodnika
  * edycja danych zawodnika
  * wybór daty urodzenia z kalendarza
  * wybór województwa z listy rozwijanej
  * wybór dominującej nogi z listy rozwijanej
  * dodawanie języka obcego do danych zawodnika
  * dodawanie linku youtube
  * usuwanie linku youtube
  * zapisanie danych/zmian w danych
* kontakt z deweloperami (dev team kontact)
* podgląd ostatnich aktywności:
  * ostatnio dodany gracz
  * ostatnio zaktualizowany gracz
  * ostatnio dodany mecz
  * ostatnio zaktualizowany mecz
  * ostatnio zaktualizowany raport 

\3 menu gracze/players
  * wybór rekordu piłkarza do edycji
  * przełączanie tabeli na widok kolejnych/poprzednich rekordów
  * pobieranie widocznych rekordów tabeli (plik csv)
  * drukowanie widoczych rekordów tabeli
  * wybór kolumn do wyświetlenia
  * filtrowanie danych
  * reset w formularzu filtrowania
  * sortowanie
      * wg imienia rosnąco/malejąco
      * wg nazwiska rosnąco/malejąco
      * wg wieku rosnąco/malejąco
      * wg pozycji rosnąco/malejąco
      * wg klubu rosnąco/malejąco
      * wg recenzji rosnąco/malejąco

\4 Gracz/player 
* mecze
  * dodawanie meczu
    * drużyna zawodnika
    * drużyna przeciwna
    * zdobyte gole - wybór z listy rozwijalnej 
    * stracone gole - wybór z listy rozwijalnej 
    * data rozegrania meczu
    * mecz domowy / mecz wyjazdowy (opcje zaznaczane)
    * kolor koszulki 
    * liga
    * czas gry - lista rozwijalna
    * numer - lista rozwijalna
    * web match 
    * general
    * recenzja
  * dodawanie raportu
  * rozpocznij mecz
    * start meczu
    * pauza meczu
    * następna połowa
    * przebieg meczu: 
      * strzały 
      * podania krótkie 
      * podania długie 
      * dośrodkowania 
      * pojedynki 1 na 1
      * strata 
      * faul 
      * odbiór 
      * inne
    * cofnij 
    * zapisz
    * usuń
* raporty
  * wybór raportu do edycji
    * dodawanie komentarzy
    * edycja i treści poszczególnych części raporty
    * formatowanie treści części raportu
    * edycja wartości recenzji (1-5)
    * zapis wprowadzonych zmian
  * dodaj raport

\5 zmiana języka polski / english
 
### Ocena interfejs aplikacji
\1 Wygląd

Czytelny, estetyczny wygląd, który nie utrudnia korzystania z aplikacji. 

\2 Intuicyjność

Aplikacja intuicyjna, łatwa w obsłudze mimo braku opisania funkcji niektórych przycisków. 

\3 Błędy

* wybór kolumn do wyświetlenia - po wyborze i zmianie na kolejne rekordy tabeli '>' zawsze wyświetla kolumnę 'recenzja' (błąd, czy zamierzone?)
* filtrowanie kolumn - aplikacja odfiltrowuje dane, jeśli występuje w nich podany ciąg znaków, nie ma opcji odfiltrowywania dokładnie podanego ciągu znaków (zamierzone, czy błąd?)
* aplikacja akceptuje przyszłą datę, jako datę urodzenia
* aplikacja akceptuje przyszłą datę, jako datę meczu 
* aplikacja akceptuje cyfry i znaki specjalne w polu imię; sugerowane ograniczenie akceptowanych warości pola
* aplikacja akceptuje cyfry i znaki specjalne w polu nazwisko; sugerowane ograniczenie akceptowanych warości pola
* pole waga - aplikacja akceptuje wagę wynoszącą '0'; sugerowane ograniczenie akceptowanych warości pola
* pole waga - aplikacja akceptuje wagę ujemną (np. '-1', '-88888888888888888'); sugerowane ograniczenie akceptowanych warości pola
* pole wzrost - aplikacja akceptuje wzrost wynoszący '0'; sugerowane ograniczenie akceptowanych warości pola
* pole wzrost - aplikacja akceptuje wzrost ujemny (np. '-1', '-88888888888888888'); sugerowane ograniczenie akceptowanych warości pola
* dodawanie zawodnika - nieprecyzyjny komunikat błędu (po wpisaniu adresu, który nie zawiera '@' i '.', albo gdy nie są one poprzedzone, rozdzielone i zakończone innymi znakami wyświetla się komunikat 'Nie udało się dodać gracza' bez wskazania przyczyny odmowy)
* edycja danych zawodnika - nieprecyzyjny komunikat błędu (po wpisaniu adresu, który nie zawiera '@' i '.', albo gdy nie są one poprzedzone, rozdzielone i zakończone innymi znakami wyświetla komunikat 'Nie udało się zaktualizować gracza')
* pole telefon - aplikacja akceptuje ciąg liter; sugerowane ograniczenie akceptowanych wartości pola
* recenzja - skala 1-5, akceptuje wartości pośrednie np. '1.5', '3.5' (zamierzone, czy błąd?)
* raport/ '+raport' przenosi do formularza '+mecz' (zamierzone, czy błąd?) 
* aplikacja akceptuje ujemny numer zawodnika (dodawanie meczu)
* aplikacja akceptuje wpisane ujemnej wartości w polu czas gry
* w funkcjonalności 'rozpocznij mecz' przyciski nie zostały opisane (po najechaniu myszką na przycisk nie wyświetla się podpowiedź o jego funkcji)
* w funkcjonalności 'rozpocznij mecz' wybór połowy meczu nie został ograniczony do dwóch

# :computer: TASK 2 :computer: Przypadki Testowe
## Subtask 1 [Pisanie przypadków testowych na podstawie User Story](https://docs.google.com/spreadsheets/d/1kGgYhcfAwo9Q-UrYPQqeadWV7xBbvT0GQWWaIVEjMQM/edit?usp=share_link)
## Subtask 2 [Pisanie przypadków testowych na podstawie “własnych doświadczeń"](https://docs.google.com/spreadsheets/d/1cZfJawMF8VghIOzEOP1XRp8eheoOJqY7NNRadsEGaIg/edit?usp=sharing)
## Subtask 3 Po co piszemy test case’y?
Przypadki testowe pozwalają nam na metodyczne podejście do testowania. Wtedy, gdy pożądane jest uzyskanie określonego pokrycia testami przygotowanie zestawu przypadków testowych może okazać się niezbędne. 
Spisane przypadki testowe mogą służyć także na etapie przygotowywania testów regresji, a także w automatyzacji testowania. 


https://user-images.githubusercontent.com/116153467/214162117-189625a5-3f3f-42f8-b111-9d7c02eb5eff.mp4



# :computer: TASK 3 :computer: Raportowanie błędów
## Subtask 2 [Testowanie według planów testów i raportowanie błędów](https://docs.google.com/spreadsheets/d/13FTtIAAc2VLeRaXbsxK6MVRgBPc27l0l0zXbACIqL98/edit?usp=sharing)
## Subtask 3 [Raport z wykonanych testów](https://docs.google.com/spreadsheets/d/1p1exlfE12LnTY-XZhSUsZyc0gE-eknjC0SJ21JXYtVM/edit?usp=sharing) 

# :computer: TASK 4 :computer: Testowanie aplikacji mobilnych
## Subtask 2 [Testowanie eksploracyjne i raportowanie błędów](https://docs.google.com/spreadsheets/d/1zonY98r-sqgGXS-CxvyrhpxA1iDgoI0v6PRLBf5PCQc/edit?usp=sharing)
## Subtask 3 Do czego służy aplikacja?

:question: Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?
Aplikacja jest wirtualną tablicą ogłoszeń dotyczących:
  * sprzedaży dóbr
  * sprzedazy usług
  * ofert pracy
  * wymiany dóbr i usług
  * oceny doświadczenia zakupowego
  * komunikacji pomiędzy uczestnikami 
Aplikacja służy zarówno użytkownikom prywatnym jak i firmom (profil użytkowika definiowany jest na etapie rejestracji konta).
Oferty są podzielone na kategorie, w ramach których można wyszukiwać. Wyszukiwanie może zostać ograniczone także wg kryterów lokalizacji, ceny, stanu przedmiotu oferty (używany/nowy/uszkodzony). 

:question:Kto ma być użytkownikiem końcowym aplikacji?

Użytkownikiem końcowym aplikacji jest osoba zdolna do czynności prawnej jaką jest zakup dobra lub usługi. 

:question: Czy według Ciebie aplikacja jest user friendly? (Przyjazna dla użytkownika- np. wchodzisz do aplikacji i szybko łapiesz do czego służą przyciski. Poczytaj na ten temat w internecie- co to znaczy, że aplikacja jest przyjazna dla użytkownika)

Aplikacja jest moim zdaniem user friendly. Jest intuicyjna, przejrzysta, ma dobrze zorganizowaną nawigację i opcje filtrowania. Jest estetyczna wizualnie, formularze w niej zastosowane są adaptują się do orientacji poziomej/pionowej, responsywność nie budzi zastrzeżeń. Linki i nawigacja działają poprawnie. 

:question: Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )

Dodałabym wersje językowe aplikacji (min. English),  łatwo dostępną opcję przełączenia języka obsługi aplikacji.

:question: Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?

Testowanie aplikacji natywnej opiera się na łatwiejszym gromaczeniu i analizowaniu danych o użytkownikach, a także ich lokalizacji. Aplikacja natywna działa bez dostępu do sieci, choć jej funkcje mogą być wówczas ograniczone. Aplikacja internetowa jest uzależniona od dostępu do sieci, a tym samym jej testowanie. Aplikacja natywna ma dostęp do danych i innych aplikacji na urządzeniu (zdjęcia/ kalendarz...), co też wymaga testowania prawidłowej integracji tych usług.

# :computer: TASK 5 :computer: SQL part 1
## Subtask 3 
\1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
```sql
SELECT * FROM `actors` 
ORDER BY surname
```
![image](https://user-images.githubusercontent.com/116153467/217796066-6c5cb191-6e87-4bef-b2ef-e05904da622d.png)

\2. Wyświetl film, który powstał w 2019 roku.
```sql
SELECT * FROM movies
WHERE year_of_production = "2019"
```
![image](https://user-images.githubusercontent.com/116153467/217797276-7a1d8efc-28d5-4cd5-b1b1-ebd114407a24.png)

\3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
```sql
SELECT * FROM movies
WHERE year_of_production > "1900" 
AND year_of_production < "1999"
```
![image](https://user-images.githubusercontent.com/116153467/217797602-e8deb8fb-fe81-4966-8343-bfc95b60b046.png)

\4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
```sql
SELECT title, price FROM movies
WHERE price < "7"
```
![image](https://user-images.githubusercontent.com/116153467/217802501-82c85cd8-0a8d-4229-823a-beba410e58c2.png)

\5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
```sql
SELECT * FROM actors
WHERE actor_id >= 4 
AND actor_id <= 7
```
![image](https://user-images.githubusercontent.com/116153467/217799106-6510e73c-ce60-493d-bd7d-d3e3208bd31f.png)

\6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
```sql
SELECT * FROM customers
WHERE customer_id IN ('2', '4', '6')
```
![image](https://user-images.githubusercontent.com/116153467/217800470-8bfed289-4ee2-4f23-9733-81a7d4a289db.png)

\7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
```sql
SELECT * FROM customers
WHERE customer_id IN ('1', '3', '5')
```
![image](https://user-images.githubusercontent.com/116153467/217800664-66f58dcd-a014-4136-9091-525ae7c14bcc.png)

\8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
```sql
SELECT * FROM actors
WHERE name LIKE "An%"
```
![image](https://user-images.githubusercontent.com/116153467/217801302-f3c400f5-cf4f-4bba-b52b-0d7029b66eb0.png)

\9. Wyświetl dane klienta, który nie ma podanego adresu email.
```sql
SELECT * FROM customers
WHERE email is NULL
```
![image](https://user-images.githubusercontent.com/116153467/217801509-d726550a-93fc-4fa9-95f7-d055d66d3f8f.png)

\10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
```sql
SELECT * FROM movies
WHERE price > 9
AND movie_id BETWEEN 2 AND 8
```
![image](https://user-images.githubusercontent.com/116153467/217802132-1572c7ea-40e0-4424-8c41-f4fe1710afbd.png)

# :computer: TASK 6 :computer: SQL part 2
## Subtask 3 
\11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈
```sql
UPDATE customers
SET surname = 'Miler'
WHERE surname = 'Muler'
```

![image](https://user-images.githubusercontent.com/116153467/219617215-054bca11-3264-46bf-9f95-d507fea1313a.png)

\12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.
```sql
SELECT s.sale_date
,c.name
,c.email
,m.title
FROM customers AS c JOIN sale AS s ON c.customer_id = s.customer_id
JOIN movies AS m ON m.movie_id = s.movie_id
WHERE m.movie_id = 4
```
![image](https://user-images.githubusercontent.com/116153467/219618767-f339d5ab-2c7a-4495-ad6e-3cb12e12da1f.png)

\13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com
```sql
UPDATE customers
SET email = 'pati@mail.com'
WHERE surname = 'Komor'
```
![image](https://user-images.githubusercontent.com/116153467/219619100-df4ba546-87cf-4582-b836-e5b648524c4c.png)

\14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).
```sql
SELECT c.name
,c.surname
,m.title
FROM customers AS c JOIN sale AS s ON c.customer_id = s.customer_id
JOIN movies AS m ON m.movie_id = s.movie_id
```
![image](https://user-images.githubusercontent.com/116153467/219621137-fdcf4f88-9407-4b9f-aae9-ba4ffc1e7579.png)

\15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag

\16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.

\17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)

\18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).

\19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał

\20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa
