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
## Subtask 2 [Testowanie eksploracyjne i raportowanie błędów]()
## Subtask 3 Do czego służy aplikacja?
* Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?
Aplikacja jest wirtualną tablicą ogłoszeń dotyczących:
** sprzedaży dóbr
** sprzedazy usług
** ofert pracy
** wymiany dóbr i usług
** oceny doświadczenia zakupowego
** komunikacji pomiędzy uczestnikami 
Aplikacja służy zarówno użytkownikom prywatnym jak i firmom (profil użytkowika definiowany jest na etapie rejestracji konta).
Oferty są podzielone na kategorie, w ramach których można wyszukiwać. Wyszukiwanie może zostać ograniczone także wg kryterów lokalizacji, ceny, stanu przedmiotu oferty (używany/nowy/uszkodzony). 
* Kto ma być użytkownikiem końcowym aplikacji?
Użytkownikiem końcowym aplikacji jest osoba zdolna do czynności prawnej jaką jest zakup dobra lub usługi. 
* Czy według Ciebie aplikacja jest user friendly? (Przyjazna dla użytkownika- np. wchodzisz do aplikacji i szybko łapiesz do czego służą przyciski. Poczytaj na ten temat w internecie- co to znaczy, że aplikacja jest przyjazna dla użytkownika)
Aplikacja jest moim zdaniem user friendly. Jest intuicyjna, przejrzysta, ma dobrze zorganizowaną nawigację i opcje filtrowania. Jest estetyczna wizualnie, formularze w niej zastosowane są adaptują się do orientacji poziomej/pionowej, responsywność nie budzi zastrzeżeń. Linki i nawigacja działają poprawnie. 
* Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )
Dodałabym wersje językowe aplikacji (min. English),  łatwo dostępną opcję przełączenia języka obsługi aplikacji.
* Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?
Testowanie aplikacji natywnej opiera się na łatwiejszym gromaczeniu i analizowaniu danych o użytkownikach, a także ich lokalizacji. Aplikacja natywna działa bez dostępu do sieci, choć jej funkcje mogą być wówczas ograniczone. Aplikacja internetowa jest uzależniona od dostępu do sieci, a tym samym jej testowanie. Aplikacja natywna ma dostęp do danych i innych aplikacji na urządzeniu (zdjęcia/ kalendarz...), co też wymaga testowania prawidłowej integracji tych usług.

